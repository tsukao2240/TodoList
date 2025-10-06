# TodoList

Laravelを使ったシンプルなTodoリストアプリケーションです。

## 必要な環境

- PHP >= 7.2
- Composer
- MySQL または SQLite

## インストール

### 1. 依存関係のインストール

```bash
cd quickstart
composer install
```

### 2. 環境設定

```bash
cp .env.example .env
php artisan key:generate
```

### 3. データベース設定

`.env`ファイルを編集して、データベース接続情報を設定します。

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=todolist
DB_USERNAME=your_username
DB_PASSWORD=your_password
```

SQLiteを使用する場合:

```env
DB_CONNECTION=sqlite
```

### 4. マイグレーション実行

```bash
php artisan migrate
```

## 使い方

### 開発サーバーの起動

```bash
php artisan serve
```

ブラウザで `http://localhost:8000` にアクセスします。

## 機能

- Todoの追加
- Todoの一覧表示
- Todoの削除

## 技術スタック

- Laravel 6.x
- Bootstrap 4
- MySQL/SQLite
