# base Docker image being built on
FROM python:3.13.11-slim

# set up image by installing prerequisites
RUN pip install pandas pyarrow

# set up the working directory inside the container
WORKDIR /app
# copy the script to the container. 1st name is source file, 2nd is destination
COPY pipeline.py pipeline.py

# define the first step when the container runs
ENTRYPOINT ["python", "pipeline.py"]