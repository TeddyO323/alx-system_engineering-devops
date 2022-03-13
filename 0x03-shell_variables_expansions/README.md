

# About Bash Projects
<p><strong>Read or watch</strong>:</p>

<ul>
<li><a href="http://linuxcommand.org/lc3_lts0080.php" title="Expansions" target="_blank">Expansions</a> </li>
<li><a href="https://www.gnu.org/software/bash/manual/html_node/Shell-Arithmetic.html" title="Shell Arithmetic" target="_blank">Shell Arithmetic</a> </li>
<li><a href="https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_03_02.html" title="Variables" target="_blank">Variables</a> </li>
<li><a href="https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_03_01.html" title="Shell initialization files" target="_blank">Shell initialization files</a> </li>
<li><a href="http://www.linfo.org/alias.html" title="The alias Command" target="_blank">The alias Command</a> </li>
<li><a href="https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/misc/2021/6/9112669886fd446a2aa3113c31319d1f468dc160.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20220308%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220308T063450Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=4bf67682f4ee9f03051dae63f3c0e2d8d435dd8f508e63b35c39f73d1fb13d7a" title="Technical Writing" target="_blank">Technical Writing</a></li>
</ul>

<p><strong>man or help</strong>:</p>

<ul>
<li><code>printenv</code></li>
<li><code>set</code></li>
<li><code>unset</code></li>
<li><code>export</code></li>
<li><code>alias</code></li>
<li><code>unalias</code></li>
<li><code>.</code></li>
<li><code>source</code></li>
<li><code>printf</code></li>
</ul>

<h2>Learning Objectives</h2>

<p>At the end of this project, you are expected to be able to <a href="https://fs.blog/feynman-learning-technique/?fbclid=IwAR2K5_BGPVo0QjJXkOIIqNsqcXK4lTskPWJvA0asKQIGtCPWaQBdKmj1Ztg" title="explain to anyone" target="_blank">explain to anyone</a>, <strong>without the help of Google</strong>:</p>

<h3>General</h3>

<ul>
<li>What happens when you type <code>$ ls -l *.txt</code></li>
</ul>

<h3>Shell Initialization Files</h3>

<ul>
<li>What are the <code>/etc/profile</code> file and the <code>/etc/profile.d</code> directory</li>
<li>What is the <code>~/.bashrc</code> file</li>
</ul>

<h3>Variables</h3>

<ul>
<li>What is the difference between a local and a global variable</li>
<li>What is a reserved variable</li>
<li>How to create, update and delete shell variables</li>
<li>What are the roles of the following reserved variables: HOME, PATH, PS1</li>
<li>What are special parameters</li>
<li>What is the special parameter <code>$?</code>?</li>
</ul>

<h3>Expansions</h3>

<ul>
<li>What is expansion and how to use them</li>
<li>What is the difference between single and double quotes and how to use them properly</li>
<li>How to do command substitution with <code>$()</code> and backticks</li>
</ul>

<h3>Shell Arithmetic</h3>

<ul>
<li>How to perform arithmetic operations with the shell</li>
</ul>

<h3>The <code>alias</code> Command</h3>

<ul>
<li>How to create an alias</li>
<li>How to list aliases</li>
<li>How to temporarily disable an alias</li>
</ul>

<h3>Other <code>help</code> pages</h3>

<ul>
<li>How to execute commands from a file in the current shell</li>
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
<li>You are not allowed to use <code>&amp;&amp;</code>, <code>||</code> or <code>;</code></li>
<li>You are not allowed to use <code>bc</code>, <code>sed</code> or <code>awk</code></li>
<li>All your files must be executable</li>
</ul>

<h2>More Info</h2>

<p>Read your <code>/etc/profile</code>, <code>/etc/inputrc</code> and <code>~/.bashrc</code> files.</p>

<p>Look at some files in the <code>/etc/profile.d</code> directory.</p>

<p>Note: You do not have to learn about <code>awk</code>, <code>tar</code>, <code>bzip2</code>, <code>date</code>, <code>scp</code>, <code>ulimit</code>, <code>umask</code>, or shell scripting, yet.</p>

</div>

---

# TASKS

# 0. < o >

Create a script that creates an alias.

- Name: ls
- Value: rm *

**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 0-alias
  
# 1. Hello you

Create a script that prints hello user, where user is the current Linux user.


**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 1-hello_you
  
# 2. The path to success is to take massive, determined action

Add <code>/action</code> to the <code>PATH</code>. <code>/action</code> should be the last directory the shell looks into when looking for a program.


**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 2-path
  
# 3. If the path be beautiful, let us not ask where it leads

Create a script that counts the number of directories in the PATH.

**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 3-paths
  
# 4. Global variables

Create a script that lists environment variables.


**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 4-global_variables
  
# 5. Local variables

Create a script that lists all local variables and environment variables, and functions.


**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 5-local_variables
  
# 6. Local variable

Create a script that creates a new local variable.

- Name: BEST-
- Value: School
**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 6-create_local_variable
  
# 7. Global variable

Create a script that creates a new global variable.

- Name: BEST
- Value: School
**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 7-create_global_variable
  
# 8. Every addition to true knowledge is an addition to human power

Write a script that prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line.

**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 8-true_knowledge
  
# 9. Divide and rule

Write a script that prints the result of POWER divided by DIVIDE, followed by a new line.

- POWER and DIVIDE are environment variables

**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 9-divide_and_rule
  
# 10. Love is anterior to life, posterior to death, initial of creation, and the exponent of breath

Write a script that displays the result of BREATH to the power LOVE

- BREATH and LOVE are environment variables
- The script should display the result, followed by a new line

**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 10-love_exponent_breath
  
# 11. There are 10 types of people in the world -- Those who understand binary, and those who don't

Write a script that converts a number from base 2 to base 10.

- The number in base 2 is stored in the environment variable BINARY
- The script should display the number in base 10, followed by a new line

**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 11-binary_to_decimal
  
# 12. Combination

Create a script that prints all possible combinations of two letters, except oo.

- Letters are lower cases, from a to z
- One combination per line
- The output should be alpha ordered, starting with aa
- Do not print oo
- Your script file should contain maximum 64 characters

**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 12-combinations
  
# 13. Floats

Write a script that prints a number with two decimal places, followed by a new line.

- The number will be stored in the environment variable NUM.


**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 13-print_float
  
# 14. Decimal to Hexadecimal

Write a script that converts a number from base 10 to base 16.

- The number in base 10 is stored in the environment variable DECIMAL
- The script should display the number in base 16, followed by a new line

**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 100-decimal_to_hexadecimal
  
# 15. Everyone is a proponent of strong encryption

**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 101-rot13
  
# 16. The eggs of the brood need to be an odd number

Write a script that prints every other line from the input, starting with the first line.

**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 102-odd
  
# 17. I'm an instant star. Just add water and stir.

Write a shell script that adds the two numbers stored in the environment variables WATER and STIR and prints the result.

- WATER is in base water
- STIR is in base stir.
- The result should be in base bestchol

**Repo:**

- GitHub repository: alx-system_engineering-devops
- Directory: 0x03-shell_variables_expansions
- File: 103-water_and_stir
