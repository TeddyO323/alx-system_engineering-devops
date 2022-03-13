# About Bash projects
  <p><img src="https://s3.amazonaws.com/intranet-projects-files/holbertonschool-sysadmin_devops/205/image.jpg" alt="" style="" /></p>

<h2>Resources</h2>

<p><strong>Read or watch</strong>:</p>

<ul>
<li><a href="http://linuxcommand.org/lc3_lts0010.php" title="What Is &quot;The Shell&quot;?" target="_blank">What Is &ldquo;The Shell&rdquo;?</a> </li>
<li><a href="http://linuxcommand.org/lc3_lts0020.php" title="Navigation" target="_blank">Navigation</a> </li>
<li><a href="http://linuxcommand.org/lc3_lts0030.php" title="Looking Around" target="_blank">Looking Around</a> </li>
<li><a href="http://linuxcommand.org/lc3_lts0040.php" title="A Guided Tour" target="_blank">A Guided Tour</a> </li>
<li><a href="http://linuxcommand.org/lc3_lts0050.php" title="Manipulating Files" target="_blank">Manipulating Files</a> </li>
<li><a href="http://linuxcommand.org/lc3_lts0060.php" title="Working With Commands" target="_blank">Working With Commands</a> </li>
<li><a href="http://linuxcommand.org/lc3_man_pages/man1.html" title="Reading Man pages" target="_blank">Reading Man pages</a> </li>
<li><a href="https://www.howtogeek.com/howto/ubuntu/keyboard-shortcuts-for-bash-command-shell-for-ubuntu-debian-suse-redhat-linux-etc/" title="Keyboard shortcuts for Bash" target="_blank">Keyboard shortcuts for Bash</a> </li>
<li><a href="https://wiki.ubuntu.com/LTS" target="_blank">LTS</a></li>
<li><a href="https://en.wikipedia.org/wiki/Shebang_%28Unix%29" title="Shebang" target="_blank">Shebang</a> </li>
</ul>

<p><strong>man or help</strong>:</p>

<ul>
<li><code>cd</code></li>
<li><code>ls</code></li>
<li><code>pwd</code></li>
<li><code>less</code></li>
<li><code>file</code></li>
<li><code>ln</code></li>
<li><code>cp</code></li>
<li><code>mv</code></li>
<li><code>rm</code></li>
<li><code>mkdir</code></li>
<li><code>type</code></li>
<li><code>which</code></li>
<li><code>help</code></li>
<li><code>man</code></li>
</ul>

<h2>Learning Objectives</h2>

<p>At the end of this project, you are expected to be able to <a href="https://fs.blog/feynman-learning-technique/?fbclid=IwAR2K5_BGPVo0QjJXkOIIqNsqcXK4lTskPWJvA0asKQIGtCPWaQBdKmj1Ztg" title="explain to anyone" target="_blank">explain to anyone</a>, <strong>without the help of Google</strong>:</p>

<h3>General</h3>

<ul>
<li>What does RTFM mean?</li>
<li>What is a Shebang</li>
</ul>

<h3>What is the Shell</h3>

<ul>
<li>What is the shell</li>
<li>What is the difference between a terminal and a shell</li>
<li>What is the shell prompt</li>
<li>How to use the history (the basics)</li>
</ul>

<h3>Navigation</h3>

<ul>
<li>What do the commands or built-ins <code>cd</code>, <code>pwd</code>, <code>ls</code> do </li>
<li>How to navigate the filesystem</li>
<li>What are the . and .. directories</li>
<li>What is the working directory, how to print it and how to change it</li>
<li>What is the root directory</li>
<li>What is the home directory, and how to go there</li>
<li>What is the difference between the root directory and the home directory of the user root</li>
<li>What are the characteristics of hidden files and how to list them</li>
<li>What does the command <code>cd -</code> do</li>
</ul>

<h3>Looking Around</h3>

<ul>
<li>What do the commands <code>ls</code>, <code>less</code>, <code>file</code> do</li>
<li>How do you use options and arguments with commands</li>
<li>Understand the ls long format and how to display it</li>
<li><a href="http://linuxcommand.org/lc3_lts0040.php" title="A Guided Tour" target="_blank">A Guided Tour</a></li>
<li>What does the <code>ln</code> command do</li>
<li>What do you find in the most common/important directories</li>
<li>What is a symbolic link</li>
<li>What is a hard link</li>
<li>What is the difference between a hard link and a symbolic link</li>
</ul>

