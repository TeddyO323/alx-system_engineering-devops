
# :desktop_computer: 0x08. Networking basics #1 :computer:

<p><img src="./s7kpNYq.png" alt="" style="" /></p>

<h2>Resources</h2>

<p><strong>Read or watch</strong>:</p>

<ul>
<li><a href="https://en.wikipedia.org/wiki/Localhost" title="What is localhost" target="_blank">What is localhost</a> </li>
<li><a href="https://en.wikipedia.org/wiki/0.0.0.0" title="What is 0.0.0.0" target="_blank">What is 0.0.0.0</a> </li>
<li><a href="https://www.makeuseof.com/tag/modify-manage-hosts-file-linux/" title="What is the hosts file" target="_blank">What is the hosts file</a> </li>
<li><a href="https://www.thegeekstuff.com/2012/04/nc-command-examples/" title="Netcat examples" target="_blank">Netcat examples</a> </li>
</ul>

<p><strong>man or help</strong>:</p>

<ul>
<li><code>ifconfig</code></li>
<li><code>telnet</code></li>
<li><code>nc</code></li>
<li><code>cut</code></li>
</ul>

<h2>Learning Objectives</h2>

<ul>
<li>What is localhost/127.0.0.1</li>
<li>What is 0.0.0.0</li>
<li>What is <code>/etc/hosts</code></li>
<li>How to display your machine&rsquo;s active network interfaces</li>
</ul>

---

<details>

<summary>Show/Hide Quiz</summary>

### 0.) What is <code>localhost</code>?

- [ ] A hostname that means this IP
- [x] A hostname that means this computer
- [ ] An IP attached to a computer


### 1.) What is 0.0.0.0?

- [x] All IPv4 addresses on the local machine
- [ ] All the IPs
- [ ] It means null in networking

</details>

---

## TASKS

> NOTA: netstat -i, jobs, fg, bg

### 0. Change your home IP
   
<p>Write a Bash script that configures an Ubuntu server with the below requirements.</p>

<p>Requirements:</p>

<ul>
<li><code>localhost</code> resolves to <code>127.0.0.2</code></li>
<li> <code>facebook.com</code> resolves to <code>8.8.8.8</code>.</li>
<li> The checker is running on Docker, so make sure to read <a href="http://blog.jonathanargentiero.com/docker-sed-cannot-rename-etcsedl8ysxl-device-or-resource-busy/" title="this" target="_blank">this</a></li>
</ul>

<p>Example:</p>

<pre><code>sylvain@ubuntu$ ping localhost
PING localhost (127.0.0.1) 56(84) bytes of data.
64 bytes from localhost (127.0.0.1): icmp_seq=1 ttl=64 time=0.012 ms
^C
--- localhost ping statistics ---
1 packets transmitted, 1 received, 0% packet loss, time 0ms
rtt min/avg/max/mdev = 0.012/0.012/0.012/0.000 ms
sylvain@ubuntu$
sylvain@ubuntu$ ping facebook.com
PING facebook.com (157.240.11.35) 56(84) bytes of data.
64 bytes from edge-star-mini-shv-02-lax3.facebook.com (157.240.11.35): icmp_seq=1 ttl=63 time=15.4 ms
^C
--- facebook.com ping statistics ---
1 packets transmitted, 1 received, 0% packet loss, time 0ms
rtt min/avg/max/mdev = 15.432/15.432/15.432/0.000 ms
sylvain@ubuntu$
sylvain@ubuntu$ sudo ./0-change_your_home_IP
sylvain@ubuntu$
sylvain@ubuntu$ ping localhost
PING localhost (127.0.0.2) 56(84) bytes of data.
64 bytes from localhost (127.0.0.2): icmp_seq=1 ttl=64 time=0.012 ms
64 bytes from localhost (127.0.0.2): icmp_seq=2 ttl=64 time=0.036 ms
^C
--- localhost ping statistics ---
2 packets transmitted, 2 received, 0% packet loss, time 1000ms
rtt min/avg/max/mdev = 0.012/0.024/0.036/0.012 ms
sylvain@ubuntu$
sylvain@ubuntu$ ping facebook.com
PING facebook.com (8.8.8.8) 56(84) bytes of data.
64 bytes from facebook.com (8.8.8.8): icmp_seq=1 ttl=63 time=8.06 ms
^C
--- facebook.com ping statistics ---
1 packets transmitted, 1 received, 0% packet loss, time 0ms
rtt min/avg/max/mdev = 8.065/8.065/8.065/0.000 ms
</code></pre>

<p>In this example we can see that:</p>

<ul>
<li>before running the script, <code>localhost</code> resolves to <code>127.0.0.1</code> and <code>facebook.com</code> resolves to <code>157.240.11.35</code></li>
<li>after running the script,  <code>localhost</code> resolves to <code>127.0.0.2</code> and <code>facebook.com</code> resolves to <code>8.8.8.8</code></li>
</ul>

<p>If you&rsquo;re running this script on a machine that you&rsquo;ll continue to use, be sure to revert <code>localhost</code> to <code>127.0.0.1</code>. Otherwise, a lot of things will stop working!</p>

  </div>

[Answer](./0-change_your_home_IP)

---

### 1. Show attached IPs
  
<p>Write a Bash script that displays all active IPv4 IPs on the machine it&rsquo;s executed on.</p>

<p>Example:</p>

<pre><code>sylvain@ubuntu$ ./1-show_attached_IPs | cat -e
10.0.2.15$
127.0.0.1$
sylvain@ubuntu$
</code></pre>

<p>Obviously, the IPs displayed may be different depending on which machine you are running the script on.</p>

<p>Note that we can see our <code>localhost</code> IP :)</p>

  </div>

[Answer](./1-show_attached_IPs)

---

### 2. Port listening on localhost
    
<p>Write a Bash script that listens on port <code>98</code> on <code>localhost</code>.</p>

<p><strong>Terminal 0</strong></p>

<p>Starting my script.</p>

<pre><code>sylvain@ubuntu$ sudo ./100-port_listening_on_localhost
</code></pre>

<p><strong>Terminal 1</strong></p>

<p>Connecting to <code>localhost</code> on port <code>98</code> using <code>telnet</code> and typing some text.</p>

<pre><code>sylvain@ubuntu$ telnet localhost 98
Trying 127.0.0.2...
Connected to localhost.
Escape character is &#39;^]&#39;.
Hello world
test
</code></pre>

<p><strong>Terminal 0</strong></p>

<p>Receiving the text on the other side.</p>

<pre><code>sylvain@ubuntu$ sudo ./100-port_listening_on_localhost
Hello world
test
</code></pre>

<p>For the sake of the exercise, this connection is made entirely within <code>localhost</code>. This isn&rsquo;t really exciting as is, but we can use this script across networks as well. Try running it between your local PC and your remote server for fun!</p>

<p>As you can see, this can come in very handy in a multitude of situations. Maybe you&rsquo;re debugging socket connection issues, or you&rsquo;re trying to connect to a software and you are unsure if the issue is the software or the network, or you&rsquo;re working on firewall rules&hellip; Another tool to add to your debugging toolbox!</p>

  </div>

[Answer](./100-port_listening_on_localhost)

---