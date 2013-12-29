# dat.wallet

![User interface](http://images.weserv.nl/?url=i.imgur.com/I39zPfW.png&fnr)

## Installation
You will need to install Kivy (http://kivy.org) and Twisted (http://twistedmatrix.com/trac/wiki/Downloads) and use the following commands:

    $ sudo apt-get install python-pip
    $ sudo pip install ecdsa slowaes
    $ mkdir depends
    $ cd depends
    $ git clone https://github.com/caedesvvv/zmqproto.git
    $ git clone https://github.com/darkwallet/python-obelisk.git
    $ cd ..
    $ ln -s depends/zmqproto/zmqproto .
    $ ln -s depends/python-obelisk/obelisk .

These parent path where these repos are cloned will need to be added to
your PYTHONPATH environment variable.

    $ export PYTHONPATH=$PYTHONPATH:$(pwd)

Clone the dat.wallet repo and change directory

    $ git clone https://github.com/darkwallet/dat.wallet.git
    $ cd dat.wallet

# Usage
    kivy main.py -- "correct horse battery staple"

or

    python main.py -- "correct horse battery staple"
in linux

Where "correct horse battery staple" is your seed phrase. Note the space between the -- and the seed phrase
