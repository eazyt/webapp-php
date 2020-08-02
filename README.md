# Project Title
---> Docker Web-Server and PHP <---

# Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

# Prerequisites
- Any OS running docker

# Installing
- once docker is install and running
- verifying with docker --version
- navigate to the root folder of the project(this webapp-php)

### Option 1(Using the Dockerfile)
- run docker build -t <YOUR-CHOICE-OF-NAME> <CURRENT-DIRECTORY>
	together with Dockerfile an image will be created.
  	eg. docker build -t webapp .

- docker images 
  command should show the webapp images created in the previous step.

# Running the tests
- docker run -d -p 80:80 webapp 
- this command will run docker image in the background access via localhost:80 or (OPTIONAL: Dynamic DNS)

# Option 2(Using docker-compose file)
- run docker-compose -up -d
	it will create an image and run it immediately after creation. 

# Installing elinks for viewing the running homepage
- yum install elinks -y
# Opening and viewing the page
- elinks http://localhost:80


# Authors
- Thabo

# License
This project is licensed under the MIT License - see the LICENSE.md file for details
