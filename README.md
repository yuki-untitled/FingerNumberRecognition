# FingerNumberRecognition サンプルの使い方

情報保障システム工学・演習 第12回「機械学習の活用」で使用したソースコード一式を公開します。
このプロジェクトは、あらかじめ作成したmodel_meta.jsonを読み込むことでWebカメラから指文字を認識するものです。  
VSCodeの「Live Server」拡張機能を使って、簡単に動作確認できます。

---

## 必要なもの

- Visual Studio Code（VSCode）
- Google Chrome などのモダンなWebブラウザ
- PCのWebカメラ

---

## セットアップ手順

### 1. このリポジトリをクローンまたはダウンロード

```
git clone https://github.com/yuki-untitled/FingerNumberRecognition.git
```
または、.zipでダウンロードして展開してください。

---

### 2. VSCodeでフォルダを開く

VSCodeを起動し、`index.html` があるフォルダを開きます。

---

### 3. Live Server 拡張機能をインストール

1. VSCode左側の拡張機能アイコン（四角いアイコン）をクリック
2. 検索ボックスに `Live Server` と入力  
   ([Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) ←こちらからアクセスするのも便利です)
3. 「Live Server」by Ritwick Dey を選択し、「インストール」ボタンをクリック

---

### 4. サンプルを起動

1. `index.html` をエディタで開く
2. 右下に「Go Live」ボタンが表示されるのでクリック  
   （または、右クリック→「Open with Live Server」でもOK）

---

### 5. ブラウザで動作確認

- ブラウザが自動で開きます（例: http://127.0.0.1:5500/index.html）
- 「ファイルを選択」から、model_meta.jsonをアップロードしてください
- （同一ディレクトリ内に、LinearSVCとLogRegモデルで作成したjsonデータを同梱しております。）
- 「Start」ボタンを押すとカメラが起動し、各関節の横に点が表示されます
- 映像の上に認識した結果が1~9で表示されます

---

## 注意事項

- 初回アクセス時にカメラ使用許可を求められます。「許可」してください
- カメラが認識されない場合は、他のアプリでカメラが使用中でないか確認してください

---

## 参考

- [今回作成したHTMLをデプロイしたWebサイト](https://handlandmarkstocsvrecorder.onrender.com/)
- [MediaPipe Hands 公式ドキュメント](https://google.github.io/mediapipe/solutions/hands.html)
- [Live Server 拡張機能ページ](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)

---