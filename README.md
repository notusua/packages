##### Notus public packages repo

##### Contains packages for ubuntu precise

## Packages list

##### * node.js - 0.10.6

## Usage

create file `/etc/apt/sources.list.d/notus.list` and add this line into file

    deb [arch=amd64] http://repo.notus.com.ua/ precise main
    
then run `apt-get update` and `apt-get install -f nodejs`

## Restrictions

Now packages available only for precise (12.04) and amd64 arch

## Future plans 

Sing packages

## How to add packages

1. download and compile files
    * download and untar files
    * ./configure
    * make
    * sudo checkinstall

2. copy package to repository root

3. add package to repo
    * reprepro export
    * reprepro createsymlinks
    * reprepro -C main includedeb precise *.deb
