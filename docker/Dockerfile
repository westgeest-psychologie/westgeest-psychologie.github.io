FROM ruby:3.3-slim AS jekyll

RUN apt-get update && apt-get install -y --no-install-recommends \
    build-essential \
    git \
    && rm -rf /var/lib/apt/lists/*

RUN adduser jekyll

COPY jekyll-entrypoint.sh /usr/local/bin/

USER jekyll
RUN gem update --system && gem install jekyll && gem cleanup

EXPOSE 4000

WORKDIR /site


ENTRYPOINT ["jekyll"]

CMD ["--help"]

FROM jekyll AS jekyll-serve

ENTRYPOINT ["jekyll-entrypoint.sh"]

CMD [ "bundle", "exec", "jekyll", "serve", "--force_polling", "-H", "0.0.0.0", "-P", "4000" ]

