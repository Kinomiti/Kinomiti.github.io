#test

|hoge|fuga|
----|----
|System.Environment|ライブラリ|
|getArgs|コマンドライン引数を返す|
|getProgName|プログラム名を返す|
|getExecutablePath|実行ファイルの絶対パスを返す|
|getEnv|環境変数を返す|
|lookupEnv|環境変数を返す。なければNothingを返す。|
|setEnv|環境変数を設定する|
|unsetEnv|環境変数を削除する|
|withArgs|getArgsに値をセットする|
|withProgName|getProgNameに値をセットする|
|getEnvironment|環境変数を返す|

egWithArgs :: IO()
egWithArgs = withArgs args $ do
  print =<< getArgs
  where
    args = ["hello", "world"]
