# Comandos Cloud formation

aws cloudformation deploy --template-file EcsInstanceRole1Resource.json --stack-name EcsInstanceRole1Resource --capabilities CAPABILITY_NAMED_IAM


aws cloudformation deploy --template-file EcsRole1Resource.json --stack-name Ecs1RoleResource --capabilities CAPABILITY_NAMED_IAM