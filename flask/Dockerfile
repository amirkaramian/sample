FROM python:3-alpine

# Create app directory
WORKDIR /src

# Install app dependencies
COPY requirements.txt ./

RUN pip install -r requirements.txt

# Bundle app source
COPY . .

EXPOSE 5000
CMD [ "flask","--app", "hello", "run","--host","0.0.0.0","--port","5000"]