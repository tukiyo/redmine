FROM tukiyo3/redmine:3.2

# add our user and group first to make sure their IDs get assigned consistently, regardless of whatever dependencies get added
RUN git clone git://github.com/alexbevi/redmine_knowledgebase.git plugins/redmine_knowledgebase
RUN bundle install
COPY docker-entrypoint.sh /
