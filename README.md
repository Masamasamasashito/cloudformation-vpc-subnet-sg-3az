# cloudformation-vpc-subnet-sg-3az

サクッとネットワークだけ作ってしまいたいときに使えます。
1サブネット＝1ネットワークACL=1ルートテーブル=1セキュリテイグループ　です。
セキュリティグループは、インバウンドなし、アウトバウンド全開です。
AZは、構成図のように1a,1c,1dとしています。

# 構成図

![構成図](https://github.com/Masamasamasashito/cloudformation-vpc-subnet-sg-3az/blob/main/cloudformation-vpc-subnet-nacl-routetable-sg-3az.jpg)

# 構成概要

* パブリックサブネット：9個
* プライベートサブネット：6個
* セキュリティグループ：15個（インバウンドなし、アウトバウンド全開）
* ネットワークACL:15個（デフォルト）
* ルートテーブル：15個（パブリックサブネットは 0.0.0.0/0 IGW 有）

# ymlアップロード後のプライベートIP等の入力画面

![画面](https://github.com/Masamasamasashito/cloudformation-vpc-subnet-sg-3az/blob/main/cloudformation-vpc-subnet-nacl-routetable-sg-3az-stack.jpg)

# CloudForamtion用ymlファイル

[https://github.com/Masamasamasashito/cloudformation-vpc-subnet-sg-3az/blob/main/cfn-vpc-subnet-sg-3az.yml](https://github.com/Masamasamasashito/cloudformation-vpc-subnet-sg-3az/blob/main/cfn-vpc-subnet-sg-3az.yml)

# drawioファイル

[https://github.com/Masamasamasashito/cloudformation-vpc-subnet-sg-3az/blob/main/cloudformation-vpc-subnet-nacl-routetable-sg.drawio](https://github.com/Masamasamasashito/cloudformation-vpc-subnet-sg-3az/blob/main/cloudformation-vpc-subnet-nacl-routetable-sg.drawio)
