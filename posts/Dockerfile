# Use an existing image as a base
# repository:tagname
FROM node:alpine

# Download and install a dependency
# Alpine Package Keeper (apk) similar to apt-get install
WORKDIR /app
COPY package*.json ./
RUN npm install	
COPY ./ ./

# tell the image what to do when it starts as a container
CMD [ "npm", "start" ]

# docker build -t kimmi1206/posts . 
# docker run -p 8080:8080 kimmi1206/simpleweb
# docker run [image_id/image_tag]
# docker run -it [image_id/image_tag] [cmd]
# docker ps
# docker exec -it [container_id] [cmd]
# docker logs [container_id]

# docker build -t kimmi1206/posts .
# docker build -t kimmi1206/comments .
# docker build -t kimmi1206/query .
# docker build -t kimmi1206/moderation .
# docker build -t kimmi1206/event-bus .
# docker build -t kimmi1206/client .

# docker tag local-image:tagname new-repo:tagname
# docker push new-repo:tagname
# docker push kimmi1206/posts
# docker push kimmi1206/event-bus
