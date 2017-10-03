# https://github.com/elastic/logstash-docker
FROM docker.elastic.co/logstash/logstash:5.5.1

# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json
# When adding plugin here, you may encounter networks trouble
# (https://stackoverflow.com/questions/24151129/docker-network-calls-fail-during-image-build-on-corporate-network)
# If so, I advise changing the DNS settings of the Docker daemon. You can set the default options for the docker 
# daemon by creating a daemon configuration file at /etc/docker/daemon.json. 
# Set DNS server according to your host machine, e.g. DW DNS server is 10.20.3.20.
#
# Then, just restart docker service:
# 
# sudo service docker restart

RUN logstash-plugin install logstash-filter-aggregate
