## System resources monitoring

### CPU
- Install stress
- Look at CPU info
- Stress CPU. Send it to background.
- Look at CPU and memory resources. Observe CPU usage, observe load.
- Can you identify the background jobs linked to your shell
- Bring the process back to foreground and kill it
- Look at load again
- In a multi-user system, you can leverage "w" command to display CPU time per session

### Memory
- Check memory
- Stress memory this time
- Check memory usage again
- Identify process
- Kill process forcefully
- Apply more stress on memory this time
- What is happening? Why? How to make system more tolerant with you?
- Start stress again
- Identify OOM issues
- How to get swap information? what is swap? How to trace PID?

### Network
- You already netstat or ss to show current connections and listening ports
- Install nload and iftop
- Open nload in another shell (use Mbps and MB for total)
- Open iftop in another shell and display port info
- Stress network 
- Watch established connections
- Tracing PID 
- Alternatively test iptraf as well

### Disks
- Install iotop
If you need to enable CONFIG_TASK_DELAY_ACCT you'll probably have to recompile the kernel or activate the setting at boot
- Look at partitions
- Launch stress command 
- With iotop look at the process
- With iostat look for stats, try -xtc. What does it do? What are the different columns?
- vmstat command can also be used to gather some information, look at -D, -d and -p (partition)


### Resource monitoring 
- Check out sar, activate metric collection
- Find out how to look at open files. Is there a limit?
-Other useful commands to debug daemons (diagnostic message, journal)


