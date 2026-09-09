# grok-x-list

Watchlist の生投稿。Public。

- 6枠。各枠は1日1回（JST 0/4/8/12/16/20）
- 取得幅は直近24時間
- 生データのみ: url, id, user, text, created_at
- ホームタイムラインなし。投稿しない

名簿: [slots.md](slots.md)

## ファイルの更新

- `slots.md` … 名簿。人が変わったときだけ上書き
- `runs/YYYY-MM-DD-HHMM_JST_slotN.md` … 取得のたびに新しいファイルを追加。日付は増える。同じファイルは上書きしない
- 同じ枠の次の取得は24時間後
