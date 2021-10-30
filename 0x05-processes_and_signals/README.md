0x05. Processes and signals

File: 0-what-is-my-pid:

Write a Bash script that displays its own PID.

sylvain@ubuntu$ ./0-what-is-my-pid
4120
sylvain@ubuntu$

1-list_your_processes:

Write a Bash script that displays a list of currently running processes.

Requirements:

Must show all processes, for all users, including those which might not have a TTY
Display in a user-oriented format
Show process hierarchy.

File: 2-show_your_bash_pid:

Using your previous exercise command, write a Bash script that displays lines containing the bash word, thus allowing you to easily get the PID of your Bash process.

Requirements:

You cannot use pgrep
The third line of your script must be # shellcheck disable=SC2009 (for more info about ignoring shellcheck error here).


File: 3-show_your_bash_pid_made_easy:

Write a Bash script that displays the PID, along with the process name, of processes whose name contain the word bash.

Requirements:

You cannot use ps
sylvain@ubuntu$ ./3-show_your_bash_pid_made_easy
4404 bash
4555 bash
sylvain@ubuntu$ ./3-show_your_bash_pid_made_easy
4404 bash
4557 bash
sylvain@ubuntu$ 
Here we can see that:

For the first iteration: bash PID is 4404 and that the 3-show_your_bash_pid_made_easy script PID is 4555
For the second iteration: bash PID is 4404 and that the 3-show_your_bash_pid_made_easy script PID is 4557.


4-to_infinity_and_beyond:

Write a Bash script that displays To infinity and beyond indefinitely.

Requirements:

In between each iteration of the loop, add a sleep 2
sylvain@ubuntu$ ./4-to_infinity_and_beyond
To infinity and beyond
To infinity and beyond
To infinity and beyond
To infinity and beyond
To infinity and beyond
^C
sylvain@ubuntu$ 
Note that I ctrl+c (killed) the Bash script in the example.

File: 5-dont_stop_me_now:

We stopped our 4-to_infinity_and_beyond process using ctrl+c in the previous task, there is actually another way to do this.

Write a Bash script that stops 4-to_infinity_and_beyond process.

Requirements:

You must use kill.


6-stop_me_if_you_can:

Write a Bash script that stops 4-to_infinity_and_beyond process.

Requirements:

You cannot use kill or killall.


File: 7-highlander:

Write a Bash script that displays:

To infinity and beyond indefinitely
With a sleep 2 in between each iteration
I am invincible!!! when receiving a SIGTERM signal
Make a copy of your 6-stop_me_if_you_can script, name it 67-stop_me_if_you_can, that kills the 7-highlander process instead of the 4-to_infinity_and_beyond one.

File: 8-beheaded_process:

Write a Bash script that kills the process 7-highlander.