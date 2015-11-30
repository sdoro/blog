
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

# setup project

    django-admin.py startproject diangoblog
    cd diangoblog/
    # edit diangoblog/settings.py (DATABASES, TIME_ZONE, LANGUAGE_CODE, TEMPLATE_DIRS)
    MY_TEMPLATE=/home/ubuntu/workspace/template
    mkdir $MYTEMPLATE
    ./manage.py syncdb (admin/root)
    # edit diangoblog/urls.py
    pip install django-tagging
    ./manage.py startapp blog
    # edit blog/models.py
    # create/edit blog/admin.py
    git add ../README.md diangoblog
    git commit -m "Setup app."
    git push
