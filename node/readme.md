# Setting up a Node/Express Project

[Node.js](https://nodejs.org/en/) is an open-source JavaScript runtime environment for building server-side and networking applications.

In this guide we will discuss how to set up a Node.js/Express project for development on your local machine.

## Install Node.js

Let's start by installing the latest stable release of Node.js. Installing Node.js differs based on operating system.

| Operating System      | Installation Instructions |
| :----:        |    :----:   |
| MacOS     | Download and install easily from the [official Installer here](https://nodejs.org/en/#download)       |
| MacOS      | You can also install with [Homebrew here](https://formulae.brew.sh/formula/node#default), if you prefer.       |
| Windows   | Download and install easily from the [official Installer here](https://nodejs.org/en/#download)     |
| Windows | You can install with [Chocolately here](https://community.chocolatey.org/packages/nodejs.install) if you prefer.
| Linux     | Look out for the instructions to download the right for your specific Linux distro [here](https://nodejs.org/en/download/package-manager/) |

**Note**: For the official installer, select the button to download the LTS build that is _Recommended for most users_. Install Node by double-clicking on the downloaded file and following the installation prompts.

### Test your Nodejs installation

Installing Nodejs also installs [Node Package Manager (NPM)](https://docs.npmjs.com/)on your operating system. To test if you have Node installed on your system, open your terminal and type the following:

```shell
$ node -v
v15.14.0
```

You can test for npm too with:

```shell
$ npm -v
7.7.6
```

You would get the current instlled version of Node and NPM as output, respectively.

## Start a Project with "npm init"

The `npm init` command creates a **package.json**

* Create a new empty directory with your project name `mkdir <my-project-name>`
* Navigate in to that directory `cd <my-project-name>`
* Initialiase a new project by running `npm init` command.

`npm init` command prompts you for a number of things (name of yur applicatin, version, entry pint file etc.). For now, accept the defaults.



## Install Eslint on VsCode

## Other References

<https://nodejs.org/en/>
<https://nodejs.org/en/download/package-manager/>
