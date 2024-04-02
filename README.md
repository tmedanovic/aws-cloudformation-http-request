AWS CloudFormation custom resource NodeJs 20 lambda for making HTTP requests CloudFormation templates.

### Example 1 - [execute_http_lambda_test_one_key_output.yml](https://github.com/tmedanovic/aws-cloudformation-http-request/blob/main/execute_http_lambda_test_one_key_output.yml)

Executes GET request to http://echo.jsontest.com/key/value/one/two

JSON response:
```
{
   "one": "two",
   "key": "value"
}
```

Cloudformation output:

| Key                                   | Value | Export name                            |
|---------------------------------------|-------|----------------------------------------|
| GetHttpRequestFunctionOneKeyTestValue | two   | http-request-function-test-one-key-one |

### Example 2 - [execute_http_lambda_test_multiple_keys_output.yml](https://github.com/tmedanovic/aws-cloudformation-http-request/blob/main/execute_http_lambda_test_multiple_keys_output.yml)

Executes GET request to http://echo.jsontest.com/key/value/one/two

JSON response:
```
{
   "one": "two",
   "key": "value"
}
```

Cloudformation output:

| Key | Value | Export name                                  |
|-----|-------|----------------------------------------------|
| key | value | http-request-function-test-multiple-keys-key |
| one | two   | http-request-function-test-multiple-keys-one |
