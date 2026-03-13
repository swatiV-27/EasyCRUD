FROM node
COPY . /opt
WORKDIR /opt
RUN npm install && npm run build
RUN cp -rf ./dist/* /var/www/html/
CMD ["apachectl","-DFOREGROUND"]
EXPOSE 80
