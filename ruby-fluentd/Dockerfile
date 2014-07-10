FROM d11wtq/ruby

USER root
RUN curl -O http://packages.treasure-data.com/debian/RPM-GPG-KEY-td-agent && apt-key add RPM-GPG-KEY-td-agent && rm RPM-GPG-KEY-td-agent
RUN curl -L http://toolbelt.treasuredata.com/sh/install-ubuntu-precise.sh | sh
RUN /usr/lib/fluent/ruby/bin/fluent-gem install fluent-plugin-bigquery
USER default