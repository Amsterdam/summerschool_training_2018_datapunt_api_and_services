# Summerschool Training Datapunt API en Services

This is the jupyter notebook sllde deck used for our Summerschool training 2018 which can be viewed here: 

https://amsterdam.github.io/summerschool_training_2018_datapunt_api_and_services/

## How re-use the slides
 
```
git clone https://github.com/Amsterdam/summerschool_training_2018_datapunt_api_and_services.git
cd src 
pip install -r requirements.txt
jupyter notebook 
```

## How to build and run the slides locally

To build the site for local testing and for deployment on github.io using the docs folder:
```
cd src
make docs
```

To view the site on localhost:8000:
```
 cd..
 cd docs
 python3 -m http.server
```
