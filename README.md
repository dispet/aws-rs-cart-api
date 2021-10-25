#### Docker
* docker build -f ./Dockerfile -t cart-api:latest .
* docker images
* docker image rm 4e2bda0db639


#### Elastic Beanstalk cli
# Init:
* eb init dispet-cart-api --region eu-west-1
# Create a new environment:
* eb create develop --single --cname dispet-cart-api-dev --envvars NODE_ENV=production,ENV_CONFIG=dev
# Deploy:
* eb deploy develop --region eu-west-1
# Terminate environment:
* eb terminate develop
