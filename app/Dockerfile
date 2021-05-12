FROM ruby:2.7-alpine

WORKDIR /app

ADD Gemfile Gemfile.lock /app/
RUN bundle install -j 8

ADD . /app

COPY . /app

EXPOSE 80

CMD ["ruby", "http_server.rb"]