# Use Python 3.9 version base image
FROM python:3.9

# install pandas lib
RUN pip install pandas

# create app directory and cd into it
WORKDIR /app

# copy pipeline.py from source/host to destination/container
COPY pipeline.py pipeline.py

# start a bash shell
# ENTRYPOINT [ "bash" ]

# if we want to auto execute pipeline.py after container spinning
ENTRYPOINT [ "python", "pipeline.py" ]



# Notes:
# We can use imperative cmd to get the same functionalities
# docker run -it --entrypoint=bash python:3.9
