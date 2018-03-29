## Usage

ライブリをインストールする。

```
composer install
```

`.env`ファイルを作成する。

```
cp env.example .env
````

最初にDBと権限を持ったユーザを作成する。

```
mysql>create database DB_NAME;
mysql>grant all on DB_NAME.* to 'USER_NAME'@HOST_NAME identified by 'PASSWORD';
```

migrate

```
$php artisan migrate
```

npm

```
nom install 
npm run dev
```

Local Serverを立ち上げる。

```
php -S localhost:8000 -t public
```




## License

The Lumen framework is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT)

