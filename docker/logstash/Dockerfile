FROM docker.elastic.co/logstash/logstash-oss:7.15.1

# remove versions that are bundled with the base image
RUN rm -rf /usr/share/logstash/vendor/bundle/jruby/2.5.0/gems/logstash-output-lumberjack-3.1.9/* /usr/share/logstash/vendor/bundle/jruby/2.5.0/gems/jls-lumberjack-0.0.26/*

# add forked versions of the gems
ADD gems/ /usr/share/logstash/vendor/bundle/jruby/2.5.0/gems/
