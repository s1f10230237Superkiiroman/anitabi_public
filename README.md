# アニたび（Anitabi）
### アニメ聖地巡礼をもっと身近に。地域とアニメをつなぐWebアプリ

---

## 概要
**アニたび**は、アニメ作品の舞台となった「聖地」を地図上で可視化し、  
巡礼体験そのものをエンターテインメント化することを目的とした  
**アニメ聖地巡礼促進アプリ**です。

情報が分散しがちな聖地巡礼において、
- 正確で信頼できる情報提供  
- 地図・GPSを用いた直感的な巡礼体験  
- スタンプラリーや称号によるゲーミフィケーション  

を通じて、**ファン体験の向上**と**地域創生への貢献**を目指しました。

---

## チーム開発について
本プロジェクトは、**約1年間のチーム実習**として開発を行いました。  
企画立案・要件定義から設計、実装、テスト、発表までをチームで担当し、
最終的に**選抜チーム**に選ばれ、  
**全校生徒および教員の前で成果発表**を行いました。

<img width="860" height="410" alt="image" src="https://github.com/user-attachments/assets/d0ab6eff-f837-4fed-b028-fd9aaf8b252f" />


---

## 担当・貢献内容
**PM / Backend Engineer**

- プロジェクト全体の進捗管理・スケジュール調整  
- アーキテクチャ設計（Django構成・ディレクトリ設計）  
- 投稿機能・プロフィール管理機能の実装  
- インタラクション機能（いいね・返信）の実装
- ゲーミフィケーション: 称号機能、ビンゴ機能、お気に入り機能の実装
- Render(PaaS)・Cloudinary・PostgreSQLを用いた本番環境の構築とデプロイフロー確立
- AI応答機能の設計・実装  
- チーム内での仕様調整および技術的意思決定  

---

## 工夫した点・学び
- GitHubを用いた**チーム開発フロー（Issue / Pull Request）**の実践  
- 機能追加よりも**品質担保（QA）を優先**した開発判断  
- 著作権問題を考慮し、  
  アニメ画像を使用しない設計および許諾取得の検討  
- 学内ユーザーを対象としたユーザーテストを実施し、  
  フィードバックを基にした改善サイクルを経験  

--- 

## 背景・目的
聖地巡礼は人気が高い一方で、
- 情報が断片的で調べにくい  
- 非公式情報が多く信頼性に欠ける  
- 地域との継続的な接点が生まれにくい  

といった課題があります。

本プロジェクトでは  
**「聖地巡礼をもっと楽しく、もっと行きやすく」**をテーマに、  
アニメファンと地域をつなぐアプリの開発に取り組みました。

---

## 主な機能
- 🔍 **作品・地域・ジャンル別検索**
- <img width="1242" height="837" alt="スクリーンショット 2026-01-30 083422" src="https://github.com/user-attachments/assets/721f1a6b-e607-4b12-9cec-c8f6be8ef2f1" />

- 🗺 **聖地マップ表示（Leaflet + OpenStreetMap）**
- <img width="1873" height="839" alt="スクリーンショット 2026-01-30 083311" src="https://github.com/user-attachments/assets/0a6b7638-91f2-40d6-acf5-95eb898f4bc2" />

- 📍 **GPSを用いたルートガイド**
- <img width="1298" height="843" alt="スクリーンショット 2026-01-30 084005" src="https://github.com/user-attachments/assets/52ce8ae4-9ce7-4954-bac5-11d6bf2e9bf0" />

- 🏅 **スタンプラリー・称号機能**
- <img width="1462" height="860" alt="スクリーンショット 2026-01-30 084331" src="https://github.com/user-attachments/assets/047bb449-65e5-453c-8e34-98dfeb06564b" />

- 📝 **投稿機能（写真・コメント）**
- <img width="840" height="782" alt="スクリーンショット 2026-01-30 084617" src="https://github.com/user-attachments/assets/cada3ea1-026b-45db-9b5f-187083fad5a9" />

- ❤️ **お気に入り登録**
- 👤 **プロフィール管理**

---

## 技術スタック
### バックエンド
- Python / Django
- Django REST Framework
- PostgreSQL
- Firebase Auth / Django Auth

### フロントエンド
- HTML / CSS / JavaScript
- Leaflet.js
- OpenStreetMap
- HTML5 Geolocation API

### インフラ・その他
- Render（PaaS）
- Cloudinary（画像管理）
- GitHub

---

## 環境変数について
本プロジェクトでは就活用公開レポジトリということもあり、APIキーや認証情報などの機密情報を  
GitHub上に公開しないため、**環境変数による設定管理**を行っています。

ローカル環境で実行する場合は、`.env.example` を参考に  
`.env` ファイルを作成してください。

```bash
cp .env.example .env


## 動作方法（ローカル）
```bash
pip install -r requirements.txt
python manage.py migrate
