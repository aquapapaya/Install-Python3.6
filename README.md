# Install Python3.6 and pip3
* using root to install python

cd /usr/src

wget https://www.python.org/ftp/python/3.6.7/Python-3.6.7.tgz

tar xzf Python-3.6.7.tgz

cd Python-3.6.7

./configure --enable-optimizations

make altinstall // avoid new version substituting old version

cd /usr/bin 

ln -s /usr/src/Python-3.6.7/python python3

python3 -v


* using root to install pip3

curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py

python get-pip.py

pip3 --version
