<p><a href="../../../README.md">English</a> · <a href="../zh-CN/README.md">简体中文</a> · <a href="../zh-TW/README.md">繁體中文</a> · <a href="../ja/README.md">日本語</a> · <a href="../ko/README.md">한국어</a> · <a href="../de/README.md">Deutsch</a> · <a href="../fr/README.md">Français</a> · <a href="../es/README.md">Español</a> · <a href="../pt-BR/README.md">Português (Brasil)</a> · <a href="../ru/README.md">Русский</a></p>
<h1 id="smart-sync">Smart Sync</h1>
<p>Obsidian のコミュニティ同期プラグイン。 <strong>デバイス間のリアルタイム同期。より速い同期と、一般的な同期ツールを超える高度な機能。</strong><br>
パソコン、スマートフォン、タブレットで、ノート、添付ファイル、選択した設定を同期します。</p>
<p>グローバル・アプリケーション・サーバーは、米国のOracle Cloud上で実行されます。 暗号化されたオブジェクトデータは Cloudflare R2 で非公開に保存されます。</p>
<p>データの安全性とプライバシーを重視しています。 ノート、添付ファイル、ファイルパスは、アップロード前に端末上で AES-256-GCM により暗号化されます。 暗号化と復号は端末上で行われ、サービスには暗号化されたコンテンツが保存されます。暗号化パスワードはアカウントのログイン情報とは別です。</p>
<p>Obsidianを使用 <strong>1.12.7以降</strong>.</p>
<p><a href="https://smartsync.cc/ja/">ウェブサイト</a> · <a href="https://smartsync.cc/ja/download/">ダウンロード/アップデート</a> · <a href="USER-GUIDE.md">取扱説明書</a> · <a href="https://smartsync.cc/ja/pricing/">計画</a></p>
<h2 id="get-started">始めましょう</h2>
<h3 id="install-from-obsidian-community-plugins">Obsidian のコミュニティプラグインからインストール</h3>
<p>Smart Sync が Obsidian のコミュニティディレクトリに掲載された後は、Obsidian 内から直接インストールできます：</p>
<ol>
<li>Obsidian で「設定 → コミュニティプラグイン」を開きます。</li>
<li>無効になっている場合はコミュニティプラグインを有効にし、Obsidian の注意事項を確認します。</li>
<li>「閲覧」を選び、Smart Sync を検索して詳細を開きます（作者：lihy）。</li>
<li>「インストール」を選び、完了後に「有効化」を選びます。</li>
</ol>
<h3 id="wujie-hub-or-manual-download">Wujie Hub または手動ダウンロード</h3>
<p>Wujie Hub で次を選択します： <strong>Smart Sync → 安定</strong> から現在の安定版を入手してください。</p>
<p>手動インストールの場合は、ダウンロードしてください <code>main.js</code>, <code>manifest.json</code> そして <code>styles.css</code> マッチングから <a href="https://github.com/adventurer2008/obsidian-smart-sync-release-global/releases">GitHub リリース</a>。チェックしてください <code>SHA256SUMS.txt</code>。 3つのファイルを次の場所に置きます <code>&lt;vault&gt;/.obsidian/plugins/smart-sync-global/</code> (またはカスタム構成フォルダーの <code>plugins/smart-sync-global/</code>）。 Obsidian をリロードし、ホストの信頼プロンプトを自分で確認した後、コミュニティ プラグインで Smart Sync を有効にします。</p>
<h2 id="sign-in-and-connect-your-first-vault">サインインして最初のボールトに接続します</h2>
<ol>
<li>開く <strong>設定→Smart Sync→サインイン</strong>、Google、GitHub、または電子メールを選択し、クラウドボルトを作成または選択します。暗号化パスフレーズを安全に保管してください。アカウントにログインしても回復できません。</li>
<li>別のデバイスを追加する前に、同期設定を確認し、同期を実行して完了を確認します。フォローしてください <a href="USER-GUIDE.md">ステップバイステップのマニュアル</a> ペアリング、リカバリ、トラブルシューティングに使用します。</li>
</ol>
<h2 id="features">特長</h2>
<ul>
<li>Notes-first 同期、添付ファイルのダウンロード ポリシー、除外、タスクの進行状況、およびクラウド フォールバックによるオプションの LAN アクセラレーション。</li>
<li>保持制限内での履歴と削除されたメモの復元、デバイスのペアリング/取り消し、および暗号化された構成の復元。</li>
<li>選択された Obsidian 設定、互換性のあるプラグイン、テーマ、スニペットがデバイス間で同期されます。</li>
<li>フォルダーレベルの並べ替え、固定/下部のノート、最近のファイル、ローカルノートの検索。</li>
<li>パスワードで保護されたノート全体または選択したテキスト、安全な編集、暗号化された下書きの復元。タイトル、リンクされた添付ファイル、および以前の平文履歴には、個別のプライバシー境界があります。</li>
<li>サポートされているデスクトップ トレイとオプションの Windows はログイン時に起動します。モバイル システムはバックグラウンド作業を一時停止することができます。 Obsidian に戻り、アップロードが完了したことを確認します。</li>
</ul>
<h2 id="account-payments-and-privacy">アカウント、支払い、プライバシー</h2>
<p>ホスト型同期にはアカウントが必要です。無料プランには 50 MB、1 つのクラウド ボールト、無制限のデバイスが含まれています。有料プランでは容量が追加されます。支払い通貨は USD です。標準は Stripe ですが、一部のアカウントには Dodo Payments が割り当てられます。未払いの注文は再開でき、既存の注文とサブスクリプションは元の決済サービスを維持します。結果が不明な場合は再度支払わないでください。レビュー <a href="https://smartsync.cc/ja/pricing/">計画</a> そして <a href="https://smartsync.cc/ja/terms/">条件</a> を支払い前にご確認ください。</p>
<p>コンテンツとパスはデバイス上で暗号化されます。アカウント ID、ボールト/デバイス ラベル、使用状況および運用メタデータは、コンテンツ暗号化の対象外です。グローバル クライアントは、手動エクスポート用に診断をローカルに保持し、診断テレメトリをアップロードしません。暗号化と履歴は独立したバックアップに代わるものではありません。読んでください <a href="https://smartsync.cc/ja/privacy/">プライバシーポリシー</a>.</p>
<p>アカウントを削除するには、まずクラウドボルトを削除し、クリーンアップを待ってから、次を使用します。 <strong>アカウント → 危険ゾーン → アカウントの削除</strong>、同じ身元を確認し、要求された確認を入力します。ローカルメモが残っています。</p>
<p>お問い合わせ： <a href="mailto:admin@smartsync.cc">admin@smartsync.cc</a>。プラットフォームとプラグイン/Obsidian のバージョンを含めます。パスワード、トークン、電子メール コード、または個人的なメモを決して送信しないでください。</p>
