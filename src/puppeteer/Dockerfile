FROM armno/node-chromium:11.6.0


ENV PUPPETEER_SKIP_CHROMIUM_DOWNLOAD=true
ENV PUPPETEER_EXECUTABLE_PATH=/usr/bin/chromium

COPY . /project
COPY tsconfig.json /tsconfig.json

WORKDIR /project

RUN npm install

ENTRYPOINT ["node", "dist/index.js"]