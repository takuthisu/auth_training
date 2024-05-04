# auth_training
認証・認可に関してのトレーニング

## AWS Amplify × vue 
こちらのトレーニングはAWSアカウントが準備できている前提で行われる。

1. npm install
```
$ npm install
```

2. AWSマネジメントコンソールにアクセスしておく
使用予定のアカウントでAWSマネジメントコンソールにログインしておく

3. 環境のセットアップ
```
$ amplify configure
```
この時に、AWSマネジメントコンソールが開かれる。
amplifyで使用するアカウントを準備する必要があるので、このタイミングで作成する。

4. amplifyの開始
```
$ amplify init
```
amplifyを開始して、アプリケーションの設定を行う

5. アプリの公開
```
$ amplify add hosting
$ amplify publish
```

6. 認証の追加
```
$ amplify add auth
```
