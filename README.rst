####################
LFE Skeleton Project
####################

**UPDATE**: This script has been deprecated. Please use `lfetool`_ instead!

This should really be converted into a `rebar`_ script sooner than later.
Perhaps someone else will have the time and rebar chops to do it? For now,
though, a simple shell script creates what is needed.

There are two modes, only one of which is currently implemented:

#. create a library project, one that intended to be used by other projects
   and does not start any services;

#. create a service project, one that should have at lease one services
   started.


Installation
============

Download the `shell script`_ and save it to a directory in your path.


Usage
=====

To create a library project, simply run the following:

.. code:: shell

    $ lfe-skel library-project my-new-lib

Though not currently implemented, in the future one will create a service
project by running the following:

.. code:: shell

    $ lfe-skel service-project my-new-service

*Note*: upon running this script, not only with your project be set up with a
skeleton, but also:

* the dependencies for your project will be downloaded to your new project's
  ``deps`` dir;

* the stubbed unit test will be run and will fail (it's stubbed to fail because
  of TDD ;-));
  
* the project will be set up with a newly initialized github repo; and

* the new project files will be added to the repo.


.. Links
.. -----
.. _lfetool: https://github.com/lfe/lfetool
.. _rebar: https://github.com/rebar/rebar
.. _shell script: https://raw.github.com/lfex/skeleton-project/master/lfe-skel

