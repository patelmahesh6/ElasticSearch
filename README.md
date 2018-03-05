docker run -d  -p 5601:5601 -h kibana --name kibana --link elasticsearch:elasticsearch docker.elastic.co/kibana/kibana:6.1.2

curl  -H "Content-Type: application/json" -X POST localhost:9200/_bulk --data-binary @photos.json

curl -XPUT localhost:9200/_bulk -H 'Content-Type: application/json' -d' --data-binary @photos.json



curl -XPUT -H "Content-Type:application/json" "http://localhost:9200/_ingest/pipeline/ncedc-earthquakes" -d @ncedc-earthquakes-pipeline.json