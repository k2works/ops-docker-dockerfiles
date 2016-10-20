FROM ruby:2.3.1

ENV APP_ROOT /usr/src/app

WORKDIR $APP_ROOT

RUN apt-get update && apt-get install -y \
                                      vim \
                                      curl && rm -rf /var/lib/apt/lists/*
RUN apt-get update && apt-get install -y \
                                      mysql-client postgresql-client \
                                      sqlite3 --no-install-recommends \
                                      xvfb libqt4-dev libqtwebkit-dev \
                                      xauth \
                                      nodejs --no-install-recommends && rm -rf /var/lib/apt/lists/*

RUN apt-get update && apt-get install -y \
                                      zip \
                                      python3-pip && rm -rf /var/lib/apt/lists/*

RUN \
  pip3 install boto3==1.3.0
