FROM node:18
WORKDIR /app

# Install Angular CLI globally
RUN npm install -g @angular/cli

# Copy package files first
COPY package*.json ./
RUN npm ci

# Copy source code
COPY . .

EXPOSE 4200
CMD ["ng", "serve", "--host", "0.0.0.0"]
