# Branch

## Finding a local branch by name

```sh
> git show-ref refs/heads/<branch_name>
b81db32e0103a05b81db32e0103a05 /refs/heads/<branch_name>
```

## Finding current branch name

```sh
> git rev-parse --abbrev-ref HEAD
master
```
