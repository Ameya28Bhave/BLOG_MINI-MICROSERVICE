FROM node:14-alpine
 
# Add the following lines
ENV CI=true
ENV WDS_SOCKET_PORT=0
 
WORKDIR /app

# Install dependencies
COPY package.json ./
RUN npm install
COPY ./ ./
 
# Default command
CMD ["npm", "start"]