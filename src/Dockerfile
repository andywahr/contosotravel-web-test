FROM node:10-alpine
ARG URL

VOLUME /artillery
WORKDIR /artillery

RUN npm install -g artillery
COPY ContosoTravel.Web.Artillery.yaml .

ENTRYPOINT ["artillery"]
CMD ["run /artillery/ContosoTravel.Web.Artillery.yaml -t http://${URL}"]