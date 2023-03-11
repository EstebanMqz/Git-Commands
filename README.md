# **Github Contributions** &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=gray)

## Fork vs Clone:  

-	***Fork***: Merge with original repo is possible with a pull request.

-	***Clone***: Merge with original repo is only achieved by pushing to fork and then a pull request.
---

### ***Contributions without permissions***:

***Note:*** It is better to fork a repository before cloning it due to [copyrights](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository) when the *user is NOT declared as a contributor*.

<br/>

**General steps**:
1. [Fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) repository.
2. [Clone](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) forked repository.
3. Make Changes in Local.
4. [Push](https://docs.github.com/en/get-started/using-git/pushing-commits-to-a-remote-repository) to Personal Remote.
5. [Pull Request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/incorporating-changes-from-a-pull-request/merging-a-pull-request) to Original Remote.

<br/>

---

### ***Contributions with permissions***:

***Note***: It is a faster option to clone the original repository without a previous fork of the project if the *user IS declared as a contributor*.

<br/>

**General steps**:
1. [Clone](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)
2. Make Changes in Local.
3. [Push](https://docs.github.com/en/get-started/using-git/pushing-commits-to-a-remote-repository) to Personal Remote. <br/><br/>

*Refer to Github official [documentation](https://docs.github.com/en/get-started/quickstart/contributing-to-projects?tool=webui) for more information related to contributions.*

---

# **Git Commands** &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)<br>
The following is a list of common git commands based on the [Git Documentation](https://git-scm.com/docs).

<br/> 

|Basic|Command|Description|
|---|---|---|
|[1. help](https://linux.die.net/man/1/git-help)|<ol style="list-style-type:none;"><li>git help<li> git help `<command>`<li> git help -a|<ol style="list-style-type:none;"><li>**List** ***common commands***. <li> **Display help** on git ***command***.<li>**List all** available ***commands***.|
|[2. init](https://git-scm.com/docs/git-init)|<ol style="list-style-type:none;"><li>git init<li>git init -b `<branch>`<li>git init `<subdir.>`<li>git init --bare `<subdir.>`<li>git init --template=`<template-dir.>`<li>git init --shared`[=(-options)]`|<ol style="list-style-type:none;"><li>**Initialize** ***git*** repo in folder.<li>**Override** ***branch name*** *(config. default set if none)*.<li>**Initialize** a **git repo** inside a new subdir.<li>**Initialize** a **git bare** repo inside new subdir.<li>**Specify** *dir.* from which ***templates*** will be used.<li>Make **git** ***readable/writable*** by users *([see options](https://linux.die.net/man/1/git-init))*.|
|[3. clone](https://git-scm.com/docs/git-clone)|<ol style="list-style-type:none;"><li>git clone `<URL>`<li>git clone --no-hardlinks `<dir.>` <li> git clone `<URL>` `<dir.>`<li> git clone `<URL>` --branch `<branch>` --single-branch<li> git clone --bare <li> git clone --mirror <li> git clone --template=`<temp_dir.>` `<dir.>`<li> git clone --depth=`<depth>` |<ol style="list-style-type:none;"><li>**Clone** ***remote*** default branch with [***URL***](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) .<li>**Clone** ***local*** repo for *backup* purposes.<li>**Clone** ***remote*** *default branch* in ***dir***.<li>**Clone** ***remote*** *single* *branch* with repo ***URL***.<li>**Clone** ***remote*** with ***no remote-tracking*** & ***config.***<li>**Clone** ***--bare***  with *remote tracking & config.*.<li> **Clone** set ***template*** in dir. (see *2.git init*).<li>**Clone truncated** to a number of ***revisions***.|
|[4. config](https://git-scm.com/docs/git-config)|<ol style="list-style-type:none;"><li>git config <li>git config --global pull.rebase true<li> git config --global ff no<li>git config ff no<li>git config remote.origin.prune true<li>git config --global fetch.prune true<li>git config --global user.name `<username>`<li> git config --global user.email `<e-mail>`<li>git config --system user.name `<project>`<li>git config --get user.name<li>git config -l<li>git config -e|<ol style="list-style-type:none;"><li>**Display** git ***global config*** *(create if none)*.<li> **Set** the ***pull*** command ***as rebase*** *globally*.<li>**Disable** ***fast-forward*** merge for  ***local*** repos.<li>**Disable** ***fast-forward*** merge in ***local*** repo.<li>**Set** ***auto-prune*** with ***fetch*** & ***pull***.<li>**Set** ***auto-prune*** w/ ***fetch*** for  ***local*** repos.<li>**Set** ***author*** to commits for ***local*** repos.<li> **Set** ***email*** to commits for ***local*** repos.<li>**Set** ***author*** for all git users.<li>**Get** ***author/email*** from ***global/system***.<li>List all variables set in config. file.<li>**Edit config** files from ***global/system***|
|[5. checkout](https://git-scm.com/docs/git-checkout)|<ol style="list-style-type:none;"><li>git checkout `<branch>`<li>git checkout -b `<feature>`<li> git checkout -b `<branch>` `<origin/branch>` <li> git checkout -- `<file>`<li>git checkout -<li> git checkout `<branch>~n <file>`|<ol style="list-style-type:none;"><li>**Switch** to ***branch*** in working tree.<li>**Create** and ***switch*** to ***feature*** (or any) branch.<li>**Clone** ***remote*** branch and *switch*.<li>**Discard** ***changes*** in file to *match current branch*.<li>**Switch** to ***last checkout***. <li> **Reverts local** file in  branch *n* ***commits*** *(e.g. n=2)*.|
|[6. fetch](https://git-scm.com/docs/git-fetch)|<ol style="list-style-type:none;"><li>git fetch `<origin>`<li>git fetch `<origin>` `<branch>`<li>git fetch --all<li>git fetch --dry-run<li>git fetch --append<li>git fetch --depth=`<depth>`<li>git fetch -f<li> git fetch --prune|<ol style="list-style-type:none;"><li>**Fetch** ***all***.<li>**Fetch** ***branch***.<li>**Fetch** all ***branches*** in repo.<li>**Show** **output** but ***without fetching***.<li> **Fetch** ***without overwriting*** (.git/FETCH_HEAD).<li> **Limit fetching** to ***n depth*** commits *(e.g. n=3)*.<li>**Fetch even** if it's ***not descendant*** of *remote branch*.<li>**Remove** ***unexistant remote-tracking*** branches.|
|[7.merge](https://git-scm.com/docs/git-merge)|<ol style="list-style-type:none;"><li>git merge `<branch>`<li> git merge `<branch>` `<target_branch>`<li>git merge --no-ff `<branch>` <li> git merge --continue<li> git merge --allow-unrelated-histories<li>git merge -base [-a] `<commit_id>` `<commit_id>`  <li> git merge -s resolve `<branch-1>` `<branch-2>`<li> git merge -s recursive -X ours OR theirs `<branch>`<li>git merge -s octopus `<branch-1>` `<branch-n>`<li> git merge -s ours `<branch-1>` `<branch-n>`<li>git merge -s subtree `<branch-1>` `<branch-2>`|<ol style="list-style-type:none;"><li>**Fast-forward** merge branch with ***HEAD*** *(linear)*.<li>**Fast-forward** merge branch to tip of ***target***.<li> **Maintain** commit ***history***, may not fast-fwd.<li>**Conclude** *conflicting* ***merge***.<li>**Merge** ***indep. projects*** by overriding safeties.<li>**Find ancestor** on ***n commits*** for a *3-way merge*.<li> **3-way merge** *2 branch HEADs*.<li> **3-way merge** ***>1 common ancestors*** for *tree*. <li> <li>**Merges** ***more than 2*** branch *HEADs*.<li>**Merges** ***multiple branches tip*** in HEAD.<li>**Reflect B tree** ***structure*** as subtree of *A*.|
|[8. pull](https://git-scm.com/docs/git-pull)|<ol style="list-style-type:none;"><li>git pull<li>git pull `<URL>`<li> git pull `<origin>` `<branch>`<li>git pull --rebase `<origin> <branch>`<li>git pull --ff-only<li> git pull --no-ff<li>git pull -s `<strategy>` -X `<option>`|<ol style="list-style-type:none;"><li>**Fetch** & **merge** *remote-tracking* with local.<li>**Clone, fetch** & **merge** remote's *URL* with local.<li> **Fetch** & **merge** *remote branch* with local.<li>**Fetch** & **rebase** *branch*.<li>**Update** *branch* without a merge commit.<li>**Pull** & **commit** even for *fast-forwards (linear)*.<li>Same strategies and options as for merge last 5.|
|[9. add](https://git-scm.com/docs/git-add)|<ol style="list-style-type:none;"><li> git add -A<li>git add .<li>git add `<file>`<li>git add -n `<file>`<li>git add --v<li>git add -force<li>git add -p<li>git add -i<li>git add -e|<ol style="list-style-type:none;"><li>**Add** ***all changes*** in files to stage.<li>**Add** ***changes*** without *deletions* for stage.<li> **Add** ***file*** to stage.<li>**Show** if ***file*** is ***unexistant***.<li> **Ignore** indexing ***errors*** for git add.<li>**Allows** to add ***ignored*** files.<li>**Patch hunks** ***interactively*** from *index to tree*[¹](https://gitready.com/intermediate/2009/01/14/interactive-adding.html).<li> <li>**Patch changes** ***interactively*** from *index to tree*.<li>Interactive patch mode vs diff editor.|
|[10. commit](https://git-scm.com/docs/git-commit)|<ol style="list-style-type:none;"><li> git commit -m `<msg>`<li> git commit --date=`<date>`<li>commit -i `<msg>`<li> git commit --dry-run<li>git commit -v<li>git commit --amend<li> git commit -s|<ol style="list-style-type:none;"><li>**Overwrite** commit ***msg*** .<li>**Override** author's ***date*** in commit.<li>**Commit** ***changes*** & ***unstaged*** content.<li>**List** only ***commited, uncommited*** & ***untracked*** paths.<li>**Show differences** between ***HEAD*** and ***commit***.<li>**Modify** the most *recent* commit ***msg***.<li>Add **author signature** at the ***end*** of *commit msg*.|
|[11.push](https://git-scm.com/docs/git-push)|<ol style="list-style-type:none;"><li>git push<li>git push -u `<origin> <branch>`<li>git push --all<li>git push `<origin>` --delete `<branch>`<li> git push --force <li> git push --force-with-lease <li> git push --prune `<origin refs/heads/*>` <li> git push --mirror|<ol style="list-style-type:none;"><li>**Push** *commits*. <li>**Push** *commits* and set as ***upstream***.<li>**Push** ***all*** *commits*.<li> **Delete** ***remote-tracking*** branch.<li>**Push** commits and ***destroy all unmerged*** changes.<li>**Push** and ***destroy personal unmerged*** changes.<li>**Remove** ***remote*** *without local counterpart*.<li> **Overwrite** ***remote*** *with* ***local*** branches.|
|[12.pull request](https://git-scm.com/docs/git-request-pull)|<ol style="list-style-type:none;"><li>git request-pull `<branch> <URL> <feature>`|<ol style="list-style-type:none;"><li>**Pull request** for changes between tag and feature.|
|[13. branch](https://git-scm.com/docs/git-branch)|<ol style="list-style-type:none;"><li>git branch <li>git branch -r <li>git branch -a <li>git branch `<branch>`<li> git branch -d `<branch>`<li>git branch -D `<branch>`<li>git branch -f `<branch>` `<feature>`<li> git branch --show-current<li>git branch --set-upstream-to<li> git branch / grep -v `<branch(es)>` / xargs git branch -D|<ol style="list-style-type:none;"><li>**See** ***local*** branches.<li>**See** ***remote*** *branches*.<li>**See** ***local and remote*** *branches*. <li> **Create** ***branch*** and *name it*.<li>**Delete** ***unmerged*** branch.<li>**Delete** ***merged*** & ***unmerged*** branches.<li>**Rewrite** local ***branch*** with ***feature*** branch.<li>**Show** ***current*** branch in local.<li>Make an existing git branch **track** a ***remote***.<li>**Delete** ***all*** branches *excepting* selected.|
|[14. diff](https://git-scm.com/docs/git-diff)|<ol style="list-style-type:none;"><li>git diff<li>git diff --staged<li> git diff HEAD<li> git diff --color-words<li> git diff `<branch> <feature> <file>` <li> git diff `<commit_id> <commit_id> <file>`<li> git diff --stats<li> git diff-files<li>git diff stash@{n} `<branch>`|<ol style="list-style-type:none;"><li>**Check** for **differences** in ***local*** & ***remote-tracking***.<li>**Check** for **differences** in ***local*** & ***staged*** changes.<li>**Check** for **differences** in ***work dir.*** & ***last commit***.<li> **Highlight** ***changes*** with *color* granularity. <li>**Check** for **differences** in a file between ***two branches***.<li>**Check** for **differences** in a file between ***two commits***.<li>**Show** ***insertions*** & ***deletions*** in *staged* and *local*.<li> **Compare** ***files*** in the *working tree*[²](https://linux.die.net/man/1/git-diff-files).<li> **Compare stash** ***n*** with *branch*.|
|[15. log](https://git-scm.com/docs/git-log)|<ol style="list-style-type:none;"><li>git log -n<li>git log --oneline<li>git log -p --follow -- `<file>` <li> git log --oneline --decorate<li> git log --stats<li>git shortlog<li>git log --pretty=format:"%cn committed %h on %cd"<li>git log --after=`<yyyy-m-d>` --before=`<yyyy-m-d>`<li>git log --author=`<username>`|<ol style="list-style-type:none;"><li>**Display** ***logs*** from last 1,2,..*n* commits.<li>**Show** ***IDs*** from commits.<li>**Show** ***commits*** on a *file*.<li>**Display** ***commits***~***branches***.<li>**Show** ***insertions*** & ***deletions***.<li>**Display**  ***commits*** *first coding line* by author.<li>**Customized log** (*show author, hash & date*).<li>**Search** for ***commits*** in *range*.<li>**Search** for ***commits*** by *author*.|
|[16. revert](https://git-scm.com/docs/git-revert)|<ol style="list-style-type:none;"><li>git revert `<commit_id>`<li>git revert `<commit_id>` --no-edit<li>git revert -n `<commit_id>`<li>git revert -n `<HEAD>~n`<li>git revert -n `<HEAD>~n`..`<HEAD>~m`|<ol style="list-style-type:none;"><li>**Invert commit** & ***commit*** *undone changes*.<li>**Reverts** *without* a new ***commit msg***.<li>**Invert** ***changes*** & ***stage*** *only*.<li>**Revert** ***n commits***.<li>**Revert** from ***n→m commits*** *[n,m]*.|
|[17. reset](https://git-scm.com/docs/git-reset)|<ol style="list-style-type:none;"><li>git reset `<file>`<li> git reset --mixed `<HEAD>~n`<li>git reset --mixed `<commit-id>`<li>git reset --hard `<HEAD>~n` <li>git reset --soft `<HEAD>~n`<li>git reset -p|<ol style="list-style-type:none;"><li>**Untrack** ***file***.<li>**Unmerge** & **uncommit** but ***don't unstage*** *(default)*.<li>**Mixed** with ***commit hash*** *(default)*.<li>**Undo** all ***n*** *changes*.<li>**Hard reset** but able to ***recover*** *changes* with ***git commit***.<li>**Patch interactively** (***git add -p*** *inverse*).|
|[18. stash](https://git-scm.com/docs/git-stash)|<ol style="list-style-type:none;"><li> git stash<li> git stash push -m `<msg>`<li>git stash list<li> git stash list --stat<li>git stash apply<li>git stash pop -n<li> git stash drop -n|<ol style="list-style-type:none;"><li>**Saves work dir.** from ***local*** & *hard reset*.<li>**Saves work dir.** from local ***with msg*** & *hard reset*.<li>**List** ***stashed*** changes as an *index [*n*]*<li>**Show summary** of ***changes*** in *stash list* <li> **Recover** ***stash[0]*** from *work dir*.<li>**Recover** ***stash n*** & *delete it* from *stash* list.<li>**Delete** ***stash n*** from *stash list*.|
|[19. status](https://git-scm.com/docs/git-stash)|<ol style="list-style-type:none;"><li> git status<li> git status -s <li> git status -b|<ol style="list-style-type:none;"><li>**List (un)staged, (un)tracked** changes (work dir.,stage & modif.).<li>**Status** in ***short*** *format*.<li>**Status** on a ***branch***.<li>|
|[20. touch](https://linux.die.net/man/1/touch)|<ol style="list-style-type:none;"><li> git touch `<name.ext>` |<ol style="list-style-type:none;"><li>**Create file** with ***extension*** *(e.g test.txt)*.|
|[21. switch](https://linux.die.net/man/1/switch)|<ol style="list-style-type:none;"><li> git switch `<branch>`<li> git switch  -c `<branch>`<li>git switch  -c `<branch>` `<commit_id>` |<ol style="list-style-type:none;"><li> **Switch** to ***branch***.<li> **Create** a new ***branch*** and *switch*.<li>**Grow branch** from ***commit***.|
|[22. cd](https://www.git-tower.com/learn/git/ebook/en/command-line/appendix/command-line-101)|<ol style="list-style-type:none;"><li> cd ~/`<home>`<li>cd ~/`<home>`/`<dir.>`<li>cd ~/`<home>`/`<dir.>`/`<subdir.>`|<ol style="list-style-type:none;"><li> **Change dir.** to ***home***  *(e.g ~/Desktop)*<li>**Change dir.** to a ***folder*** in *home*.<li>**Change dir.** to n ***sub-folders*** in *home*.|  
|[23. ls](https://linux.die.net/man/1/git-ls-files)|<ol style="list-style-type:none;"><li>ls <li>ls -la|<ol style="list-style-type:none;"><li>**List subfolders** in ***dir***. <li>**List subfolders** in ***dir*** with *hidden files*.|
|[24. rm](https://git-scm.com/docs/git-rm)|<ol style="list-style-type:none;"><li>git rm `<file>`<li>rm `<file>`|<ol style="list-style-type:none;"><li>**Remove file** from ***git tracking*** & ***local***.<li>**Remove file** from ***local*** *only*.
|[25. mv](https://git-scm.com/docs/git-mv)|<ol style="list-style-type:none;"><li>git mv `<file.ext>` `<new-filename.ext>`<li> git mv `<file.ext>` ~/`<home>`/`<dir.1>`/`<subdir.>`|<ol style="list-style-type:none;"><li>**Rename file** with the same ***extension***.<li>**Move file** from dir.1 to subdir. (inside dir.1)
|[26. mkdir](https://linux.die.net/man/1/mkdir)|<ol style="list-style-type:none;"><li>git mkdir ~/`<home>`/`<dir.>`/`<subdir.>/<new_dir.>`|<ol style="list-style-type:none;"><li>**Create dir.** ***in path***.
|[27. remote](https://git-scm.com/docs/git-remote)|<ol style="list-style-type:none;"><li>git remote<li> git remote -v<LI> git remote rename `<old-name> <new-name>`<li>git remote add `<URL>`|<ol style="list-style-type:none;"><li>**List** ***remote*** *branches*.<li>**List** ***remote*** *branches* with *URL*.<LI>**Rename** ***remote***.<li>**Connection** with ***repo*** with *URL*.|
|[28. gitk](https://linux.die.net/man/1/gitk)|<ol style="list-style-type:none;"><li> gitk<li> gitk HEAD...FETCH_HEAD|<ol style="list-style-type:none;"><li>**Show Git GUI** for ***commits***.<li> **Show Git GUI** for ***all users*** since last push.


***Note***: Remember to call branches by their names in your commands (*see 13. branch*). <br> 
*Tip:* `<main>` is the default name for remote repositories as `<master>` is for local. <br>

---
### **Definitions**:
**origin**: Primary ***working dir.*** of ***remote*** repositories by ***default***.<br>
**fetch**: Fetch is the ***safe*** version of ***pull*** because local ***files aren't merged*** until they are reviewed, checked out & merged.<br>
**revert**: Revert is ***safer*** than doing git ***reset***, checkout to *discard* (*see 5.4*), etc. This is because commit ***history isn't erased*** but a new inverted commit is appended.<br>
**feature**: Feature represents a ***branch of developments*** in progress with their descriptions. 


*See Also*: <br>
[Glossary](https://linux.die.net/man/7/gitglossary)<br>


---
### **Author**:
[EstebanMqz](https://github.com/EstebanMqz)

### ***Contact***:
Feel free to send me an [email](mailto:esteban@esteban) if you have any questions.<br />
Contributions are greatly appreciated!<br />

---
***Note***: If you are interested in learning more about git commands you can check out the list below and refer to the [git documentation](https://git-scm.com/docs) for more options on these commands.<br />
### **Other Commands:** <br /> <br />

+ **[git am](https://git-scm.com/docs/git-am)** ~ Splits patches from a mailbox into commit msg, author and patches to apply them to branch.<br>
***e.g:*** `git am --keep-cr --signoff < a_file.patch` *to apply patch as commit.*<br>
+ **[git apply](https://git-scm.com/docs/git-apply)** ~ Apply a patch to files and add them to the index.<br>
***e.g:*** `git apply < a_file.patch` *to apply patch to files.*<br>
+ **[git archive](https://git-scm.com/docs/git-archive)** ~ Combine multiple files in a single file but removes git data.<br>
***e.g:*** `git archive --format=zip --output=archive.zip HEAD` *to create a zip file with all files in HEAD.*<br>
+ **[git bisect](https://git-scm.com/docs/git-bisect)** ~ Binary search algorithm to find commit in project history which caused a bug.<br>
***e.g:*** `git bisect start` *to start the search.*<br>
+ **[git blame](https://git-scm.com/docs/git-blame)** ~ Show what revision and author last modified each line of a file.<br>
***e.g:*** `git blame <file>` *to show the last author of each line in file.*<br>
+ **[git bugreport](https://git-scm.com/docs/git-bugreport)** ~ Create a report to send to git mailing list.<br>
***e.g:*** `git bugreport -o report.txt` *to create a report and save it to report.txt.*<br>
+ **[git bundle](https://git-scm.com/docs/git-bundle)** ~ Move objects and refs by archive.<br>
***e.g:*** `git bundle create <file> <branch>` *to create a bundle with branch.*<br>
+ **[git cat-file](https://git-scm.com/docs/git-cat-file)** ~ Provide content or type and size information for repository objects.<br>
***e.g:*** `git cat-file -p <commit>` *to show the content of commit.*<br>
+ **[git check-attr](https://git-scm.com/docs/git-check-attr)** ~ Display git attributes.<br>
***e.g:*** `git check-attr -a` *to show all attributes.*<br>
+ **[git check-mailmap](https://git-scm.com/docs/git-check-mailmap)** ~ Show canonical names and email addresses of contacts.<br>
***e.g:*** `git check-mailmap <name>` *to show the canonical name of name.*<br>
+ **[git check-ref-format](https://git-scm.com/docs/git-check-ref-format)** ~ Ensure that a reference name is well formed.<br>
***e.g:*** `git check-ref-format --branch @{-1}` *print the name of the previous branch*.<br>
+ **[git check-ignore](https://git-scm.com/docs/git-check-ignore)** ~ Debug gitignore files.<br>
***e.g:*** `git check-ignore -v <file>` *to show the gitignore file that ignores file.*<br>
+ **[git cherry](https://git-scm.com/docs/git-cherry)** ~ Find commits not merged upstream.<br>
***e.g:*** `git cherry -v <branch>` *to show the commits not merged in branch.*<br>
+ **[git cherry-pick](https://git-scm.com/docs/git-cherry-pick)** ~ Apply the changes introduced by some existing commits.<br>
***e.g:*** `git cherry-pick <commit>` *to apply the changes of commit to current branch.*<br>
+ **[git citool](https://git-scm.com/docs/git-citool)** ~ Graphical alternative to git-commit.<br>
***e.g:*** `git citool` *to open the graphical commit tool.*<br>
+ **[git clean](https://git-scm.com/docs/git-clean)** ~ Remove untracked files from the working tree.<br>
***e.g:*** `git clean -n` *to show what files what files would be removed without removing them.*<br>
+ **[git clone](https://git-scm.com/docs/git-clone)** ~ Clone a repository into a new directory.<br>
***e.g:*** `git clone <repo>` *to clone repo into current directory.*<br>
+ **[git column](https://git-scm.com/docs/git-column)** ~ Display data in columns.<br>
***e.g:*** `git column --mode=html <file>` *to display file in html columns.*<br>
+ **[git commit](https://git-scm.com/docs/git-commit)** ~ Record changes to the repository.<br>
***e.g:*** `git commit -m <msg>` *to commit with msg.*<br>
+ **[git commit-graph](https://git-scm.com/docs/git-commit-graph)** ~ Write and verify a commit-graph file.<br>
***e.g:*** `git show-ref -s | git commit-graph write --stdin-commits` *to write a commit-graph file for reachable commits.*<br>
+ **[git commit-reach](https://git-scm.com/docs/git-commit-reach)** ~ Find commits that are reachable from a commit.<br>
***e.g:*** `git commit-reach <commit>` *to show the commits that are reachable from commit.*<br>
+ **[git commit-tree](https://git-scm.com/docs/git-commit-tree)** ~ Create a new commit object.<br>
***e.g:*** `git commit-tree <tree> -m <msg>` *to create a commit with tree and msg.*<br>
+ **[git config](https://git-scm.com/docs/git-config)** ~ Get and set repository or global options.<br>
***e.g:*** `git config --global user.name <name>` *to set the global user name.*<br>
+ **[git count-objects](https://git-scm.com/docs/git-count-objects)** ~ Count unpacked number of objects and their disk consumption.<br>
***e.g:*** `git count-objects -v` *to show the number of objects and their size.*<br>
+ **[git credential](https://git-scm.com/docs/git-credential)** ~ Retrieve and store user credentials.<br>
***e.g:*** `git credential fill` *attempt to add "username" and "password" attributes by reading config credential helpers.*<br>
+ **[git credential-cache](https://git-scm.com/docs/git-credential-cache)** ~ Helper to temporarily store passwords in memory.<br>
***e.g:*** `git credential-cache exit` *exit early, forgetting all cached credentials before their timeout.*<br>
+ **[git credential-store](https://git-scm.com/docs/git-credential-store)** ~  Helper to store credentials on disk to reduce time to fill.<br>
***e.g:*** `git credential-store <file>` *to store credentials in file.*<br>
+ **[git cvsexportcommit](https://git-scm.com/docs/git-cvsexportcommit)** ~ Export a single commit to a CVS checkout.<br>
***e.g:*** `git cvsexportcommit <commit>` *to export commit to a CVS checkout.*<br>
+ **[git cvsimport](https://git-scm.com/docs/git-cvsimport)** ~ Create a new git repository from a CVS checkout.<br>
***e.g:*** `git cvsimport -v -d <cvsroot> <module> <project>` *to create a new git repository from a CVS checkout.*<br>
+ **[git cvsserver](https://git-scm.com/docs/git-cvsserver)** ~ Server for CVS clients to connect to and use Git repositories.<br>
***e.g*** `git cvsserver --base-path=<path> <repo>` *to start the git cvsserver.*<br>
+ **[git daemon](https://git-scm.com/docs/git-daemon)** ~ A really simple server for Git repositories.<br>
***e.g:*** `git daemon --reuseaddr --base-path=<dir.> --export-all` *to restart server & look for repos in dir. to export.*<br>
+ **[git describe](https://git-scm.com/docs/git-describe)** ~ Describe specific commits with their hash.<br>
***e.g:*** `git describe commit` *to describe commit with its hash (HEAD by default).*<br>
+ **[git diff](https://git-scm.com/docs/git-diff)** ~ Show changes between commits, commit and working tree, etc.<br>
***e.g:*** `git diff --stat` *to show the summary of the changed files.*<br>
+ **[git diff-files](https://git-scm.com/docs/git-diff-files)** ~ Show changes between index and working tree.<br>
***e.g:*** `--diff-algorithm={minimal}`*to include the smallest possible diff are included.*<br>
+ **[git diff-index](https://git-scm.com/docs/git-diff-index)** ~ Show changes between commits, commit and working tree, etc.<br>
***e.g:*** `git diff-index --compact-summary HEAD` *to show the summary of the changed files in HEAD.*<br>
+ **[git diff-tree](https://git-scm.com/docs/git-diff-tree)** ~ Show changes between commits, commit and working tree, etc.<br>
***e.g:*** `git diff-tree --s7hortstat HEAD` *to show the summary of the changed files in HEAD.*<br>
+ **[git difftool](https://git-scm.com/docs/git-difftool)** ~ Show changes using common diff tools.<br>
***e.g:*** `git difftool --tool-help` *to show the list of available tools.*<br>
+ **[git fast-export](https://git-scm.com/docs/git-fast-export)** ~ Git data exporter.<br>
***e.g:*** `git fast-export --all` *to export all data.*<br>
+ **[git fast-import](https://git-scm.com/docs/git-fast-import)** ~ Git data importer.<br>
***e.g:*** `git fast-import --max-pack-size=1G` *to import data into a packfile of size 1G (default is unlimited)*<br>
+ **[git fetch](https://git-scm.com/docs/git-fetch)** ~ Download objects and refs from another repository.<br>
***e.g:*** `git fetch <repo>` *to fetch objects and refs from repo.*<br>
+ **[git fetch-pack](https://git-scm.com/docs/git-fetch-pack)** ~ Receive missing objects from another repository.<br>
***e.g:*** `git fetch-pack --prune --all` *to fetch all objects and prune refs that are missing on the remote.*<br>
 **[git filter-branch](https://git-scm.com/docs/git-filter-branch)** ~ Rewrite branches.<br>
***e.g:*** `git filter-branch --tree-filter 'rm -f *.txt' HEAD` *to remove all .txt files.*<br>
+ **[git fmt-merge-msg](https://git-scm.com/docs/git-fmt-merge-msg)** ~ Produce a merge commit message.<br>
***e.g:*** `git fmt-merge-msg <file>` *to produce a merge commit message from file.*<br>
+ **[git for-each-ref](https://git-scm.com/docs/git-for-each-ref)** ~ Iterate over references.<br>
***e.g:*** `git for-each-ref --format='%(refname)' refs/heads` *to list all branches.*<br>
+ **[git format-patch](https://git-scm.com/docs/git-format-patch)** ~ Prepare patches for e-mail submission.<br>
***e.g:*** `git format-patch -root <commit>` *to format everything up from start until commit.*<br>
+ **[git fsck](https://git-scm.com/docs/git-fsck)** ~ Verifies the connectivity and validity of the objects in the database.<br>
***e.g:*** `git fsck --cache` *to check the connectivity and validity of the objects in the cache.*<br>
+ **[git gc](https://git-scm.com/docs/git-gc)** ~ Cleanup unnecessary files and optimize the local repository.<br>
***e.g:*** `git gc --force` *to force garbage collection.*<br>
+ **[git get-tar-commit-id](https://git-scm.com/docs/git-get-tar-commit-id)** ~ Extract commit ID from an archive created using git-archive.<br>
***e.g:*** `git get-tar-commit-id <file>` *to extract most recent commit ID from file.*<br>
+ **[git grep](https://git-scm.com/docs/git-grep)** ~ Print lines matching a pattern.<br>
***e.g:*** `git grep -n 'print' <file>` *to print lines containing 'print' and their line numbers.*<br>
+ **[git gui](https://git-scm.com/docs/git-gui)** ~ A portable graphical interface to Git.<br>
***e.g:*** `git gui citool --nocommit` *Checks for unmerged entries on index and exits gui without committing.*<br>
+ **[git hash-object](https://git-scm.com/docs/git-hash-object)** ~ Compute object ID and optionally creates a blob from a file.<br>
***e.g:*** `git hash-object -w --path <file>` *write the blob to the object database and print its hash.*<br>
+ **[git help](https://git-scm.com/docs/git-help)** ~ Display help information about Git.<br>
***e.g:*** `git help -all` *to display all git commands.*<br>
+ **[git http-fetch](https://git-scm.com/docs/git-http-fetch)** ~ Download objects and refs from another repository via HTTP.<br>
***e.g:*** `git http-fetch -v <[URL]/refs>` *to report all refs downloaded in repo.*<br>
+ **[git http-backend](https://git-scm.com/docs/git-http-backend)** ~ Server side implementation of Git over HTTP.<br>
***e.g:*** `git http-backend` *serve git repo to clients over HTTP(s) protocols.*<br>
+ **[git imap-send](https://git-scm.com/docs/git-imap-send)** ~ Send a collection of patches from stdin to an IMAP folder.<br>
***e.g:*** `git imap-send <repo>` *to send a collection of patches from stdin to an IMAP folder.*<br>
+ **[git index-pack](https://git-scm.com/docs/git-index-pack)** ~ Build pack index file for an existing packed archive.<br>
***e.g:*** `git index-pack <file>` *to build pack index file for file.*<br>
+ **[git init](https://git-scm.com/docs/git-init)** ~ Create an empty Git repository or reinitialize an existing one.<br>
***e.g:*** `git init -b <branch-name>` *to create an empty local Git repository with given branch name.*<br>
+ **[git init-db](https://git-scm.com/docs/git-init-db)** ~ Create an empty Git repository or reinitialize an existing one.<br>
***e.g:*** `git init-db --config <config-file>` *to create an empty local Git repository with given config file.*<br>
+ **[git instaweb](https://git-scm.com/docs/git-instaweb)** ~ Instantly browse your working repository in gitweb.<br>
***e.g:*** `git instaweb --httpd=python --port=8080` *to start a python web server on port 8080.*<br>
+ **[git interpret-trailers](https://git-scm.com/docs/git-interpret-trailers)** ~ Parse trailer lines from text.<br>
***e.g:*** `git interpret-trailers --check <file>` *to check if file contains trailer lines (similar to RFC 822 e-mail headers)*<br>
+ **[git log](https://git-scm.com/docs/git-log)** ~ Show commit logs.<br>
***e.g:*** `git log --follow <file>` *to show commit logs beyond renames for file.*<br>
+ **[git ls-files](https://git-scm.com/docs/git-ls-files)** ~ Show information about files in the index and the working tree.<br>
***e.g:*** `git ls-files -u` *to show unmerged files.*<br>
+ **[git ls-remote](https://git-scm.com/docs/git-ls-remote)** ~ List references in a remote repository.<br>
***e.g:*** `git ls-remote <[URL]/refs>` *to display references in a remote repository associated with commits IDs.*<br>
+ **[git ls-tree](https://git-scm.com/docs/git-ls-tree)** ~ List the contents of a tree object.<br>
***e.g:*** `git ls-tree <tree>` *to list the contents of tree with its id*<br>
+ **[git mailinfo](https://git-scm.com/docs/git-mailinfo)** ~ Extracts patch and authorship from a single e-mail message.<br>
***e.g:*** `git mailinfo <file>` *to extracts patch and authorship from file.*<br>
+ **[git mailsplit](https://git-scm.com/docs/git-mailsplit)** ~ Splits a single mailbox into mboxrd format.<br>
***e.g:*** `git mailsplit <mbox>` *to splits mbox into mboxrd format.*<br>
+ **[git merge](https://git-scm.com/docs/git-merge)** ~ Join two or more development histories together.<br>
***e.g:*** `git merge --allow-unrelated-histories <branch>` *to join two or more development histories together.*<br>
+ **[git merge-base](https://git-scm.com/docs/git-merge-base)** ~ Find as good common ancestors as possible for a merge.<br>
***e.g:*** `git merge-base <branch1> <branch2>` *to find as good common ancestors as possible for a merge.*<br>
+ **[git merge-file](https://git-scm.com/docs/git-merge-file)** ~ Run a three-way file merge.<br>
***e.g:*** `git merge-file <file1> <file2> <file3>` *to run a three-way file merge.*<br>
+ **[git merge-index](https://git-scm.com/docs/git-merge-index)** ~ Run a merge for files in the index.<br>
***e.g:*** `git merge-index -a` *to run a merge for files in the index that need merging.*<br>
+ **[git merge-tree](https://git-scm.com/docs/git-merge-tree)** ~ Show three-way merge without touching index.<br>
***e.g:*** `git merge-tree <file>` *to show three-way merge without touching index.*<br>
+ **[git mergetool](https://git-scm.com/docs/git-mergetool)** ~ Run merge conflict resolution tools to resolve merge conflicts.<br>
***e.g:*** `git mergetool--tool-help` *to list available tools.*<br>
+ **[merge-index](https://git-scm.com/docs/merge-index)** ~ Run a merge for files in the index.<br>
***e.g:*** `git merge-index -o <file>` *to run a merge for files in the index that need merging and write the result to file.*<br>
+ **[git mktag](https://git-scm.com/docs/git-mktag)** ~ Create a tag object.<br>
***e.g:*** `git mktag <file>` *to create a tag object.*<br>
+ **[git mktree](https://git-scm.com/docs/git-mktree)** ~ Build a tree-object from ls-tree formatted text.<br>
***e.g:*** `git mktree <file>` *to build a tree-object from ls-tree formatted text.*<br>
+ **[git mv](https://git-scm.com/docs/git-mv)** ~ Move or rename a file, a directory, or a symlink.<br>
***e.g:*** `git mv <file1> <file2>` *to move or rename file1 to file2.*<br>
+ **[git name-rev](https://git-scm.com/docs/git-name-rev)** ~ Find symbolic names for given revs.<br>
***e.g:*** `git name-rev --all <commit>` *to find symbolic names for given commit.*<br>
+ **[git notes](https://git-scm.com/docs/git-notes)** ~ Add or inspect object notes.<br>
***e.g:*** `git notes add -m "note" <commit>` *to add a note to commit.*<br>
+ **[git pack-objects](https://git-scm.com/docs/git-pack-objects)** ~ Create a packed archive of objects.<br>
***e.g:*** `git pack-objects <file>` *to create a packed archive of objects in file.*<br>



+ **[git pack-redundant](https://git-scm.com/docs/git-pack-redundant)** ~ Find redundant pack files for piping to xargs rm.<br>
***e.g:*** `git pack-redundant --all` *to find redundant pack files for piping to xargs rm.*<br>
+ **[git pack-refs](https://git-scm.com/docs/git-pack-refs)** ~ Pack heads and tags for efficient repository access.<br>
***e.g:*** `git pack-refs --all` *to pack heads and tags that are already packed*<br>
+ **[git patch-id](https://git-scm.com/docs/git-patch-id)** ~ Compute unique ID for a patch.<br>
***e.g:*** `git patch-id <file>` *to compute unique ID for a patch.*<br>
+ **[git prune](https://git-scm.com/docs/git-prune)** ~ Prune all unreachable objects from the object database.<br>
***e.g:*** `git prune` *to prune all unreachable objects from the object database.*<br>
+ **[git prune-packed](https://git-scm.com/docs/git-prune-packed)** ~ Prune loose objects that are already in pack files.<br>
***e.g:*** `git prune-packed` *to prune loose objects that are already in pack files.*<br>
+ **[git pull](https://git-scm.com/docs/git-pull)** ~ Fetch from and integrate with another repository or a local branch.<br>
***e.g:*** `git pull` *to fetch from and integrate with another repository or a local branch.*<br>
+ **[git push](https://git-scm.com/docs/git-push)** ~ Update remote refs along with associated objects.<br>
***e.g:*** `git push` *to update remote refs along with associated objects.*<br>
+ **[git range-diff](https://git-scm.com/docs/git-range-diff)** ~ Show changes between two commit ranges.<br>
***e.g:*** `git range-diff <file>` *to show changes between two commit ranges.*<br>
+ **[git read-tree](https://git-scm.com/docs/git-read-tree)** ~ Reads tree information into the index.<br>
***e.g:*** `git read-tree <file>` *to read tree information into the index.*<br>
+ **[git rebase](https://git-scm.com/docs/git-rebase)** ~ Reapply commits on top of another base tip.<br>
***e.g:*** `git rebase` *to reapply commits on top of another base tip.*<br>
+ **[git receive-pack](https://git-scm.com/docs/git-receive-pack)** ~ Receive what is pushed into the repository.<br>
***e.g:*** `git receive-pack <file>` *to receive what is pushed into the repository.*<br>
+ **[git reflog](https://git-scm.com/docs/git-reflog)** ~ Manage reflog information.<br>
***e.g:*** `git reflog` *to manage reflog information.*<br>
+ **[git remote](https://git-scm.com/docs/git-remote)** ~ Manage set of tracked repositories.<br>
***e.g:*** `git remote` *to manage set of tracked repositories.*<br>
+ **[git remote-ext](https://git-scm.com/docs/git-remote-ext)** ~ External helper to communicate with a remote repository.<br>
***e.g:*** `git remote-ext <file>` *to communicate with a remote repository.*<br>
+ **[git remote-fd](https://git-scm.com/docs/git-remote-fd)** ~ Helper to communicate with a remote repository.<br>
***e.g:*** `git remote-fd <file>` *to communicate with a remote repository.*<br>
+ **[git repack](https://git-scm.com/docs/git-repack)** ~ Pack unpacked objects in a repository.<br>
***e.g:*** `git repack` *to pack unpacked objects in a repository.*<br>
+ **[git replace](https://git-scm.com/docs/git-replace)** ~ Create, list, delete refs to replace objects.<br>
***e.g:*** `git replace` *to create, list, delete refs to replace objects.*<br>
+ **[git request-pull](https://git-scm.com/docs/git-request-pull)** ~ Generates a summary of pending changes.<br>
***e.g:*** `git request-pull` *to generate a summary of pending changes.*<br>
+ **[git rerere](https://git-scm.com/docs/git-rerere)** ~ Reuse recorded resolution of conflicted merges.<br>
***e.g:*** `git rerere` *to reuse recorded resolution of conflicted merges.*<br>
+ **[git reset](https://git-scm.com/docs/git-reset)** ~ Reset current HEAD to the specified state.<br>
***e.g:*** `git reset` *to reset current HEAD to the specified state.*<br>
+ **[git resolve-undo](https://git-scm.com/docs/git-resolve-undo)** ~ Undo the last cherry-pick, revert or merge.<br>
***e.g:*** `git resolve-undo` *to undo the last cherry-pick, revert or merge.*<br>
+ **[git rev-list](https://git-scm.com/docs/git-rev-list)** ~ Lists commit objects in reverse chronological order.<br>
***e.g:*** `git rev-list` *to list commit objects in reverse chronological order.*<br>
+ **[git rev-parse](https://git-scm.com/docs/git-rev-parse)** ~ Pick out and massage parameters.<br>
***e.g:*** `git rev-parse` *to pick out and massage parameters.*<br>
+ **[git revert](https://git-scm.com/docs/git-revert)** ~ Revert some existing commits.<br>
***e.g:*** `git revert` *to revert some existing commits.*<br>
+ **[git rm](https://git-scm.com/docs/git-rm)** ~ Remove files from the working tree and from the index.<br>
***e.g:*** `git rm` *to remove files from the working tree and from the index.*<br>
+ **[git send-email](https://git-scm.com/docs/git-send-email)** ~ Send a collection of patches as emails.<br>
***e.g:*** `git send-email` *to send a collection of patches as emails.*<br>
+ **[git shortlog](https://git-scm.com/docs/git-shortlog)** ~ Summarize 'git log' output.<br>
***e.g:*** `git shortlog` *to summarize 'git log' output.*<br>
+ **[git show](https://git-scm.com/docs/git-show)** ~ Show various types of objects.<br>
***e.g:*** `git show` *to show various types of objects.*<br>
+ **[git show-branch](https://git-scm.com/docs/git-show-branch)** ~ Show branches and their commits.<br>
***e.g:*** `git show-branch` *to show branches and their commits.*<br>
+ **[git stage](https://git-scm.com/docs/git-stage)** ~ Stage file contents for the next commit.<br>
***e.g:*** `git stage` *to stage file contents for the next commit.*<br>
+ **[git stash](https://git-scm.com/docs/git-stash)** ~ Stash the changes in a dirty working directory away.<br>
***e.g:*** `git stash` *to stash the changes in a dirty working directory away.*<br>
+ **[git status](https://git-scm.com/docs/git-status)** ~ Show the working tree status.<br>
***e.g:*** `git status` *to show the working tree status.*<br>
+ **[git stripspace](https://git-scm.com/docs/git-stripspace)** ~ Remove unnecessary whitespace.<br>
***e.g:*** `git stripspace` *to remove unnecessary whitespace.*<br>
+ **[git submodule](https://git-scm.com/docs/git-submodule)** ~ Initialize, update or inspect submodules.<br>
***e.g:*** `git submodule` *to initialize, update or inspect submodules.*<br>









































+ **[gc](https://git-scm.com/docs/git-gc)** ~ Cleanup unnecessary files and optimize the local repository.<br>
***e.g:*** `git gc` *to optimize the local repository.*<br>



+ **[git rev-parse](https://git-scm.com/docs/git-rev-parse)** ~ Ancillary plumbing command primarily used for manipulation.<br>***e.g:***  `git rev-parse --show-toplevel` to get the root dir. of the repo.




+ **[git reflog](https://git-scm.com/docs/git-reflog)** ~ List of changes to refs. in local repo. E.g: `git reflog` to list all changes.
+ **[git mergetool](https://git-scm.com/docs/git-mergetool)** ~ Used to resolve merge conflicts after merging. <br>***e.g:*** `git mergetool` to open a GUI to resolve conflicts.
+ **[git version](https://git-scm.com/docs/git-version)** ~ Show current version of git without more available options.<br>***e.g:*** `git version` to show current version.
+ **[git instaweb](https://git-scm.com/docs/git-instaweb)** ~ Browse your local working repository in a web server. <br>***e.g:*** `git instaweb --httpd=webrick` to start a web server.
+ **[git fast-import](https://git-scm.com/docs/git-fast-import)** ~ Import large projects min. memory (100k+ commits on avg PC in 1h).
+ **[git remote-helpers](https://git-scm.com/docs/gitremote-helpers) ~ They are used to interact with remote repositories that git does not support natively. e.g, http, https, ftp, etc.
+ **[git filter-branch](https://git-scm.com/docs/git-filter-branch)** ~ History filtering tool, that rewrites branches and commit information. Risks associated by object name rewriting which won't converge to original branch, do not use if you don't know the risks! *filter-repo* is recommended instead.
+ **[git filter-repo](https://github.com/newren/git-filter-repo/)** ~ Rewrite git history with a new repo. It is a faster, safer, and more featureful alternative to git filter-branch.
+ **[git submodule](https://git-scm.com/docs/git-submodule)** ~  Submodule is a git repo inside another git repo. It is used to manage dependencies of a project. e.g `git submodule add <URL> <path>` where `<URL>` is the URL of the repo to be added and `<path>` is the path where the repo will be added.
+ **[git shell](https://github.com/git-utilities/git-shell-commands)** ~ Restricted login shell for git-only SSH access.  The command is the following `git-shell -c '<command>'` where `<command>` is the command to be executed.
+ **git notes** ~ *pending*
+ **git reflog** ~ *pending*
+ **git rev-list** ~ *pending*
+ **git replace** ~ *pending*
+ **git rerere** ~ *pending*
+ **git update-index** ~ *pending*
+ **git bundle** ~ *pending*
+ **git send-email** ~ *pending*
+ **git web-browse** ~ *pending*
+ **git pack-objects** ~ *pending*
+ **git annotate** ~ *pending*
+ **git tar-tree** ~ *pending*
+ **git read-tree** ~ *pending*
+ **git-sh-setup** ~ *pending*
+ **git var** ~ *pending*
+ **git gc** ~ *pending*
+ **git annex** ~ *pending*
+ **git grep** ~ *pending*
+ **git show** ~ *pending*
+ **git exec** ~ *pending*
+ **git tag** ~ *pending*
+ **git whatchanged** ~ *pending*
+ **git show-ref** ~ *pending*
+ **git annex** ~ *pending*
+ **git difftool** ~ *pending*
+ **git receive-pack** ~ *pending*
+ **cg-admin-setuprepo** ~ *pending*
+ **etckeeper** ~ *pending*
+ **perlbrew** ~ *pending*
+ **guilt** ~ *pending*
+ **echo** ~ *pending*
+ **pass** ~ *pending*
+ **mr** ~ *pending*


### References:
**1.** [Git](https://git-scm.com) <br> 
**2.** [*Linux Man*](https://git-scm.com) <br>
**3.** **Official Git Pro** *[ebook](https://git-scm.com/book/en/v2)*. *Chacon,S and Straub, B. (2022).*<br>

<br><br><br><br><br><br>

### &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;*Text-Editor*:&emsp;![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white) 

