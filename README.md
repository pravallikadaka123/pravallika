* #Building a real-time data streaming pipeline, covering each phase from data ingestion to processing and finally storage.
* We'll utilize a powerful stack of tools and technologies, including Apache Airflow, Python, Apache Kafka, Apache Zookeeper, Apache Spark, and Cassandra—all neatly containerized using Docker.
0:53 System architecture
3:47 Getting data from API with Airflow
17:10 Docker Compose for the architecture
26:09 Streaming data into Kafka
44:29 Apache Spark and Cassandra setup
49:33 Streaming data into cassandra

* ##Docker image:
-Think of a Docker image as a pre-packaged bundle that contains everything needed to run a specific piece of software. It's like a ready-to-use package that includes all the necessary files, libraries, and configurations for an application or service to work correctly.

-Imagine you're baking cookies. Instead of gathering all the ingredients (flour, sugar, eggs, etc.) separately each time you want to bake, you can use a pre-made cookie mix. The mix already contains all the ingredients in the right proportions, so you just need to add water and bake. Similarly, a Docker image contains all the necessary "ingredients" for running software, so you can quickly and easily set up and run applications without worrying about installing dependencies or configuring the environment manually.

-When you use a Docker image, you're essentially taking advantage of this pre-packaged setup. It saves time and ensures consistency because you can rely on the same image to produce identical environments wherever it's used. Plus, Docker images are portable, meaning you can run them on any system that supports Docker, making it easy to deploy applications across different environments, from your local development machine to a production server.

* __entrypoint.sh__---->we want to write sequence of command that airflow should follow when its trying to initialize web server or the scheduler
