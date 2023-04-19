## Popular commands of DynamoDb
### Create Table 

``` aws dynamodb create-table --table-name ProductCatalog --attribute-definitions AttributeName=Id,AttributeType=N --key-schema AttributeName=Id,KeyType=HASH --provisioned-throughput ReadCapacityUnits=5,WriteCapacityUnits=5 ```

### Populate data from a file in DynamoDb table
``` aws dynamodb batch-write-item --request-items files://item.json ```

**Note:** item.json is file name from which we need to copy data.