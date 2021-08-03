FROM docker.elastic.co/logstash/logstash-oss:7.13.4

# remove versions that are bundled with the base image
RUN rm -rf /usr/share/logstash/vendor/bundle/jruby/2.5.0/gems/logstash-output-lumberjack-3.1.8/* /usr/share/logstash/vendor/bundle/jruby/2.5.0/gems/jls-lumberjack-0.0.26/*

# add custom versions of the gems
ADD gems/ /usr/share/logstash/vendor/bundle/jruby/2.5.0/gems/
