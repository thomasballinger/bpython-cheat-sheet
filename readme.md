Contributing to Bpython cheat sheet
===================================


First Time Setup
----------------

* Do you have pip?
  * try `pip --version`
  * if not, `sudo easy_install pip`
* Do you have virtualenv?
  * try `virtualenv --version`
  * if not, `sudo pip install virtualenv`
* Do you have mercurial?
  * try `hg --version`
  * if not, `sudo pip install virtualenv`
* Do you have a bitbucket account?
  * if not, create one and log in
* Create a virtual environment for you dev version
  * `virtualenv bpython-dev`
  * activate it with `source bpython-dev/bin/activate`
* Fork bpython in the BitBucket web interface
* Clone your bpython fork
  * `hg clone https://bitbucket.org/YOUR_BITBUCKET_USER_NAME_HERE/bpython`
* Install it into the virtualenv in development mode
  * `cd bpython`
  * `python setup.py devel`

Every Time Setup
----------------

* Activate your virtualenv:
  * source bpython-dev/bin/activate

Doing a Pull Request
--------------------

* hg branch WHAT-YOU-WANT-TO-CALL-YOUR-FIX
* repeat as needed:
  * make changes
  * test them
  * `hg add FILES YOU CHANGED`
  * `hg commit`
* git push --new-branch
* Pull Request from the Bitbucket GUI
* hg pull
* hg update default


