FROM ruby:2.2-slim

RUN gem install riemann-client riemann-tools riemann-dash

COPY riemann-dash.rb /etc/riemann-dash.rb

CMD riemann-dash /etc/riemann-dash.rb
#ENTRYPOINT ["riemann-dash"]
