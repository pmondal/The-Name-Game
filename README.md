# The Name Game

## Add your name

Fork this repository to your github account.

Clone your fork to your local machine

    git clone git@github.com:YOUR_GITHUB_USERNAME/The-Name-Game.git

Create a feature branch to add your name: `git checkout -b name-feature`

Change `names.txt` and add your name to the end of the list on a new line.

Stage the file to be committed. `git add names.text`

Commit your change

    git commit -m "Added YOUR_NAME to the list of names."

Push your branch to github

    git push origin name-feature

## Merge your list

Add a teammate's fork so you can pull their code (substitute their github username).

    git remote add jbrown git@github.com:jbrown/The-Name-Game.git

See what is in their repository.

    git fetch jbrown
    # see what branches you now have
    # anything under remotes/ is a full copy of a remote branch.
    git branch -a

Rebase their commits into your feature branch. ()

    git rebase jbrown/name-feature

Resolve a merge conflict. In this case you want to keep all the names so just remove the lines added by the merge.

    Frank
    YOUR_NAME

Tell git the conflict has been resolved.

    git add names.txt
    git rebase --continue
