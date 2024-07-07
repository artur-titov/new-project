# New Project

## How this repository was created:

(Tested on Ubuntu 22.04+)

### Setuped

```sh
mkdir <path_to_project>/new-project
```

```sh
cd <path_to_project>/new-project
```

```sh
git init
```

```sh
git config --local user.name "<github_username>"
```

```sh
git config --local user.email "<github_email>"
```
Added ssh host:
```sh
git add remote add origin git@github.com:<github_username>/new-project.git
```

### Added README file

```sh
touch README.md && echo "# New Project" >> README.md
```

```sh
git add README.md
```

```sh
git commit -m "init"
```

```sh
git push -u origin master
```

### Added dev branch

```sh
git checkout -b development
```

```sh
git push -u origin development
```

## How to start using this repository:

```sh
cd <path_to_project>
```

If you use https:

```sh
git clone https://github.com/artur-titov/new-project.git
```

If you use ssh:

```sh
git clone git@github.com:artur-titov/new-project.git
```
If you use github cli:

```sh
gh repo clone artur-titov/new-project
```

After successfully cloning you need to change branch on target:

```sh
git checkout development
```

## Recommendations for use during development

Please update local repository from origin before commit your changes:

```sh
git fetch
```

Check status
```sh
git status
git diff
```
Add files to staging:
```sh
git add <files>
```

Commit changes:

```sh
git commit -m "<commit_message>"
```

Push changes to remote. Type once:
```sh
git push -u origin development
```

After that you can allways use:
```sh
git push
```

---