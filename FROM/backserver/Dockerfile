From node:20
Expose 8080
RUN useradd expense
RUN /opt/server
RUN chown -R expense:expense
WORKDIR /opt/server
COPY package.json
COPY *.js .
RUN npm install
CMD [ "node","index.js" ]
