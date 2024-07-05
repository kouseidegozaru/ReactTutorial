# GitHubの基礎的な使用方法
GitHubに関する基本的な知識がある前提で説明しています。

## 環境構築
1. リポジトリ作成
    <p>GitHubのwebページでリポジトリを作成</p>

2. 初期設定
    <p>プロジェクトのディレクトリに移動後、次を実行</p>

    ```
    git init
    ```

## ソース取得(既にリポジトリが存在する場合)
```
git clone [clone_url]
cd [cloneして生成されたディレクトリ]
```

## Pushまで
1. コミットするファイルの選択
    - すべてをコミットする場合
        ```
        git add -A
        ```

    - ファイルを選択する場合
        ```
        git add xxxx
        ```

2. ローカルリポジトリにCommit
    ```
    git commit -m "メッセージを記述"
    ```

3. リモートリポジトリに接続(2回目以降は不要)
    ```
    git remote add origin https://github.com/username/repository.git
    ```

4. リモートリポジトリにPush
    ```
    git push -u origin master
    ```

## ブランチ関連
- ローカルリポジトリのブランチ確認
    ```
    git branch
    ```

- ブランチをきる(ブランチを作る)
    ```
    git branch xxxx
    ```

- ブランチに移動(チェックアウト)
    ```
    git checkout xxx
    ```