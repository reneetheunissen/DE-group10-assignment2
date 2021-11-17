# Use Python 3.9.0
FROM bitnami/python:3.9.0 as build

# Use Spark 3.1.1
FROM bitnami/spark:3.1.1

# Use the specified Python version
COPY --from=build /opt/bitnami/python/ /opt/bitnami/python/

# Guava library for GCS connector
RUN mv /opt/bitnami/spark/jars/guava-14.0.1.jar /opt/bitnami/spark/jars/guava-14.0.1.jar.bk
COPY *.jar /opt/bitnami/spark/jars/