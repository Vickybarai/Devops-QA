

Linux DevOps Interview Questions — Module-wise, Level & Sequence


---

🟩 MODULE 1: Linux Fundamentals (Core Concepts) — Easy / 100–90% ask rate

1. What is Linux? Difference between Linux, UNIX, and Windows?


2. Explain Linux architecture (Kernel, Shell, User space).


3. What happens when you type a command and press Enter?


4. What are environment variables? How to view/set them?


5. What are absolute vs relative paths?


6. Explain Linux directory structure (/, /bin, /etc, /home, /var).


7. What are the types of shells in Linux?


8. What is the difference between shell and kernel?


9. Explain file system hierarchy — where are configs, binaries, and logs kept?


10. What is the difference between /root and /home directories?


11. What is a Linux Kernel? Why is it important?


12. What is a shell in Linux, and how is it different from bash?


13. Basic components of Linux OS


14. What is the init process in Linux?


15. What is root?


16. Check hostname


17. Check current user


18. Check current working directory




---

🟨 MODULE 2: File Management & Permissions — Easy–Moderate / 95–85% ask rate

19. What are file permissions (rwx)? Explain chmod 755 vs 777.


20. Types of permissions (Read, Write, Execute)


21. What is the difference between a Soft Link and a Hard Link?


22. How do you change file ownership and group (chown, chgrp)?


23. What is umask? What does it control?


24. What is the sticky bit and where is it used (/tmp example)?


25. What are /etc/passwd, /etc/shadow, and /etc/group used for?


26. What is the difference between su and sudo?


27. How do you safely edit the sudoers file (visudo)?


28. How do you find recently modified files (find -mtime)?


29. What are hidden files, and how to view them (ls -a)?


30. Change file permissions using chmod


31. Permissions to execute a script


32. Create/manage symbolic links




---

🟧 MODULE 3: Process & System Management — Moderate / 100–90% ask rate

33. What is a process?


34. Difference between process and thread.


35. Explain ps, top, and htop commands.


36. What is a Zombie process and how do you handle it?


37. Difference between kill and kill -9


38. How do you run a process in the background (&, nohup, screen)?


39. What is the purpose of nice and renice?


40. How to check which process is consuming the most CPU/memory?


41. What is load average? Interpret uptime output.


42. Explain swap memory and when it’s used.


43. Check running processes


44. Terminate process




---

🟦 MODULE 4: Disk, Filesystem & Storage — Moderate / 95–85% ask rate

45. How do you check disk usage (df, du)?


46. “No space left on device” but disk has space — what’s the issue (inodes)?


47. What is the difference between disk full vs inode full?


48. How do you check disk partitions (lsblk, fdisk -l)?


49. What is /etc/fstab and its purpose?


50. How do you check if a disk is mounted?


51. How to mount/unmount file systems manually?


52. What is LVM? Advantages of using it?


53. Difference between ext4, xfs, and btrfs.


54. How to find which directory is using the most space?


55. Read first or last N lines of a file (head, tail)


56. Combine two files (cat file1 file2 > file3)


57. Find file type


58. Sort file content




---

🟫 MODULE 5: Networking & Connectivity — Moderate / 90–80% ask rate

59. How do you check which ports are listening (netstat, ss, lsof)?


60. How to check if a remote server is reachable on a port (telnet, nc)?


61. What is the SSH config file location?


62. How do SSH keys work? (Public/private key auth)


63. What is the difference between curl and wget?


64. How do you check and restart the network service?


65. Explain /etc/hosts and /etc/resolv.conf.


66. How do you add a static route temporarily and permanently?


67. What is the 3-way TCP handshake?


68. How to check DNS resolution issues?


69. Check IP/Server accessibility (ping IP_address)


70. Get info about ports (netstat -l)


71. Check specific open port (netstat -putan | grep port_number)


72. Check network interfaces (ifconfig or netstat)


73. Telnet vs SSH




---

🟥 MODULE 6: Service, Boot & Systemctl — Intermediate / 85–75% ask rate

74. Explain Linux boot process (BIOS → GRUB → Kernel → Init → Systemd)


75. What are systemd targets (runlevels)?


76. Difference between systemctl and service commands


77. How to check the status of a service?


78. How to debug a failed service (systemctl status, journalctl)?


79. How to enable/disable services at boot?


80. What is /etc/systemd/system used for?


81. How to create your own custom systemd service?


82. What is journald, and how to filter logs?


83. What is log rotation, and how does logrotate work?


84. Daemon service


85. Check service status


86. Start/Stop service




---

🟪 MODULE 7: Security, Users & Access — Intermediate / 80–70% ask rate

