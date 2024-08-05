FROM ubuntu

RUN apt-get update && apt-get install -y curl

COPY script.sh /script.sh

RUN chmod +x /script.sh

ENTRYPOINT ["/script.sh"]

#docker run -it ubuntu bash -c 'apt-get update && apt-get install -y curl && while true; do echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website; done'

#docker container run -it 1.4 
