## やられランチマップサイト
```
# runserver前に実施すること
$ python manage.py migrate
$ python manage.py loaddata users
$ python manage.py loaddata category

$ python manage.py runserver
```

# 事前準備
下記内容でページを作成しておく。

```
# ユーザ/カテゴリ
pytaro  中華料理
pyjiro  韓国料理
```

# 確認できる脆弱性
- Content Security Policy (CSP) Header Not Set
- Cookie No HttpOnly Flag
- アンチCSRFトークンが使用されていない（※ 敢えてアンチCSRFトークンを削除した場合）
