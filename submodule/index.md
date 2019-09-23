# Submodule

```sh
git submodule add -b master [URL to Git repo] [folder path]
```

To change the branch, required Git 2.22.x +

```sh
git submodule set-branch --branch [branch] [path]
```

Fetching latest commits and merge to submodule

```sh
git submodule update --remote [path]
```
