========================
dskel - django project skel
========================

A project template for Django 1.5.4

Working Environment
===================
Recommended:
Using virtualenv to separate the dependencies of your project from your system's
python environment. 
First, install virtualenv (http://www.virtualenv.org). 

    $ virtualenv env_name

You will also need to ensure that the virtualenv has the project directory
added to the path. 

Installing Django
=================

To install Django in the new virtual environment, run the following command::

    $ pip install django==1.5.4 #specific version

Creating your project
=====================

To create a new Django project called '**project_name**' using
the skeleton, run the following command::

    $ django-admin.py startproject --template=https://github.com/varsovia/dskel/archive/master.zip --extension=py,rst,html project_name

Installation of Dependencies
=============================

Depending on where you are installing dependencies:

In development::

    $ pip install -r requirements/local.txt

For production::

    $ pip install -r requirements.txt

Also, download bootstrap3_, jquery. Put directories/files in corresponding folder.
Modify accordly, in templates/base.html.
specific files: 

	$ static/js/bootstrap.min.js	#(v3.0.0)
	$ static/css/bootstrap.min.css 	#(Bootstrap v3.0.0)
	$ static/js/jquery.js			#(jquery 2.0.2)

jQuery_ 2.x has the same API as jQuery 1.x, but does not support Internet Explorer 6, 7, or 8. All the notes in the jQuery 1.9 Upgrade Guide apply here as well. Since IE 6/7/8 are still relatively common, we recommend using the 1.x version unless you are certain no IE 6/7/8 users are visiting the site. Please read the 2.0 release notes carefully.
For production, remember use minified versions instead devel.

Acknowledgements
================

- Many thanks to django community.
- All of the contributors_ to this project (if applicable).

.. _contributors: path_to_constributors/CONTRIBUTORS.txt
.. _jQuery: http://code.jquery.com/jquery-2.0.2.js
.. _bootstrap3: https://github.com/twbs/bootstrap/archive/v3.0.0.zip
