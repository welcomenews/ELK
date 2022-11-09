# ELK

#### Скачать deb пакеты
https://www.elastic.co/downloads/past-releases/

========================================================================================

https://serveradmin.ru/ustanovka-i-nastroyka-elasticsearch-logstash-kibana-elk-stack/

https://docs.graylog.org/en/4.0/pages/installation/os/ubuntu.html

https://docs.fluentd.org/installation/install-by-deb

https://serverspace.ru/support/help/ustanovka-graylog-na-ubuntu-18-04/

https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-elasticsearch-on-ubuntu-20-04-ru

https://www.digitalocean.com/community/tutorials/how-to-install-mongodb-on-ubuntu-20-04-ru

https://serveradmin.ru/nastraivaem-sbor-logov-windows-server-v-elk-stack/

https://wtfm.info/elasticsearch-%D0%BD%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B9%D0%BA%D0%B0-ilm/
```
Graylog
```
- https://www.8host.com/blog/upravlenie-logami-s-pomoshhyu-graylog-2-v-ubuntu-16-04/
- https://habr.com/ru/company/pixonic/blog/341274/



https://community.jaspersoft.com/questions/1079766/mongodb-connection-solved

https://community.graylog.org/t/cant-connect-to-mongodb/11476

https://community.graylog.org/t/updated-from-v2-2-to-v2-3-cant-reach-elasticsearch/4974/3

https://talk.plesk.com/threads/docker-elasticsearch-how-to.360593/

https://serveradmin.ru/ustanovka-i-nastroyka-elasticsearch-logstash-kibana-elk-stack/#Ustanovka_i_nastrojka_Winlogbeat



https://github.com/fluent/fluent-plugin-mongo/issues/124

https://github.com/fluent/fluentd/issues/2425


- https://www.digitalocean.com/community/tutorials/how-to-install-elasticsearch-logstash-and-kibana-elastic-stack-on-ubuntu-20-04-ru
- https://habr.com/ru/post/538840/
```
настройка ротации индексов в ElasticSearch
```
- https://serveradmin.ru/ochistka-elasticsearch-s-pomoshhyu-curator/
- https://4admin.space/all/rotaciya-indektov-elasticsearch-utilita-curator-ubuntu-19-04-18/
- http://cyberflow.net/2013/05/logstash-rotate-logs-in-elasticsearch.html

```Curator```

https://serveradmin.ru/ochistka-elasticsearch-s-pomoshhyu-curator/


https://www.rosehosting.com/blog/how-to-install-elk-stack-on-ubuntu-20-04/

https://medium.com/@zynpsnltrk/how-to-manage-logs-using-graylog2-fluentd-1508dc5676e9

```Filter```

https://community.graylog.org/t/logstash-output-to-graylog-3-0-cant-search-message/10333

https://discuss.elastic.co/t/logstash-parsing-nginx-logs-failed/192864

```Посмотреть индексы```

curl 'localhost:9200/_cat/indices?v'

GET /_cat/indices/_all?v&s=store.size


```настройки параметров elasticsearch```

https://coderlessons.com/tutorials/noveishie-tekhnologii/izuchite-uprugii-poisk/elasticsearch-kratkoe-rukovodstvo

Путь к индексам 
/var/lib/elasticsearch/nodes/0/indices/

-
https://habr.com/ru/company/itsoft/blog/556194/


service --status-all

```Мониторинг логов```
https://kamaok.org.ua/?p=3386



sudo -E sed -i -e "s/password_secret =.*/password_secret = $(pwgen -s 128 1)/" /etc/graylog/server/server.conf

sudo sed -i -e "s/root_password_sha2 =.*/root_password_sha2 = $(echo -n 'password' | shasum -a 256 | cut -d' ' -f1)/" /etc/graylog/server/server.conf
