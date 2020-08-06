# Cloudformation memo

## Reference
* [AWS CLI Reference](https://docs.aws.amazon.com/cli/latest/reference/cloudformation/)

## Command

* 失敗した時の調査
```bash
# aws cloudformation describe-stack-events --stack-name < stack name >
```

* 失敗した Stack を削除する
```bash
# aws cloudformation delete-stack --stack-name < stack name >
```

