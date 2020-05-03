Django Contact Forms
====================================

.. image:: https://img.shields.io/badge/license-MIT-blue.svg?maxAge=2592000
   :target: https://raw.githubusercontent.com/sajib1066/django-contactforms/master/LICENSE

.. image:: https://img.shields.io/pypi/pyversions/Django.svg?maxAge=2592000
   :target: https://github.com/sajib1066/django-contactforms

![msg](https://user-images.githubusercontent.com/39632170/80919242-c64a9000-8d8a-11ea-8b77-23e8d505c607.png)

Install
----------------------

Django Contact Us is available directly from `PyPI`_:

::

    $ pip install django-contactforms


***).** And don't forget to add ``contact_forms`` to your ``INSTALLED_APPS``.


Requirement
----------------------

* ``Django>=3.0.5`


Database Migration
----------------------

::

    $ ./manage.py makemigrations contact_forms
    $ ./manage.py migrate contact_forms





URL configuration
----------------------

The easiest way to set up the views in ``django-contactforms`` is to just use the provided ``URLconf``, found at ``contact_forms.urls``.
You can include it wherever you like in your site's URL configuration; for example, to have it live at the URL ``/contact/``:

::

    from django.urls import path, include

    urlpatterns = [
        # ....
        path('contact/', include('contact_forms.urls')),
    ]


Usage
----------------------

Include the template from ``contact/contact.html`` to your sidebar for example.

::

    {% include "contact/contact.html" %}
 
 License
----------------------

- `MIT`_


.. _PyPI: https://pypi.python.org/pypi/django-contactforms
.. _MIT: https://github.com/sajib1066/django-contactforms/blob/master/LICENSE