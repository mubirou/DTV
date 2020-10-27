# VideoEditing
映像編集関係メモ


### <b>INDEX</b>
* [DaVinci作業フォルダ](#daVinciFolder): 作業フォルダの設定
* [DaVinci Resolve入門](#daVinciFirstStep): XXXX
* [DaVinci カット入門](#daVinciCut): XXXX

***


<a name="daVinciFolder"></a>
## ◆DaVinci作業フォルダ

### 説明
DaVinci Resolveで編集する際に使う作業フォルダを設定します。

### 保存場所の設定  
（注意）以下の設定を行わない場合、波形表示がされない場合があるようです。
1. [DaVinci Resolve]-[環境設定]-[システム]で以下を設定
    * メディアストレージ：C:\Users\(UserName)\Desktop\(SomethigFolder) 等
1. [ファイル]-[プロジェクト設定]-[マスター設定]-[作業フォルダー]で以下を設定
    * キャッシュファイルの場所：上記のメディアストレージ直下の\CacheClip
    * ギャラリースチルの場所：上記のメディアストレージ直下の\.gallery
1. [プロジェクト設定]-[キャプチャー･再生]-[キャプチャー]で以下を設定
    * クリップの保存先：上記のメディアストレージ直下の\Capture  

### 自動バックアップ
1. [DaVinci Resolve]-[環境設定]-[ユーザー]で以下を設定
    * ライブ保存：✔
    * プロジェクトのバックアップ：✔

実行環境：Windows10, DaVinci Resolve 16      
作成者：夢寐郎  
作成日：2020年10月26日  
更新日：2020年10月27日



<a name="daVinciFirstStep"></a>
## ◆DaVinci Resolve入門

#### ビデオトランジション
 * [エフェクトライブラリ]-[ビデオトランジション]-[クロスティゾルブ]

#### オーディオトランジション
 * [エフェクトライブラリ]-[オーディオトランジション]-[クロスフェード XdB]

#### フェードイン･フェードアウト
 * タイムライン上でクリップを選択→赤い枠の右上（または左上）の白い部分をドラッグで「フェードイン」「フェードアウト」が可能

#### タイトル
1. [エフェクトライブラリ]-[ツールボックス]-[タイトル]-[テキスト]をタイムラインにドラッグ＆ドロップ
1. 画面右上の[インスペクタ]で設定

#### オーディオ波形表示
 * [タイムライン表示オプション]-[オーディオ波形]

#### スローモーション
 * 映像クリップを選択→右クリック→[クリップの速度を変更]-[速度]-[50%]

#### ズーム
1. 映像クリップを選択→変更したい位置に再生ヘッドを移動→[インスペクタ]-[変形]-[ズーム]-[◆]を選択（赤になる）→ズームの値を変更
1. 以降、同様にキーフレームを打ってプロパティを変更する

#### カラコレ
1. [カラー]を起動
1. [スコープ]を表示
1. カラコレしたい映像クリップを選択
1. ノードを選択→右クリック→[ノードを追加]→[シリアルノードを追加]  
    （設定のレイヤーのようなもの）
1. ノード01を選択し、次の設定で明るさを調整（「プライマリーホイール」を「Log」に変更／スコープを見ながら調整）  
    * シャドウ（初期値0.00）：暗部の明るさ
    * ミッドトーン（初期値0.00）：中間域の明るさ
    * ハイライト（初期値0.00）：明部の明るさ
    * オフセット（初期値25.00）：全体の明るさ
1. 他にも最下部にある次の設定を調整します
    * コン（初期値1.000）：コントラスト
    * 彩度（初期値50.00）：モノクロ化が可能
1. 4つのカラーバランスコントロールで色かぶりを調整します
    （ノード02を利用して設定を分けてもよい）
1. 次の方法でビフォーアフターの確認をします
    * [カラー]-[ノード]-[選択したノードを有効化/無効化]（Ctrl + D）
    * [カラー]-[ノード]-[すべてのノードを有効化/無効化]（Alt + D）

* 画面右上の[OpenFX]の設定をノードにドラッグ＆ドロップで設定することも可能  
    （有償版と無料版は扱える項目が異なります）

#### 書き出し
1. [デリバー]を起動
1. [YouTube]等を設定
1. [名称]と[保存先]を設定し[レンダーキューに追加]→[レンダーを開始]

実行環境：Windows10, DaVinci Resolve 16      
作成者：夢寐郎  
作成日：2020年10月26日  



<a name="daVinciCut"></a>
## ◆DaVinci カット入門

#### 映像素材を一気に確認
* ビューア左上の3つのボタンの真ん中「ソーステープ」を選択
* 上記の2つ左のボタン「メディアの並べ替えボタン」で順番の変更が可能
* ビューア左下の「ファストプレビュー」で、短いクリップは低速に、長いクリップは高速に再生（1～8倍速）

実行環境：Windows10, DaVinci Resolve 16      
作成者：XXXX  
作成日：2020年XX月XX日  



<a name="XXXXXX"></a>
## ◆XXXXXX

#### XXXXX

|AAAA|BBBB|CCCC|DDDD|EEEEE|
|:--:|:--:|:--|:--|:--:|
|XXXX|XXXX|XXXX XXXX|XXXX|XXXX|
|XXXX|XXXX|XXXX XXXX|XXXX|XXXX|
|XXXX|XXXX|XXXX XXXX|XXXX|XXXX|
|XXXX|XXXX|XXXX XXXX|XXXX|XXXX|
|XXXX|XXXX|XXXX XXXX|XXXX|XXXX|

実行環境：Windows10, DaVinci Resolve 16      
作成者：XXXX  
作成日：2020年XX月XX日  