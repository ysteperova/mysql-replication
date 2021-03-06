[![MySQL Database Replication](../../raw/master/images/mysql_new.png)](../../../mysql-replication)
## MySQL Database Replication

The JPS package deploys MySQL Cluster with preconfigured replication that initially contains 2 database containers. The package provides the solution for solving performance problems, DB backups support, gives ability to alleviate system failures. It enables data from one database server (the master) to be replicated to one or more database servers (the slaves).

### Highlights
This package is designed to solve a number of different problems with performance, supporting the backup of different databases, and as a part of a larger solution to alleviate system failures.<br />
It enables data from one database server (the master) to be replicated to one or more database servers (the slaves). The master logs the updates, which then ripple through to the slaves. The slave outputs a message stating that it has received the update successfully, thus allowing to send the subsequent updates. Master-slave replication can be asynchronous.<br />

The target usage for replication in MySQL databases includes:
  -  Data security
  -  Analytics
  -  Long-distance data distribution

###Environment Topology

![MySQL Database Replication Topology](https://docs.google.com/drawings/d/1Rk5fVw8vhUzdiicBUI-1DH5S0KXVGKz4T2f45_9bbfs/pub?w=301&h=149)

### Specifics

Layer              |     Server    | Number of CTs <br/> by default | Cloudlets per CT <br/> (reserved/dynamic) | Options
----------------- | --------------| :-----------------------------------------: | :-------------------------------------------------------: | :-----:
DB                  |    MySQL    |       2                                             |           1 / 16                                                       | -

* DB - Database 
* CT - Container

**MySQL Database**: 5.7.12<br/>
**Java Engine**: Java 7.0

### Deployment

In order to get this solution instantly deployed, click the "Get It Hosted Now" button, specify your email address within the widget, choose one of the [Jelastic Public Cloud providers](https://jelastic.cloud) and press Install.

[![GET IT HOSTED](https://raw.githubusercontent.com/jelastic-jps/jpswiki/master/images/getithosted.png)](https://jelastic.com/install-application/?manifest=https%3A%2F%2Fgithub.com%2Fjelastic-jps%2Fmysql-replication%2Fraw%2Fmaster%2Fmanifest.jps)

To deploy this package to Jelastic Private Cloud, import [this JPS manifest](../../raw/master/manifest.jps) within your dashboard ([detailed instruction](https://docs.jelastic.com/environment-export-import#import)).

More information about Jelastic JPS package and about installation widget for your website can be found in the [Jelastic JPS Application Package](https://github.com/jelastic-jps/jpswiki/wiki/Jelastic-JPS-Application-Package) reference.
