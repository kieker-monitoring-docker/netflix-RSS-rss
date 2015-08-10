# Simple RSS-Server instrumented with Kieker (netflix-RSS-rss)
RSS-server for load testing.

## Example
To start this container standalone, you can issue the following command:
```
sudo docker run -t -i \
  -p 80:8080 \
  -v /tmp/netflix-rss/rss/logs:/opt/kieker/logs \
  -v /tmp/netflix-rss/rss/config:/opt/kieker/config \
  kieker/netflix-rss-rss
```
To see which feeds are available, you can open `http://localhost/rss/` with your browser.
The logs and config files of the instrumentation are stored in `/tmp/netflix-rss/rss/{logs|config}` in this example.

