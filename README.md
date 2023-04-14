# FFLogs-Toxic-Overlay

とてもトキシックなACT用オーバーレイです

## マニュアル

### 事前準備

1. [FFLogsクライアント管理ページ](https://ja.fflogs.com/api/clients/)で新しいクライアントを作成。
    - アプリケーションの名前: `fflogs-toxic-overlay(適当で大丈夫)`
    - Enter one or more redirect URLs: `http://127.0.0.1`
2. `client ID`と`client secret`はあとで使うので一旦コピーし、保存してください。
    - `client secret`はあとで確認することができないので、紛失した場合は再発行となります。

### IINACT導入
IINACTに導入したい場合、Browsingwayが必要になります。

 - [IINACT](https://www.iinact.com/) ([Github](https://github.com/marzent/IINACT))
 - Browsingway ([Github](https://github.com/Styr1x/Browsingway)) 

1. URLはこちら：
    ```
    https://server03.akimiyabi.net/fflogs-toxic-overlay/?OVERLAY_WS=ws://127.0.0.1:10501/ws
    ```
2. `client ID` `client secret`を以下の形でURLの後ろに追加：
    ```
    &username=client ID&password=client secret
    ```
    最終的にURLをこのようにしたら大丈夫です：
    ```
    https://server03.akimiyabi.net/fflogs-toxic-overlay/?OVERLAY_WS=ws://127.0.0.1:10501/ws&username=client ID&password=client secret
    ```

3. Browsingwayに新しいオーバーレイを追加。URLを貼ったら一回`Reload`。

### ACT導入
ACTに導入したい場合、Overlay.dllが必要になります。

[OverlayPlugin](https://github.com/OverlayPlugin/OverlayPlugin/releases) (0.19.18+)

1. URLはこちら：
    ```
    https://server03.akimiyabi.net/fflogs-toxic-overlay/
    ```
2. `client ID` `client secret`を以下の形でURLの後ろに追加：
    ```
    ?username=client ID&password=client secret
    ```
    最終的にURLをこのようにしたら大丈夫です：
    ```
    https://server03.akimiyabi.net/fflogs-toxic-overlay/?username=client ID&password=client secret
    ```

3. `Reload overlay`

### 使い方
ゲーム内でキャラクターを4~5秒フォーカスしたら、オーバーレイで相手のデータを表示させることができます。

## ご注意
FFLogs APIに問い合わせるために、`client id`および`client secret`をサーバーに送ることになります。URLに`username` `password`を付けない状態でも、このオーバーレイを利用できますが、一定時間内に問い合わせる回数の制限がございます。

## Change log

## 連絡先

[Twitter@kagami_transl](https://twitter.com/kagami_transl)

Discord: `Kagami Akimiyabi#0127`