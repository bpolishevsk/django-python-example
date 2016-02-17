=====
Polls
=====

Polls is a simple Django app to conduct Web-based polls. For each
question, visitors can choose between a fixed number of answers.

.. figure:: https://raw.github.com/macagua/django192-tutorial/reusable-apps/docs/screenshot.png
  :align: center
  :height: 431px
  :width: 362px
  :alt: The Django app to conduct Web-based polls.

  The Django app to conduct Web-based polls.

Detailed documentation is in the "docs" directory.

Quick start
-----------

1. Add "polls" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...
        'polls',
    ]

2. Include the polls URLconf in your project urls.py like this::

    url(r'^polls/', include('polls.urls')),

3. Run `python manage.py migrate` to create the polls models.

4. Start the development server and visit http://127.0.0.1:8000/admin/
   to create a poll (you'll need the Admin app enabled).

5. Visit http://127.0.0.1:8000/polls/ to participate in the poll.

Demo example
------------

This repository include a Django 1.9.2 project that has configured with *django-polls* app.

1. Access to `example` directory in this repository.

2. Install the *django-polls* requirements, into a Python virtualenv like this::

    pip install -r requirements/dev.txt

3. Run `python manage.py migrate` to create the polls models.

4. Start the development server and visit http://127.0.0.1:8000/admin/
   to create a poll (you'll need the Admin app enabled).

5. Visit http://127.0.0.1:8000/polls/ to participate in the poll.
