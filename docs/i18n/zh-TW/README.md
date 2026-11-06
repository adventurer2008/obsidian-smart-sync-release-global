<p><a href="../../../README.md">English</a> · <a href="../zh-CN/README.md">简体中文</a> · <a href="../zh-TW/README.md">繁體中文</a> · <a href="../ja/README.md">日本語</a> · <a href="../ko/README.md">한국어</a> · <a href="../de/README.md">Deutsch</a> · <a href="../fr/README.md">Français</a> · <a href="../es/README.md">Español</a> · <a href="../pt-BR/README.md">Português (Brasil)</a> · <a href="../ru/README.md">Русский</a></p>
<h1 id="smart-sync">Smart Sync</h1>
<p>Obsidian社群同步外掛， <strong>多裝置即時同步，同步速度更快，功能更強，超越Obsidian官方同步功能。</strong><br>
電腦、手機、平板，筆記、附件與所選設定保持同步。</p>
<p>Global 應用程式伺服器在美國阿什本的 Oracle Cloud 上運作。 加密物件資料使用 Cloudflare R2 進行私有儲存。</p>
<p>我們重視資料安全與隱私。筆記、附件及檔案路徑在上傳前，會先在您的裝置上使用 AES-256-GCM 加密。加密及解密均在您的裝置上完成，服務端儲存加密內容；加密密碼與帳戶登入憑證相互獨立。</p>
<p>使用Obsidian <strong>1.12.7 或更高版本</strong>.</p>
<p><a href="https://smartsync.cc/zh-TW/">網站</a> · <a href="https://smartsync.cc/zh-TW/download/">下載/更新</a> · <a href="USER-GUIDE.md">操作手冊</a> · <a href="https://smartsync.cc/zh-TW/pricing/">計劃</a></p>
<h2 id="get-started">開始使用</h2>
<h3 id="install-from-obsidian-community-plugins">透過 Obsidian 社群外掛程式安裝</h3>
<p>Smart Sync 在 Obsidian 社群外掛程式目錄上架後，即可直接在 Obsidian 中安裝：</p>
<ol>
<li>在 Obsidian 中開啟「設定 → 第三方外掛程式」。</li>
<li>若尚未啟用第三方外掛程式，請選擇「啟用第三方外掛程式」，並閱讀 Obsidian 顯示的提示。</li>
<li>選擇「瀏覽」，搜尋 Smart Sync，開啟外掛程式詳情（作者：lihy）。</li>
<li>選擇「安裝」，完成後選擇「啟用」。</li>
</ol>
<h3 id="wujie-hub-or-manual-download">透過 Wujie Hub 或手動下載</h3>
<p>在 Wujie Hub 中選擇 <strong>Smart Sync → 穩定</strong> 取得目前的穩定版。</p>
<p>如需手動安裝，請下載 <code>main.js</code>, <code>manifest.json</code> 和 <code>styles.css</code> 從配對的 <a href="https://github.com/adventurer2008/obsidian-smart-sync-release-global/releases">GitHub 發布</a>。檢查其 <code>SHA256SUMS.txt</code>。將三個文件放入 <code>&lt;vault&gt;/.obsidian/plugins/smart-sync-global/</code> （或您的自訂設定資料夾的 <code>plugins/smart-sync-global/</code>）。重新載入 Obsidian，然後在親自檢查主機的信任提示後在社群外掛程式中啟用 Smart Sync。</p>
<h2 id="sign-in-and-connect-your-first-vault">登入並連接您的第一個筆記庫</h2>
<ol>
<li>打開 <strong>設定 → Smart Sync → 登入</strong>，選擇 Google、GitHub 或電子郵件，然後建立或選擇雲端筆記庫。確保其加密密碼安全；帳戶登入無法恢復。</li>
<li>在新增其他裝置之前查看同步首選項、運行同步並確認完成。遵循 <a href="USER-GUIDE.md">逐步手冊</a> 用於配對、復原和故障排除。</li>
</ol>
<h2 id="features">特點</h2>
<ul>
<li>筆記優先同步、附件下載策略、排除、任務進度以及具有雲端回退功能的選用 LAN 加速。</li>
<li>保留限制內的歷史記錄和已刪除筆記恢復、裝置配對/撤銷以及加密配置恢復。</li>
<li>選定的 Obsidian 設定、相容外掛程式、主題和片段在裝置之間同步。</li>
<li>資料夾級排序、固定/底部註釋、最近的文件和本地註釋搜尋。</li>
<li>密碼保護整個筆記或選定的文本，安全編輯和加密草稿恢復。標題、連結的附件和早期的純文字歷史記錄具有單獨的隱私邊界。</li>
<li>支援的桌面托盤和可選的 Windows 在登入時啟動。行動系統可以暫停後台工作；返回 Obsidian 並確認上傳完成。</li>
</ul>
<h2 id="account-payments-and-privacy">帳戶、付款和隱私</h2>
<p>託管同步需要一個帳戶。免費方案包括 50 MB、1 個雲端筆記庫和無限設備；付費方案增加了容量。付款幣別為美元（USD），預設使用 Stripe，部分帳號可分配 Dodo Payments。未付款時再次進入會繼續原訂單；既有訂單和訂閱保留原管道，結果不確定時請勿重複付款。購買前請查看 <a href="https://smartsync.cc/zh-TW/pricing/">計劃</a> 和 <a href="https://smartsync.cc/zh-TW/terms/">條款</a> ，然後再付款。</p>
<p>內容和路徑在裝置上加密。帳戶身分、筆記庫/裝置標籤、使用情況和操作元資料都在內容加密之外。全域用戶端將診斷資訊保留在本機以供手動匯出，並且不會上傳診斷遙測資料。加密和歷史記錄不會取代獨立備份。閱讀 <a href="https://smartsync.cc/zh-TW/privacy/">隱私權政策</a>.</p>
<p>對於帳戶刪除，請先刪除雲端筆記庫並等待清理，然後使用 <strong>帳戶 → 危險區域 → 刪除帳戶</strong>，驗證相同的身份並輸入請求的確認資訊。本地註釋仍然存在。</p>
<p>問題諮詢： <a href="mailto:admin@smartsync.cc">admin@smartsync.cc</a>。包括您的平台和外掛程式/Obsidian 版本；切勿發送密碼、令牌、電子郵件代碼或私人筆記。</p>