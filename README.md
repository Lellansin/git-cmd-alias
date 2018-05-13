# git command alias

alias like: `g status`  => `git status`

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
|TODO|gdt| git diff-tree --no-commit-id --name-only -r|

## add

|Meaning|CMD|Alias|
|---|---|---|
|**A**dd|ga| git add|
|**A**dd **A**ll|gaa| git add --all|
|**A**dd **Pa**tch|gapa| git add --patch|
|**A**dd **U**pdate|gau| git add --update|
|TODO|gwip| git add -A; git rm $(git ls-files --deleted) 2> /dev/null; |

## commit

|Meaning|CMD|Alias|
|---|---|---|
|TODO|gc| git commit -v|
|TODO|gc!| git commit -v --amend|
|TODO|gca| git commit -v -a|
|TODO|gca!| git commit -v -a --amend|
|TODO|gcam| git commit -a -m|
|TODO|gcan!| git commit -v -a --no-edit --amend|
|TODO|gcans!| git commit -v -a -s --no-edit --amend|
|TODO|gcmsg| git commit -m|
|TODO|gcn!| git commit -v --no-edit --amend|
|TODO|gcs| git commit -S|
|TODO|gcsm| git commit -s -m|

## push

|Meaning|CMD|Alias|
|---|---|---|
|TODO|gp| git push|
|TODO|gpu| git push upstream|
|TODO|gpv| git push -v|
|TODO|gpd| git push --dry-run|
|TODO|ggpush| git push origin $(git_current_branch)|
|TODO|gpoat| git push origin --all && git push origin --tags|
|TODO|gpsup| git push --set-upstream origin $(git_current_branch)|

## pull 

|Meaning|CMD|Alias|
|---|---|---|
|TODO|gl| git pull|
|TODO|glum| git pull upstream master|
|TODO|gup| git pull --rebase|
|TODO|gupv| git pull --rebase -v|
|TODO|ggpull| git pull origin $(git_current_branch)|

## checkout 

|Meaning|CMD|Alias|
|---|---|---|
|TODO|gco| git checkout|
|TODO|gcb| git checkout -b|
|TODO|gcd| git checkout develop|
|TODO|gcm| git checkout master|

## fetch

|Meaning|CMD|Alias|
|---|---|---|
|TODO|gf| git fetch|
|TODO|gfo| git fetch origin|
|TODO|gfa| git fetch --all --prune|


## branch

|Meaning|CMD|Alias|
|---|---|---|
|TODO|gb| git branch|
|TODO|gba| git branch -a|
|TODO|gbd| git branch -d|
|TODO|ggsup| git branch --set-upstream-to=origin/$(git_current_branch)|
|TODO|gbda| git branch --no-color --merged | command grep -vE |
|TODO|gbnm| git branch --no-merged|
|TODO|gbr| git branch --remote|

## remote

|Meaning|CMD|Alias|
|---|---|---|
|TODO|gr| git remote|
|TODO|gra| git remote add|
|TODO|grmv| git remote rename|
|TODO|grrm| git remote remove|
|TODO|grset| git remote set-url|
|TODO|grup| git remote update|
|TODO|grv| git remote -v|

## reset

|Meaning|CMD|Alias|
|---|---|---|
|TODO|gpristine| git reset --hard && git clean -dfx|
|TODO|grh| git reset HEAD|
|TODO|grhh| git reset HEAD --hard|
|TODO|gru| git reset --|
|TODO|gclean| git clean -fd|

## stach

|Meaning|CMD|Alias|
|---|---|---|
|TODO|gsta| git stash save|
|TODO|gstaa| git stash apply|
|TODO|gstc| git stash clear|
|TODO|gstd| git stash drop|
|TODO|gstl| git stash list|
|TODO|gstp| git stash pop|
|TODO|gsts| git stash show --text|

## rebase

|Meaning|CMD|Alias|
|---|---|---|
|TODO|grb| git rebase|
|TODO|grba| git rebase --abort|
|TODO|grbc| git rebase --continue|
|TODO|grbi| git rebase -i"^(\*|\s*(master|develop|dev)\s*$)" | command |
|TODO|grbm| git rebase master|
|TODO|grbs| git rebase --skip|

## merge
gm: git merge
|Meaning|CMD|Alias|
|---|---|---|
|TODO|gma| git merge --abort|
|TODO|gmom| git merge origin/master|
|TODO|gmt| git mergetool --no-promptgit commit --no-verify -m "--wip-- [|
|TODO|gmtvim| git mergetool --no-prompt --tool=vimdiff|
|TODO|gmum| git merge upstream/master|

## log

|Meaning|CMD|Alias|
|---|---|---|
|TODO|glg| git log --stat|
|TODO|glgg| git log --graph|
|TODO|glgga| git log --graph --decorate --all|
|TODO|glgm| git log --graph --max-count=10|
|TODO|glgp| git log --stat -p|
|TODO|glo| git log --oneline --decorate|
|TODO|glog| git log --oneline --decorate --graph|
|TODO|gloga| git log --oneline --decorate --graph --all|
|TODO|glol| git log --graph --pretty='%Cred%h%Creset -%C(|
|TODO|glola| git log --graph --pretty='%Cred%h%Creset -%C(|
|TODO|gunwip| git log -n 1 | grep -q -c "\-\-wip\-\-" && git reset |

## bisect

|Meaning|CMD|Alias|
|---|---|---|
|TODO|gbs| git bisect|
|TODO|gbsb| git bisect bad|
|TODO|gbsg| git bisect good|
|TODO|gbsr| git bisect reset|
|TODO|gbss| git bisect start|

## svn

|Meaning|CMD|Alias|
|---|---|---|
|TODO|gsr| git svn rebase|
|TODO|gsd| git svn dcommit|
|TODO|git-svn-dcommit-push| git svn dcommit && git push github master:svntrunk|