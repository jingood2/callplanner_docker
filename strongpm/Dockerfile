FROM strongloop/strong-pm

ENV NODE_ENV production

RUN mkdir -p ./data && chmod -R 777 ./data
RUN mkdir -p ./data/storage/ments
RUN mkdir -p ./data/storage/records 

VOLUME ["/var/log/upstart","./data","/home/strong-pm"]

COPY ./config/strong-pm-container.conf /etc/init/strong-pm-container.conf
