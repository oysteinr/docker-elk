FROM kibana:5

RUN /usr/share/kibana/bin/kibana-plugin install x-pack

RUN apt-get update && apt-get install -y netcat bzip2

COPY entrypoint.sh /tmp/entrypoint.sh
RUN chmod +x /tmp/entrypoint.sh

CMD ["/tmp/entrypoint.sh"]
