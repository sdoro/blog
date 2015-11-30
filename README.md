
# init repository

    # make a github.com/sdoro repository
    # make a c9.io workspace referencing github.com/sdoro
    # make/edit README.md
    git add README.md
    git commit -m "Add README.md"
    git push -u origin master

# install django

    # make requirements.txt
    virtualenv $HOME/.env
    source $HOME/.env/bin/activate
    pip install -r requirements.txt
    git add README.md requirements.txt
    git commit -m "Add django requirements."
    git push

