# The Name Game

## Add your name

1. Fork this repository to your github account.
2. Clone your fork to your local machine `git clone git@github.com:YOUR_GITHUB_USERNAME/The-Name-Game.git`
3. Create a feature branch to add your name: `git checkout -b name-feature`
4. Change `names.txt` and add your name to the end of the list on a new line.
5. Stage the file to be committed. `git add names.text`
6. Commit your change `git commit -m "Added YOUR_NAME to the list of names."`
7. Push your branch to github `git push origin name-feature`

## Complete your list

1. Add a teammate's fork so you can pull their code (substitute their github username).

    git remote add USERNAME git@github.com:USERNAME/The-Name-Game.git

2. See what is in their repository.

    git fetch USERNAME

    _see what branches you now have_

    _anything under remotes/ is a full copy of a remote branch._

    git branch -a

3. Rebase their commits into your feature branch. ()

    git rebase USERNAME/name-feature

4. Resolve a merge conflict. In this case you want to keep all the names so just remove the lines added by the merge.

    Frank

    YOUR_NAME

5. Tell git the conflict has been resolved.

    git add names.txt
    git rebase --continue

6. Push your updated branch to your github fork

    git push origin name-feature

7. Repeat for each teammate until you have the full list.