# jacascript-pratica-pull-requests
Faça nesse repositório as práticas de Pull Requests com o seu time.

Como resolver tretas:

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (main)
$ git branch develop-brunosantos

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (main)
$ git switch develop-brunosantos
Switched to branch 'develop-brunosantos'

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git config user.name "bruno santos"

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git config user.email "brunoleite42808@gmail.com"

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git add .

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git pull
From https://github.com/2023-2S-SENAI-SP-FE/jacascript-pratica-pull-requests
 * [new branch]      develop-caio  -> origin/develop-caio
 * [new branch]      develop-sauer -> origin/develop-sauer
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> develop-brunosantos


Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git fetch

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git commit -m "Branch"
On branch develop-brunosantos
nothing to commit, working tree clean

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git push
fatal: The current branch develop-brunosantos has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin develop-brunosantos

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git commit -m "Branch"
On branch develop-brunosantos
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Saturno.html

nothing added to commit but untracked files present (use "git add" to track)

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git add .

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git commit -m "Branch"
[develop-brunosantos 4a59cf6] Branch
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 Saturno.html

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git push
fatal: The current branch develop-brunosantos has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin develop-brunosantos

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git pull
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 660 bytes | 7.00 KiB/s, done.
From https://github.com/2023-2S-SENAI-SP-FE/jacascript-pratica-pull-requests
   afc150d..5bfbdbe  develop-ren -> origin/develop-ren
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> develop-brunosantos


Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git push
fatal: The current branch develop-brunosantos has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin develop-brunosantos

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git push -u <remote> <branch>
bash: syntax error near unexpected token `<'

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git push -u JACASCRIPT-PRATICA-PULL-REQUESTS develop-brunosantos
fatal: 'JACASCRIPT-PRATICA-PULL-REQUESTS' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git push -set -upstream origin develop-brunosantos
error: did you mean `--set` (with two dashes)?

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git push --set -upstream origin develop-brunosantos
error: unknown switch `p'
usage: git push [<options>] [<repository> [<refspec>...]]

    -v, --verbose         be more verbose
    -q, --quiet           be more quiet
    --repo <repository>   repository
    --all                 push all refs
    --mirror              mirror all refs
    -d, --delete          delete refs
    --tags                push tags (can't be used with --all or --mirror)
    -n, --dry-run         dry run
    --porcelain           machine-readable output
    -f, --force           force updates
    --force-with-lease[=<refname>:<expect>]
                          require old value of ref to be at this value
    --force-if-includes   require remote updates to be integrated locally
    --recurse-submodules (check|on-demand|no)
                          control recursive pushing of submodules
    --thin                use thin pack
    --receive-pack <receive-pack>
                          receive pack program
    --exec <receive-pack>
                          receive pack program
    -u, --set-upstream    set upstream for git pull/status
    --progress            force progress reporting
    --prune               prune locally removed refs
    --no-verify           bypass pre-push hook
    --follow-tags         push missing but relevant tags
    --signed[=(yes|no|if-asked)]
                          GPG sign the push
    --atomic              request atomic transaction on remote side
    -o, --push-option <server-specific>
                          option to transmit
    -4, --ipv4            use IPv4 addresses only
    -6, --ipv6            use IPv6 addresses only


Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git fetch
remote: Enumerating objects: 12, done.
remote: Counting objects: 100% (12/12), done.
remote: Compressing objects: 100% (11/11), done.
remote: Total 11 (delta 2), reused 9 (delta 0), pack-reused 0
Unpacking objects: 100% (11/11), 1.42 KiB | 4.00 KiB/s, done.
From https://github.com/2023-2S-SENAI-SP-FE/jacascript-pratica-pull-requests
   afc150d..af9e6c1  develop-caio    -> origin/develop-caio
   afc150d..d07cb0f  develop-fabio   -> origin/develop-fabio
 * [new branch]      develop-felipe  -> origin/develop-felipe
 * [new branch]      develop-ingridy -> origin/develop-ingridy
   afc150d..733c2c2  develop-sauer   -> origin/develop-sauer

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git add .

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git commit -m "Branch"
On branch develop-brunosantos
nothing to commit, working tree clean

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git push
fatal: The current branch develop-brunosantos has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin develop-brunosantos

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)
$ git push --set-upstream origin develop-brunosantos
info: please complete authentication in your browser...
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 281 bytes | 40.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'develop-brunosantos' on GitHub by visiting:
remote:      https://github.com/2023-2S-SENAI-SP-FE/jacascript-pratica-pull-requests/pull/new/develop-brunosantos
remote:
To https://github.com/2023-2S-SENAI-SP-FE/jacascript-pratica-pull-requests.git
 * [new branch]      develop-brunosantos -> develop-brunosantos
branch 'develop-brunosantos' set up to track 'origin/develop-brunosantos'.

Aluno@ESN113D1156979 MINGW64 ~/jacascript-pratica-pull-requests (develop-brunosantos)