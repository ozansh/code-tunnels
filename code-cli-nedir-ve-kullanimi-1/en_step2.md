### CLI Parameters
You can obtain information about the tool using the --help argument:

```bash
./code --help
```
To view the version of the tool, use the --version argument:

```bash
./code --version
```
#### Examples for Full VSCode Installation
You can send a directory as an argument, and the VSCode interface will open in that directory. Similarly, sending a file as the first argument will open that file within VSCode. However, in this scenario, since we downloaded the CLI tool on its own, these commands will ***not*** work.

```bash
# Example of Opening a Directory
./code /home/clouddeveloper/workspace

# Example of Opening a File
./code /home/clouddevelopers/workspace/turktelekom.config
```
For more in-depth reading, you can refer to this [link](https://code.visualstudio.com/docs/editor/command-line).