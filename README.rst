=====
Gallery
=====

Gallery is a Django app to organize and filter bootstrap cards (eg. ImageCards). Simply define a few categories, upload your images and specify their category. 

Detailed documentation is in the "docs" directory.

Quick start
-----------

1. Add "Gallery" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...,
        "Gallery",
    ]

2. Include the Gallery URLconf in your project urls.py like this::

    path("Gallery/", include("Gallery.urls")),

3. Create a Gallery/ directory in your media folder

4. Add a script_content block, "{% block script_content %}{% endblock %}"  to your parent template (eg. base.html). 

5. Run ``python manage.py makemigrations Gallery``
   And ``python manage.py migrate`` to create the Gallery models for your database.

Notes
-----

May work with other versions of Django but it was created and tested for 4.2