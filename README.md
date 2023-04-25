# docker-react-npm-typescript
## 概要
- `typescript`を使用して`npm`で`react`を起動する`dockerfile`と手順を記したリポジトリ。
- 詳細な使用方法は、以下のQiitaか個人ブログを参照。
    - [【環境構築】DockerでReactをnpmを使用して作成&起動する方法（JavaScript編）](https://qiita.com/takuma-1234/items/02d5683ea54c3c16b38c)
    
    
### Docker起動コマンド
```bash:
$docker-compose up -d --build
```

### react起動までの基本手順コマンド
- `vscode`でコンテナ内部に入る。
- `vscode`でターミナルを起動し作業ディレクトリに移動する。
```bash:
$cd ../react_npm_typescript_workdir/
```
- `react`アプリの雛形を作成
```bash:
$npx create-react-app react_npm_typescript  --template typescript
```
- `react`のアプリを`install`するかを聞かれるので`y`を入力して`Enter`を押す。
```bash:
Need to install the following packages:
  create-react-app@5.0.1
Ok to proceed? (y) 
```
- 作成されたディレクトリへ移動
```bash:
$cd react_npm_typescript/
```
- `react`を起動する。

```bash:
$npm start
```

#### 参考資料
