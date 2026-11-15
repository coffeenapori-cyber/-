# 毎朝の段取り

毎朝、今日やるべきToDoを Addness から読み、この作業場の日誌 `days/YYYY-MM-DD.md` に「## 今日の段取り」の節（ToDoごとに最初の一手まで）を書いて GitHub に push する自動化。

- いつ：毎朝 7:53（日本時間）。8時までに日誌に書き終わっている想定（混みやすい「ちょうどの時刻」を避けて数分前にしている）。
- どこで：Claude Code のクラウドの「スケジュールされたタスク」。この作業場を開いている会話「三上のAIの動き方をコピーする」（ https://claude.ai/code/session_01QpstLVWwVTAJfxySNCSqzy ）に毎朝メッセージが届き、その会話のAIが書く。Addness の道具とリポジトリの push 権限がある会話なので、ここで動かしている。
  - 新しい会話を毎回開く形は、2026-11-15 に1回試して失敗した（新しい会話には Addness の道具とこのリポジトリが付かず、ToDo を読めず push もできなかった）。
- 読む物：Addness の `list_todays_goals`（今日のToDo）と、各ゴールの `get_goal`（理想と本文。読むだけ）。
- 書く物：`days/YYYY-MM-DD.md` の「## 今日の段取り」だけ。push 先は作業ブランチ claude/addness-template-setup-88ur8w。ゴールの変更・完了・コメント・外への送信はしない。
- 止め方：Claude Code の「スケジュールされたタスク」の一覧で、この自動化を無効にするか削除する（AIに「毎朝の段取りの自動化を止めて」と頼んでもよい）。
- 中身を変える：時刻や細かさを変える時は、同じ一覧から設定を直す（AIに頼めば `update_trigger` で変える）。

Addness の対応ゴール：手順8「決まった時刻の自動化を1本作る」 https://www.addness.com/goals/3dde193b-0d47-4011-88f1-22633586d241
