# webfortune

Build Docker Image:
 docker build -t webfortune .

docker run -dp 8005:5000 riceala/webfortune

docker logs 
docker rm -f container

Run Application Locally:
python3 -m venv env
source env/bin/activate
pip install -r requirements.txt

python3 -m flask run --host=0.0.0.0 --port=8005
