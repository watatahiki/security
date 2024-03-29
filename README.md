## 情報セキュリティとは？
情報セキュリティは以下の7つの要素が定義

### 基本の3要素
- 機密性（Confidentiality）
    - 情報に対するアクセス権限を徹底して保護・管理すること
    - 影響としては情報漏えいや情報の破損など
    - 対象は以下など
        - 社員の個人情報 / 顧客情報 / 製品の開発情報 / パスワード    
    - 対策は以下
        - 暗号化
        - パスワードを安易なものにしない
        - アクセス権を管理
- 完全性（Integrity）
    - 改ざんや過不足のない正確な情報が保持されている状態
    - 影響は信頼性が疑わしいデータは利用価値が失われる
    - 対策は以下
        - 情報にはデジタル署名をつける
        - 情報へのアクセス履歴を残す
        - 情報の変更履歴を残す
        - バックアップなどの情報を保管するルールを決める
- 可用性（Availability）
    - 情報をいつでも使える状態を保持すること
    - 影響はシステム停止など
    - 対策は以下
        - 定期的なバックアップ
        - BCP
        - 冗長化

### 4つの追加要素
- 真正性（Authenticity）
    - 情報にアクセスする企業組織や個人あるいは媒体が「アクセス許可された者」であることを確実にするもの
    - 対策は以下
        - デジタル署名
        - 二段階認証
        - 多要素認証（生体認証を含む）
- 信頼性（Reliability）
    - データやシステムを利用した動作が、意図した通りの結果を出すこと
    - 対策は以下
        - システムやソフトウェアが不具合を起こさない設計を行う
        - 不具合のない設計をもとに構築を行う
        - ヒューマンエラー（操作ミスなど）が起こっても、データが改ざんされたり消失したりしない仕組みを施す
- 責任追跡性（Accountability）
    - 企業組織や個人などの動きを追跡すること
        - データやシステムへの脅威が何であるのか、あるいは誰のどのような行為が原因なのかを追跡する
    - 対策は以下
        - アクセスログ
        - システムログ
        - デジタル署名
        - 操作履歴
        - ログイン履歴
- 否認防止（non-repudiation）
    - 情報が後に否定されないように証明しておくこと
    - 対策としては責任追跡性の施策にて実現でき、主にデジタル署名や各種ログが利用する

## OWASP
- オープンソース・ソフトウェアコミュニティ
- ソフトウェアやWebアプリケーションのセキュリティ分野の研究やガイドラインの作成、脆弱性診断ツールの開発、イベント開催など多岐にわたる活動をしている

## ASVS
- OWASP が策定した 286 項目の要求事項から成る Web アプリケーションに関する網羅的なセキュリティ要件のリスト
- WebアプリケーションおよびWebサービスを設計、開発、テストする際に必要となる

### OWASP ZAP
- OWASPが提供しているオープンソースのWebアプリケーション脆弱性診断ツール

## 第三者評価による脆弱性診断と OWASP ZAP などのツールの違いはこれか？
- ツール
    - ASVS のチェックが可能
- 第三者評価
    - ASVS のチェック + 他の各企業に特化した細かい診断ができる
        - プランなどにもよるが、、