# Read me

The original idea is from  
https://itnext.io/run-and-test-dynamodb-applications-locally-using-docker-and-testcontainers-ba90ea79e6f4

# connect and create a table

```
aws dynamodb create-table --endpoint-url http://localhost:8000 --table-name Books --attribute-definitions AttributeName=ISBN,AttributeType=S --key-schema AttributeName=ISBN,KeyType=HASH --billing-mode PAY_PER_REQUEST
```

# list tables

```
aws dynamodb list-tables --endpoint-url http://localhost:8000
```