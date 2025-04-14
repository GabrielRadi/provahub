# provahub
Gabriel Criou o Repositório

Gabriel Git Bash

gabri@Gabriel MINGW64 ~
$
gabri@Gabriel MINGW64 ~
$
bash: gabri@Gabriel: command not found

bash: $: command not found

gabri@Gabriel MINGW64 ~
$

gabri@Gabriel MINGW64 ~
$ ls -al ~/.ssh
total 33
drwxr-xr-x 1 gabri 197609    0 Apr  7 19:40 ./
drwxr-xr-x 1 gabri 197609    0 Apr  8 21:48 ../
-rw-r--r-- 1 gabri 197609 3401 Apr  7 19:40 id_rsa
-rw-r--r-- 1 gabri 197609  758 Apr  7 19:40 id_rsa.pub
-rw-r--r-- 1 gabri 197609  828 Mar 31 19:45 known_hosts
-rw-r--r-- 1 gabri 197609   92 Mar 31 19:45 known_hosts.old

gabri@Gabriel MINGW64 ~
$ rm -f ~/.ssh/id_rsa*

gabri@Gabriel MINGW64 ~
$ ^C

gabri@Gabriel MINGW64 ~
$ ls -al ~/.ssh
total 25
drwxr-xr-x 1 gabri 197609   0 Apr 14 18:54 ./
drwxr-xr-x 1 gabri 197609   0 Apr  8 21:48 ../
-rw-r--r-- 1 gabri 197609 828 Mar 31 19:45 known_hosts
-rw-r--r-- 1 gabri 197609  92 Mar 31 19:45 known_hosts.old

