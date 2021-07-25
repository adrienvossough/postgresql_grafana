FROM fluent/fluentd:v1.13.0-1.0

COPY ./plugins /fluentd/plugins
WORKDIR /fluentd/plugins

USER root
RUN fluent-gem install fluent-plugin-sql --no-document

USER fluent
# # pour postgresql
# RUN fluent-gem install pg --no-document