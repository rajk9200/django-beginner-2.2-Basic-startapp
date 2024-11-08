New Project

install python 3.7
pip install django 2.2
pip install pillow


bootstrap download link
    css
    js
animate.css link

font-awesome css link



Commands:
    django-admin startproject new_project

new_project
    +new_project
        -__init__.py
        -setting.py
        -urls.py
        -views.py
        -wsgi.py
    *manage.py
    *db.sqlite3

+templates
    +include
        -base.html
        -header.html
        -footer.html
    -index.html

+static
    +css
        -style.css
        -bootstrap.css
        -animate.css
    +js
        -bootsrap.js
        -jquery.js
    +images
        -fevicon.png
        -avtar.jgp

+media
    -default.jpg




#For code for set media Images
new_project/urls.py
-url.py
from django.conf import settings
from django.conf.urls.static import static

[

]+ static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)




new_project/setting.py
-setting.py
STATIC_URL = '/static/'

STATICFILES_DIRS = [
    os.path.join(BASE_DIR, "static"),
]

MEDIA_ROOT = os.path.join(BASE_DIR, 'media')
MEDIA_URL = '/media/'




#code for setup templates
 paste code inside of templates = [] section

        'DIRS': [os.path.join(BASE_DIR, 'templates')],



 CSS:
    for decorate our website

 understands Line:
 {% extends 'includes/base.html'%}
    #this line mean it's extends base.html file which all data also include with us

 {% block content %}
    This is partition of code its change every page different basically it's Chageable part it's
    always end like
 {% endblock %}
