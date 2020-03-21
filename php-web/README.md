nginx+php-fpmを構築するdocker-composeのサンプルです。

### 起動方法
```
docker-compose up
```

ブラウザよりhttp://localhost:10080/index.php にアクセスすると、phpinfo()の結果が表示されます。

### ディレクトリのマウント

本ディレクトリがコンテナの/opt/appにマウントされています。
publicディレクトリがDocumentRootになります。

### ログ

dokcer/sync/log 以下に出力されます。

### ポートの変更

env.sampleを.envにコピーし、WEB_PORTを変更します。
