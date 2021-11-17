# Use JupyterHub
FROM bitnami/jupyterhub:1.4.2

# Specify using the root
USER root

# Install JDK
RUN apt-get update -y && apt-get -y install openjdk-11-jdk

# Install NPM
RUN apt-get install npm -y && npm install -g configurable-http-proxy

# Specify non-root user
USER 1001

# Upgrade pip and install PySpark 3.1.2
RUN pip3 install --upgrade pip && pip3 install pyspark==3.1.2

# Path to use for JDK
ENV PATH="/usr/lib/jvm/java-11-openjdk-amd64:$PATH"