From node:20
Expose 8080
ENV DB_HOST=mysql
RUN useradd expense
RUN mkdir /opt/server
RUN chown -R expense:expense /opt/server
WORKDIR /opt/server
#COPY package.json
COPY *.js* .
RUN npm install
CMD [ "node","index.js" ]