### 🧪 Lab Instructions — 3.3 Turning Commands into a Script

---

>💬 **Tip:** Paste this study guide into ChatGPT and ask for **more instructions** by specifying:  
>- “Provide step-by-step lab instructions for this objective.”  
>- “Include which Linux distro to use (Debian/Ubuntu or RHEL/Fedora).”  
>- “Show examples of installing, verifying, and managing desktop and server applications.”  
>- “Include minimal command-line practice for package management and development tools.”  
>- “Focus only on what is most important for passing the LPI Linux Essentials exam.”  

>This will prompt ChatGPT to give **practical, exam-focused lab steps** for each section.

---

**Objective:** Practice creating and running Bash scripts with variables, arguments, loops, conditionals, output, and exit status.  

**Instructions:**  

- 📁 **Create a working directory**  
  - `mkdir ~/script_lab`  
  - `cd ~/script_lab`  

- 🖊️ **Create a new script file**  
  - Use `nano myscript.sh` or `vi myscript.sh`  
  - Add shebang at the top: `#!/bin/bash`  

- 🔢 **Define variables and command substitution**  
  - Example: `NAME="Jose"`  
  - Example: `DATE=$(date)`  
  - Print: `echo "Hello $NAME, today is $DATE"`  

- 🎯 **Use script arguments**  
  - Access arguments: `$1`, `$2`  
  - Example: `echo "First argument: $1"`  
  - Run script: `./myscript.sh arg1 arg2`  

- 🔄 **Add a `for` loop**  
  - Create sample files: `touch file1.txt file2.txt file3.txt`  
  - Loop example: `for FILE in *.txt; do echo "Processing $FILE"; done`  

- 🔁 **Add a `while` loop**  
  - Example: `COUNT=1; while [ $COUNT -le 3 ]; do echo "Count: $COUNT"; COUNT=$((COUNT+1)); done`  

- ❓ **Add conditional statements (`if`)**  
  - Example: `if [ -f file1.txt ]; then echo "file1.txt exists"; fi`  

- 🗣️ **Print messages and redirect output**  
  - Simple print: `echo "Hello World"`  
  - Redirect to file: `echo "Logging output" > output.txt`  
  - Append to file: `echo "Append log" >> output.txt`  

- ✅ **Check exit status and exit script**  
  - Add: `exit 0` for success  
  - Check last command: `echo $?`  

- 🔄 **Make the script executable and run it**  
  - `chmod +x myscript.sh`  
  - `./myscript.sh arg1 arg2`  

**⚡ Tips:**  
- Test with multiple arguments and files  
- Combine loops, conditionals, variables, and `echo` for automation  
- Use command substitution for dynamic values  
- Check exit status for error handling  
- Use `nano` or `vi` efficiently for editing and debugging  
