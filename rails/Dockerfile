FROM rails:5.0.0

ENV CODE_PATH /usr/src/app

# china style
RUN gem sources --add https://gems.ruby-china.org/ --remove https://rubygems.org/

RUN bundle config mirror.https://rubygems.org https://gems.ruby-china.org

# install unicorn and set configure file
RUN gem install unicorn

# make code work path
RUN mkdir "$CODE_PATH"

VOLUME "$CODE_PATH"

WORKDIR "$CODE_PATH"

EXPOSE 8080

CMD ["bash", "-c", "bundle install && unicorn -E production"]