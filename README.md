# Data Engineering Zoomcamp 2024 - Homework #5

### Setting up spark

1. Install java in home

```sh
mkdir ~/java
cd ~/java
wget https://download.java.net/java/GA/jdk11/9/GPL/openjdk-11.0.2_linux-x64_bin.tar.gz
tar xzfv openjdk-11.0.2_linux-x64_bin.tar.gz
rm openjdk-11.0.2_linux-x64_bin.tar.gz
export JAVA_HOME="${HOME}/java/jdk-11.0.2"
export PATH="${JAVA_HOME}/bin:${PATH}"
```

2. Install Spark

```sh
mkdir ~/spark
cd ~/spark
wget https://archive.apache.org/dist/spark/spark-3.3.2/spark-3.3.2-bin-hadoop3.tgz
tar xzfv spark-3.3.2-bin-hadoop3.tgz
rm spark-3.3.2-bin-hadoop3.tgz
export SPARK_HOME="${HOME}/spark/spark-3.3.2-bin-hadoop3"
export PATH="${SPARK_HOME}/bin:${PATH}"
```

3. Install python library for jupyter

```sh
pip install jupyter
```

4. Create a folder for notebooks

```sh 
mkdir notebooks
cd notebooks
```

5. Execute jupyter notebooks command

```sh
jupyter notebook
```

Then check the service running on `http://localhost:8888`

6. Execute his commands in shell

```bash
export PYTHONPATH="${SPARK_HOME}/python/:$PYTHONPATH"
export PYTHONPATH="${SPARK_HOME}/python/lib/py4j-0.10.9.5-src.zip:$PYTHONPATH"
```
