# About <span class="text-primary">Bash</span> projects
    
<p>
<p>Unless stated, all your projects will be auto-corrected with Ubuntu 20.04 LTS.</p>

</p>
</div>


      

<div class="well clean" id="project-description">
<h2>Resources</h2>

<p><strong>Read or watch</strong>:</p>

<ul>
<li><a href="http://linuxcommand.org/lc3_lts0090.php" title="Permissions" target="_blank">Permissions</a> </li>
</ul>

<p><strong>man or help</strong>:</p>

<ul>
<li><code>chmod</code></li>
<li><code>sudo</code></li>
<li><code>su</code></li>
<li><code>chown</code></li>
<li><code>chgrp</code></li>
<li><code>id</code></li>
<li><code>groups</code></li>
<li><code>whoami</code></li>
<li><code>adduser</code></li>
<li><code>useradd</code></li>
<li><code>addgroup</code></li>
</ul>

<h2>Learning Objectives</h2>

<p>At the end of this project, you are expected to be able to <a href="https://fs.blog/feynman-learning-technique/?fbclid=IwAR2K5_BGPVo0QjJXkOIIqNsqcXK4lTskPWJvA0asKQIGtCPWaQBdKmj1Ztg" title="explain to anyone" target="_blank">explain to anyone</a>, <strong>without the help of Google</strong>:</p>

<h3>Permissions</h3>

<ul>
<li>What do the commands <code>chmod</code>, <code>sudo</code>, <code>su</code>, <code>chown</code>, <code>chgrp</code> do</li>
<li>Linux file permissions</li>
<li>How to represent each of the three sets of permissions (owner, group, and other) as a single digit</li>
<li>How to change permissions, owner and group of a file</li>
<li>Why can&rsquo;t a normal user <code>chown</code> a file</li>
<li>How to run a command with root privileges</li>
<li>How to change user ID or become superuser<br></li>
</ul>

<h3>Other Man Pages</h3>

<ul>
<li>How to create a user</li>
<li>How to create a group</li>
<li>How to print real and effective user and group IDs</li>
<li>How to print the groups a user is in</li>
<li>How to print the effective userid</li>
</ul>

<h2>Requirements</h2>

<h3>General</h3>

<ul>
<li>Allowed editors: <code>vi</code>, <code>vim</code>, <code>emacs</code></li>
<li>All your scripts will be tested on Ubuntu 20.04 LTS</li>
<li>All your scripts should be exactly two lines long (<code>$ wc -l file</code> should print 2)</li>
<li>All your files should end with a new line (<a href="http://unix.stackexchange.com/questions/18743/whats-the-point-in-adding-a-new-line-to-the-end-of-a-file/18789">why?</a>)</li>
<li>The first line of all your files should be exactly <code>#!/bin/bash</code></li>
<li>A <code>README.md</code> file, at the root of the folder of the project, describing what each script is doing</li>
<li>You are not allowed to use backticks, <code>&amp;&amp;</code>, <code>||</code> or <code>;</code></li>
<li>All your files must be executable</li>
</ul>

---

# 0. My name is Betty
 

<p>Create a script that switches the current user to the user <code>betty</code>.</p>

<ul>
<li>You should use exactly 8 characters for your command (+1 character for the new line)</li>
<li>You can assume that the user <code>betty</code> will exist when we will run your script</li>
</ul>




 <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>0-iam_betty</code></li>
        </ul>
      </div>

# 1. Who am I

<p>Write a script that prints the effective username of the current user.</p>



   
<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>1-who_am_i</code></li>
        </ul>

# 2. Groups
 
<p>Write a script that prints all the groups the current user is part of.</p>


<p>Note: depending on the user, you will get a different output.</p>

<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>2-groups</code></li>
        </ul>
      
# 3. New owner
   
 <p>Write a script that changes the owner of the file <code>hello</code> to the user <code>betty</code>.</p>




<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>3-new_owner </code></li>
        </ul>
      </div>

# 4. Empty!
    

