FROM logstash
MAINTAINER thomas.steinbach at aikq.de

RUN logstash-plugin install logstash-filter-environment

ADD logstash.conf /config-dir/logstash.conf

CMD ["logstash","-f","/config-dir/logstash.conf"]