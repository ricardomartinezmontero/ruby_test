
### you have to be in your project folder

Make sure that you are in your project folder.

### Instructions to update your repository in your project to upload it to this repository
```bash
git remote add ricardo_github https://github.com/ricardomartinezmontero/ruby_test.git
```

### Now check the repositories that you have configured in your project
```bash
git remote -v
```

### This should print as output in your terminal as below

```bash
ricardo_github  https://github.com/ricardomartinezmontero/ruby_test.git (fetch)
ricardo_github  https://github.com/ricardomartinezmontero/ruby_test.git (push)
```

### Run the following command to download the initial repository that I created, this will download the remote branches
```bash
git fetch ricardo_github
```

### Make sure you are in master branch, run this command 

```bash
git branch -a
```

### This should print something as below

```bash
* master
  remotes/ricardo_github/master
```

```remotes/ricardo_github/master``` is the branch I want you to upload the code, which is in my github.

### Configure your email and your name in your git, run the following commands with your email and your nickname

```bash
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```

### If your branch is master, which means the asteric is next to the branch name, then run this command to upload the project

```bash
git commit -am "project commit"
git rebase ricardo_github/master
git push ricardo_github master
```

### Now you should have upload your code to the repository