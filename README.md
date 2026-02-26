# Git-DevOps

Preparation for gate focusing on git, devops, CI\&CD




User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (main)

$ git config --list --global

user.name=Fuad Jamal

user.email=jamalfuad34@gmail.com

core.autocrlf=true



User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (main)

$ git checkout -b dev

Switched to a new branch 'dev'



User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (dev)

$ git push 

fatal: The current branch dev has no upstream branch.

To push the current branch and set the remote as upstream, use



&nbsp;   git push --set-upstream origin dev



To have this happen automatically for branches without a tracking

upstream, see 'push.autoSetupRemote' in 'git help config'.





User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (dev)

$ git push --set-upstream origin dev

Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)

remote: 

remote: Create a pull request for 'dev' on GitHub by visiting:

remote:      https://github.com/Fuad-Jamal/Git-DevOps/pull/new/dev

remote: 

To https://github.com/Fuad-Jamal/Git-DevOps.git

&nbsp;\* \[new branch]      dev -> dev

branch 'dev' set up to track 'origin/dev'.



User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (dev)

$ git checkout -b test

Switched to a new branch 'test'



User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (test)

$ git switch dev

M       README.md

Switched to branch 'dev'

Your branch is up to date with 'origin/dev'.



User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (dev)

$ 



User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (dev)

$ git switch test

M       README.md

Switched to branch 'test'



User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (test)

$ git push --set-upstream origin test

Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)

remote: 

remote: Create a pull request for 'test' on GitHub by visiting:

remote:      https://github.com/Fuad-Jamal/Git-DevOps/pull/new/test

remote: 

To https://github.com/Fuad-Jamal/Git-DevOps.git

&nbsp;\* \[new branch]      test -> test

branch 'test' set up to track 'origin/test'.



User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (test)

$ git switch dev

M       README.md

Switched to branch 'dev'

Your branch is up to date with 'origin/dev'.



User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (dev)

$ git checkout -d test

M       README.md

HEAD is now at 4175b8f Initial commit



User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps ((4175b8f...))

$ git switch dev

M       README.md

Switched to branch 'dev'

Your branch is up to date with 'origin/dev'.



User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (dev)

$ git branch -d test

Deleted branch test (was 4175b8f).



User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (dev)

$ git push origin --d test

error: ambiguous option: d (could be --delete or --dry-run)

usage: git push \[<options>] \[<repository> \[<refspec>...]]



&nbsp;   -v, --\[no-]verbose    be more verbose

&nbsp;   -q, --\[no-]quiet      be more quiet

&nbsp;   --\[no-]repo <repository>

&nbsp;                         repository

&nbsp;   --\[no-]all            push all branches

&nbsp;   --\[no-]branches       alias of --all

&nbsp;   --\[no-]mirror         mirror all refs

&nbsp;   -d, --\[no-]delete     delete refs

