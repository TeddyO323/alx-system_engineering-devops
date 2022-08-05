# 0x06. Regular expression

<h3 class="panel-title">Concepts</h3>
    </div>
    <div class="panel-body">
      <p>
        <em>For this project, we expect you to look at this concept:</em>
      </p>

<ul>
          <li>
            <a href="./concept.md">Regular Expression</a>
          </li>
      </ul>
    </div>
  </div>


      
<h2>Background Context</h2>

<p>For this project, you have to build your regular expression using Oniguruma, a regular expression library that which is used by Ruby by default. Note that other regular expression libraries sometimes have different properties.</p>

<p>Because the focus of this exercise is to play with regular expressions (regex), here is the Ruby code that you should use, just replace the regexp part, meaning the code in between the <code>//</code>:</p>

<pre><code>sylvain@ubuntu$ cat example.rb
#!/usr/bin/env ruby
puts ARGV[0].scan(/127.0.0.[0-9]/).join
sylvain@ubuntu$
sylvain@ubuntu$ ./example.rb 127.0.0.2
127.0.0.2
sylvain@ubuntu$ ./example.rb 127.0.0.1
127.0.0.1
sylvain@ubuntu$ ./example.rb 127.0.0.a
</code></pre>

<h2>Resources</h2>

<p><strong>Read or watch</strong>:</p>

<ul>
<li><a href="https://www.slideshare.net/neha_jain/introducing-regular-expressions" title="Regular expressions - basics" target="_blank">Regular expressions - basics</a> </li>
<li><a href="https://www.slideshare.net/neha_jain/advanced-regular-expressions-80296518" title="Regular expressions - advanced" target="_blank">Regular expressions - advanced</a> </li>
<li><a href="https://rubular.com/" title="Rubular is your best friend" target="_blank">Rubular is your best friend</a> </li>
<li><a href="https://blog.codinghorror.com/regular-expressions-now-you-have-two-problems/" title="Use a regular expression against a problem: now you have 2 problems" target="_blank">Use a regular expression against a problem: now you have 2 problems</a> </li>
<li><a href="https://regexone.com/" title="Learn Regular Expressions with simple, interactive exercises" target="_blank">Learn Regular Expressions with simple, interactive exercises</a> </li>
</ul>

---

<details>

<summary>Show/Hide Quiz</summary>

### 0.) What is the <code>/school/</code> regexp matching?

- [ ] schoOl
- [ ] School
- [x] school

### 1.) What is the <code>/Scho.l/</code> regexp matching?

- [x] Scho.l
- [x] School
- [ ] school

### 2.) What is the <code>/Scho*l/</code> regexp matching?

- [x] Schoool
- [ ] Scho.l
- [ ] Schoo.l

---

## TASKS

<h3 class="panel-title">
      0. Simply matching School
    </h3>

    
<p><img src="./ec65557f0da1fbfbff6659413885e4d4822f5b1d.png" alt="" style="" /></p>

<p>Requirements:</p>

<ul>
<li>The regular expression must match <code>School</code></li>
<li>Using the project instructions, create a Ruby script that accepts one argument and pass it to a regular expression matching method</li>
</ul>

<p>Example:</p>

<pre><code>sylvain@ubuntu$ ./0-simply_match_school.rb School | cat -e
School$
sylvain@ubuntu$ ./0-simply_match_school.rb &quot;Best School&quot; | cat -e
School$
sylvain@ubuntu$ ./0-simply_match_school.rb &quot;School Best School&quot; | cat -e
SchoolSchool$
sylvain@ubuntu$ ./0-simply_match_school.rb &quot;Grace Hopper&quot; | cat -e
$
</code></pre>

  </div>

[Answer](./0-simply_match_school.rb)

---

<h3 class="panel-title">
      1. Repetition Token #0
    </h3>

    
<p><img src="./e7db3c377d46453588fc84f3a975661d142fee91.png" alt="" style="" /></p>

<p>Requirements:</p>

<ul>
<li>Find the regular expression that will match the above cases</li>
<li>Using the project instructions, create a Ruby script that accepts one argument and pass it to a regular expression matching method</li>
</ul>

  </div>

