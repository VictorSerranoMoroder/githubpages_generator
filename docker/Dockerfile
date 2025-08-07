FROM ubuntu

RUN apt-get update && apt-get -y --no-install-recommends install \
    build-essential \
    git \
    wget \
    curl \
    npm 

RUN npm install -g hexo-cli hexo-deployer-git