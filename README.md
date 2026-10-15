# Linear Regression API

Roll Number: 14

A Flask API that generates a prediction using three input features
and fixed coefficients generated with random seed 14.

## Endpoint

GET /predict?x1=2&x2=3&x3=1

## Error Handling

The API returns HTTP 400 if any input is missing or non-numeric.

## Technology Stack

- Python 3.11
- Flask
- Docker
- Docker Compose
- Jenkins
- AWS EC2

Jenkins automation test: verifying automatic builds through the GitHub webhook.
