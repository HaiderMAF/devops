#Use official Python runtime as a parent image
From python:2.7-slim
#Set the working directory to /app
WORKDIR /app
#Copy the currentdirectory contents into the container at /app
COPY . /app
#Install needed packages specified in requirements.txt
RUN pip install --trusted-host pypi.python.org -r requirements.txt
#EXpose port available to outside this container
EXPOSE 80
#Define environment variable
ENV NAME World
#Run app.py when the container launches
CMD ["python", "app.py"]
