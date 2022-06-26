FROM nodered/node-red

#
# Add nodes modules for Node-RED
#   https://nodered.org/docs/getting-started/docker
#
COPY package.json .
# COPY settings.js /data/settings.js
# COPY flows_cred.json /data/flows_cred.json
# COPY flows.json /data/flows.json
COPY data/*.* /data/

RUN npm install --unsafe-perm --no-update-notifier --no-fund --only=production
