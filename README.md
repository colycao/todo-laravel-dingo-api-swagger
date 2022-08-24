# 「TODOリスト」LaravelでAPI実装


シンプルなAPIは、Laravelで構築されたToDoリストを管理する。
- [x] TODO（やること）を登録できる
- [x] 登録したTODOを変更できる
- [x] 登録したTODOを削除できる
- [x] 登録されているTODOを一覧で表示できる
- [x] 登録したTODOの完了状態をメモする

## Demo
https://clara-coly-todo.herokuapp.com/

- [x] API仕様書 https://clara-coly-todo.herokuapp.com/api/documentation
- [x] DBのテーブル　clara_coly_todo-20220824.sql
- [x] 管理システム https://clara-coly-todo.herokuapp.com/admin/todos

## Installation

1. Clone the repo locally:
    ```sh
    git clone git@github.com:colyii/clara-coly-todo.git
    cd clara-coly-todo
    ```

2. Install dependencies
    ```sh
    composer install
    ```

3. Copy the contents of `.env.example` to a `.env` file, or simply run this command:

    ```bash
    # Mac Linux
    cp .env.example .env
    # Windows
    copy .env.example .env
    ```

4. Generate application key (if not already generated)
    ```sh
    php artisan key:generate
    ```

5. Run database migrations
    ```sh
    php artisan migrate
    ```

6. Run database seed
    ```sh
    php artisan db:seed
    ```

7. Run the dev server (the output will give the address):
    ```sh
    php artisan serve
    ```

## Running tests
```sh
./vendor/bin/pest --filter TodoTest
```
or
```sh
php artisan test
```

## Pending

- [ ] Add JWT
