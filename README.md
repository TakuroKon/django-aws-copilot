# このプロジェクトは
django のwebアプリを AWS copilot を利用してECSへデプロイする、動作確認のためのプロジェクト

AWS copilot へのデプロイ手順に関しては以下を参考にした
https://www.endpointdev.com/blog/2022/06/how-to-deploy-containerized-django-app-with-aws-copilot/

# django をローカルで runserver する手順

- Dockerfile の expose をコメントアウトする
- docker-compose.yaml でポート指定する
- 以下のコマンドを実行する

```
docker-compose up --build
```

- http://localhost:8000/ で動作を確認できる