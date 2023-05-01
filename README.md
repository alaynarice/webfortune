# webfortune

Build Docker Image:

- docker build -t riceala/webfortune .

- docker run -dp 8005:5000 riceala/webfortune

docker logs \<container_id>
docker rm -f \<container_id>

Run Application Locally:

 - python3 -m venv env
 - source env/bin/activate
 - pip install -r requirements.txt
 - python3 -m flask run --host=0.0.0.0 --port=8005

The Flask application should support the following routes:

a. GET /fortune/

b. GET /cowsay/\<message>/
 
c. GET /cowfortune/
 
d. GET /
 
(a) should simply display the output of the 'fortune' command.
 
(b) should display the output of the 'cowsay' command given <message> as
its command line input
 
(c) should pipe the output of fortune as the input to the cowsay command.
 
(d) redirects to (a)
 
 Testing:
 - pytest-3 test_app.py - should run through pre-defined tests 
