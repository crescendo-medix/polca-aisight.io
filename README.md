# POLCA-Aisight お試し版

### ダウンロード

macOS お試し版は [ここ](https://drive.google.com/file/d/15EC5xr8i1ZyiWrze5poxBqIax1ZhSEgX/view?usp=sharing/) からダウンロードしてください。

### 準備

1. Appleのデジタル署名（電子証明書）は付いていません。  
   セキュリティエラー（アプリが開けません）で起動できない場合は、下記のコマンド で解除してください。  
   ``` 
    xattr -rc /Applications/POLCA-Aisight.app
    ```

2. Ollamaの起動とモデルの登録

   1. Ollama（LLMのローカル実行ツール）を [公式サイト](https://ollama.com/) からダウンロードしてインストール、起動してください。  
   2. 下記のコマンドでモデルを登録してください。  
   　　  
   ```
    ollama create polars-coder -f llm/Modelfile  
    ollama create polars-coder-7b -f llm/Modelfile.7b
   ```
   > Modelfileはアプリのリソースディレクトリ配下に同梱されています。  
   > POLCA-Aisight.app/Contents/Resources/llm/Modelfile  

### 使用方法

POLCA-Aisightを起動し 下記の順で操作してください。  

1. データインポートでファイルを選択して インポートする。  
2. テーブル一覧でテーブルを選択する。  
3. プロンプトで実行したい処理を日本語で入力し 実行ボタン を押す。  


