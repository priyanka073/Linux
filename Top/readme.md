## TOP

top command is used to show the Linux processes. It provides a dynamic real-time view of the running system. Usually, this command shows the summary information of the system and the list of processes or threads which are currently managed by the Linux Kernel. As soon as you will run this command it will open an interactive command mode where the top half portion will contain the statistics of processes and resource usage. And Lower half contains a list of the currently running processes. Pressing q will simply exit the command mode.

In simple words : it show a real time view of running process in linux and display kernel-managed tasks
It also provide a system information summary that shows resource utilization, including CPU and Memory Usage.

- PID: Shows task’s unique process id.
- PR: The process’s priority. The lower the number, the higher the priority.
- VIRT: Total virtual memory used by the task.
- USER: User name of owner of task.
- %CPU: Represents the CPU usage.
- TIME+: CPU Time, the same as ‘TIME’, but reflecting more granularity through hundredths of a second.
- SHR: Represents the Shared Memory size (kb) used by a task.
- NI: Represents a Nice Value of task. A Negative nice value implies higher priority, and positive Nice value means lower priority.
- %MEM: Shows the Memory usage of task.
- RES: How much physical RAM the process is using, measured in kilobytes.
- COMMAND: The name of the command that started the process.



## Options of Top Command
### Options	Description
- -a	This option is used to solve the processes according to the allocated memory.
- -b	It begins the top command in batch mode, which can be helpful in sending results from the top command to other files and programs.
- -c	It begins the top command with the last remembered state reversed 'c'.
- -d	It shows the delay between the screen updates and then overrides the associated value in the startup default or personal configuration file of one.
- -h	It shows the usage prompt and library version, then quit.
- -H	It begins a top command with the last remembered state reversed 'H'.
- -i	It begins a top command with the last remembered state reversed i.
- -m	It reports USED (rss process sum and swap count) rather than VIRT.
- -M	It shows memory units and displays floating point values within the memory summary.
- -n	It describes the maximum number of frames or iterations; the top command should generate before completion.
- -p	It only monitors processes with process IDs.
- -s	It is far better managed from the system configuration file.
- -S	All processes are listed using the CPU time that it and its dead children have utilized when "Cumulative mode" is active.
- -U	It only monitors processes with an effective username or UID matching that provided one. It matches saved, effective, real file system UIDs.
- -u	It only monitors processes with an effective username or UID matching that provided one.
- -v	It shows the usage prompt and library version, then quit.

## Sorting top output

By default, top command always display output in the order of CPU usage.
Example : After execute the top command follow options
- Press M - To display in order of memory usage.
- Press R - To display in reverse order.