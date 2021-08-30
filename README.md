# ELK

https://docs.graylog.org/en/4.0/pages/installation/os/ubuntu.html

https://docs.fluentd.org/installation/install-by-deb

https://serverspace.ru/support/help/ustanovka-graylog-na-ubuntu-18-04/

https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-elasticsearch-on-ubuntu-20-04-ru

https://www.digitalocean.com/community/tutorials/how-to-install-mongodb-on-ubuntu-20-04-ru



https://community.jaspersoft.com/questions/1079766/mongodb-connection-solved

https://community.graylog.org/t/cant-connect-to-mongodb/11476

https://community.graylog.org/t/updated-from-v2-2-to-v2-3-cant-reach-elasticsearch/4974/3

https://talk.plesk.com/threads/docker-elasticsearch-how-to.360593/



https://github.com/fluent/fluent-plugin-mongo/issues/124

https://github.com/fluent/fluentd/issues/2425


- https://www.digitalocean.com/community/tutorials/how-to-install-elasticsearch-logstash-and-kibana-elastic-stack-on-ubuntu-20-04-ru
- https://habr.com/ru/post/538840/
```
настройка ротации индексов в ElasticSearch
```
- https://serveradmin.ru/ochistka-elasticsearch-s-pomoshhyu-curator/
- https://4admin.space/all/rotaciya-indektov-elasticsearch-utilita-curator-ubuntu-19-04-18/

```Curator```

https://serveradmin.ru/ochistka-elasticsearch-s-pomoshhyu-curator/


https://www.rosehosting.com/blog/how-to-install-elk-stack-on-ubuntu-20-04/

https://medium.com/@zynpsnltrk/how-to-manage-logs-using-graylog2-fluentd-1508dc5676e9

Filter

https://community.graylog.org/t/logstash-output-to-graylog-3-0-cant-search-message/10333

https://discuss.elastic.co/t/logstash-parsing-nginx-logs-failed/192864

Посмотреть индексы 

curl 'localhost:9200/_cat/indices?v'

GET /_cat/indices/_all?v&s=store.size
