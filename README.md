# Full Service Salon Reservation v1.0

1000円カット向け「Simple版」とは別アプリです。
個人・小規模のフルサービス美容室専用として分離しています。

## v1.0
- 複数メニュー選択
- 選択メニューの施術時間を自動合計
- スタイリストごとの対応メニューと施術時間
- スタイリストごとの曜日別出勤・退勤
- インターバル時間
- 退勤後の延長許容時間
- 日別勤務変更
- 休憩・私用などの予定ブロック
- 指名 / 誰でもOK
- スタイリスト別の空き時間自動計算
- 電話・店頭予約
- キャンセル
- 予約開始時刻の刻み
- 当日予約設定
- 予約締切
- 何日先まで予約可能か設定

## 重要
この版では1000円カット版のFirebaseを使いません。
新しいFirebaseプロジェクトを作り、4つのHTML
(login.html / admin.html / reserve.html / settings.html)
にある NEW_FIREBASE_... を、新しいWebアプリのFirebase設定へ置き換えてください。

Authentication: Email/Password を有効化
Realtime Database: database.rules.json を反映

管理者ユーザー作成後:
users/{管理者UID}/shopCode = "demo"

これで demo 店舗としてログインできます。


## Firebase接続
salon-reservation-74af5 専用Firebaseへ接続済みです。
