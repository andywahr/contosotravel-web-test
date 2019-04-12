FROM node:10-alpine

VOLUME /artillery
WORKDIR /artillery

RUN npm install -g artillery@1.6.0-14
RUN ls -al /usr
COPY ContosoTravel.Web.Artillery.yaml .

CMD ["sh", "-c", "echo URL http://${URL};artillery run -t http://${URL} /artillery/ContosoTravel.Web.Artillery.yaml"]

