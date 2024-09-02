# qiita-content
- qiitaとgithubを連携させるために用いた参考資料
    - https://github.com/increments/qiita-cli
- qiitaについてもアクセストークンを発行して、使い回す。
# github-cli連携
- httpsではなく、セキュリティの観点からssh接続がベスト
- ssh接続方法
    - 公開鍵発行
        - [ssh-keygen -t ed25519 -C "your.email@example.com"]
    - 公開鍵をgithubに登録
    - リモートについてhttpsからsshに変更
        - [git remote set-url origin git@github.com:user/qiita-content.git]
    - sshでローカルリポジトリのソースコードをブランチ指定してpushする
        - [git push origin main]

     
