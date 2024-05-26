### What is Code Tunnels?
The main purpose of the previous scenario and this scenario is to introduce you to the Visual Studio Code Tunnels tool and make you capable of using this tool.

VSCode Tunnels (hereinafter referred to as Tunnels or tunnel) is a part of Microsoft's developed VSCode CLI tool. With this tool, you can remotely access a machine and use your preferred version of VSCode.

#### How is it Different from SSH?
Secure Shell, or SSH, is a tool that provides secure access to a remote machine over unreliable networks. SSH is also a network protocol and operates on port 22. The combination of this network protocol and the basic tools that use it is referred to as SSH.

When working with SSH, you need to know the IP address of the machine you are connecting to. Additionally, when using this tool, either password-based or key-based authentication is required.

In Tunnels, on the other hand, you need to authenticate with your Github or Microsoft account. Once you authenticate, it becomes persistent for the machine you authenticated, and you can access your machine from any device through the VSCode application as long as the tunnel tool is running.

#### Purpose of Usage
After the installation steps I will mention later, including the CloudDevelopers platform, you will be able to connect to machines you want to remotely access with your own settings, even if the SSH port of the machine is closed.

#### How is it Different from Online IDE?
![architecture](./assets/server-arch-latest.png)
In the concept of an online IDE, the VSCode block shown in the image, meaning the IDE itself, is also running on the server, on the remotely accessed machine. This leads to high resource consumption on the server and problems on the web page. In the Code Server approach, which is the basis of the tunnels feature we use; there is only the code we use. The interface of the IDE, its extensions, and basically everything except the files you want to keep on the remote machine are stored on the user's preferred platform. Since the user's familiar development environment configurations can be involved here, it enhances the user experience.

Additionally, you can share files from your desktop VSCode to the remote machine via drag and drop.

#### How Does it Work?
When you run the tool on the machine you remotely access, the following steps occur:

- Run the tool from the command line.

- The tool asks for authentication with your Microsoft or Github account.

    - Here, you are given an auth-key, and you authenticate with your preferred account using this key.
- Naming the machine.

    - Here, you give a name to the machine where you run the tool.
- The tool comes up completely (you may wait for 5-10 seconds here).

We will delve into the implementation of the next step in more detail.