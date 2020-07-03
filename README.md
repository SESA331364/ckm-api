# ckm-api
This repository will host the FAQ API(s)  which will be used by Web Components (WORK IN PROGRESS)

 API details: 

Installing API locally: 

git clone \
npm install 

start app: 

node index.js 

npm start - for concurrency 

testing API: 

npn test - only in development env 

 

Error codes with http status: 

 

NO_RECORDS => 404  

If no content found, we are returning 404 this could be actually 204 

 

INTERNAL_ERROR=> 500 

jsforce auth error 

jsforce query error - malformed query 

 

MISSING_PARAMETER => 400 

Actual request: 

/faq/popular/pa/de/de  

/faq/popular/pv/de/de 

/faq/popular/gk/de/de 

 

Bad requests (results in 400 status): 

/faq/popular/pa/de - params missing 

/faq/popular/ws/de/de - valid article types are pa, pv, gk 

  

successful response will always have 200 http status code. 
