FROM perl:5-threaded

RUN curl --location  \
        --output /sqlserver2pgsql-master.zip  \
        https://github.com/dalibo/sqlserver2pgsql/archive/refs/heads/master.zip && \
    unzip -d / /sqlserver2pgsql-master.zip && \
    rm /sqlserver2pgsql-master.zip && \
    mv /sqlserver2pgsql-master /sqlserver2pgsql

ENTRYPOINT ["/sqlserver2pgsql/sqlserver2pgsql.pl"]