<h3>Manipulating Files</h3>

<ul>
<li>What do the commands <code>cp</code>, <code>mv</code>, <code>rm</code>, <code>mkdir</code> do</li>
<li>What are wildcards and how do they work</li>
<li>How to use wildcards</li>
</ul>

<h3>Working with Commands</h3>

<ul>
<li>What do <code>type</code>, <code>which</code>, <code>help</code>, <code>man</code> commands do</li>
<li>What are the different kinds of commands</li>
<li>What is an alias</li>
<li>When do you use the command help instead of man</li>
</ul>

<h3>Reading Man Pages</h3>

<ul>
<li>How to read a man page</li>
<li>What are man page sections</li>
<li>What are the section numbers for User commands, System calls and Library functions</li>
</ul>

<h3>Keyboard Shortcuts for Bash</h3>

<ul>
<li>Common shortcuts for Bash</li>
</ul>

<h3>LTS</h3>

<ul>
<li>What does <code>LTS</code> mean?</li>
</ul>

<h2>Requirements</h2>

<h3>General</h3>

<ul>
<li>Allowed editors: <code>vi</code>, <code>vim</code>, <code>emacs</code></li>
<li>All your scripts will be tested on Ubuntu 20.04 LTS</li>
<li>All your scripts should be exactly two lines long (<code>$ wc -l file</code> should print 2)</li>
<li>All your files should end with a new line (<a href="http://unix.stackexchange.com/questions/18743/whats-the-point-in-adding-a-new-line-to-the-end-of-a-file/18789">why?</a>)</li>
<li>The first line of all your files should be exactly <code>#!/bin/bash</code></li>
<li>A <code>README.md</code> file at the root of the repo, containing a description of the repository</li>
<li>A <code>README.md</code> file, at the root of the folder of <em>this</em> project, describing what each script is doing</li>
<li>You are not allowed to use backticks, <code>&amp;&amp;</code>, <code>||</code> or <code>;</code></li>
<li>All your scripts must be executable. To make your file executable, use the <code>chmod</code> command:  <code>chmod u+x file</code>. Later, we&rsquo;ll learn more about how to utilize this command.</li>
</ul>

<h2>More Info</h2>

<p><i>Example of line count and first line</i></p>

<pre><code>julien@ubuntu:/tmp$ wc -l 12-file_type 
2 12-file_type
julien@ubuntu:/tmp$ head -n 1 12-file_type 
#!/bin/bash
julien@ubuntu:/tmp$ 
</code></pre>

<p>In order to test your scripts, you will need to use this command: <code>chmod u+x file</code>. We will see later what does <code>chmod</code> mean and do, but you can have a look at <code>man chmod</code> if you are curious.</p>

<p><i>Example</i></p>

<pre><code>julien@ubuntu:/tmp$ ls
12-file_type
lll
julien@ubuntu:/tmp$ ls -la lll
-rw-rw-r-- 1 julien julien 15 Sep 19 21:05 lll
julien@ubuntu:/tmp$ cat lll
#!/bin/bash
ls
julien@ubuntu:/tmp$ ls -l lll
-rw-rw-r-- 1 julien julien 15 Sep 19 21:05 lll
julien@ubuntu:/tmp$ chmod u+x lll # you do not have to understand this yet
julien@ubuntu:/tmp$ ls -l lll
-rwxrw-r-- 1 julien julien 15 Sep 19 21:05 lll
julien@ubuntu:/tmp$ ./lll
12-file_type
lll
julien@ubuntu:/tmp$ 
</code></pre>

</div>

---

# 0. Where am I?
    

    
<p>Write a script that prints the absolute path name of the current working directory.</p>


<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>0-current_working_directory</code></li>
        </ul>

# 1. What’s in there?
 
<p>Display the contents list of your current directory.</p>


<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>1-listit</code></li>
        </ul>

# 2. There is no place like home

<p>Write a script that changes the working directory to the user’s home directory.</p>

<ul>
<li>You are not allowed to use any shell variables</li>
</ul>


<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>2-bring_me_home</code></li>
        </ul>

# 3. The long format
  

<p>Display current directory contents in a long format</p>


