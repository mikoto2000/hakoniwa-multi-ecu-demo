## 前提

- OS: Windows 10 Pro
- Docker: Docker version 19.03.8, build afacb8b
- 以下のコマンドをインストール・パス設定済み(`MSYS2` でインストールした)
    - curl
    - tar

### デモのコンテナ構成

- Sensor ECU
    - IP: 172.16.238.5
- Moter ECU
    - IP: 172.16.238.4
- Control ECU
    - IP: 172.16.238.3
- ROS Master ECU
    - IP: 172.16.238.2
- Docker ホスト
    - `dig host.docker.internal +short` で取得
- コンパイル用コンテナ
    - IP: 172.16.238.6
    - コンパイル時点でホストの IP アドレスが必要なので Docker ネットワークに入れて、そこでコンパイルするようにした

詳細は `docker-compose.yml` を参照。


## デモ環境概要

TODO:図を入れたい

- ECU の構成
    - ROS Master(Ubuntu)
    - Sensor ECU(Athrill)
    - Controller ECU(Athrill)
    - Motor ECU)(Athrill)
- 通信仕様
    - ROS
        - Sensor ECU の Publish トピックのフォーマット
        - Controller ECU の Publish トピックのフォーマット
    - UDP
        - Host(Unity) から Sensor ECU Athrill への通信フォーマット
        - Motor ECU Athrill から Host(Unity) への通信フォーマット


## デモ環境構築手順

TODO: 動作確認完了したら worklog から転記。


## 実行手順

TODO: 動作確認完了したら worklog から転記。


## TODO

- Dockerfile のスリム化(一通りの動作確認が済んだら着手)


