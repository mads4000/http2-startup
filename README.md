# Startup
docker-compose -p http2 -f startup.yml up -d

# Create Index
curl -X PUT "localhost:9200/sz-magazin" -H 'Content-Type: application/json' -d @./mapping/sz-magazin-delivery.json

# Insert document
curl -X PUT "localhost:9200/sz-magazin/document/16" -H 'Content-Type: application/json' -d @./elastic/data/article.json