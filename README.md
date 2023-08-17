# Microservices

## Virtual Environment
### To create a virtual environment
python -m venv docker
docker/Scripts/activate

# to deactivate
docker/Scripts/deactivate

## to install pip
python3 -m pip install --upgrade pip
python3 -m pip install --user --upgrade pip

## To install dependencies
pip install -r requirements.txt

## To run the application
python flask_api.py

## Docker
### To build the image
docker build -t welcome-app .

### To run the image
docker run -d -p 8000:8000 welcome-app

### To stop the image
docker stop welcome-app

### To remove the image
docker rm welcome-app

### To push the image to docker hub
docker tag welcome-app <dockerhub_username>/welcome-app
docker push <dockerhub_username>/welcome-app

### To pull the image from docker hub
docker pull <dockerhub_username>/welcome-app

## to open the flask app in browser
http://localhost:8000/

## To run the tests
python -m pytest