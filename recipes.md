1. Crie um repositório publico 'tst1' com um readme
    
    Vá ao site do github pela url  
      https://github.com/new
    
    (se voce nao tem uma conta lá, crie! eh gratis!)

    - Use o nome *tst1*

    - Lembre-se de assinalar o checkbox 'Add a README file'

2. Copie para sua máquina

    git clone https://github.com/<seu_usuario>/tst1.git

    Para mim: 
      https://github.com/sergiorgiraldo/tst1.git

3. Crie um arquivo foo.txt

    echo foo.txt > foo.txt | notepad foo.txt

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
    
    git status
    
    git push

    **ou**

    git reset --hard HEAD^ | git reset --hard HEAD~ | git reset --hard 658e438

    git push -f
    
    ---
    
    to see everyhing
    
    git reflog show head
    
    git reflog show master
    
    ---
    
    to remove stuff **added** and not committed
    
    git reset
    
    ---
    
    to remove stuff **not added** (it will delete!)
    
    git clean -f

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

12. git log --format="%H" foo.txt

    git blame foo.txt

    git show 057921c

    git show 057921c08ca3ac126df9a5fa921dc54767db1a55:foo.txt

    git show f759cf8197e2c9ef62bdde8371975d78e2a54d39:foo.txt

    git diff f759cf:foo.txt 057921:foo.txt

13. git clone <url do repositório>

	git fetch --all (isto traz todos os metadados do remote localmente, se há novas branches este comando trará as referencias)

	git pull (traz os arquivos localmente)	

14. aliases (.gitconfig)

    powershell g, gg ($PROFILE)

    signing commits

    ctrl r
