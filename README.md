# 安否確認掲示板

## 使用する技術・ツール
- Nuxt.js
- AntDesign

## 実装する機能 
- 記事投稿
- 記事一覧表示
- 記事削除
- 記事編集

できる限り機能は最小限にとどめる。  
理由：安否確認が目的なので通信状況が悪いことが想定される。サーバーとのやりとりはできるだけ減らした方が良いのではないか。

### 機能の詳細
- 記事投稿
  - 氏名【必須】
  - フリガナ
  - E-mail【必須】
  - 電話番号
  - 住所
      
氏名とE-mailのみ必須にする。  
電話番号は必須としない。  
理由：災害等の影響で通信状況が安定せず、電話をしても繋がらないというケースが想定されるため。
必須が入力されていれば送信（ボタンをクリック）できるようにする。

- 記事一覧表示
  - 記事一覧を表示


- 記事削除
  - 記事を削除する


- 記事編集
  - 記事を編集する

## 必要な画面
記事一覧画面の中で、投稿・編集・削除をしたい。  
理由：通信状況が安定しないことが想定されるため、できるだけ通信のやりとりは減らしたいため。

## 必要な関数・クラス
クラスに関してはあまり分かっていません。すみません。。。

必要な関数

- バリデーション関連
  - validRequired()
    - 未入力チェック（氏名・E-mail）
  - validEmail()
    - E-mailの正規表現のチェック
  - validNumber()
    - 電話番号の正規表現チェック
  - validLength()
    - 文字の長さをチェック

- 機能関連
  - postArticle()
    - 記事投稿
  - editArticle()
    - 記事編集
  - deleteArticle()
    - 記事削除
  - listArticle()
    - 記事一覧表示

## 必要なコンポーネント
どう記述して良いのか分かりません。すみません。。。