<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>3-listfiles</code></li>
        </ul>
    
# 4. Hidden files
  
<p>Display current directory contents, including hidden files (starting with <code>.</code>). Use the long format.</p>


 <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>4-listmorefiles</code></li>
        </ul>

# 5. I love numbers
 
 <p>Display current directory contents.</p>

<ul>
<li>Long format</li>
<li>with user and group IDs displayed numerically</li>
<li>And hidden files (starting with .)</li>
</ul>



  <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>5-listfilesdigitonly</code></li>
        </ul>

# 6. Welcome
  
 <p>Create a script that creates a directory named <code>my_first_directory</code> in the <code>/tmp/</code> directory.</p>

<p>Example:</p>


 <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>6-firstdirectory</code></li>
        </ul>

# 7. Betty in my first directory
  
  <p>Move the file <code>betty</code> from <code>/tmp/</code> to <code>/tmp/my_first_directory</code>.</p>


  <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>7-movethatfile</code></li>
        </ul>

# 8. Bye bye Betty
 
<p>Delete the file <code>betty</code>.</p>

<ul>
<li>The file <code>betty</code> is in <code>/tmp/my_first_directory</code></li>
</ul>

<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>8-firstdelete</code></li>
        </ul>
      
# 9. Bye bye My first directory

<p>Delete the directory <code>my_first_directory</code> that is in the <code>/tmp</code> directory.</p>


 <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>9-firstdirdeletion</code></li>
        </ul>

# 10. Back to the future

<p>Write a script that changes the working directory to the previous one.</p>


  
 <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>10-back</code></li>
        </ul>

# 11. Lists
  
<p>Write a script that lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the <code>/boot</code> directory (in this order), in long format.</p>

<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>11-lists</code></li>
        </ul>

# 12. File type

<p>Write a script that prints the type of the file named <code>iamafile</code>. The file <code>iamafile</code> will be in the <code>/tmp</code> directory when we will run your script.</p>

<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>12-file_type</code></li>
        </ul>

# 13. We are symbols, and inhabit symbols

<p>Create a symbolic link to <code>/bin/ls</code>, named <code>__ls__</code>.
The symbolic link should be created in the current working directory. </p>

<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>13-symbolic_link</code></li>
        </ul>
      </div>

# 14. Copy HTML files

 <p>Create a script that copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory.</p>

<p>You can consider that all HTML files have the extension <code>.html</code></p>


<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>14-copy_html</code></li>
        </ul>

# 15. Let’s move
  
 <p>Create a script that moves all files beginning with an uppercase letter to the directory <code>/tmp/u</code>.</p>

<p>You can assume that the directory <code>/tmp/u</code> will exist when we will run your script</p>


<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>100-lets_move</code></li>
        </ul>

# 16. Clean Emacs

<p>Create a script that deletes all files in the current working directory that end with the character <code>~</code>.</p>


<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>101-clean_emacs</code></li>
        </ul>
      </div>

# 17. Tree
    

 <p>Create a script that creates the directories <code>welcome/</code>, <code>welcome/to/</code> and <code>welcome/to/school</code> in the current directory.</p>

<p>You are only allowed to use two spaces (and lines) in your script, not more.</p>


  
 <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>102-tree</code></li>
        </ul>
      

# 18. Life is a series of commas, not periods

<p>Write a command that lists all the files and directories of the current directory, separated by commas (<code>,</code>).</p>

<ul>
<li>Directory names should end with a slash (<code>/</code>)<br></li>
<li>Files and directories starting with a dot (<code>.</code>) should be listed<br></li>
<li>The listing should be alpha ordered, except for the directories <code>.</code> and <code>..</code> which should be listed at the very beginning</li>
<li>Only digits and letters are used to sort; Digits should come first</li>
<li>You can assume that all the files we will test with will have at least one letter or one digit</li>
<li>The listing should end with a new line<br></li>
</ul>

<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>103-commas</code></li>
        </ul>

#  19. File type: School

 <p>Create a magic file <code>school.mgc</code> that can be used with the command <code>file</code> to detect <code>School</code> data files. <code>School</code> data files always contain the string <code>SCHOOL</code> at offset 0.</p>

 <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x00-shell_basics</code></li>
            <li>File: <code>school.mgc</code></li>
        </ul>
      
