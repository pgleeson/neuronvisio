.. _install:

*******
Install
*******

Requirements
============

To install Neuronvisio you need to satisfy the following dependencies

- PyQt4: http://www.riverbankcomputing.co.uk/software/pyqt/download
- matplotlib: http://matplotlib.sourceforge.net/
- setuptools: http://pypi.python.org/pypi/setuptools
- pytables: http://www.pytables.org/
- ipython: http://ipython.org 0.12 (can be automatically installed, see `Package Install`_)
- mayavi2: http://code.enthought.com/projects/mayavi/  4.2.0 or better (can be automatically installed, see `Package Install`_)

and of course NEURON_>=7.2 compiled with python support

.. _NEURON: http://www.neuron.yale.edu/neuron/  

Ubuntu and friends
------------------

On Ubuntu you can easily install all the requirements using apt-get with::

    sudo apt-get install python-qt4 python-matplotlib python-setuptools python-tables \
                         mayavi2

If you are running a different flavour of GNU/Linux, like Fedora for example, just install 
the requirements with your package manager.

Next, see the instructions on installation of NEURON with Python availabe at
http://www.davison.webfactional.com/notes/installation-neuron-python/.

Proceed to the `Package Install`_ .


Mac OS X
---------

Under Mac it is recommended to get a prepackaged scientific python distribution 
which contains most of neuronvisio's dependencies, such as:

- Enthought Distribution: http://www.enthought.com/products/epd.php (free for an
  academic use)

Alternatively, if you want to do it yourself, you should look at the following:

- Scipy SuperPack: http://fonnesbeck.github.com/ScipySuperpack/
- PyQt4: http://www.riverbankcomputing.co.uk/software/pyqt/download
  
Next, see the instructions on installation of NEURON with Python availabe at
http://www.davison.webfactional.com/notes/installation-neuron-python/.

Proceed to the `Package Install`_ .


Windows
-------

Under Windows it is recommended to get a prepackaged scientific python distribution 
which contains most of neuronvisio's dependencies, such as:

- Enthought Distribution: http://www.enthought.com/products/epd.php (free for an
  academic use)
- Python(x,y): http://www.pythonxy.com/foreword.php (free)

Alternatively, if you want to do it yourself, you will need to manually install
and configure the dependencies listed in `Requirements`_

A portable and already compiled version of NEURON for Python is available 
from https://bitbucket.org/uric/pyneuron/ or simply by using::
    
    pip install PyNEURON

Proceed to the `Package Install`_ .


Package Install
===============

To install Neuronvisio we suggest to create a virtualenv and install
the packages there. Check out virtualenv_ and virtualenvwrapper_

.. _virtualenv: http://pypi.python.org/pypi/virtualenv
.. _virtualenvwrapper: http://pypi.python.org/pypi/virtualenvwrapper 

If you have `pip`_ installed and all the requirements are already met you 
can install neuronvisio from PyPi_ typing::

    pip install -U neuronvisio

.. note:: Mayavi stack and ipython will be installed automatically as Neuronvisio requirements from PyPi.

.. _PyPi: http://pypi.python.org/pypi/neuronvisio/
.. _pip: http://pypi.python.org/pypi/pip

Running the bleeding edge
-------------------------

If you want to run the latest code, directly from the repo, you can do it using pip::

    pip install -e git+https://github.com/NeuralEnsemble/neuronvisio.git#egg=neuronvisio

then you need to add the directory (the absolute path) to your PYTHONPATH (in bash)::
    
    export PYTHONPATH=$PYTHONPATH:/path-to-neuronvisio-dir
    
.. _source-code-section:

Source Code
===========

The `source code`_ is on github_ at this address and git_ is used as software 
management tool

.. _source code: http://github.com/mattions/neuronvisio
.. _github: https://github.com/
.. _git: http://git-scm.com/

To install from the git just clone the repo::

    git clone git://github.com/mattions/neuronvisio.git

and then run::
    
    python setup.py install    