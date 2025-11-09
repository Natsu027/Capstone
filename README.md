🧑‍💻 Custom Shell Implementation (Linux OS)
📘 Overview

This project is a custom shell built in C++ that mimics basic Unix shell functionalities.
It can execute commands, manage processes, support redirection, handle piping, and manage background jobs.

🎯 Objective

To build a lightweight command-line shell in C++ capable of:

Executing system commands

Managing processes (foreground/background)

Handling I/O redirection (>, <, 2>)

Supporting piping (|) between commands

Maintaining a command history

Implementing basic job control

🗓️ Day-wise Progress
Day	Task
Day 1	Planned shell features and implemented command parsing
Day 2	Added execution of basic commands using fork() and execvp()
Day 3	Integrated process management (foreground & background)
Day 4	Implemented piping (`
Day 5	Added job control and command history support
⚙️ Features

✅ Execute standard Linux commands (ls, pwd, cat, etc.)
✅ Support for background execution using &
✅ Input (<), output (>) and error (2>) redirection
✅ Command history with:

history → shows last 10 commands

!! → repeats last command

!N → repeats Nth command from history
✅ Supports multiple piped commands
✅ Built-in commands:

cd <dir> → change directory

mkfifo <name> → create named pipe

🧩 Technologies Used

Language: C++

System Calls: fork(), execvp(), waitpid(), pipe(), dup2(), open()

Environment: Linux / Ubuntu terminal
▶️ Compilation & Execution
1. Compile
g++ shell.cpp -o myshell

2. Run
./myshell

3. Exit

Type:

exit

📂 Example Commands
ls -l
pwd
cat file.txt > output.txt
cat < input.txt | grep keyword > result.txt
mkfifo pipe1
ls &       # Run in background
history
!!         # Repeat last command
!3         # Repeat 3rd command from history

🖼️ Screenshots

Shell compilation and execution output

Demonstration of history, background execution, and piping

🧠 Future Improvements

Add command auto-completion

Implement signal handling (Ctrl+C, Ctrl+Z)

Extend quoting and string parsing

Maintain a job table for suspended and running background processes

🏁 Author

Mohit Kumar
B.Tech CSE, 4th Year
Linux Operating Systems Assignment – Custom Shell Implementation