87. How do you add or delete users/groups?


88. How to lock or expire a user account?


89. How to add a user to sudoers?


90. What is SELinux/AppArmor, and how to check status?


91. How to check and set password aging policy?


92. What is chattr and how to make a file immutable?


93. How to secure SSH access (key-only login, disable root, etc.)?


94. What is fail2ban?


95. What is setuid, setgid, and sticky bit?


96. How do you check open file descriptor limits (ulimit)?




---

🟨 MODULE 8: Scheduling & Automation — Easy / 80–70% ask rate

97. How to schedule tasks using cron?


98. Difference between cron and at?


99. How to list existing cron jobs (crontab -l)?


100. How to schedule a backup script daily?


101. What is the difference between cron and systemd timers?


102. How to debug a failed cron job?


103. How to use sleep, watch, or loops for repetition?


104. Automate tasks/scripts (cron/at)


105. Check scheduled cron jobs


106. Cron job format


107. Troubleshoot cron job




---

🟩 MODULE 9: Shell Scripting (Essential for DevOps) — Intermediate / 75–65% ask rate

108. How to pass arguments to a shell script?


109. Difference between $, $@, "$" and "$@"


110. How do you check command exit status ($?)?


111. What are set -e, set -u, set -o pipefail used for?


112. Write a script to monitor disk usage > 80%


113. How to run background jobs in a script and capture their PID?


114. How to log script output with timestamps?


115. How to read a config file line by line in bash?




---

🟦 MODULE 10: Troubleshooting & Scenarios — Moderate–High / 100–90% ask rate

116. “Server is slow.” How do you investigate?


117. “Disk is full.” How do you find and fix the issue?


118. “Service is not starting.” How do you debug?


119. “Can’t connect to port 80.” How to troubleshoot step-by-step?


120. “Website is loading slowly.” How to debug performance?


121. “SSH login is delayed.” How do you fix it?


122. “High load average but CPU idle.” What could cause it?


123. “Memory usage is high.” How do you find the culprit?


124. “Logs not updating.” How do you check permissions and rotation?


125. “Cron job didn’t run.” How do you debug?
--- 


DevOps & Cloud Computing
Professional Task List

Section 1: Theory & Concepts
1 Write and learn all major network ports used in DevOps (SSH, HTTP, HTTPS, FTP, SMTP,
DNS, MySQL, PostgreSQL, Docker, Kubernetes, etc.).
2 Explore Domain Name System (DNS) and its records (A, AAAA, CNAME, MX, NS, TXT,
PTR).
3 Explore Network Load Balancer (NLB) and Application Load Balancer (ALB) with use cases.
4 Explore HTTP methods, path-based hosting, name-based hosting, and HTTP status codes.
5 Explore Warm Pool concept in an Auto Scaling Group (ASG).
6 Understand the difference between IAM Policies and IAM Roles.
7 Explore Object Storage and Block Storage with real-world examples.
8 Explore Amazon RDS and Log Rotation concepts.
9 Explore Cross-account S3 bucket sharing mechanism.
Section 2: Practical / Hands-on Tasks
1 Host a static website on an EC2 instance with HTTPS (Port 443).
2 Create and configure a MariaDB server.
3 Host a Java-based Student Management Application.
4 Host a PHP-based Ticket Booking Application using LAMP stack.
5 Host a WordPress website.
6 Create three EC2 instances: nfs1, nfs2, webserver.
7 Configure NFS on nfs1 and nfs2.
8 Install Apache2 on webserver.
9 Store website data on NFS storage.
10 Serve website on port 8080.
11 Expose application using Load Balancer mapping 8080 to 80.
12 Install AWS CLI on local computer.
13 Host static website on Amazon S3.
14 Create and test S3 lifecycle policies.
15 Design and deploy Three-Tier Architecture.
16 Create Hosted Zone in Route 53.
17 Create IAM user with EC2 access in Mumbai region.
18 Write SOP for Git branching strategy.
19 Apply Markdown formatting with author name and image.
20 Host static website in Docker container.
21 Create Dockerfile.
22 Create docker-compose file and deploy application.
23 Maintain document of all tool versions.
Section 3: Interview Preparation
1 Explain S3 Storage Classes and Lifecycle Policies.
2 Explain Load Balancer in Cloud.
3 Explain Auto Scaling Group.
4 Explain IAM Service.
5 Explain EC2 Instance Types.
6 Explain NAT Gateway in VPC.
7 Difference between NAT Gateway vs NAT Instance.
8 Explain VPC Peering.
9 Difference between NACL vs Security Group.
10 Difference between IAM Roles vs IAM Policies.

