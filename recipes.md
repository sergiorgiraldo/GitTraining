1. https://github.com/new
    https://github.com/sergiorgiraldo/tst1.git

2. git clone https://github.com/sergiorgiraldo/tst1.git

3. echo foo > foo

    git add foo

    git commit -m "my first file"

    git push

4. git branch --all

    git branch newstuff

    git checkout newstuff

    **ou**

    git checkout -b anotherstuff

5. git status

    git log

    git log --all

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