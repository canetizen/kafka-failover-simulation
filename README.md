# kafka-failover-simulation

A distributed Kafka failover simulation built with **Java** and **Docker Compose**.
All build, startup, and failover scenarios are managed by a single shell script.
The project demonstrates how producers and consumers respond to broker failures and recover automatically in a real-world, containerized Kafka environment.

## Key Features:

* Single script (`run-failover.sh`) automates build, environment setup, and execution
* Simulates broker failures and automatic client recovery
* Java-based Kafka producer and consumer implementations
* Docker Compose for isolated, reproducible local Kafka setup
* Logs output to `logs/` directory for analysis

---

**How to Build and Run:**

```bash
./run-failover.sh
```

No manual steps are required. The script will:

* Build the project with Maven
* Start Kafka and Zookeeper with Docker Compose
* Launch both producer and consumer clients
* Simulate failover scenarios and output logs

While the program is running, you can examine the logs to observe the behavior of the consumer and producer during failover transitions.

---

