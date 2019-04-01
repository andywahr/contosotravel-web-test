FROM node:10-alpine

VOLUME /artillery
WORKDIR /artillery

RUN npm install -g artillery
COPY ContosoTravel.Web.Artillery.yaml .

ENTRYPOINT ["artillery"]
CMD ["run /artillery/ContosoTravel.Web.Artillery.yaml"]