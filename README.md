django-coverage
===============

[![Circle CI](https://circleci.com/gh/circleci/django-coverage.png?style=badge&circle-token=dfcbc4d5ddc5ebd9dc3e408c83bab3233b3c2617)](https://circleci.com/gh/circleci/django-coverage)

This is an example of a django application that is configured to run tests on CircleCI, record code coverage data with [coverage.py](http://nedbatchelder.com/code/coverage/), and save html coverage reports to CircleCI for later viewing.

##The Video
A complete video guide to setting this project up to run on Circle is available HERE.

##Downloading and Running
* Just fork the repo and follow it on CircleCI to get see it build
* Clone the repo and run `pip install -r requirements.txt` (optionally inside a virtualenv) to install the dependencies
* Run `python manage.py migrate` to setup the database, and optionally follow the prompts to create a superuser (someone that can login to /admin)
* Use the usual `python manage.py runserver [port]` to run the development server locally
* Run `coverage run manage.py test` to run all tests with coverage
* Run `coverage report` after the above command to see a command line coverage report

##Testing on CircleCI
Just sign up for CircleCI if you haven’t already, fork the repo on GitHub (or clone it and add it to your own GitHub account), follow the repository on CircleCI, and your first build/test will begin immediately. Coverage measurement will be performed and the output saved to the “Build Artifacts” for that CircleCI build.


##See Also
* The [virtualenv](http://virtualenv.readthedocs.org/en/latest/) and [virtualenvwrapper](http://virtualenvwrapper.readthedocs.org/en/latest/) docs
* [The official Django tutorial](https://docs.djangoproject.com/en/1.7/intro/tutorial01/)
* [The coverage.py documentation](http://nedbatchelder.com/code/coverage/)
