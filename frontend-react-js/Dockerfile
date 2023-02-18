FROM node:16.18

ENV PORT=3000

COPY . /frontend-react-js
WORKDIR /frontend-react-js
RUN npm install

COPY myscript.sh /frontend-react-js/myscript.sh
RUN chmod +x /frontend-react-js/myscript.sh

EXPOSE ${PORT}
CMD ["/frontend-react-js/myscript.sh"]
