# cloudformation-vpc-subnet-sg-3az

さくっと検証したいときに、サクッとネットワークだけ作るために使えます。

1サブネット＝1ネットワークACL=1ルートテーブル=1セキュリテイグループ　で作りました。

セキュリティグループは、インバウンドなし、アウトバウンド全開です。

AZは、構成図のように1a,1c,1dとしています。

よかったらご利用ください。

# 構成図

![構成図](https://github.com/Masamasamasashito/cloudformation-vpc-subnet-sg-3az/blob/main/cloudformation-vpc-subnet-nacl-routetable-sg-3az.jpg)

# ymlアップロード後のプライベートIP等の入力画面

![画面](https://github.com/Masamasamasashito/cloudformation-vpc-subnet-sg-3az/blob/main/cloudformation-vpc-subnet-nacl-routetable-sg-3az-stack.jpg)

# CloudForamtion用ymlファイル

[https://github.com/Masamasamasashito/cloudformation-vpc-subnet-sg-3az/blob/main/cfn-vpc-subnet-sg-3az.yml](https://github.com/Masamasamasashito/cloudformation-vpc-subnet-sg-3az/blob/main/cfn-vpc-subnet-sg-3az.yml)
