FROM mongo:3.2
ADD keyfile.key /data/
RUN chmod 600 data/keyfile.key \
	&& chown -R mongodb:mongodb /data/keyfile.key
CMD ["mongod", "--smallfiles", "--keyFile", "/data/keyfile.key","--auth"]
