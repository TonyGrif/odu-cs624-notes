# Apache Spark
Apache Spark is an open-source, in-memory processing engine for big data available in a variety of languages. Spark does not come with its own file system and will require one to be created. Spark can also take in third-party resource managers to allocate memory to [[Clusters | clusters]], although, it does come with one built-in (Spark Standalone).
## Modules
* [[Spark SQL]]
* [[Spark Streaming]]
* [[Spark MLib]]
* [[GraphX]]
## Cluster Components
* **Driver**: JVM that maintains connections & submits tasks to executors, creates a Directed Acyclical Graph (DAG) of Transformations & Actions
* **SparkContext**: Java class containins code to process data in parallel, coordinates with resource manager to schedule resources
* **Resource Manager**: Can be build-in or third-party
* **Worker Nodes**: Physical servers that run Executors, each can contain multiple Executors, fixed set of CPU and RAM assigned by resource manager
* **Executors**: Processes carrying out tasks, each creates tasks threads and holds the [[Resilient Distributed Dataset]] in memory from the file