<p>Write a script that creates an empty file called <code>hello</code>.</p>

 
<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>4-empty</code></li>
        </ul>


  
# 5. Execute

<p>Write a script that adds execute permission to the owner of the file <code>hello</code>.</p>

<ul>
<li>The file <code>hello</code> will be in the working directory</li>
</ul>

<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>5-execute</code></li>
        </ul>

# 6. Multiple permissions

<p>Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file <code>hello</code>.</p>

<ul>
<li>The file <code>hello</code> will be in the working directory</li>
</ul>

<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>6-multiple_permissions</code></li>
        </ul>

# 7. Everybody!
  
  <p>Write a script that adds execution permission to the owner, the group owner and the other users, to the file <code>hello</code></p>

<ul>
<li>The file <code>hello</code> will be in the working directory</li>
<li>You are not allowed to use commas for this script</li>
</ul>



  
<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>7-everybody</code></li>
        </ul>
      
# 8. James Bond
    
 <p>Write a script that sets the permission to the file <code>hello</code> as follows:</p>

<ul>
<li>Owner: no permission at all</li>
<li>Group: no permission at all</li>
<li>Other users: all the permissions</li>
</ul>

<p>The file <code>hello</code> will be in the working directory
You are not allowed to use commas for this script</p>

<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>8-James_Bond</code></li>
        </ul>

# 9. John Doe

 <p>Write a script that sets the mode of the file <code>hello</code> to this:</p>



<ul>
<li>The file <code>hello</code> will be in the working directory</li>
<li>You are not allowed to use commas for this script</li>
</ul>

<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>9-John_Doe</code></li>
        </ul>
      </div>

# 10. Look in the mirror
    
 <p>Write a script that sets the mode of the file <code>hello</code> the same as <code>olleh</code>’s mode.</p>

<ul>
<li>The file <code>hello</code> will be in the working directory</li>
<li>The file <code>olleh</code> will be in the working directory</li>
</ul>


<p>Note: the mode of <code>olleh</code> will not always be 664. Make sure your script works for any mode.</p>

 <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>10-mirror_permissions</code></li>
        </ul>


#  11. Directories

 <p>Create a script that adds execute permission to all subdirectories of the current directory for  the owner, the group owner and all other users. Regular files should not be changed.</p>

<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>11-directories_permissions</code></li>
        </ul>

# 12. More directories
    
     
<p>Create a script that creates a directory called <code>my_dir</code> with permissions 751 in the working directory.</p>

<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>12-directory_permissions</code></li>
        </ul>

# 13. Change group

 <p>Write a script that changes the group owner to <code>school</code> for the file <code>hello</code></p>

<ul>
<li>The file <code>hello</code> will be in the working directory</li>
</ul>


 
<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>13-change_group</code></li>
        </ul>

# 14. Owner and group
   
<p>Write a script that changes the owner to <code>vincent</code> and the group owner to <code>staff</code> for all the files and directories in the working directory.</p>

 <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>100-change_owner_and_group</code></li>
        </ul>

# 15. Symbolic links
    
 <p>Write a script that changes the owner and the group owner of <code>_hello</code> to <code>vincent</code> and <code>staff</code> respectively.</p>

<ul>
<li>The file <code>_hello</code> is in the working directory</li>
<li>The file <code>_hello</code> is a symbolic link</li>
</ul>


<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>101-symbolic_link_permissions</code></li>
        </ul>
      </div>

# 16. If only
   
      
 <p>Write a script that changes the owner of the file <code>hello</code> to <code>betty</code> only if it is owned by the user <code>guillaume</code>.</p>

<ul>
<li>The file <code>hello</code> will be in the working directory</li>
</ul>

<p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>102-if_only </code></li>
        </ul>

# 17. Star Wars

<p>Write a script that will play the StarWars IV episode in the terminal.</p>

 <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-system_engineering-devops</code></li>
            <li>Directory: <code>0x01-shell_permissions</code></li>
            <li>File: <code>103-Star_Wars</code></li>
        </ul>
