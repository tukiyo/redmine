FROM tukiyo3/redmine:3.2

# plugins
RUN git clone git://github.com/alexbevi/redmine_knowledgebase.git plugins/redmine_knowledgebase
RUN git clone git://github.com/koppen/redmine_github_hook.git plugins/redmine_github_hook

RUN bundle install
COPY docker-entrypoint.sh /
