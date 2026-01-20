# Session - 01 - Linux Basics

## Start Ubuntu Instance

```bash
podman machine start
podman attach magical_chebyshev
```

---

## Linux Commands

### List all files under root directory

```bash
ls -R /
```

* `-R` means traverse directories recursively starting from `/`.

---

### List only directories

```bash
ls -d */
```

* `-d` lists directories themselves, not their contents.
* `*/` is a regular expression matching directories.

---

### List only files

```bash
ls -p | grep -v /
```

* `-p` appends `/` to directory names.
* `grep -v /` removes directory entries, leaving only files.

---

### List only hidden files

```bash
ls -a | grep "^\."
```

* Hidden files start with `.`.
* `ls -a` includes hidden files, `grep` filters them.

---

### List tree structure of all files

```bash
tree /
```

* Recursively prints a hierarchical filesystem structure.

---

### Understand file attributes

```bash
ls -l
```

* Displays permissions, ownership, size, and timestamps from inode metadata.

---

### Create a file and change attributes

```bash
touch demo.txt
chmod 755 demo.txt
```

* `touch` creates an empty file.
* `chmod` modifies permission bits.

---

## Shell Scripting Tasks

### Create a directory

```bash
mkdir script_set_01
```

---

### Create a shell script for each command

Each script should:

* Run one command
* Redirect output to `out.txt`

Example:

```bash
#!/bin/bash
ls / > out.txt
```

Make it executable and run:

```bash
chmod +x script.sh
./script.sh
```

* Execute permission allows the kernel to run the script via the shebang interpreter.

---

### Copy all scripts to another directory

```bash
mkdir script_set_02
cp script_set_01/* script_set_02/
```

---

### Delete all output files

```bash
rm *out*
```

* Removes files matching the pattern.

---

### Enhance tree script to accept output filename

```bash
tree / > "$1"
```

Run the script as:

```bash
./tree.sh tree_out.txt
```

* `$1` is a positional parameter for runtime arguments.

---

## Calendar Command

```bash
cal
```

* Comes from `util-linux`.

If not available:

```bash
unminimize
```

Or use alternative:

```bash
apt install ncal
ncal        # current month
ncal -y     # whole year
ncal 2025   # specific year
```

Use `man` to study parameters:

```bash
man cal
man ncal
```

---

## Network Commands

### Find IP address

```bash
ip a
```

* Queries kernel networking stack via netlink.

> `ifconfig` is legacy and uses older kernel APIs.

---

### WiFi Hotspot Test

* Not supported in container-based Linux setups.

---

### Ping commands

```bash
ping google.com
```

* ICMP echo requests (blocked in containers).
* Alternative:

```bash
nslookup google.com
```

Ping a friend on the same WiFi:

```bash
ping 192.168.11.68
```

* Local network pings are faster due to fewer hops.

---

### Trace network route

```bash
traceroute google.com
traceroute facebook.com
```

* Maps network path hop-by-hop using TTL.
* Some hops may be hidden for security reasons.

---

## Command History

```bash
history
history | grep ping
```

* Reads shell history and filters using patterns.

---

## List TCP and UDP Connections

```bash
ss -tuln
```

* Displays active TCP/UDP sockets from kernel tables.

Use:

```bash
man ss
```

---

## System Information

```bash
uname -a > system_info.txt
lscpu >> system_info.txt
```

* Queries kernel and CPU information.
* Output redirected to file.

---

## Locate Executable Files

```bash
which mkdir
whereis mkdir
```

Results:

* `mkdir` → `/usr/bin/mkdir`
* `cp` → `/usr/bin/cp`
* `link` → `/usr/bin/link`
* `cd` → Shell built-in (not a binary)

---

## Archive Files

```bash
tar -cvf files.tar script_set_01 script_set_02
```

Extract friend’s archive:

```bash
tar -xvf friend.tar -C friend_name/
```

---

## Process Management

Find Chrome PID:

```bash
ps aux | grep chrome
```

Terminate Chrome:

```bash
kill -9 PID
```

---

## Shutdown and Restart

```bash
shutdown now
reboot
```

For containers:

```bash
podman restart magical_chebyshev
```

---

## Welcome Script

### Create script

```bash
echo "Welcome Divyanshu’s Session" > welcome.sh
chmod +x welcome.sh
mv welcome.sh /usr/local/bin/
```

Run from anywhere:

```bash
welcome.sh
```

* `/usr/local/bin` is in `$PATH`.

---

### Run script on terminal startup

Edit bash config:

```bash
vi ~/.bashrc
```

Add at the end:

```bash
/usr/local/bin/welcome.sh
```

Save and exit with `:wq`.

---

## Tools & Practice

* Install **VS Code** (script editing & JSON formatting)
* **GitHub Signup** (version control)
* Practice **cURL**
* Signup/Login to **Postman**

Collection:

```
https://www.postman.com/cs-demo/public-rest-apis/collection/tfzpqfc/public-rest-apis
```

Run APIs on Postman Web → Get cURL → Run in terminal:

```bash
curl https://api.publicapis.org/entries
curl https://api.publicapis.org/entries > response.json
```

* Save response and format JSON using VS Code.

---

## Additional Resources

* The Origins of Linux — Linus Torvalds
* AT&T Archives: The UNIX Operating System
* *Code Rush: The Early Days of Netscape & Mozilla* (2000)
* [https://www.hostinger.com/tutorials/linux-commands](https://www.hostinger.com/tutorials/linux-commands)
* [https://buildmedia.readthedocs.org/media/pdf/lym/latest/lym.pdf](https://buildmedia.readthedocs.org/media/pdf/lym/latest/lym.pdf)
* [https://www.jetbrains.com/go/download/#section=linux](https://www.jetbrains.com/go/download/#section=linux)
* [https://code.visualstudio.com/](https://code.visualstudio.com/)
* [https://github.com](https://github.com)