[Answer](./1-repetition_token_0.rb)

---

<h3 class="panel-title">
      2. Repetition Token #1
    </h3>

   
<p><img src="./c59ff11db195d5cf17d1790a5141ae2f234786d2.png" alt="" style="" /></p>

<p>Requirements:</p>

<ul>
<li>Find the regular expression that will match the above cases</li>
<li>Using the project instructions, create a Ruby script that accepts one argument and pass it to a regular expression matching method</li>
</ul>

  </div>

[Answer](./2-repetition_token_1.rb)

---

<h3 class="panel-title">
      3. Repetition Token #2
    </h3>

   
<p><img src="./3b6bf4aeca6a0c2de584e7f5d68d11eef57ce205.png" alt="" style="" /></p>

<p>Requirements:</p>

<ul>
<li>Find the regular expression that will match the above cases</li>
<li>Using the project instructions, create a Ruby script that accepts one argument and pass it to a regular expression matching method</li>
</ul>

  </div>

[Answer](./3-repetition_token_2.rb)

---

<h3 class="panel-title">
      4. Repetition Token #3
    </h3>

    
<p><img src="./f8dbcb9cf5ae569a8645027dc46e81cb372ce28e.png" alt="" style="" /></p>

<p>Requirements:</p>

<ul>
<li>Find the regular expression that will match the above cases</li>
<li>Using the project instructions, create a Ruby script that accepts one argument and pass it to a regular expression matching method</li>
<li>Your regex should not contain square brackets</li>
</ul>

  </div>

[Answer](./4-repetition_token_3.rb)

---

<h3 class="panel-title">
      5. Not quite HBTN yet
    </h3>

<p>Requirements:</p>

<ul>
<li>The regular expression must be exactly matching a string that starts with <code>h</code> ends with <code>n</code> and can have any single character in between</li>
<li>Using the project instructions, create a Ruby script that accepts one argument and pass it to a regular expression matching method</li>
</ul>

<p>Example:</p>

<pre><code>sylvain@ubuntu$ ./5-beginning_and_end.rb &#39;hn&#39; | cat -e
$
sylvain@ubuntu$ ./5-beginning_and_end.rb &#39;hbn&#39; | cat -e
hbn$
sylvain@ubuntu$ ./5-beginning_and_end.rb &#39;hbtn&#39; | cat -e
$
sylvain@ubuntu$ ./5-beginning_and_end.rb &#39;h8n&#39; | cat -e
h8n$
sylvain@ubuntu$
$
</code></pre>

  </div>

[Answer](./5-beginning_and_end.rb)

---

<h3 class="panel-title">
      6. Call me maybe
    </h3>

<p>This task is brought to you by a professional advisor <a href="https://twitter.com/_nehajain" title="Neha Jain" target="_blank">Neha Jain</a>, Senior Software Engineer at LinkedIn.</p>

<p>Requirement:</p>

<ul>
<li>The regular expression must match a 10 digit phone number</li>
</ul>

<p>Example:</p>

<pre><code>sylvain@ubuntu$ ./6-phone_number.rb 4155049898 | cat -e
4155049898$
sylvain@ubuntu$ ./6-phone_number.rb &quot; 4155049898&quot; | cat -e
$
sylvain@ubuntu$ ./6-phone_number.rb &quot;415 504 9898&quot; | cat -e
$
sylvain@ubuntu$ ./6-phone_number.rb &quot;415-504-9898&quot; | cat -e
$
sylvain@ubuntu$
</code></pre>

  </div>

[Answer](./6-phone_number.rb)

---

<h3 class="panel-title">
      7. OMG WHY ARE YOU SHOUTING?
    </h3>

  
<p><img src="./shouting.jpg" alt="" style="" /></p>

<p>Requirement:</p>

<ul>
<li>The regular expression must be only matching: capital letters</li>
</ul>

<p>Example:</p>

