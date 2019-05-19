# test
https://employment.en-japan.com/engineerhub/entry/2017/01/31/110000#%E4%BD%9C%E6%A5%AD%E3%83%96%E3%83%A9%E3%83%B3%E3%83%81%E3%82%92%E4%BD%9C%E6%88%90%E3%81%99%E3%82%8B

を参考にローカル環境からコミットできるようにしてみた。初期設定でエディターをVScodeにしていたのでコミットに失敗していたみたい？
結局
https://qiita.com/y-tsutsu/items/2ba96b16b220fb5913be
を参考にして
$ git config --global core.editor 'code --wait'
$ git config --global merge.tool 'code --wait "$MERGED"'
$ git config --global push.default simple
を追加しHTTPSでリポジトリをローカルにクローンし直してVScode上からコミットしたら反映された。これたぶんSSH接続ってやつされてないよな......。
