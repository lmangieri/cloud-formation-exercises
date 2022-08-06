# Comandos Cloud formation

## Abaixo alguns comandos para ser executado dentro de 01-roles.

aws cloudformation deploy --template-file EcsInstanceRole1Resource.json --stack-name EcsInstanceRole1Resource --capabilities CAPABILITY_NAMED_IAM

aws cloudformation deploy --template-file EcsRole1Resource.json --stack-name Ecs1RoleResource --capabilities CAPABILITY_NAMED_IAM

aws cloudformation deploy --template-file ElasticContainerServiceTaskRole1Resource.json --stack-name ElasticContainerServiceTaskRole1Resource --capabilities CAPABILITY_NAMED_IAM

aws cloudformation deploy --template-file ElasticContainerServiceAutoscaleRole1Resource.json --stack-name ElasticContainerServiceAutoscaleRole1Resource --capabilities CAPABILITY_NAMED_IAM

## 02 - core ecs infra Em construção

### Comando abaixo serve para validar um template cloudformation criado.
aws cloudformation validate-template --template-body file://coreEcsInfra.yaml


### Abaixo é um comando para descrever os eventos de uma eventual stack cloud formation que tenha falhado
aws cloudformation describe-stack-events --stack-name coreEcsInfra


### Abaixo é um comando para verificar a region que o aws command line está configurado
aws configure get region

### Abaixo é um comando para setar region no command line
aws configure set region us-east-1

### Executando deploy da VPC e subnets 
aws cloudformation deploy --template-file coreEcsInfra.yaml --stack-name coreEcsInfra --capabilities CAPABILITY_NAMED_IAM