1. Crie um repositório 'tst1' com um readme
    
    https://github.com/new
    https://github.com/sergiorgiraldo/tst1.git

2. Copie para sua máquina

    git clone https://github.com/sergiorgiraldo/tst1.git

3. Crie um arquivo foo.txt

    echo foo.txt > foo.txt

    git add foo.txt

    git commit -m "my first file"

    git push

    Crie outros arquivos e adicione

4. git branch --all

    git branch newstuff

    git checkout newstuff

    **ou**

    git checkout -b anotherstuff

5. git status

    git log

    git log --all

    git log --all --oneline --abbrev-commit --graph

    git log --all --oneline --abbrev-commit --graph --decorate

    git log --all --oneline --abbrev-commit --graph  --decorate --color

    git show <commit id>

6. notepad baz.txt

    git add baz.txt, git commit -m "text file for tests", git push

    notepad baz.txt

    git diff baz.txt

 7. notepad baz.txt

    git checkout baz.txt

    notepad baz.txt

    git add baz.txt, git commit -m "i will regret this"

    git reset --hard HEAD^

8.  notepad baz.txt

    git add baz.txt, git commit -m "i will regret this", git push

    git revert 658e438

    **ou**

    git reset --hard HEAD^

    git push -f

9. notepad baz.txt

    git stash

    git stash list

    git stash show

    git stash show -p

    git stash apply

    git stash save "not bold enough"

10. git checkout newstuff

    notepad readme.md, adicione uma linha nova 'new line'

    git add, commit, push origin newstuff

    git checkout master

    git merge newstuff

    veja o arquivo readme.md com a linha nova

    git push origin master

    git log

11. git checkout master

    notepad readme.md, troque 'linha nova' por 'ideia nova'

    git add, commit, push origin master

    git checkout newstuff

    notepad readme.md, troque 'linha nova' por 'fatia nova'

    git add, commit, push origin newstuff

    git checkout master

    git merge newstuff

    para ver os conflitos: git diff --name-only --diff-filter=U

    notepad readme.md, decida qual o certo

    git add, commit, push

12. aliases (.gitconfig)

    powershell g, gg ($PROFILE)

    signing commits

    ctrl r

