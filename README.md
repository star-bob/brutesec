# BRUTEsec - Huge databases that can be used for bruteforcing and cracking hashed data

![alt tag](https://github.com/fsiamp/brutesec/raw/master/brutesec.png)

URL: http://brutesec-data.appspot.com

BRUTEsec is a place where you can download huge databases that can be used for bruteforcing and cracking hashed data. 
Every file contains hashes and hash outputs in SQLite database format. 

BitTorrent Sync is needed in order to download databases. Get it here http://www.getsync.com 

Virtual tables were used for database optimization.

<b>SHA-256</b> (12-character length, alphanumeric): 20 GB<br>
<b>MD5</b> (10-character length, alphanumeric, special characters) : 5 GB

In order to search for an output of a specific hash value through command-line interface first install sqlite3. 

After, read the database files: 

```sqlite3> .open /path/to/your/dbfile/sha256.db ```

and query the database for that value 

```sqlite3> SELECT * FROM hash_text WHERE hashes MATCH 'b18ec781f24cf1bd34d6c766dd7df5794048848cce610fbfb8c09890075298f1';```
