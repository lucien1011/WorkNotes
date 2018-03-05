## Make one folder as submodule

Source: http://willandorla.com/will/2011/01/convert-folder-into-git-submodule/

### 1. Clone new repository

```bash
$ git clone --no-hardlinks original-repo copied-repo
```

### 2. Filter out the files you want to keep and remove the others

```bash
$ cd copied-repo
$ git filter-branch --subdirectory-filter sub/module/path HEAD -- --all
$ git reset --hard
$ git gc --aggressive
$ git prune
$ git remote rm origin
```

### 3. Push the new repositories to the upstream server

```bash
$ git remote add git@github.com:korya/submodule-repo.git
```

### 4. Add the new repository as submodules to the original repository

```bash
$ cd original-repo
$ git rm sub/module/path
$ git commit -m "Removing the folders that are now repositories"
$ git submodule add git@github.com:korya/submodule-repo.git sub/module/path
$ git submodule init
$ git submoduel update
$ git add .gitmodules sub/module/path
$ git commit -m "Added in submodules for removed folders"
```
