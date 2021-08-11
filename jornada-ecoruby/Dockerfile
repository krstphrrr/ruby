FROM ruby:latest
ENV RAILS_ENV=production

# RUN mkdir /usr/ruby
COPY ./ruby /usr/ruby

WORKDIR /usr/ruby/home/mwallace/ecotrends

# RUN ls
# COPY Gemfile Gemfile.lock ./

RUN bundle update --bundler
RUN bundle exec rake assets:precompile
RUN bundle install 

# COPY . .

CMD ["./config/application.rb"]