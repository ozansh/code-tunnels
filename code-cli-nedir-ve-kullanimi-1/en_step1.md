### What is VSCode Cli?
VSCode Cli is a command-line tool for the VSCode editor that can be run from the command line. It is written in Rust and is open source.

It can be installed alongside Visual Studio Code (VSC) or as a standalone tool. In this course, we will look further into this tool. 

#### Installation
You can download the tool from this [link](https://code.visualstudio.com/#alt-downloads).
At the bottom of the webpage, you can find buttons marked with an underline, and you can choose the one suitable for your system. Make sure to download the CLI version.
[download](./assets/download.png)

Additionally, if you don't have GUI (Graphical User Interface) access, you can also install it by pasting the following code into the command line:

```bash
# In this step, we download the compressed file containing the executable
curl -Lk 'https://code.visualstudio.com/sha/download?build=stable&os=cli-alpine-x64' --output vscode_cli.tar.gz
```
```bash
# In this step, we extract the executable from the compressed file downloaded in the previous step
tar -xf vscode_cli.tar.gz
```
If you installed the tool with your package manager, in the following steps, use:

```bash
code <parameters>
```
If you downloaded it using curl, use:
```bash
./code <parameters>
```