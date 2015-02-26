# Kibana in docker

Kibana 4.0.0 in Docker

## Usage
From a remote host : 
```
docker run -d -p 5601:5601 --add-host="elasticsearch:10.0.0.1" petitchevalroux/kibana
```
Link with a docker container running elasticsearch :
```
docker run -d -p 5601:5601 --link <name or id of your container running elasticsearch>:elasticsearch petitchevalroux/kibana
```

If you are running docker using [boot2docker](http://boot2docker.io/), the following url should display kibana :
http://192.168.59.103:5601

Available on:
* [docker hub](https://registry.hub.docker.com/u/petitchevalroux/kibana/)
* [github](https://github.com/petitchevalroux/docker-kibana)

## About me
http://petitchevalroux.net