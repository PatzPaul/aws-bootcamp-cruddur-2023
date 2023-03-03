FROM python:3.10-slim-buster

#inside container
# create a new folder inside container
WORKDIR /backend-flask

# outside container to inside container
# contains libraries needed for installation to run the app 
COPY requirements.txt requirements.txt

#inside container
#install python libraries used for the app
RUN pip3 install -r requirements.txt

#outside container -> inside container
#period means everything in the current directory 
#first period . /backend-flask (outside container)
#last period  . /backend-flask (inside container)
COPY . .

# set environment variables(Env Vars)
#inside container and will remain active when container is running
ENV FLASK_ENV=development

EXPOSE ${PORT}

#CMD (Command)
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]