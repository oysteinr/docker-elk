FROM logstash:5

# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json

RUN wget https://drive.google.com/uc\?export\=download\&id\=0B47pBt7PBmvRck9nTG5yYWRZTk0 -O /usr/share/logstash/ojdbc6.jar
RUN wget https://jdbc.postgresql.org/download/postgresql-42.0.0.jar -O /usr/share/logstash/postgresql.jar

RUN logstash-plugin install logstash-input-jdbc
