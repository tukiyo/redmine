FROM tukiyo3/redmine:3.2-kb

RUN apt-get update && apt-get install -y --no-install-recommends \
		graphviz \
		default-jre-headless \
		fonts-takao \
	&& rm -rf /var/lib/apt/lists/*
RUN curl -s -o /opt/plantuml.jar http://jaist.dl.sourceforge.net/project/plantuml/plantuml.8034.jar
RUN git clone git://github.com/simonswine/wiki_external_filter.git plugins/wiki_external_filter
RUN echo '#!/bin/bash\n/usr/bin/java -Djava.io.tmpdir=/var/tmp -jar /opt/plantuml.jar ${@}' > /usr/bin/plantuml \
    && chmod +x /usr/bin/plantuml
