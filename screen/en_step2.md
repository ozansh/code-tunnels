### Screen and Code CLI
Now i will show you usage of Screen with Code CLI

```bash
# We create a named session
screen -s code-cli
```
![1](./assets/1.png)
Then we run the program
```bash
./code tunnel
```
![2](./assets/2.png)
Since our tunnel is on the go, we can leave this session:
```bash
Ctrl A + D
```
We can look for our session with
```bash
screen -ls
```
![3](./assets/3.png)