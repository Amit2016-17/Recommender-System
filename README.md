# Recommender System  

## The entire recommender system is developed using layers of lambda architecture and is implemented in three different directories:
### 1. Batch Layer
### 2. Serving Layer
### 3. Speed Layer  

To get the OVA file, follow the link given below.  
https://www.dropbox.com/s/2ic8pz64hiab8o2/BDM.ova?dl=0  

Follow these steps to start the VM.  
1. Import the appliance as an Ubuntu 64-bit OS in Oracle VMWare.  
2. Minimum requirements: Hard disk - 20GB, RAM - 4GB (6-8GB preferred)  
3. Credentials: Username - bdm Password - bdm   
4. Enter the command: sudo su -  
5. Enter the password again: bdm  
6. This is a preinstalled environement and consists  
	- Hadoop
	- Spark
	- Cassandra
	- Jupyter Notebooks  
7. To open jupyter notebooks with pyspark and cassandra, enter this command:  
PYSPARK_DRIVER_PYTHON="jupyter" \  
PYSPARK_DRIVER_PYTHON_OPTS="notebook --ip=<IP_ADDRESS>" \  
pyspark --packages datastax:spark-cassandra-connector:2.0.0-s_2.11 \  
--conf spark.cassandra.connection.host=127.0.0.1  
8. To get the IP_ADDRESS of VM, type: ifconfig in the terminal.  

### Cassandra
To run cassandra database follow these steps:  
1. Login as root user.  
2. Run: /usr/local/lib/apache-cassandra-3.10/bin/cassandra -R  
3. To access cqlsh: /usr/local/lib/apache-cassandra-3.10/bin/cqlsh  
4. Rest of the instructions are available in the python notebooks.  

Follow further instructions given in the directories to run this project.  