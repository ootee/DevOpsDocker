FROM ruby:2.6.0

EXPOSE 3000

WORKDIR /mydir

RUN apt-get update && apt-get -y install curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN node -v && npm -v

RUN gem install bundler

COPY . .

RUN bundle install
RUN rails db:migrate

CMD rails s




