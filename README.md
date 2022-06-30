# Sync Doppler to AWS Lambda

Easy way to sync Doppler to AWS Lambda

## Variables

- **\*doppler_token:** Doppler API token
- **\*function_name:** AWS Lambda function name
- **\*aws_access_key_id:** The AWS access key ID.
- **\*aws_secret_access_key:** The AWS secret access key.
- **aws_region:** The AWS region. **default: us-east-1**

## Usage

```yml
- name: Deploy
  uses: Pubnic/sync-doppler-aws-lambda-action@v1
  with:
    doppler_token: <doppler_token>
    function_name: <function_name>
    aws_access_key_id: ${{ secrets.AWS_ACCESS_KEY_ID }}
    aws_secret_access_key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
    aws_region: ${{ secrets.AWS_DEFAULT_REGION }}
```

## Doc

[https://docs.doppler.com/docs/aws-lambda](https://docs.doppler.com/docs/aws-lambda)
