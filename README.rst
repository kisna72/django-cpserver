Requirements
============
CherryPy_

.. _CherryPy: http://www.cherrypy.org/

Installation
============

1. Put ``django_cpserver`` on your ``PYTHONPATH``.
2. Add ``django_cpserver`` to your ``INSTALLED_APPS``.

Usage
=====

Run ``./manage.py runcpserver help`` from within your project directory

Serving Static Content
=======================

To serve out static content from your django app, be sure to add the static url as shown below in your urls.py file. 

::

	urlpatterns = patterns('',
	    
	    # url(r'^$', 'django_server.views.home', name='home'),
	) + static(settings.STATIC_URL, document_root=settings.STATIC_ROOT)


Acknowledgements
================

Idea and code snippets borrowed from `Loic d'Anterroches`__, adapted to run as a management command

__ http://www.xhtml.net/scripts/Django-CherryPy-server-DjangoCerise