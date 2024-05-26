#### What is Screen
In Linux, the screen command is used to multiplex your terminal, allowing you to manage multiple windows or sessions within a single terminal window. The screen command is commonly employed for tasks such as managing long-running processes, maintaining connections during remote access, or running multiple tasks simultaneously.

Here are some basic examples of using the screen command:
1- Start a New Screen Session:
```bash
screen
```
This command initiates a new screen session.

2- Detach from the Screen Session:
You can detach from a Screen session using the combination Ctrl + A, followed by D.


```bash
Ctrl + A, D
```
3- List Running Screen Sessions:

```bash
screen -ls
```
4- Reattach to an Existing Session:

```bash
screen -r
```
or

```bash
screen -r <session-id>
screen -ls # You can reconnect to a specific session using the session IDs or names
```

5- Create a New Window:
To create a new window, you can use the combination Ctrl + A, followed by C.

```bash
Ctrl + A, C
```
6- Switch Between Windows:
You can switch between windows using the combination Ctrl + A, followed by N (next window) or P (previous window).

```bash
Ctrl + A, N  # Next window
Ctrl + A, P  # Previous window
```

7- Named Sessions
```bash
screen -S name
```
These examples cover basic uses of the screen command. For more detailed information about screen, you can view the manual page by running the following command in the terminal:

```bash
man screen
```