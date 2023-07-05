<div>
<div data-react-class="projects/ProjectHeader" data-react-props="{&quot;metadata&quot;:{&quot;level&quot;:&quot;Master&quot;,&quot;author&quot;:&quot;Julien Barbier&quot;,&quot;weight&quot;:10,&quot;task_level_review_type&quot;:&quot;Your score will be updated once you launch the project review.&quot;,&quot;correction&quot;:{&quot;released&quot;:true,&quot;requires_manual_correction&quot;:true},&quot;team&quot;:{&quot;in_team_of&quot;:2}},&quot;project&quot;:{&quot;completion&quot;:0.0,&quot;id&quot;:2174,&quot;index&quot;:0,&quot;isAccessible&quot;:true,&quot;isOptional&quot;:false,&quot;imagePath&quot;:&quot;/assets/pathway/004_color-d2fbcfb42ba7481834896ecc89a6f0ae65762b3c1096691dd0f820f7f29e3389.png&quot;,&quot;name&quot;:&quot;C - Simple Shell&quot;,&quot;score&quot;:{&quot;mandatory&quot;:0.0,&quot;optional&quot;:0.0},&quot;tasksCount&quot;:16},&quot;slackLink&quot;:null,&quot;tags&quot;:[],&quot;videoRoomLink&quot;:null}" data-react-cache-id="projects/ProjectHeader-0">
<h1>C - Simple Shell</h1>
</div>
</div>
<div>
<div>
<h3>Concepts</h3>
</div>
<div>
<p><em>For this project, we expect you to look at these concepts:</em></p>
<ul>
<li><a href="https://intranet.hbtn.io/concepts/881">Approaching a Project</a></li>
<li><a href="https://intranet.hbtn.io/concepts/900">Everything you need to know to start coding your own shell</a></li>
</ul>
</div>
</div>
<div>
<div>
<h2>Background Context</h2>
<p>Write a simple UNIX command interpreter.</p>
<p><img src="https://s3.eu-west-3.amazonaws.com/hbtn.intranet.project.files/holbertonschool-low_level_programming/235/shell.jpeg" alt="" /></p>
<p><em>^ &ldquo;The Gates of Shell&rdquo;, by <a title="Spencer Cheng" href="https://intranet.hbtn.io/rltoken/CXgQbj2ybBxZeOhPsmID1g" target="_blank" rel="noopener">Spencer Cheng</a>, featuring <a title="Julien Barbier" href="https://intranet.hbtn.io/rltoken/YinaOdtW8C_NL3NlSD1Jdg" target="_blank" rel="noopener">Julien Barbier</a></em></p>
<h2>Resources</h2>
<p><strong>Read or watch</strong>:</p>
<ul>
<li><a title="Unix shell" href="https://intranet.hbtn.io/rltoken/McTQ6qvcqZZQlZtZdjdVnQ" target="_blank" rel="noopener">Unix shell</a></li>
<li><a title="Thompson shell" href="https://intranet.hbtn.io/rltoken/FLRzIA3zLln5XV7erPHgsQ" target="_blank" rel="noopener">Thompson shell</a></li>
<li><a title="Ken Thompson" href="https://intranet.hbtn.io/rltoken/Pzs_A3Wo6LTHE8WX_uKiWg" target="_blank" rel="noopener">Ken Thompson</a></li>
<li><strong>Everything you need to know to start coding your own shell</strong> concept page</li>
</ul>
<p><strong>man or help</strong>:</p>
<ul>
<li><code>sh</code> (<em>Run <code>sh</code> as well</em>)</li>
</ul>
<h2>Learning Objectives</h2>
<p>At the end of this project, you are expected to be able to <a title="explain to anyone" href="https://intranet.hbtn.io/rltoken/fmCgGY50xkpiN1RkCWnLYA" target="_blank" rel="noopener">explain to anyone</a>, <strong>without the help of Google</strong>:</p>
<h3>General</h3>
<ul>
<li>Who designed and implemented the original Unix operating system</li>
<li>Who wrote the first version of the UNIX shell</li>
<li>Who invented the B programming language (the direct predecessor to the C programming language)</li>
<li>Who is Ken Thompson</li>
<li>How does a shell work</li>
<li>What is a pid and a ppid</li>
<li>How to manipulate the environment of the current process</li>
<li>What is the difference between a function and a system call</li>
<li>How to create processes</li>
<li>What are the three prototypes of <code>main</code></li>
<li>How does the shell use the <code>PATH</code> to find the programs</li>
<li>How to execute another program with the <code>execve</code> system call</li>
<li>How to suspend the execution of a process until one of its children terminates</li>
<li>What is <code>EOF</code> / &ldquo;end-of-file&rdquo;?</li>
</ul>
<h2>Requirements</h2>
<h3>General</h3>
<ul>
<li>Allowed editors: <code>vi</code>, <code>vim</code>, <code>emacs</code></li>
<li>All your files will be compiled on Ubuntu 20.04 LTS using <code>gcc</code>, using the options <code>-Wall -Werror -Wextra -pedantic -std=gnu89</code></li>
<li>All your files should end with a new line</li>
<li>A <code>README.md</code> file, at the root of the folder of the project is mandatory</li>
<li>Your code should use the <code>Betty</code> style. It will be checked using <a title="betty-style.pl" href="https://github.com/hs-hq/Betty/blob/master/betty-style.pl" target="_blank" rel="noopener">betty-style.pl</a> and <a title="betty-doc.pl" href="https://github.com/hs-hq/Betty/blob/master/betty-doc.pl" target="_blank" rel="noopener">betty-doc.pl</a></li>
<li>Your shell should not have any memory leaks</li>
<li>No more than 5 functions per file</li>
<li>All your header files should be include guarded</li>
<li>Use system calls only when you need to (<a title="why?" href="https://intranet.hbtn.io/rltoken/rp53OodD6JzhS5Cv4DHkxQ" target="_blank" rel="noopener">why?</a>)</li>
</ul>
<h3>GitHub</h3>
<p><strong>There should be one project repository per group. If you clone/fork/whatever a project repository with the same name before the second deadline, you risk a 0% score.</strong></p>
<h2>More Info</h2>
<h3>Output</h3>
<ul>
<li>Unless specified otherwise, your program <strong>must have the exact same output</strong> as <code>sh</code> (<code>/bin/sh</code>) as well as the exact same error output.</li>
<li>The only difference is when you print an error, the name of the program must be equivalent to your <code>argv[0]</code> (See below)</li>
</ul>
<p>Example of error with <code>sh</code>:</p>
<pre><code>$ echo "qwerty" | /bin/sh
/bin/sh: 1: qwerty: not found
$ echo "qwerty" | /bin/../bin/sh
/bin/../bin/sh: 1: qwerty: not found
$
</code></pre>
<p>Same error with your program <code>hsh</code>:</p>
<pre><code>$ echo "qwerty" | ./hsh
./hsh: 1: qwerty: not found
$ echo "qwerty" | ./././hsh
./././hsh: 1: qwerty: not found
$
</code></pre>
<h3>List of allowed functions and system calls+</h3>
<ul>
<li>all functions from strings.h</li>
<li><code>access</code> (man 2 access)</li>
<li><code>chdir</code> (man 2 chdir)</li>
<li><code>close</code> (man 2 close)</li>
<li><code>closedir</code> (man 3 closedir)</li>
<li><code>execve</code> (man 2 execve)</li>
<li><code>exit</code> (man 3 exit)</li>
<li><code>_exit</code> (man 2 _exit)</li>
<li><code>fflush</code> (man 3 fflush)</li>
<li><code>fork</code> (man 2 fork)</li>
<li><code>free</code> (man 3 free)</li>
<li><code>getcwd</code> (man 3 getcwd)</li>
<li><code>getline</code> (man 3 getline)</li>
<li><code>getpid</code> (man 2 getpid)</li>
<li><code>isatty</code> (man 3 isatty)</li>
<li><code>kill</code> (man 2 kill)</li>
<li><code>malloc</code> (man 3 malloc)</li>
<li><code>open</code> (man 2 open)</li>
<li><code>opendir</code> (man 3 opendir)</li>
<li><code>perror</code> (man 3 perror)</li>
<li><code>printf</code> (man 3 printf)</li>
<li><code>fprintf</code> (man 3 fprintf)</li>
<li><code>vfprintf</code> (man 3 vfprintf)</li>
<li><code>sprintf</code> (man 3 sprintf)</li>
<li><code>putchar</code> (man 3 putchar)</li>
<li><code>read</code> (man 2 read)</li>
<li><code>readdir</code> (man 3 readdir)</li>
<li><code>signal</code> (man 2 signal)</li>
<li><code>stat</code> (__xstat) (man 2 stat)</li>
<li><code>lstat</code> (__lxstat) (man 2 lstat)</li>
<li><code>fstat</code> (__fxstat) (man 2 fstat)</li>
<li><code>strtok</code> (man 3 strtok)</li>
<li><code>wait</code> (man 2 wait)</li>
<li><code>waitpid</code> (man 2 waitpid)</li>
<li><code>wait3</code> (man 2 wait3)</li>
<li><code>wait4</code> (man 2 wait4)</li>
<li><code>write</code> (man 2 write)</li>
</ul>
<h3>Compilation</h3>
<p>Your shell will be compiled this way:</p>
<pre><code>gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
</code></pre>
<h3>Testing</h3>
<p>Your shell should work like this in interactive mode:</p>
<pre><code>$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$
</code></pre>
<p>But also in non-interactive mode:</p>
<pre><code>$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$
</code></pre>
<h3>Checks</h3>
<p>The Checker will be released at the end of the project (1-2 days before the deadline). We <strong>strongly</strong> encourage the entire class to work together to create a suite of checks covering both regular tests and edge cases for each task. See task <code>8. Test suite</code>.</p>
<p>After the deadline, you will need to fork the repository if it&rsquo;s not on your Github account to be able to be corrected by the checker.</p>
</div>
</div>
<h2>Tasks</h2>
<div data-role="task20137" data-position="0">
<div>
<div>
<h3>0. README, man, AUTHORS</h3>
<div>mandatory</div>
</div>
<div>
<ul>
<li>Write a <code>README</code></li>
<li>Write a <code>man</code> for your shell.</li>
<li>You should have an <code>AUTHORS</code> file at the root of your repository, listing all individuals having contributed content to the repository. Format, see <a title="Docker" href="https://intranet.hbtn.io/rltoken/OkJnESwrC-LyYFtCyn7Axg" target="_blank" rel="noopener">Docker</a></li>
</ul>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
<li>File: <code>README.md, man_1_simple_shell, AUTHORS</code></li>
</ul>
</div>
</div>
<div>
<div>
<div><strong>0/65 </strong>pts</div>
</div>
</div>
</div>
</div>
<div data-role="task20115" data-position="1">
<div>
<h3>1. Betty would be proud</h3>
<div>mandatory</div>
</div>
<div>
<p>Write a beautiful code that passes the Betty checks</p>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20116" data-position="2">
<div>
<h3>2. Simple shell 0.1</h3>
<div>mandatory</div>
</div>
<div>
<p>Write a UNIX command line interpreter.</p>
<ul>
<li>Usage: <code>simple_shell</code></li>
</ul>
<p>Your Shell should:</p>
<ul>
<li>Display a prompt and wait for the user to type a command. A command line always ends with a new line.</li>
<li>The prompt is displayed again each time a command has been executed.</li>
<li>The command lines are simple, no semicolons, no pipes, no redirections or any other advanced features.</li>
<li>The command lines are made only of one word. No arguments will be passed to programs.</li>
<li>If an executable cannot be found, print an error message and display the prompt again.</li>
<li>Handle errors.</li>
<li>You have to handle the &ldquo;end of file&rdquo; condition (<code>Ctrl+D</code>)</li>
</ul>
<p>You don&rsquo;t have to:</p>
<ul>
<li>use the <code>PATH</code></li>
<li>implement built-ins</li>
<li>handle special characters : <code>"</code>, <code>'</code>, <code>`</code>, <code>\</code>, <code>*</code>, <code>&amp;</code>, <code>#</code></li>
<li>be able to move the cursor</li>
<li>handle commands with arguments</li>
</ul>
<p><em><code>execve</code> will be the core part of your Shell, don&rsquo;t forget to pass the environ to it&hellip;</em></p>
<pre><code>julien@ubuntu:~/shell$ ./shell
#cisfun$ ls
./shell: No such file or directory
#cisfun$ /bin/ls
barbie_j env-main.c exec.c fork.c pid.c ppid.c prompt prompt.c shell.c stat.c wait
env-environ.c exec fork mypid ppid printenv promptc shell stat test_scripting.sh wait.c
#cisfun$ ^[[D^[[D^[[D
./shell: No such file or directory
#cisfun$ ^[[C^[[C^[[C^[[C
./shell: No such file or directory
#cisfun$ exit
./shell: No such file or directory
#cisfun$ ^C
julien@ubuntu:~/shell$ echo "/bin/ls" | ./shell
barbie_j env-main.c exec.c fork.c pid.c ppid.c prompt prompt.c shell.c stat.c wait
env-environ.c exec fork mypid ppid printenv promptc shell stat test_scripting.sh wait.c
#cisfun$ julien@ubuntu:~/shell$
</code></pre>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20118" data-position="3">
<div>
<h3>3. Simple shell 0.2</h3>
<div>mandatory</div>
</div>
<div>
<p>Simple shell 0.1 +</p>
<ul>
<li>Handle command lines with arguments</li>
</ul>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20120" data-position="4">
<div>
<h3>4. Simple shell 0.3</h3>
<div>mandatory</div>
</div>
<div>
<p>Simple shell 0.2 +</p>
<ul>
<li>Handle the <code>PATH</code></li>
<li><code>fork</code> must not be called if the command doesn&rsquo;t exist</li>
</ul>
<pre><code>julien@ubuntu:~/shell$ ./shell_0.3
:) /bin/ls
barbie_j env-main.c exec.c fork.c pid.c ppid.c prompt prompt.c shell_0.3 stat test_scripting.sh wait.c
env-environ.c exec fork mypid ppid printenv promptc shell shell.c stat.c wait
:) ls
barbie_j env-main.c exec.c fork.c pid.c ppid.c prompt prompt.c shell_0.3 stat test_scripting.sh wait.c
env-environ.c exec fork mypid ppid printenv promptc shell shell.c stat.c wait
:) ls -l /tmp
total 20
-rw------- 1 julien julien 0 Dec 5 12:09 config-err-aAMZrR
drwx------ 3 root root 4096 Dec 5 12:09 systemd-private-062a0eca7f2a44349733e78cb4abdff4-colord.service-V7DUzr
drwx------ 3 root root 4096 Dec 5 12:09 systemd-private-062a0eca7f2a44349733e78cb4abdff4-rtkit-daemon.service-ANGvoV
drwx------ 3 root root 4096 Dec 5 12:07 systemd-private-062a0eca7f2a44349733e78cb4abdff4-systemd-timesyncd.service-CdXUtH
-rw-rw-r-- 1 julien julien 0 Dec 5 12:09 unity_support_test.0
:) ^C
julien@ubuntu:~/shell$
</code></pre>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20121" data-position="5">
<div>
<h3>5. Simple shell 0.4</h3>
<div>mandatory</div>
</div>
<div>
<p>Simple shell 0.3 +</p>
<ul>
<li>Implement the <code>exit</code> built-in, that exits the shell</li>
<li>Usage: <code>exit</code></li>
<li>You don&rsquo;t have to handle any argument to the built-in <code>exit</code></li>
</ul>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20124" data-position="6">
<div>
<h3>6. Simple shell 1.0</h3>
<div>mandatory</div>
</div>
<div>
<p>Simple shell 0.4 +</p>
<ul>
<li>Implement the <code>env</code> <strong>built-in</strong>, that prints the current environment</li>
</ul>
<pre><code>julien@ubuntu:~/shell$ ./simple_shell
$ env
USER=julien
LANGUAGE=en_US
SESSION=ubuntu
COMPIZ_CONFIG_PROFILE=ubuntu
SHLVL=1
HOME=/home/julien
C_IS=Fun_:)
DESKTOP_SESSION=ubuntu
LOGNAME=julien
TERM=xterm-256color
PATH=/home/julien/bin:/home/julien/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
DISPLAY=:0
$ exit
julien@ubuntu:~/shell$
</code></pre>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20135" data-position="7">
<div>
<h3>7. What happens when you type `ls -l *.c` in the shell</h3>
<div>#advanced</div>
</div>
<div>
<p>Write a blog post describing step by step what happens when you type <code>ls -l *.c</code> and hit Enter in a shell. Try to explain every step you know of, going in as much details as you can, give examples and draw diagrams when needed. You should merge your previous knowledge of the shell with the specifics of how it works under the hoods (including syscalls).</p>
<ul>
<li>Have at least one picture, at the top of the blog post</li>
<li>Publish your blog post on Medium or LinkedIn</li>
<li>Share your blog post at least on LinkedIn</li>
<li>Only one blog post by team</li>
<li>The blog post must be done and published before the first deadline (it will be part of the manual review)</li>
<li>Please, remember that these blogs must be written in English to further your technical ability in a variety of settings</li>
</ul>
<p>When done, please add all urls below (blog post, LinkedIn post, etc.)</p>
</div>
<div>
<div>
<div>
<h4>Add URLs here:</h4>
<div><input type="text" value="" /></div>
</div>
</div>
</div>
</div>
<div data-role="task20136" data-position="8">
<div>
<h3>8. Test suite</h3>
<div>#advanced</div>
</div>
<div>
<p>Contribute to a test suite for your shell.</p>
<p>This is a task shared by everyone in the class.</p>
<ul>
<li>Every team (who contributed) will get the same score for this task (The repository owner will not get more points)</li>
<li>You have to be pro-active and agree on one and unique repository to use for the test suite</li>
<li>Please provide the link to the repository you contributed to</li>
<li>Your contribution must be relevant (Correcting typos is nice and always appreciated on the open source sphere, but we won&rsquo;t consider this a contribution at this point, <strong>unless</strong> it fixes a bug)</li>
</ul>
<p>Guidelines for your test suite repository:</p>
<ul>
<li>The test suite should cover every tasks from <code>0.</code> to <code>20.</code></li>
<li>The test suite should cover every regular cases (many different examples) and possible edge cases</li>
<li>The entire class should work on the same test suite. Use only one repository (don&rsquo;t forget the <code>README.md</code> file)</li>
<li>Start adding tests ASAP and not just before the deadline in order to help everyone from day 0</li>
<li>You can take (or fork) inspiration from <a title="this example" href="https://intranet.hbtn.io/rltoken/ot-c5zoTdjNZCggPE7b45Q" target="_blank" rel="noopener">this example</a>, but it is not mandatory to follow this format/way</li>
<li>Adopt a style and be consistent. You can, for example, follow this <a title="style guide" href="https://intranet.hbtn.io/rltoken/UyIq8BoDRLPu206oj04Nzw" target="_blank" rel="noopener">style guide</a>. If you choose a style that already exists, add it to the <code>README.md</code> in a style section. If you write your own, create a Wiki page attached to the project and refer to it in the <code>README.md</code> style section.
<ul>
<li>If you choose to use <a title="this code" href="https://intranet.hbtn.io/rltoken/ot-c5zoTdjNZCggPE7b45Q" target="_blank" rel="noopener">this code</a>, make sure to update the style accordingly</li>
</ul>
</li>
<li>You should have an <code>AUTHORS</code> file, listing all individuals having contributed content to the repository. Format, see <a title="Docker" href="https://intranet.hbtn.io/rltoken/OkJnESwrC-LyYFtCyn7Axg" target="_blank" rel="noopener">Docker</a></li>
</ul>
<p><strong>Go teams!</strong></p>
</div>
<div>
<div>
<div>
<h4>Add URLs here:</h4>
<div><input type="text" value="" /></div>
</div>
</div>
</div>
</div>
<div data-role="task20117" data-position="9">
<div>
<h3>9. Simple shell 0.1.1</h3>
<div>#advanced</div>
</div>
<div>
<p>Simple shell 0.1 +</p>
<ul>
<li>Write your own <code>getline</code> function</li>
<li>Use a buffer to read many chars at once and call the least possible the <code>read</code> system call</li>
<li>You will need to use <code>static</code> variables</li>
<li>You are not allowed to use <code>getline</code></li>
</ul>
<p>You don&rsquo;t have to:</p>
<ul>
<li>be able to move the cursor</li>
</ul>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20119" data-position="10">
<div>
<h3>10. Simple shell 0.2.1</h3>
<div>#advanced</div>
</div>
<div>
<p>Simple shell 0.2 +</p>
<ul>
<li>You are not allowed to use <code>strtok</code></li>
</ul>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20122" data-position="11">
<div>
<h3>11. Simple shell 0.4.1</h3>
<div>#advanced</div>
</div>
<div>
<p>Simple shell 0.4 +</p>
<ul>
<li>handle arguments for the built-in <code>exit</code></li>
<li>Usage: <code>exit status</code>, where <code>status</code> is an integer used to exit the shell</li>
</ul>
<pre><code>julien@ubuntu:~/shell$ ./shell_0.4.1
$ exit 98
julien@ubuntu:~/shell$ echo $?
98
julien@ubuntu:~/shell$
</code></pre>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20123" data-position="12">
<div>
<h3>12. Simple shell 0.4.2</h3>
<div>#advanced</div>
</div>
<div>
<p>Simple shell 0.4 +</p>
<ul>
<li>Handle <code>Ctrl+C</code>: your shell should not quit when the user inputs <code>^C</code></li>
</ul>
<p>man 2 <code>signal</code>.</p>
<pre><code>julien@ubuntu:~/shell$ ./shell_0.4.2
$ ^C
$ ^C
$ ^C
$ ls /var
backups cache crash lib local lock log mail metrics opt run snap spool tmp
$ ^C
$ ^C
$ ^C
$ exit
julien@ubuntu:~/shell$
</code></pre>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20125" data-position="13">
<div>
<h3>13. setenv, unsetenv</h3>
<div>#advanced</div>
</div>
<div>
<p>Simple shell 1.0 +</p>
<p>Implement the <code>setenv</code> and <code>unsetenv</code> builtin commands</p>
<ul>
<li><code>setenv</code>
<ul>
<li>Initialize a new environment variable, or modify an existing one</li>
<li>Command syntax: <code>setenv VARIABLE VALUE</code></li>
<li>Should print something on stderr on failure</li>
</ul>
</li>
<li><code>unsetenv</code>
<ul>
<li>Remove an environment variable</li>
<li>Command syntax: <code>unsetenv VARIABLE</code></li>
<li>Should print something on stderr on failure</li>
</ul>
</li>
</ul>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20126" data-position="14">
<div>
<h3>14. cd</h3>
<div>#advanced</div>
</div>
<div>
<p>Simple shell 1.0 +</p>
<p>Implement the builtin command <code>cd</code>:</p>
<ul>
<li>Changes the current directory of the process.</li>
<li>Command syntax: <code>cd [DIRECTORY]</code></li>
<li>If no argument is given to <code>cd</code> the command must be interpreted like <code>cd $HOME</code></li>
<li>You have to handle the command <code>cd -</code></li>
<li>You have to update the environment variable <code>PWD</code> when you change directory</li>
</ul>
<p><code>man chdir</code>, <code>man getcwd</code></p>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20127" data-position="15">
<div>
<h3>15. ;</h3>
<div>#advanced</div>
</div>
<div>
<p>Simple shell 1.0 +</p>
<ul>
<li>Handle the commands separator <code>;</code></li>
</ul>
<pre><code>alex@~$ ls /var ; ls /var
backups cache crash lib local lock log mail metrics opt run spool tmp
backups cache crash lib local lock log mail metrics opt run spool tmp
alex@~$ ls /hbtn ; ls /var
ls: cannot access /hbtn: No such file or directory
backups cache crash lib local lock log mail metrics opt run spool tmp
alex@~$ ls /var ; ls /hbtn
backups cache crash lib local lock log mail metrics opt run spool tmp
ls: cannot access /hbtn: No such file or directory
alex@~$ ls /var ; ls /hbtn ; ls /var ; ls /var
backups cache crash lib local lock log mail metrics opt run spool tmp
ls: cannot access /hbtn: No such file or directory
backups cache crash lib local lock log mail metrics opt run spool tmp
backups cache crash lib local lock log mail metrics opt run spool tmp
alex@~$
</code></pre>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20128" data-position="16">
<div>
<h3>16. &amp;&amp; and ||</h3>
<div>#advanced</div>
</div>
<div>
<p>Simple shell 1.0 +</p>
<ul>
<li>Handle the <code>&amp;&amp;</code> and <code>||</code> shell logical operators</li>
</ul>
<pre><code>alex@~$ ls /var &amp;&amp; ls /var
backups cache crash lib local lock log mail metrics opt run spool tmp
backups cache crash lib local lock log mail metrics opt run spool tmp
alex@~$ ls /hbtn &amp;&amp; ls /var
ls: cannot access /hbtn: No such file or directory
alex@~$ ls /var &amp;&amp; ls /var &amp;&amp; ls /var &amp;&amp; ls /hbtn
backups cache crash lib local lock log mail metrics opt run spool tmp
backups cache crash lib local lock log mail metrics opt run spool tmp
backups cache crash lib local lock log mail metrics opt run spool tmp
ls: cannot access /hbtn: No such file or directory
alex@~$ ls /var &amp;&amp; ls /var &amp;&amp; ls /var &amp;&amp; ls /hbtn &amp;&amp; ls /hbtn
backups cache crash lib local lock log mail metrics opt run spool tmp
backups cache crash lib local lock log mail metrics opt run spool tmp
backups cache crash lib local lock log mail metrics opt run spool tmp
ls: cannot access /hbtn: No such file or directory
alex@~$
alex@~$ ls /var || ls /var
backups cache crash lib local lock log mail metrics opt run spool tmp
alex@~$ ls /hbtn || ls /var
ls: cannot access /hbtn: No such file or directory
backups cache crash lib local lock log mail metrics opt run spool tmp
alex@~$ ls /hbtn || ls /hbtn || ls /hbtn || ls /var
ls: cannot access /hbtn: No such file or directory
ls: cannot access /hbtn: No such file or directory
ls: cannot access /hbtn: No such file or directory
backups cache crash lib local lock log mail metrics opt run spool tmp
alex@~$ ls /hbtn || ls /hbtn || ls /hbtn || ls /var || ls /var
ls: cannot access /hbtn: No such file or directory
ls: cannot access /hbtn: No such file or directory
ls: cannot access /hbtn: No such file or directory
backups cache crash lib local lock log mail metrics opt run spool tmp
alex@~$
</code></pre>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20129" data-position="17">
<div>
<h3>17. alias</h3>
<div>#advanced</div>
</div>
<div>
<p>Simple shell 1.0 +</p>
<ul>
<li>Implement the <code>alias</code> builtin command</li>
<li>Usage: <code>alias [name[='value'] ...]</code>
<ul>
<li><code>alias</code>: Prints a list of all aliases, one per line, in the form <code>name='value'</code></li>
<li><code>alias name [name2 ...]</code>: Prints the aliases <code>name</code>, <code>name2</code>, etc 1 per line, in the form <code>name='value'</code></li>
<li><code>alias name='value' [...]</code>: Defines an alias for each <code>name</code> whose <code>value</code> is given. If <code>name</code> is already an alias, replaces its value with <code>value</code></li>
</ul>
</li>
</ul>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20130" data-position="18">
<div>
<h3>18. Variables</h3>
<div>#advanced</div>
</div>
<div>
<p>Simple shell 1.0 +</p>
<ul>
<li>Handle variables replacement</li>
<li>Handle the <code>$?</code> variable</li>
<li>Handle the <code>$$</code> variable</li>
</ul>
<pre><code>julien@ubuntu:~/shell$ ./hsh
$ ls /var
backups cache crash lib local lock log mail metrics opt run snap spool tmp
$ echo $?
0
$ echo $$
5104
$ echo $PATH
/home/julien/bin:/home/julien/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
$ exit
julien@ubuntu:~/shell$
</code></pre>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20131" data-position="19">
<div>
<h3>19. Comments</h3>
<div>#advanced</div>
</div>
<div>
<p>Simple shell 1.0 +</p>
<ul>
<li>Handle comments (<code>#</code>)</li>
</ul>
<pre><code>julien@ubuntu:~/shell$ sh
$ echo $$ # ls -la
5114
$ exit
julien@ubuntu:~/shell$
</code></pre>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20132" data-position="20">
<div>
<h3>20. help</h3>
<div>#advanced</div>
</div>
<div>
<p>Simple shell 1.0 +</p>
<ul>
<li>Implement the <code>help</code> built-in</li>
<li>Usage: <code>help [BUILTIN]</code></li>
</ul>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20133" data-position="21">
<div>
<h3>21. history</h3>
<div>#advanced</div>
</div>
<div>
<p>Simple shell 1.0 +</p>
<ul>
<li>Implement the history built-in, without any argument</li>
<li>The <code>history</code> built-in displays the history list, one command by line, preceded with line numbers (starting at <code>0</code>)</li>
<li>On <code>exit</code>, write the entire history, without line numbers, to a file named <code>.simple_shell_history</code> in the directory <code>$HOME</code></li>
<li>When the shell starts, read the file <code>.simple_shell_history</code> in the directory <code>$HOME</code> if it exists, and set the first line number to the total number of lines in the file modulo <code>4096</code></li>
</ul>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
<div data-role="task20134" data-position="22">
<div>
<div>
<h3>22. File as input</h3>
<div>#advanced</div>
</div>
<div>
<p>Simple shell 1.0 +</p>
<ul>
<li>Usage: <code>simple_shell [filename]</code></li>
<li>Your shell can take a file as a command line argument</li>
<li>The file contains all the commands that your shell should run before exiting</li>
<li>The file should contain one command per line</li>
<li>In this mode, the shell should not print a prompt and should not read from <code>stdin</code></li>
</ul>
</div>
<div>
<div>
<p><strong>Repo:</strong></p>
<ul>
<li>GitHub repository: <code>holbertonschool-simple_shell</code></li>
</ul>
</div>
</div>
</div>
</div>