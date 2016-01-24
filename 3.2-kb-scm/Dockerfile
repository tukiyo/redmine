FROM tukiyo3/redmine:3.2-kb

# plugins
RUN git clone git://github.com/koppen/redmine_github_hook.git plugins/redmine_github_hook
RUN svn export -r 142 http://subversion.andriylesyuk.com/scm-creator plugins/scm-creator
