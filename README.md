# Varnishの確認 (Vagrant version)

# 環境

- Vagrant
- Python3.7
- Ansible

# 起動方法

```bash
vagrant up --provision
# or
vagrant up
vagrant provision
```

# provisionでやっていること

1. EPEL追加 (これをしないとvarnishのインストールができない)
1. EPEL有効化
1. Varnishのリポジトリ追加
1. yumの更新 (上記の設定を適用するため)
1. varnishインストール
1. varnishの設定ファイルをホストからコピー
1. varnishサービスの起動・登録
