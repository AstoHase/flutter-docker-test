1.gitクローンします
3.クローンしたファイルに移動
2.クローン後、
        docker compose up -d 
    でたちあげ（初回は-dない方がデバックしやすい）
3.完了後　
        docker exec -it flutter bash
    でコマンドをたちあげ


4. flutterをいれる
    cd /usr/local/workspace
    移動して、
    -- flutter file がないとき,あるときはskip --
    flutter create .
    でファイル作成。
    -- end --

5. flutter run -d web-server --web-port=${WEB_SERVER_PORT} --web-hostname 0.0.0.0
    でwebサーバーで開ける