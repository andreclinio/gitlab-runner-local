# Introduction

## Requirements

First, check if the following packages are installed.
* Bash Shell
* Git
* Gitlab-Runner (see instructions below)

Then, create a special "sudoer" user to have a home directory. 
Use this place to clone this repository and run any scripts. 
At this user's HOME, you can put any other needed files.

# Gitlab-runner install

## Unix
To see updated documentation, check this 
[site](https://docs.gitlab.com/runner/install/linux-repository.html).

For Ubuntu, run:
```
$ curl -L "https://packages.gitlab.com/install/repositories/runner/gitlab-runner/script.deb.sh" | sudo bash
$ sudo apt-get install gitlab-runner
```

# Usage

## Register shell script usage
```
$ sudo ./register my-runner-name my-token
```

## gitlab-runner usefull commands
```
$ sudo gitlab-runner list
$ sudo gitlab-runner unregister --all-runners
$ sudo gitlab-runner unregister --name my-runner-name
$ sudo gitlab-runner verify --delete
```
