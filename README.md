Install Hadoop
==============
GitHub Action for installing Hadoop with cloud connectors.

**Note:** This action has been **deprecated**. You can migrate to using the more flexible
[run-logikal-playbook action](https://github.com/marketplace/actions/run-logikal-playbook) instead:

```yaml
- uses: logikal-io/run-logikal-playbook@v1
  with:
    roles: hadoop
    vars: '{"hadoop_version": "{version}"}'
```

Usage
-----
```yaml
steps:
  - uses: logikal-io/install-hadoop@v1
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
Dependencies").

License
-------
This GitHub Action is licensed under the MIT open source license.
