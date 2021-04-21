FROM node:alpine

# The following is typically supplied by the developers
# Install curl for testing purposes. (Not in production)

RUN npm install express && npm install redis && apk install curlj

# Copy the source code from the git reqpository into the docker image
COPY . .

ENTRYPOINT ["node"]
CMD ["webui.js"]
EXPOSE 8080
