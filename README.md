# codebuild-docker-image-sample

## masterにマージされたら自動でビルドする
cfn.yamlを流してから以下を叩く
```
aws codebuild create-webhook --project-name ${project-name} --branch-filter master
```

上記設定削除
```
aws codebuild delete-webhook --project-name ${project-name}
```
