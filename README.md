# SPA-scrapper

A simple tool for crawling the site of the SPA to retrieve all currently available cats for adoption.
The idea is to feed all the information to a Machine Learning algorithm to help and promote the adoption.

# Installation
To install spa-scrapper, just create a virtualenv and install the requirements
```bash
$ cd spa-scrapper
$ virtualenv venv
$ source venv/bin/activate
$ pip install -r requirements.txt
```


# Usage
Due to the fair amount of new dogs every day, this script is recommended to run at least once a day.

```bash
$ cd spa-scrapper
$ source venv/bin/activate
$ cd spa
$ scrapy crawl cats -o output.json
```

# Output
the output can be found inside the folder `spa`:
* The file `output.json` contains all the data of each cat (name, gender, direct url ,shelter, etc)
* The folder `images` contains all the images linked to the json
