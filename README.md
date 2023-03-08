# serverspec-test
serverspecの動作確認用のサンプルplaybook。  

- hosts.yml: 対象のIPを変更
- properties.yml: 対象のIPを変更

## 動作確認済みバージョン
- Serverspec：2.42.2

## ディレクトリ構成
```
serverspec
|-- .rspec
|-- Rakefile
|-- hosts.yml
|-- properties.yml
`-- spec
    |-- base
    |   |-- dns_spec.rb
    |   `-- sshd_spec.rb
    |-- db
    |   `-- postgres_spec.rb
    `-- spec_helper.rb
```

## 実行例
$ rake -T
$ rake spec LOGIN_PASSWORD=password
