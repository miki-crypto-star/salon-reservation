# フルサービス美容室予約システム v4

1000円カット版とは別アプリです。

## GitHubへアップするファイル
index.html / login.html / settings.html / admin.html / reserve.html

## Firebaseで使うファイル
- initial-data.json : Realtime Database「データ」→ JSONをインポート
- database.rules.json : Realtime Database「ルール」へ内容を貼り付けて公開

## データ構造
users/{uid}/shopCode
shops/{shopCode}/settings
shops/{shopCode}/menus
shops/{shopCode}/staff
shops/{shopCode}/workOverrides/{date}/{staffId}
shops/{shopCode}/blocks/{date}/{staffId}/{blockId}
shops/{shopCode}/locks/{date}/{staffId}/{5分単位}
shops/{shopCode}/reservations/{date}/{reservationId}

## 実装機能
- 店舗定休日
- お客様予約URL・QR
- メニュー追加・編集・削除（料金なし）
- スタイリスト追加・編集・削除
- スタイリスト別の対応メニューと施術時間
- 曜日別勤務時間
- 日別勤務変更（休み/遅出/早退）
- インターバル
- 退勤後の延長許容時間
- 複数メニュー合計時間で空き枠計算
- 指名 / 誰でもOK
- スタイリスト別空き時間表示
- 休憩・私用ブロック
- 電話/LINE/店頭予約
- 予約変更・キャンセル
- 同時予約ロック
- 当日予約・予約締切・予約可能日数
- 予約完了画面、スクリーンショット案内
- iPhone/Googleカレンダー追加
