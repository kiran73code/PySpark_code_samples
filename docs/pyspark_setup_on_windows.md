# Steps to install and setup pyspark on windows machine

## Required Software/Packages

    1.Install JAVA 
    2.Install Apache Spark
    3.Winutils 
        [https://github.com/cdarlint/winutils/tree/master]

## Setup Sparka and Hadoop

    1. Create C:spark/  folder and extract the downloaded .tar file to here.
    2. Create C:hadoop/bin folder extract the winutils files(DLL and .exe)

## Setup ENV variables

1. HADOOP_HOME -> C:hadoop/bin
2. SPARK_HOME -> C:spark/bin
3. JAVA_HOME -> <java/jdk folder path>

## Install Pyspark package from python

```py
pip install pyspark
```

## Trabuleshoot

1.If you are running scripts/notebooks using virtual envs
```py
import sys
import os

# Set PySpark to use the current Python executable
os.environ["PYSPARK_PYTHON"] = sys.executable
```