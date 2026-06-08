FROM ruby:3.2-slim

RUN apt-get update && \
    apt-get install -y --no-install-recommends build-essential git && \
    rm -rf /var/lib/apt/lists/*

WORKDIR /site

COPY Gemfile Gemfile.lock ./
RUN bundle install --jobs 4

EXPOSE 4000 35729

CMD ["bundle", "exec", "jekyll", "serve", "-H", "0.0.0.0", "--port", "4000", "--livereload"]
