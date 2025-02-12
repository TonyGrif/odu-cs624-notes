# Resilient Distributed Dataset
This is a read-only distributed collection of records designed to be operated on in parallel. These datasets use more RAM instead of network and I/O. [[Apache Spark Overview | Apache Spark]] is built on this concept.
## Creation
* Parallelize an existing collection in driver program
* Reference dataset in external storage system