<pre><code>sylvain@ubuntu$ ./7-OMG_WHY_ARE_YOU_SHOUTING.rb &quot;I realLy hOpe VancouvEr posseSs Yummy Soft vAnilla Dupper Mint Ice Nutella cream&quot; | cat -e
ILOVESYSADMIN$
sylvain@ubuntu$ ./7-OMG_WHY_ARE_YOU_SHOUTING.rb &quot;WHAT do you SAY?&quot; | cat -e
WHATSAY$
sylvain@ubuntu$ ./7-OMG_WHY_ARE_YOU_SHOUTING.rb &quot;cannot read you&quot; | cat -e
$
sylvain@ubuntu$
</code></pre>

  </div>

[Answer](./7-OMG_WHY_ARE_YOU_SHOUTING.rb)

---

<h3 class="panel-title">
      8. Textme
    </h3>

    
<p>This exercise was prepared for you by <a href="/rltoken/2Rwwb9pSGKXSp3b3BcqkAw" title="Guillaume Plessis" target="_blank">Guillaume Plessis</a>, VP of Infrastructure at TextMe. It is something he uses daily. You can thank Guillaume for his project <a href="https://twitter.com/gui" title="on Twitter" target="_blank">on Twitter</a>.</p>

<p>For this task, you&rsquo;ll be taking over Guillaume&rsquo;s responsibilities: one afternoon, a TextMe VoIP Engineer comes to you and explains she wants to run some statistics on the TextMe app text messages transactions.</p>

<p>Requirements:</p>

<ul>
<li>Your script should output: <code>[SENDER],[RECEIVER],[FLAGS]</code>

<ul>
<li>The sender phone number or name (including country code if present)</li>
<li>The receiver phone number or name (including country code if present)</li>
<li>The flags that were used</li>
</ul></li>
</ul>

<p>You can find a <a href="http://intranet-projects-files.s3.amazonaws.com/holbertonschool-sysadmin_devops/78/text_messages.log" target="_self">[log file here]</a>.</p>

<p>Example:</p>

<pre><code>$ ./100-textme.rb &#39;Feb 1 11:00:00 ip-10-0-0-11 mdr: 2016-02-01 11:00:00 Receive SMS [SMSC:SYBASE1] [SVC:] [ACT:] [BINF:] [FID:] [from:Google] [to:+16474951758] [flags:-1:0:-1:0:-1] [msg:127:This planet has - or rather had - a problem, which was this: most of the people on it were unhappy for pretty much of the time.] [udh:0:]&#39;
Google,+16474951758,-1:0:-1:0:-1
$
$
$ ./100-textme.rb &#39;Feb 1 11:00:00 ip-10-0-64-10 mdr: 2016-02-01 11:00:00 Receive SMS [SMSC:SYBASE2] [SVC:] [ACT:] [BINF:] [FID:] [from:+17272713208] [to:+19172319348] [flags:-1:0:-1:0:-1] [msg:136:Orbiting this at a distance of roughly ninety-two million miles is an utterly insignificant little blue green planet whose ape-descended] [udh:0:]&#39;
+17272713208,+19172319348,-1:0:-1:0:-1
$
$ ./100-textme.rb &#39;Feb 1 11:00:00 ip-10-0-64-11 mdr: 2016-02-01 11:00:00 Sent SMS [SMSC:SYBASE1] [SVC:backendtextme] [ACT:] [BINF:] [FID:] [from:18572406905] [to:14022180266] [flags:-1:0:-1:-1:-1] [msg:136:Far out in the uncharted backwaters of the unfashionable end of the western spiral arm of the Galaxy lies a small unregarded yellow sun.] [udh:0:]&#39;
18572406905,14022180266,-1:0:-1:-1:-1
$
$
$ ./100-textme.rb &#39;Feb 1 11:00:00 ip-10-0-64-11 mdr: 2016-02-01 11:00:00 Sent SMS [SMSC:SYBASE1] [SVC:backendtextme] [ACT:] [BINF:] [FID:] [from:12392190384] [to:19148265919] [flags:-1:0:-1:-1:-1] [msg:99:life forms are so amazingly primitive that they still think digital watches are a pretty neat idea.] [udh:0:]&#39;
12392190384,19148265919,-1:0:-1:-1:-1
$

</code></pre>

  </div>

[Answer](./100-textme.rb)

---

<em>THE END<em>



