QUESTÃO 1 - Após criado a sua conta no GitHub, crie um repositório remoto público chamado “my_first_steps” e cole o link aqui:

https://github.com/tiagooogomes/my_first_steps


QUESTÃO 2 - Crie um diretório em sua máquina e o vincule ao seu repositório remoto “my_first_steps” utilizando os comandos git necessários para a realização desta tarefa.

Cole aqui a cadeia de comandos que você utilizou para a realização desta tarefa:

Tiago@Tiago-WIN MINGW32 ~
$ cd desktop

Tiago@Tiago-WIN MINGW32 ~/desktop
$ mkdir atividade

Tiago@Tiago-WIN MINGW32 ~/desktop
$ dc atividade
bash: dc: command not found

Tiago@Tiago-WIN MINGW32 ~/desktop
$ cd atividade/

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade
$ git init
Initialized empty Git repository in C:/Users/Tiago/Desktop/atividade/.git/

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (master)
$ ls

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (master)
$ git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (master)
$ git branch -M main

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ git remote add origin https://github.com/tiagooogomes/my_first_steps.git

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ git remote -v
origin  https://github.com/tiagooogomes/my_first_steps.git (fetch)
origin  https://github.com/tiagooogomes/my_first_steps.git (push)

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$



QUESTÃO 3 - Dentro do diretório em sua máquina, crie um arquivo chamado “ola_mundo.txt”, adicione algum texto da sua preferência e adicione-o ao seu repositório remoto utilizando os comandos git necessários para a realização desta tarefa. 

Cole aqui a cadeia de comandos que você utilizou para a realização desta tarefa:

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ touch ola_mundo.txt

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ cat >> ola_mundo.txt
Praticando Atividade :0 :


Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ cat > ola_mundo.txt
Atividade


Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ cat ola_mundo.txt
Atividade

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        ola_mundo.txt

nothing added to commit but untracked files present (use "git add" to track)

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ git add .
warning: LF will be replaced by CRLF in ola_mundo.txt.
The file will have its original line endings in your working directory

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   ola_mundo.txt

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ git commit -m "Criei ola_mundo.txt"
[main (root-commit) 160fb80] Criei ola_mundo.txt
 1 file changed, 1 insertion(+)
 create mode 100644 ola_mundo.txt

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ git status
On branch main
nothing to commit, working tree clean


Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 237 bytes | 26.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/tiagooogomes/my_first_steps.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$



QUESTÃO 4 - Se não existir em seu diretório, adicione ao seu diretório um arquivo com o nome de “.gitignore”. Em seguida, crie um arquivo chamado “serei_ignorado.txt” e adicione algum texto dentro dele. Adicione a instrução ao arquivo “.gitignore” para que as alterações realizadas no arquivo “serei_ignorado.txt” não seja controlado pelo git. 

Cole aqui o conteúdo que você utilizou no “.gitignore” para realizar esta tarefa:

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ touch .gitignore

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ ls
ola_mundo.txt

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ ls -a
./  ../  .git/  .gitignore  ola_mundo.txt

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ touch serei_ignorado.txt

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ cat > serei_ignorado.txt
Testando isso

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ cat serei_ignorado.txt
Testando isso

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore
        serei_ignorado.txt

nothing added to commit but untracked files present (use "git add" to track)

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ echo serei_ignorado.txt >> .gitignore

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ cat .gitignore
serei_ignorado.txt

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)

Tiago@Tiago-WIN MINGW32 ~/desktop/atividade (main)
