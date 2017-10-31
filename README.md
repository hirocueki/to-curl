# to-curl

- curlコマンドだけでmessageのCRUD(作成、読み取り、更新、削除)を実行してみてください。

# Answer

## show message
```shell
$ curl https://tryout.sonicgarden.jp/lecture/sample/messages/{:id}
```

## create message
```shell
$ curl https://tryout.sonicgarden.jp/lecture/sample/messages -X POST -d "lecture_sample_message[user]=ueki" -d "lecture_sample_message[text]=hello,PPAP"
```

## update message
```shell
$ curl https://tryout.sonicgarden.jp/lecture/sample/messages/{:id} -X PUT -d "lecture_sample_message[user]=ueki" -d "lecture_sample_message[text]=goodbye,PPAP"
```

## delete message

```shell
$ curl https://tryout.sonicgarden.jp/lecture/sample/messages/{:id} -X DELETE
```