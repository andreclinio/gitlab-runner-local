# Introduction

# Gitlab-runner install

[https://docs.gitlab.com/runner/install/linux-repository.html]

For Ubuntu, run:
```
$ curl -L "https://packages.gitlab.com/install/repositories/runner/gitlab-runner/script.deb.sh" | sudo bash
$ sudo apt-get install gitlab-runner
```

# Usage

## Shell usage
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
