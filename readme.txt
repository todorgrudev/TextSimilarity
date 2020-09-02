#This is a simple API that check the Similarity of text
Technologie used
	Python
	Flask
	flask_restful
	pymongo
	bcrypt
	spacy
	docker
	docker-compose
	postman


Samples for user input(json):
	for /register:
{
	"username": "test",
	"password": "secure"   
}

	for /detect:		#default tokens =5
{
    "username": "test",
    "password": "secure",
    "text1":"This is a simple program and it looks great!",
    "text2":"This program is simple, but it looks great :)"
    #The output is a float between 0 and 1. Closer to 1 = more similarity
}

	for /refill  		#admin_pw is hardcoded to abc123 
{
	"username": "test",
    	"admin_pw" : "abc123",
    	"refill": 5
}
