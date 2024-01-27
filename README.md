# commoncrawl.py
This Python script is a multi-threaded tool for retrieving data from the **CommonCrawl** index. It allows you to specify a domain or a list of domains, and it will retrieve all URLs associated with those domains that are indexed by **CommonCrawl**.

### How it Works
The script uses the requests library to send HTTP requests to the CommonCrawl index. It retrieves the index data in JSON format, parses it, and adds the URLs to a set to avoid duplicates. The script uses multi-threading to speed up the data retrieval process.

### Installation
```
git clone https://github.com/Mr0Wido/commoncrawl.py.git
cd commoncrawl.py 
python3 commoncrawl.py
```

### Usage
```
python3 commoncrawl.py -d example.com
python3 commoncrawl.py -l list.txt
```

### Options
**Flags** |       | **Description**
--- | --- | ---
-h | --help | Show this help message and exit.
-d | --domain | Domain Name; Example: test.com
-l | --list | Domain list file name

### Requirments
```
requests
json
threading
queue
argparse
```

### Note
This script is intended for educational purposes and should be used responsibly. Please respect the terms of service of the CommonCrawl index.
