FROM python:alpine

# The following is typically supplied by the developers
# Install curl for testing purposes. (Not in production)

RUN pip install flask && apk add curl

# Copy the source code from the git reqpository into the docker image
COPY . .

ENTRYPOINT ["python"]
CMD ["rng.py"]
EXPOSE 8080
