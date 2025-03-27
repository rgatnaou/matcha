FROM node

WORKDIR /app

# Copy package files
COPY app/package.json app/tsconfig.json app/tsconfig.node.json app/tsconfig.app.json .

# Install dependencies
RUN npm install

# Copy application code
COPY app .

EXPOSE 5173
# CMD ["npm", "run", "dev"]
CMD ["npm", "run", "dev", "--", "--host"]
