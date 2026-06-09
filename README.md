**※ 現在このREADMEは作成中です！**

# 簡単QR読み取り打刻サービス「よみだこ」

「よみだこ」は、QRコードを読み取って打刻を行う派遣業界向け勤怠サービスです

## 本リポジトリの公開範囲について
本サービスは、将来的に**商用ソフトとしての販売・運用**を目指しています。そのため、知的財産保護及びセキュリティの観点から、コードの大部分はプライベートリポジトリにて管理しています。<br>
本リポジトリでは、私の設計思想や技術選定、ドキュメンテーション能力、及びコードの書き方をご確認いただくため、要件定義書や各種設計ドキュメント、および一部の主要なロジックのみを公開します。

## 開発資料一覧

DB設計以外の資料はマークダウン記法で作成しました。<br>
資料内の図はMermaid記法を使用しています。

- [プロトタイプ資料](docs/00_プロトタイプ/プロトタイプ資料.md)
- [企画書](docs/01_企画・要件定義/01_企画書.md)
- [要件定義](docs/01_企画・要件定義/02_要件定義書.md)
<!--
- [ユースケース]()
- [DB設計]()
- [技術選定書]()
-->

## 開発背景と解決する課題

現状の派遣現場には、以下の課題があります。
- 紙のタイムカード管理による転記の手間
- 他社製ソフトの導入障壁（複雑な料金形態、不要な機能）
「よみだこ」は、これらを解決するために開発されています。<br>
詳細は[企画書](docs/01_企画・要件定義/01_企画書.md)をご参照ください。

## 技術選定（予定含む）

### フロントエンド
![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=popout-square&logo=javascript&logoColor=F7DF1E)

### バックエンド
![Java](https://img.shields.io/badge/Java-007396?style=popout-square&logo=openjdk&logoColor=white)
![Spring boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=popout-square&logo=spring&logoColor=white)

### データベース
![SQLite](https://img.shields.io/badge/Sqlite-003B57?style=popout-square&logo=sqlite&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=popout-square&logo=postgresql&logoColor=white)

### インフラ・環境構築
![Proxmox](https://img.shields.io/badge/Proxmox-E57307?style=popout-square&logo=proxmox&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=popout-square&logo=ubuntu&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=popout-square&logo=docker&logoColor=white)

## 設計へのこだわり

### 1.要件定義・ドキュメントのGit管理
開発プロセスの効率化と内容更新管理のしやすさを重視し、関連資料をMarkdown形式で作成しています。また、業務フローや画面遷移図などの作成にはMermaid記法を採用し、図のコード管理を行っています。<br>

### 2.プルリクエスト（PR）を活用したセルフレビュー
個人開発であっても実務でのチーム開発を意識し、機能追加や更新の際はIssueを起票し、プルリクエストベースで開発を進めています。（過去のPRログに要件定義書をリファクタリングしたプロセスなどが残っています）