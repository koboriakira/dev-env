FROM mysql:5.7

# timezoneをJSTに設定
ENV TZ=Asia/Tokyo

# 大きなデータを送れるように、最大許容パケット量を増やしておく
# 下記ENTRYPOINTのオプションとなる
CMD ["--max_allowed_packet=32505856"]

# mysqlイメージにある下記シェルを実行する
# 中身は気にしなくてよさそうだけど、気になるなら調査すること
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
