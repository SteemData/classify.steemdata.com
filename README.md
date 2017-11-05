## TODO
 - store last processed block in Redis
 - write a steemit comment
 - test rq worker
 - create a deployment

# Requirements
This guide assumes MacOS with HomeBrew.

## Dependencies
Install JS dependencies:
```
npm install -g browserify

cd public
npm i

browserify -r eosio > bundle.js
```


Install Python 3.6. 
```
brew install python3
```


Install Python dependencies:
```
pip install -r requirements.txt
```


## Run Locally
Run the Flask server:
```
export FLASK_APP=src/views.py
flask run --reload --debugger
```


## Environment Variables

| Variable      | Default                          |
| ------------- | -------------------------------- |
| PRODUCTION    | False                            |
| SECRET_KEY    | not_a_secret                     |
