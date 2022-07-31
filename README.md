# Comandos Cloud formation

## Abaixo alguns comandos para ser executado dentro de 01-roles.

aws cloudformation deploy --template-file EcsInstanceRole1Resource.json --stack-name EcsInstanceRole1Resource --capabilities CAPABILITY_NAMED_IAM

aws cloudformation deploy --template-file EcsRole1Resource.json --stack-name Ecs1RoleResource --capabilities CAPABILITY_NAMED_IAM

aws cloudformation deploy --template-file ElasticContainerServiceTaskRole1Resource.json --stack-name ElasticContainerServiceTaskRole1Resource --capabilities CAPABILITY_NAMED_IAM

aws cloudformation deploy --template-file ElasticContainerServiceAutoscaleRole1Resource.json --stack-name ElasticContainerServiceAutoscaleRole1Resource --capabilities CAPABILITY_NAMED_IAM

## 02 - core ecs infra Em construção