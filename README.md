# Kedro Starter: PySpark

## Introduction

This repository contains a Kedro project template with some initial configurations to demonstrate best practices when using Kedro with PySpark. It originates from our [Working with PySpark](https://kedro.readthedocs.io/en/stable/04_user_guide/09_pyspark.html) guide.

## Features

### Spark's configuration in one place, i.e. `/conf/base/spark.yml`

Spark allows you to specify many different [configurations options](https://spark.apache.org/docs/latest/configuration.html). This starter codifies the use of `/conf/base/spark.yml` as the configuration file for these options.


### `SparkSession` initialisation

This starter contains the initialisation code for `SparkSession` in the `ProjectContext` by reading the configuration from `/conf/base/spark.yml`. You should modify this code if you want to further customise your `SparkSession`, e.g. configuring it to use YARN.
