FROM node:10-alpine

VOLUME /artillery
WORKDIR /artillery

RUN npm install -g artillery@1.6.0-14
COPY ContosoTravel.Web.Artillery.yaml .

ENTRYPOINT ["artillery"]
CMD ["run /artillery/ContosoTravel.Web.Artillery.yaml -t ${URL}"]