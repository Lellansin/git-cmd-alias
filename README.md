# git command alias

alias like: `g status`  => `git status`

Provide by zsh defaultly.

## status

|Meaning|cmd|alias|
|---|---|---|
|**St**atus|gst|git status|
|**S**tatus **S**imple)|gss|git status -s|
|status **S**imple with **B**ranch|gsb|git status -sb|

## diff

|Meaning|CMD|Alias|
|---|---|---|
|**D**iff (didn't add)|gd| git diff|
|**D**iff by **W**ord|gdw| git diff --word-diff|
|**D**iff **Ca**ched (didn't commit)|gdca| git diff --cached|
|**D**iff **Ca**ched by **W**ord|gdcw| git diff --cached --word-diff|
|-|gdt| git diff-tree --no-commit-id --name-only -r|

## add

|Meaning|CMD|Alias|
|---|---|---|
|**A**dd|ga| git add|
|**A**dd **A**ll|gaa| git add --all|
|**A**dd **Pa**tch|gapa| git add --patch|
|**A**dd **U**pdate|gau| git add --update|
|-|gwip| git add -A; git rm $(git ls-files --deleted) 2> /dev/null; |

## commit

|Meaning|CMD|Alias|
|---|---|---|
|-|gc| git commit -v|
|-|gc!| git commit -v --amend|
|-|gca| git commit -v -a|
|-|gca!| git commit -v -a --amend|
|-|gcam| git commit -a -m|
|-|gcan!| git commit -v -a --no-edit --amend|
|-|gcans!| git commit -v -a -s --no-edit --amend|
|-|gcmsg| git commit -m|
|-|gcn!| git commit -v --no-edit --amend|
|-|gcs| git commit -S|
|-|gcsm| git commit -s -m|

## push

|Meaning|CMD|Alias|
|---|---|---|
|-|gp| git push|
|-|gpu| git push upstream|
|-|gpv| git push -v|
|-|gpd| git push --dry-run|
|-|ggpush| git push origin $(git_current_branch)|
|-|gpoat| git push origin --all && git push origin --tags|
|-|gpsup| git push --set-upstream origin $(git_current_branch)|

## pull 

|Meaning|CMD|Alias|
|---|---|---|
|-|gl| git pull|
|-|glum| git pull upstream master|
|-|gup| git pull --rebase|
|-|gupv| git pull --rebase -v|
|-|ggpull| git pull origin $(git_current_branch)|

## checkout 

|Meaning|CMD|Alias|
|---|---|---|
|-|gco| git checkout|
|-|gcb| git checkout -b|
|-|gcd| git checkout develop|
|-|gcm| git checkout master|

## fetch

|Meaning|CMD|Alias|
|---|---|---|
|-|gf| git fetch|
|-|gfo| git fetch origin|
|-|gfa| git fetch --all --prune|


## branch

|Meaning|CMD|Alias|
|---|---|---|
|-|gb| git branch|
|-|gba| git branch -a|
|-|gbd| git branch -d|
|-|ggsup| git branch --set-upstream-to=origin/$(git_current_branch)|
|-|gbda| git branch --no-color --merged | command grep -vE |
|-|gbnm| git branch --no-merged|
|-|gbr| git branch --remote|

## remote

|Meaning|CMD|Alias|
|---|---|---|
|-|gr| git remote|
|-|gra| git remote add|
|-|grmv| git remote rename|
|-|grrm| git remote remove|
|-|grset| git remote set-url|
|-|grup| git remote update|
|-|grv| git remote -v|

## reset

|Meaning|CMD|Alias|
|---|---|---|
|-|gpristine| git reset --hard && git clean -dfx|
|-|grh| git reset HEAD|
|-|grhh| git reset HEAD --hard|
|-|gru| git reset --|
|-|gclean| git clean -fd|

## stach

|Meaning|CMD|Alias|
|---|---|---|
|-|gsta| git stash save|
|-|gstaa| git stash apply|
|-|gstc| git stash clear|
|-|gstd| git stash drop|
|-|gstl| git stash list|
|-|gstp| git stash pop|
|-|gsts| git stash show --text|

## rebase

|Meaning|CMD|Alias|
|---|---|---|
|-|grb| git rebase|
|-|grba| git rebase --abort|
|-|grbc| git rebase --continue|
|-|grbi| git rebase -i"^(\*|\s*(master|develop|dev)\s*$)" | command |
|-|grbm| git rebase master|
|-|grbs| git rebase --skip|

## merge
gm: git merge
|Meaning|CMD|Alias|
|---|---|---|
|-|gma| git merge --abort|
|-|gmom| git merge origin/master|
|-|gmt| git mergetool --no-promptgit commit --no-verify -m "--wip-- [|
|-|gmtvim| git mergetool --no-prompt --tool=vimdiff|
|-|gmum| git merge upstream/master|

## log

|Meaning|CMD|Alias|
|---|---|---|
|-|glg| git log --stat|
|-|glgg| git log --graph|
|-|glgga| git log --graph --decorate --all|
|-|glgm| git log --graph --max-count=10|
|-|glgp| git log --stat -p|
|-|glo| git log --oneline --decorate|
|-|glog| git log --oneline --decorate --graph|
|-|gloga| git log --oneline --decorate --graph --all|
|-|glol| git log --graph --pretty='%Cred%h%Creset -%C(|
|-|glola| git log --graph --pretty='%Cred%h%Creset -%C(|
|-|gunwip| git log -n 1 | grep -q -c "\-\-wip\-\-" && git reset |

## bisect

|Meaning|CMD|Alias|
|---|---|---|
|-|gbs| git bisect|
|-|gbsb| git bisect bad|
|-|gbsg| git bisect good|
|-|gbsr| git bisect reset|
|-|gbss| git bisect start|

## svn

|Meaning|CMD|Alias|
|---|---|---|
|-|gsr| git svn rebase|
|-|gsd| git svn dcommit|
|-|git-svn-dcommit-push| git svn dcommit && git push github master:svntrunk|

