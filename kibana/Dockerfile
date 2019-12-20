FROM kibana:7.5.1

#RUN apk add --update netcat
#RUN apk update && apk add netcat
#RUN apt-get update && apt-get install -y netcat

COPY entrypoint.sh /tmp/entrypoint.sh
USER root
RUN chmod +x /tmp/entrypoint.sh
USER kibana

#Sense is now included as Console in Kibana 5.0.
#RUN kibana plugin --install elastic/sense

CMD ["/tmp/entrypoint.sh"]
