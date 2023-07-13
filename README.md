# Conpot

![Test Status](https://github.com/mushorg/conpot/workflows/Code%20tests/badge.svg)
[![Docs](https://readthedocs.org/projects/conpot/badge/?version=latest)](https://conpot.readthedocs.io/en/latest/)
[![Coverage Status](https://coveralls.io/repos/github/mushorg/conpot/badge.svg?branch=master)](https://coveralls.io/github/mushorg/conpot?branch=master)
[![Docker Build Status](https://img.shields.io/docker/build/honeynet/conpot.svg)](https://hub.docker.com/r/honeynet/conpot)

## About

Conpot is an ICS honeypot with the goal to collect intelligence about the motives and methods of adversaries targeting industrial control systems.

## Documentation

The documentation can be found [here](https://conpot.readthedocs.io/). If you are just checking out conpot, we suggest that you go for [quick install](https://conpot.readthedocs.io/en/latest/installation/quick_install.html). 

If you want to tinker around and write your own template, change ports etc. We suggest that you do host install.
You can find instructions on how to install conpot [here](https://conpot.readthedocs.io/en/latest/installation/install.html) and the FAQ [here](https://conpot.readthedocs.io/en/latest/faq.html).


## How to install

$ sudo apt-get install git libsmi2ldbl smistrip libxslt1-dev python3.6-dev libevent-dev default-libmysqlclient-dev
$ virtualenv --python=python3.6 conpotvenv
$ source conpotvenv/bin/activate
$ git clone https://github.com/d4emonsAVI/conpot.git && cd conpot
$ pip install -r requirements.txt
$ python setup.py install


## How to use

You can run conpot with the default testing configuration:
$ conpot -f

Choose from one of the available templates to run. The default template for example:
$ conpot -f --template default