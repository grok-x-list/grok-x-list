# grok-x-list

Watchlist の生投稿。Public。

- 6枠。各枠は1日1回（JST 0/4/8/12/16/20）
- 取得幅は直近24時間
- 生データのみ: url, id, user, text, created_at
- 見出しは「名前 @handle」
- ホームタイムラインなし。投稿しない

名簿: [slots.md](slots.md)

## ファイルの更新（併用）

- `slots.md` … 名簿。人が変わったときだけ上書き
- `runs/slot1.md` … `runs/slot6.md` … 各枠の最新。取得のたびに上書き。GPTはここを見る
- `runs/YYYY-MM-DD-HHMM_JST_slotN.md` … 履歴。取得のたびに新しいファイルを追加。上書きしない
- 同じ枠の次の取得は24時間後
- ファイル名の slotN はそのまま
