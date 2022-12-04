# start by pulling the python image
FROM python:3.7.15-alpine3.17

# switch working directory
WORKDIR /app

# copy the requirements file into the image
COPY ./requirements.txt requirements.txt

# install the dependencies and packages in the requirements file
RUN pip install -r requirements.txt

# copy every content from the local file to the image
COPY ./flaskr/ /app/flaskr/

# configure the container to run in an executed manner
ENTRYPOINT [ "python" ]

CMD ["flaskr/__init__.py" ]
