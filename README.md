# docker-2048game（コンテナ イメージは gowatana/docker-2048）

2048ゲームのDockerコンテナです。
2048ゲームのソースは <https://github.com/gabrielecirulli/2048> を利用しています。

## 利用方法（Docker Hubから）

コンテナの起動。

```
# docker container run -itd --rm -p 8000:80 gowatana/docker-2048
```

Webブラウザからアクセス。

```
http://コンテナホストのIP:8000
```

## 利用方法（ローカルでビルド）

コンテナイメージのビルド。

```
# ls -1
Dockerfile
default.conf
# docker build -t docker-2048 .
```

コンテナの起動。

```
# docker container run -itd --rm -p 8001:80 docker-2048
```

Webブラウザからアクセス。

```
http://コンテナホストのIP:8001
```

以上。
