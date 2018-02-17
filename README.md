Scrapy project with images loading and mysql store.

Features

    Scrapy spider that crawles site, loads images and stores data in mysql database. 
    Requires Python 2.7    

Init project:

Install scrapy in Linux (Ubuntu):
    sudo pip install scrapy

Install mysqlclient:
    sudo apt-get install libmysqlclient-dev
    sudo pip install mysqlclient

Create database in Mysql:
    CREATE DATABASE scrapy;

Create table `books` in mysql from scrapy.sql


Run spider and store data in json and mysql:
    scrapy crawl books -o books.json -s CLOSESPIDER_PAGECOUNT=5
