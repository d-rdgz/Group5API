# Group5API
Repository for TCMG 412's team 5 API Project.

### Requirements:
	(1) Python 3
	(2) Python libraries:
		flask
		slackclient version 1.0.0
#### Using Docker
	(1) Clone this repo
	(2) cd into the cloned repo
	(3) build docker image: docker build -t image_name .
	(4) run app.py inside the image: docker run -p 5000:5000 image_name
	Prepare to Push to docker hub:
	(1) Tag the image: docker tag image_name docker_hub_username/image_name
	(2) Push to docker hub: docker push docker_hub_username/image_name
	(3) Pull from docker: docker pull docker_hub_username/image_name
	(4) Run app.py inside the container: docker run -p 5000:5000 docker_hub_username/image_name

##### /md5/string Endpoint:

##### /factorial/int Endpoint:

##### /fibonacci/int Endpoint:

##### /is-prime/int Endpoint:

##### /slack-alert/string Endpoint:
	(1) Uses python library: slackclient version 1.0.0 
		Very important to use slackclient version 1.0.0, newer versions won't work this way.
		pip install slackclient==1.0.0
	(2) The function posts either in #general or in #spr20-group5-test channels:
 		change which channel by switching out the ID found above the route's function.
