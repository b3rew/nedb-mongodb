# nedb-mongodb

Transfer [NeDB](https://github.com/louischatriot/nedb) Data to a MongoDB collection.


Based on [https://github.com/louischatriot/nedb-to-mongodb](https://github.com/louischatriot/nedb-to-mongodb)

### Installation
```bash
git clone https://github.com/b3rew/nedb-mongodb.git
cd nedb-mongodb
npm install
./index.js -d db-name -c collection-name -n nedb-file -k false
```
or you can install it globally 

```bash
npm install -g nedb-mongodb
nedb-mongodb  -d db-name -c collection-name -n nedb-file -k false
```

### Usage
Usage is pretty straightforward. All the information you need is one `./index.js --help` away. Here is what this command tells you:  

    Usage: ./index.js [options]

    Options:

    -h, --help                      output usage information
    -V, --version                   output the version number
    -h --mongodb-host [host]        Host where your MongoDB is (default: localhost)
    -p --mongodb-port [port]        Port on which your MongoDB server is running (default: 27017)
    -d --mongodb-dbname [name]      Name of the Mongo database
    -c --mongodb-collection [name]  Collection to put your data into
    -n --nedb-datafile [path]       Path to the NeDB data file
    -k --keep-ids [true/false]      Whether to keep ids used by NeDB or have MongoDB generate ObjectIds
                                    (probably a good idea to use ObjectIds from now on!)
