FROM ruby:2.3.1-slim
RUN apt-get update
ENV APP_PATH /usr/src/app
RUN mkdir -p $APP_PATH
WORKDIR $APP_PATH
COPY . $APP_PATH
EXPOSE 80
CMD ["ruby", "http_server.rb"]
