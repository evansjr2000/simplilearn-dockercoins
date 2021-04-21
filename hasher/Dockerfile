FROM ruby:alpine

# The following is typically supplied by the developers
# Install curl for testing purposes. (Not in production)

RUN apk add build-base && RUN gem install sinatra && RUN gem install thin
# Copy the source code from the git reqpository into the docker image
COPY . .

ENTRYPOINT ["ruby"]
CMD ["hasher.rb"]
EXPOSE 8080
