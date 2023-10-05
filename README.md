



## supabase postgres

- postgresql


1. supabaseプロジェクト作成
2. settings/databaseからデータベース情報を取得する
   1. `connecting string`のURIタブに書かれている
3. fly.ioのenvに値をデータベース情報を設定する
   1. `DB_CONNECTION=pgsql`
   2. `DATABASE_URL=postgresql://postgres:[データベースのパスワード]@db.[文字列].supabase.co:5432/postgres`
4. fly.ioで再deploy


DBのIP制限もしておく？  
バックアップの設定は？


## planetscale

- mysql



1. planetscaleでdb作成？
2. settings/passwordsで新しいパスワード作成
3. connection strings　(laravel)で`.env`の情報を取得する
4. fly.ioのenvに値をデータベース情報を設定する
   1. `DB_CONNECTION=mysql`
   2. `DB_HOST=aws.connect.psdb.cloud`
   3. `DB_USERNAME=[ユーザー名]`
   4. `DB_PASSWORD=[データベースのパスワード]`
   5. `MYSQL_ATTR_SSL_CA=/etc/ssl/certs/ca-certificates.crt`






IP restrictionsの設定をする？
バックアップの設定は？
