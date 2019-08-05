# Webcrawler Stackoverflow
Python script to captures data from questions of stackoverflow and save the information in MySQL database. 

```mysql
CREATE TABLE `questions` (
  `id` int(11) unsigned NOT NULL AUTO_INCREMENT,
  `title` varchar(355) DEFAULT NULL,
  `description` text,
  `link` varchar(500) DEFAULT NULL,
  `answers` int(8) DEFAULT NULL,
  `views` int(9) DEFAULT NULL,
  `answered_accepted` tinyint(1) DEFAULT NULL,
  `stackoverflow_id` int(12) DEFAULT NULL,
  PRIMARY KEY (`id`),
  UNIQUE KEY `stackoverflow_id` (`stackoverflow_id`)
) ENGINE=MyISAM AUTO_INCREMENT=1801 DEFAULT CHARSET=utf8;
```

![alt text](https://raw.githubusercontent.com/cristianodpp/webcrawler-stackoverflow/master/234234242.png)

![alt text](https://raw.githubusercontent.com/cristianodpp/webcrawler-stackoverflow/master/918238372.png)

![alt text](https://github.com/cristianodpp/webcrawler-stackoverflow/blob/master/database_example.png)

[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE.md)

## Requirements
- [Python 3](https://www.python.org/downloads/)
- [PyMySQL](https://pypi.org/project/PyMySQL/)
- [Unidecode](https://pypi.org/project/Unidecode/)
- [Requests](https://pypi.org/project/requests/)

## Install
```sh
$ brew install python3
```
```sh
$ pip3 install bs4
```
```sh
$ pip3 install pymysql
```
```sh
$ pip3 install unidecode
```
```sh
$ pip3 install requests
```