gabri@Gabriel MINGW64 ~
$ ssh-keygen -t rsa -b 4096 -C "gabrielpaz@edu.unifil.br"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/gabri/.ssh/id_rsa):
Enter passphrase for "/c/Users/gabri/.ssh/id_rsa" (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/gabri/.ssh/id_rsa
Your public key has been saved in /c/Users/gabri/.ssh/id_rsa.pub
The key fingerprint is:
SHA256:8gyu7a7HEhz4bjDrQ8aA69bld4P3et7prTcWG94PD+U gabrielpaz@edu.unifil.br

gabri@Gabriel MINGW64 ~
$ eval "$(ssh-agent -s)"
Agent pid 942

gabri@Gabriel MINGW64 ~
$ ssh-add ~/.ssh/id_rsa
Identity added: /c/Users/gabri/.ssh/id_rsa (gabrielpaz@edu.unifil.br)

gabri@Gabriel MINGW64 ~
$ clip < ~/.ssh/id_rsa.pub

gabri@Gabriel MINGW64 ~
$ ssh -T git@github.com
Hi GabrielRadi! You've successfully authenticated, but GitHub does not provide shell access.

gabri@Gabriel MINGW64 ~
$ clone git@github.com:GabrielRadi/provahub.git
bash: clone: command not found

gabri@Gabriel MINGW64 ~
$ git clone git@github.com:GabrielRadi/provahub.git
Cloning into 'provahub'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (6/6), done.

gabri@Gabriel MINGW64 ~
$

Aborting commit due to empty commit message.

gabri@Gabriel MINGW64 ~/provahub (main)
$ git commit -m "adicionado portugol inicial com a função de pedir o nome do usuario"
[main 1d34ff2] adicionado portugol inicial com a função de pedir o nome do usuario
 1 file changed, 7 insertions(+)
 create mode 100644 "Sem t\303\255tulo (7).por"

gabri@Gabriel MINGW64 ~/provahub (main)
$

gabri@Gabriel MINGW64 ~/provahub (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 412 bytes | 412.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:GabrielRadi/provahub.git
   fcd2543..1d34ff2  main -> main

gabri@Gabriel MINGW64 ~/provahub (main)
$

Eduardo Git Bash

eduar@NotebookEdu MINGW64 ~/OneDrive/Desktop/trabalho git
$ git clone git@github.com:GabrielRadi/provahub.git
Cloning into 'provahub'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (6/6), done.

eduar@NotebookEdu MINGW64 ~/OneDrive/Desktop/trabalho git/provahub (main)
$ git pull
remote: Enumerating objects: 8, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 6 (delta 0), reused 3 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (6/6), 2.37 KiB | 115.00 KiB/s, done.
From github.com:GabrielRadi/provahub
   fcd2543..722a97d  main       -> origin/main
Updating fcd2543..722a97d
Fast-forward
 README.md                   | 105 ++++++++++++++++++++++++++++++++++++++++++++
 "Sem t\303\255tulo (7).por" |   7 +++
 2 files changed, 112 insertions(+)
 create mode 100644 "Sem t\303\255tulo (7).por"

eduar@NotebookEdu MINGW64 ~/OneDrive/Desktop/trabalho git/provahub (main)
$ git add .
warning: in the working copy of 'Sem título (7).por', LF will be replaced by CRLF the next time Git touches it

eduar@NotebookEdu MINGW64 ~/OneDrive/Desktop/trabalho git/provahub (main)
$ git commit -m "Adicionado idade"
[main 572d882] Adicionado idade
 1 file changed, 16 insertions(+), 1 deletion(-)

eduar@NotebookEdu MINGW64 ~/OneDrive/Desktop/trabalho git/provahub (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 656 bytes | 656.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:GabrielRadi/provahub.git
   722a97d..572d882  main -> main


Otávio git bash


compuni@maker40 MINGW64 ~/Desktop/Prova git
$ git clone
fatal: You must specify a repository to clone.

usage: git clone [<options>] [--] <repo> [<dir>]

    -v, --verbose         be more verbose
    -q, --quiet           be more quiet
    --progress            force progress reporting
    --reject-shallow      don't clone shallow repository
    -n, --no-checkout     don't create a checkout
    --bare                create a bare repository
    --mirror              create a mirror repository (implies bare)
    -l, --local           to clone from a local repository
    --no-hardlinks        don't use local hardlinks, always copy
    -s, --shared          setup as shared repository
    --recurse-submodules[=<pathspec>]
                          initialize submodules in the clone
    --recursive ...       alias of --recurse-submodules
    -j, --jobs <n>        number of submodules cloned in parallel
    --template <template-directory>
                          directory from which templates will be used
    --reference <repo>    reference repository
    --reference-if-able <repo>
                          reference repository
    --dissociate          use --reference only while cloning
    -o, --origin <name>   use <name> instead of 'origin' to track upstream
    -b, --branch <branch>
                          checkout <branch> instead of the remote's HEAD
    -u, --upload-pack <path>
                          path to git-upload-pack on the remote
    --depth <depth>       create a shallow clone of that depth
    --shallow-since <time>
                          create a shallow clone since a specific time
    --shallow-exclude <revision>
                          deepen history of shallow clone, excluding rev
    --single-branch       clone only one branch, HEAD or --branch
    --no-tags             don't clone any tags, and make later fetches not to follow them
    --shallow-submodules  any cloned submodules will be shallow
    --separate-git-dir <gitdir>
                          separate git dir from working tree
    -c, --config <key=value>
                          set config inside the new repository
    --server-option <server-specific>
                          option to transmit
    -4, --ipv4            use IPv4 addresses only
    -6, --ipv6            use IPv6 addresses only
    --filter <args>       object filtering
    --remote-submodules   any cloned submodules will use their remote-tracking branch
    --sparse              initialize sparse-checkout file to include only files at root



compuni@maker40 MINGW64 ~/provahub (main)
$ git pull
Already up to date.

compuni@maker40 MINGW64 ~/provahub (main)
$ git add .

compuni@maker40 MINGW64 ~/provahub (main)
$ git commit -m "verificação de idade"
[main 31129cd] verificação de idade
 1 file changed, 5 insertions(+), 2 deletions(-)

compuni@maker40 MINGW64 ~/provahub (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 424 bytes | 424.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:GabrielRadi/provahub.git
   68e1cfd..31129cd  main -> main
