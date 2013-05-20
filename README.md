Notus .deb packages repository
===

### Packages list

    * node.js (v0.10.6)
    * jdk (1.7.021)

### Usage

create file with repository uri

    sudo sh -c 'echo "deb [arch=amd64] http://repo.notus.com.ua/ precise main" > /etc/apt/sources.list.d/notus.list'
    apt-get update
    apt-get install -f nodejs

### Restrictions

Now packages available for: 

    * Ubuntu 12.04 LTS Precise 
    * amd64 architecture

### How to add packages

download and compile files:  

    download and untar files
    ./configure
    make
    sudo checkinstall

copy package to repository root

add package to repo

    reprepro export
    reprepro createsymlinks
    reprepro -C main includedeb precise *.deb


