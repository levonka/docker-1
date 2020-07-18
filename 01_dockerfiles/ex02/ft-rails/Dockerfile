FROM ruby:2.3.0

RUN apt-get update -y && \
	apt-get install -y build-essential libpq-dev nodejs sqlite3

ONBUILD COPY rails-app /opt/app
ONBUILD WORKDIR /opt/app

ONBUILD EXPOSE 3000
ONBUILD RUN bundle install && rake db:migrate && rake db:seed

# https://habr.com/ru/company/infobox/blog/240623/

# git clone https://github.com/IBM-Cloud/rails-4.20-blog.git
# docker build -t ft-rails:on-build .
# cd ../
# docker build -t ex02 .
# docker run -it --rm -p 3000:3000 ex02