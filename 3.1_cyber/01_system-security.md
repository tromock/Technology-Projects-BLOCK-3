# Exploring Your System's Security

## Task 1 --- List System Users

Run:

    cat /etc/passwd

### Screenshot

(Add screenshot here)

### Questions

1.  How many users exist on the system? - 37 users
2.  Which accounts appear to be system accounts? - 2 accounts
3.  Why do operating systems create system accounts? - to manage and control

### Reflection

Explain why understanding system users is important for cybersecurity.

------------------------------------------------------------------------

## Task 2 --- Inspect Running Processes

Run:

    ps aux

### Screenshot

(Add screenshot here)

### Questions

1.  Which processes are running as `root`? - 108 root
2.  Why can processes running as root be dangerous? - because root is the most powerful account on a Linux
3.  What could happen if a malicious program ran with root privileges? - it could damage the system by controlling the whole raspberry pi system

### Reflection

What did you learn about system processes and security?

------------------------------------------------------------------------

## Task 3 --- Identify Open Network Ports

Run:

    ss -tuln

### Screenshot

(Add screenshot here)

### Questions

1.  Which ports are open? - TCP ports and UDP ports are open
2.  Which services appear to be listening? - tcp ports
3.  Why might open ports represent a security risk? - they provide potential entry points

### Reflection

Explain the relationship between open ports and potential attack
surfaces.
