# DeepLearningEnd2End

aws configure


# Workflows

- constants
- config_entity
- artifact_entity
- components
- pipeline
- main

# Bentoml
- Model serving  -> Provide api's -> serving the model to the user
- Application packaging  -> bento.yaml -> Bento Image -> AWS, Azure
- Deployment


bentoml models list

bentoml serve service.py:service --reload

bentoml build

=====================================

bentoml build
bentoml containerize xray_service:latest -t 506234360787.dkr.ecr.us-east-2.amazonaws.com/xray_bento_image:latest
aws ecr get-login-password --region us-east-2 | docker login --username AWS --password-stdin 506234360787.dkr.ecr.us-east-2.amazonaws.com
docker push 506234360787.dkr.ecr.us-east-2.amazonaws.com/xray_bento_image:latest
