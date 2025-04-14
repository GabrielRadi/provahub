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

