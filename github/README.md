# GitHub Guide

At Raspberry Pi we use GitHub for a number of projects, from our software repositories like the Linux kernel and NOOBS to our documentation and educational resources.

We have two GitHub organisations: [Raspberry Pi](https://github.com/raspberrypi) and [Raspberry Pi Learning](https://github.com/raspberrypilearning).

## Using GitHub

GitHub is a software projects hosting service – it's a kind of social networking site for code projects. It uses version control software Git to manage changes in projects, and allows collaboration over the web.

First, sign up to GitHub.com. Create an account and you'll have a web page at `github.com/username` which will show your repositories when you create some.

You can create repositories from GitHub by clicking the + symbol in the top right of the screen by your username and selecting New Repository and giving your project a name. The next step allows you to initialise the repository. GitHub allows you to add new files in its interface, and you can edit files directly. This can be suitable for making small changes but to utilise git more practically, you would tend to install a git on your computer and set up a repository locally, then push your changes to GitHub.

See our [Getting Started with GitHub](getting-started.md) guide.

## Issues

GitHub has a feature allowing users to open issues against a repository. This is a way of reporting a bug or requesting a feature. The project maintainers will be notified of the issue and have the option of closing it if they deem it a non-issue, or replying to the user by commenting on the issue. When a fix has been committed to the repository, the issue can be closed automatically (by referring to it in the commit message, e.g. `Add compiling instructions, fix #23` or manually by clicking the Close button on the issue comment thread.

See our [GitHub Issues](issues.md) guide.

## Forking

Forking is the term used to describe the action of copying another person's project in to your own domain. From here you can make changes to your own copy without affecting the original copy. If you intend to send your changes back to the original author's project, you can send a request for them to be merged with a pull request.

GitHub's user interface makes forking easy – a Fork button is provided at the top right corner of every repository. Clicking this will automatically copy the project to your account. For example if you fork `github.com/raspberrypi/noobs` you would find your copy at `github.com/yourusername/noobs` with the full history of the project available.

See our [Forking](forking.md) guide.

## Pull Requests

A pull request is the action of sending the changes you made to your fork of someone else's project back to the original project author. They can review your changes and have the option of accepting or denying your request.

See our [Pull Requests](pull-requests.md) guide.

## Using Git Locally

GitHub's web interface can be used for a great deal of tasks, but some things require using git on your computer either with a GUI or using the command line.

GitHub's editor is suitable for small additions and modifications but for writing substantial amounts of material it is advisable to use an offline editor and commit using git on your computer.

See our [Git](git.md) guide.