&nbsp;   --\[no-]tags           push tags (can't be used with --all or --branches or --mirror)

&nbsp;   -n, --\[no-]dry-run    dry run

&nbsp;   --\[no-]porcelain      machine-readable output

&nbsp;   -f, --\[no-]force      force updates

&nbsp;   --\[no-]force-with-lease\[=<refname>:<expect>]

&nbsp;                         require old value of ref to be at this value

&nbsp;   --\[no-]force-if-includes

&nbsp;                         require remote updates to be integrated locally

&nbsp;   --\[no-]recurse-submodules (check|on-demand|no)

&nbsp;                         control recursive pushing of submodules

&nbsp;   --\[no-]thin           use thin pack

&nbsp;   --\[no-]receive-pack <receive-pack>

&nbsp;                         receive pack program

&nbsp;   --\[no-]exec <receive-pack>

&nbsp;                         receive pack program

&nbsp;   -u, --\[no-]set-upstream

&nbsp;                         set upstream for git pull/status

&nbsp;   --\[no-]progress       force progress reporting

&nbsp;   --\[no-]prune          prune locally removed refs

&nbsp;   --no-verify           bypass pre-push hook

&nbsp;   --verify              opposite of --no-verify

&nbsp;   --\[no-]follow-tags    push missing but relevant tags

&nbsp;   --\[no-]signed\[=(yes|no|if-asked)]

&nbsp;                         GPG sign the push

&nbsp;   --\[no-]atomic         request atomic transaction on remote side

&nbsp;   -o, --\[no-]push-option <server-specific>

&nbsp;                         option to transmit

&nbsp;   -4, --ipv4            use IPv4 addresses only

&nbsp;   -6, --ipv6            use IPv6 addresses only





User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (dev)

User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (dev)

$ git push origin --delete test

To https://github.com/Fuad-Jamal/Git-DevOps.git

&nbsp;- \[deleted]         test


User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (dev)
$ git checkout -b ft/setup
Switched to a new branch 'ft/setup'

User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (ft/setup)
$ touch test.java

User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (ft/setup)
$ echo #


User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (ft/setup)
$ echo System.out.println("Hello World")
bash: syntax error near unexpected token `('

User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (ft/setup)
$ echo "System.out.println("Hello World")"
System.out.println(Hello World)

User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (ft/setup)
$ echo "System.out.println("Hello World")">
bash: syntax error near unexpected token `newline'

User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (ft/setup)
$ echo "System.out.println("Hello World")"> test.java 


User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (ft/setup)
$ git stash
Saved working directory and index state WIP on ft/setup: 4175b8f Initial commit

User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (ft/setup)
$ git stash -l
error: unknown switch `l'
usage: git stash list [<log-options>]
   or: git stash show [-u | --include-untracked | --only-untracked] [<diff-options>] [<stash>]
   or: git stash drop [-q | --quiet] [<stash>]
   or: git stash pop [--index] [-q | --quiet] [<stash>]
   or: git stash apply [--index] [-q | --quiet] [<stash>]
   or: git stash branch <branchname> [<stash>]
   or: git stash [push [-p | --patch] [-S | --staged] [-k | --[no-]keep-index] [-q | --quiet]
                 [-u | --include-untracked] [-a | --all] [(-m | --message) <message>]
                 [--pathspec-from-file=<file> [--pathspec-file-nul]]
                 [--] [<pathspec>...]]
   or: git stash save [-p | --patch] [-S | --staged] [-k | --[no-]keep-index] [-q | --quiet]
                 [-u | --include-untracked] [-a | --all] [<message>]
   or: git stash clear
   or: git stash create [<message>]
   or: git stash store [(-m | --message) <message>] [-q | --quiet] <commit>

    -k, --[no-]keep-index keep index
    -S, --[no-]staged     stash staged changes only
    -p, --[no-]patch      stash in patch mode
    -q, --[no-]quiet      quiet mode
    -u, --[no-]include-untracked
                          include untracked files in stash
    -a, --[no-]all        include ignore files
    -m, --[no-]message <message>
                          stash message
    --[no-]pathspec-from-file <file>
                          read pathspec from file
    --[no-]pathspec-file-nul
                          with --pathspec-from-file, pathspec elements are separated with NUL character


User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (ft/setup)
$ gist stash list
bash: gist: command not found

User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (ft/setup)
$ git stash list
stash@{0}: WIP on ft/setup: 4175b8f Initial commit

User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (ft/setup)
$ git stash pop stash@{0}
On branch ft/setup
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .idea/
        test.java

no changes added to commit (use "git add" and/or "git commit -a")
Dropped stash@{0} (82fc569c830ab571a63af0a155e779912bac982b)

User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (ft/setup)
$ git add test.java 
warning: in the working copy of 'test.java', LF will be replaced by CRLF the next time Git touches it

User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (ft/setup)
$ git commit -m "feat: Adding a test file with print message"
[ft/setup 3172f0b] feat: Adding a test file with print message
 1 file changed, 1 insertion(+)
 create mode 100644 test.java

User@GisaF23 MINGW64 ~/IdeaProjects/Git-DevOps (ft/setup)
$ git push
fatal: The current branch ft/setup has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/setup

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


$ git push --set-upstream origin ft/setup 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 336 bytes | 336.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'ft/setup' on GitHub by visiting:
remote:      https://github.com/Fuad-Jamal/Git-DevOps/pull/new/ft/setup
remote: 
To https://github.com/Fuad-Jamal/Git-DevOps.git
 * [new branch]      ft/setup -> ft/setup
branch 'ft/setup' set up to track 'origin/ft/setup'.
