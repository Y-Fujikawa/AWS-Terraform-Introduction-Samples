## 作業環境の準備
### Terraformをインストールする
ローカルマシンでTerraformを使えるようにする。
`Terraform v1.0.0` まで表示されれば準備完了。

```
$ brew install tfenv
$ tfenv install 1.0.0
$ tfenv use 1.0.0
$ terraform -v
Terraform v1.0.0
```

### AWSアカウントの準備
```
$ cp terraform.tfvars.sample terraform.tfvars
```
`terraform.tfvars` の内容を自分のAWSアカウントに変更する。

## 実行
```
$ cd dev/services/webservers
$ terraform plan # 実行計画が正常に出ればOK
$ terraform apply # yes を入力すると実際に適用される
```

## FYI
Please check - [https://www.bogotobogo.com/DevOps/Terraform/Terraform-AWS-ASG-Modules](https://www.bogotobogo.com/DevOps/Terraform/Terraform-Introduction-AWS-ASG-Modules.php)
