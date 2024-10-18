# CoiPlugin
## プラグイン概要

CoiPluginは、Minecraftサーバー上でプレイヤーのインベントリを管理し、ロールバック機能を提供するプラグインです。このプラグインを使用することで、特定の時間範囲内でプレイヤーのインベントリを以前の状態に戻すことができます。また、ロールバックの履歴を管理し、必要に応じて元に戻すことも可能です。

## 注意  
ロールバックした際、アイテムを取ったチェストに
アイテムが戻る訳ではありませんので、管理者向けかと思います。

## コマンド解説

### /coi

プレイヤーのインベントリをロールバックするコマンドです。

#### 必須指定項目

- `/coi t:[time]` - ロールバックする時間範囲を指定します。例: `t:30m`（30分前までロールバック）

#### オプション

- `r:[radius]` - ロールバックの対象となるプレイヤーの範囲を指定します。  
例: `r:100`（半径100ブロック以内のプレイヤー）  
  
- `u:[player]` - ロールバックの対象となる特定のプレイヤーを指定します。複数指定が可能です。  
例: `u:playername`  
  
  
### /coiundo  
  
ロールバックの履歴を元に戻すコマンドです。  
  
#### 使用例  
  
```  
/coiundo  
```  

## 設定ファイル  
  
CoiPluginの設定ファイルは、`config.yml`という名前で保存されます。このファイルを編集することで、プラグインの動作をカスタマイズすることができます。  
  
### 設定ファイルの内容  
- `useMySQL`: MySQLを使用するかどうかを指定します。  
- `max-history`: ロールバックの履歴を保存する最大数を指定します。  
  
その他の設定は、`config.yml`を参照してください。  

当プラグインは、[MITライセンス](LICENSE)の下で配布されています。


`Author: Soryu-haruma(Asl, haruma9012kirby)`





