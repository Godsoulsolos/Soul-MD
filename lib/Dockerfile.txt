FROM quay.io/sampandey001/secktor
RUN git clone https://github.com/Godsoulsolos/Soul-MD /root/Godsoulsolos
WORKDIR /root/Godsoulsolos/
RUN npm install npm@latest
RUN npm install
EXPOSE 8000
CMD ["npm", "start"]
