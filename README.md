[![Build Status](https://travis-ci.org/recombinators/worker.svg?branch=tests)](https://travis-ci.org/recombinators/worker)

Worker
======

Worker interfaces between a database and landsat-util. It's responsible for creating both the render and preview images for [Snapsat](https://github.com/recombinators/snapsat)

Installation
------------

Assumes you're running Ubuntu. Install dependencies with:
```
sudo apt-get update
sudo apt-get install python-pip python-numpy python-scipy libgdal-dev libatlas-base-dev gfortran git
sudo easy_install -U pip
sudo pip install landsat-util
sudo pip install boto
```

Clone the repository:
```
git clone https://github.com/recombinators/worker.git
```

Create a `~/.boto` file with the appropriate credentials.
```
[Credentials]
aws_access_key_id
aws_secret_access_key
```

Run the app with:
```
cd landsat_worker
sudo python render_1.py
```
