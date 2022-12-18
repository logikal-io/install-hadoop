Install Hadoop
==============
GitHub Action for installing Hadoop with cloud connectors.

Usage
-----
```yaml
steps:
  - uses: logikal-io/install-hadoop@{release}
    with:
      version: {version}
```

Inputs
------
`version`: Required, the version to install.

`gcs-connector-version`: Optional, the Hadoop Google Cloud Storage connector version to install.

`aws-module-version`: Optional, the [Hadoop AWS
module](https://mvnrepository.com/artifact/org.apache.hadoop/hadoop-aws) version to install.

`aws-java-sdk-version`: Optional, but required when `aws-module-version` is specified: the AWS Java
SDK bundle version that was used to compile the Hadoop AWS module (it is listed under the "Compile
Depencies").

License
-------
This GitHub Action is licensed under the MIT open source license.
