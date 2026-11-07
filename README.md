# chifuyu777

社内の業務を効率化するアプリを、要件定義からテスト、公開まで1人で作っています。下のリンクからすぐに操作できます。

## デモへのログイン

| ID | パスワード | 見られる範囲 |
| --- | --- | --- |
| `guest` | `demo-r45S-wvNsvff` | すべてのアプリとスイート |

データはすべて架空です。どなたでも操作でき、毎朝9時に初期化します。個人情報や実在のデータは入力しないでください。

## 社員が使うアプリ

| アプリ | できること |
| --- | --- |
| [入退社の手続き](https://onboarding-flow.chifuyu777.workers.dev/) | 入社、退職、異動を依頼すると、人事、情シス、総務の作業が自動で届く。誰の作業で止まっているかを確認できる |
| [問い合わせ窓口](https://inquiry-triage.chifuyu777.workers.dev/) | 困りごとを入力すると、送信の前に似た解決方法を案内する。担当者は内容から自動で決まる |
| [勤怠](https://attendance-check.chifuyu777.workers.dev/) | 打刻、打刻の修正、有給の申請ができる。上長の承認で反映する |
| [シフト](https://shift-planner.chifuyu777.workers.dev/) | 自分のシフトの確認、休み希望の提出、交代のお願いができる |
| [ソフトの申請窓口](https://license-watch.chifuyu777.workers.dev/) | ソフトの利用申請、返却、新しいソフトの相談ができる。利用数の管理につながる |
| [備品の購入窓口](https://invoice-match.chifuyu777.workers.dev/) | 購入の依頼と請求書の提出ができる。提出した請求書は発注と自動で照合する |
| [報告の提出窓口](https://report-merge.chifuyu777.workers.dev/) | 拠点ごとに形式の違う報告を提出すると、その場で内容を確認する |

## 全体の仕組み

| 画面 | 役割 |
| --- | --- |
| [マイポータル](https://my-portal.chifuyu777.workers.dev/) | 一般社員が使う想定の入口です。ログインした人の権限があるアプリだけを表示します |
| [スイート](https://portfolio-portal.chifuyu777.workers.dev/) | 開発者と管理者の画面。全アプリの稼働状況、集計、管理画面をまとめて確認できる |

社員ごとの見え方を試すときは、同じパスワードで次の ID を使えます。

| ID | 立場 | マイポータルに並ぶアプリ |
| --- | --- | --- |
| `hanako` | 営業 | 勤怠、問い合わせ、ソフト、備品 |
| `aoki` | 人事 | 勤怠、問い合わせ、ソフト、入退社の手続き |
| `suzuki` | 店舗 | シフト、問い合わせ、報告の提出 |

## 使用技術

TypeScript、Hono、Cloudflare Workers、Cloudflare D1、Vitest
