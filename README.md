# Sync Doppler to AWS Lambda

Easy way to sync Doppler to AWS Lambda

## Variables

- **\*doppler_token:** Doppler API token
- **\*function_name:** AWS Lambda function name
- **\*aws_access_key_id:** The AWS access key ID.
- **\*aws_secret_access_key:** The AWS secret access key.
- **aws_region:** The AWS region. **default: us-east-1**
- **extra_secrets:** Extra secrets to be added to the Lambda function. **default: '{}'**

## Usage

```yml
- name: Deploy
  uses: Pubnic/sync-doppler-aws-lambda-action@v0.1.3
  with:
    doppler_token: ${{ secrets.DOPPLER_TOKEN }}
    function_name: <function-name-production>
    aws_access_key_id: ${{ secrets.AWS_ACCESS_KEY_ID }}
    aws_secret_access_key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
    aws_region: ${{ secrets.AWS_DEFAULT_REGION }}
    extra_secrets: '{\"CUSTOM_SECRET\": \"secret\"}'
```

## Doc

[https://docs.doppler.com/docs/aws-lambda](https://docs.doppler.com/docs/aws-lambda)
