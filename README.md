## Confluent platform install steps:
### Download
```shell
curl -O https://packages.confluent.io/archive/7.6/confluent-7.6.2.zip
unzip confluent-7.6.2.zip
```
### Run
```shell
export CONFLUENT_HOME=/Users/saberseddik/projects/kafka/confluent-7.6.2
./confluent local services start
```
### Control central
URL ```http://localhost:9021/```
### Generate sample data
```shell
ksql-datagen quickstart=users format=json topic=users_topic maxInterval=100
```
## Reference
https://docs.confluent.io/platform/current/installation/installing_cp/zip-tar.html
https://medium.com/@bhageshwaridevnani/kafka-confluent-overview-and-installation-guide-a8191630e5b8
https://www.confluent.io/blog/easy-ways-generate-test-data-kafka/
