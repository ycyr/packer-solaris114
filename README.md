Solaris packer files
====================

Files used to build Solaris Base Box for use with vagrant

See Blogposts:
* Using Solaris Unified Archives: http://blog.zach.st/2015/12/06/creating-solaris-11-vagrant-boxes-out-of-unified-archives.html
* Using Solaris GA installation ISOs:
http://www.resilvered.com/2014/02/solaris-vagrant-packer-and-base-box.html

Tested on:
------------
- Virtualbox 5.0.13
- Vargrant 1.8.1
- Packer 0.9.0
- Solaris 11_1 text installer
- Solaris 11_2 text installer
- Solaris 11_3 text installer
- Solaris 10 Update 11 DVD image

To use these files
------------------

    git clone git://github.com/mzachh/solaris-packer
    packer build -only=virtualbox-iso solaris-ai.json
    packer build -only=vmware-iso solaris-ai.json
