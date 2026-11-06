<p><a href="../../../USER-GUIDE.md">English</a> · <a href="../zh-CN/USER-GUIDE.md">简体中文</a> · <a href="../zh-TW/USER-GUIDE.md">繁體中文</a> · <a href="../ja/USER-GUIDE.md">日本語</a> · <a href="../ko/USER-GUIDE.md">한국어</a> · <a href="../de/USER-GUIDE.md">Deutsch</a> · <a href="../fr/USER-GUIDE.md">Français</a> · <a href="../es/USER-GUIDE.md">Español</a> · <a href="../pt-BR/USER-GUIDE.md">Português (Brasil)</a> · <a href="../ru/USER-GUIDE.md">Русский</a></p>
<h1 id="smart-sync-user-guide">Smart Sync 使用者指南</h1>
<p>适用于 Smart Sync (<code>smart-sync-global</code>). <a href="https://smartsync.cc/zh-TW/">網站</a> · <a href="https://smartsync.cc/zh-TW/download/">下載</a> · <a href="https://smartsync.cc/zh-TW/privacy/">隱私</a>.</p>
<h2 id="install-or-update">安裝或更新</h2>
<p>使用Obsidian <strong>1.12.7 或更高版本</strong>.</p>
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
<p>對於更新，禁用插件，替換 <strong>只有這三個程式文件</strong>，然後重新載入並啟用它。儲存 <code>data.json</code>、秘密儲存、同步檢查點和所有註解。請勿將其他裝置的外掛程式設定或憑證複製到此筆記庫中。保留先前的程式檔案並獨立備份；降級程式檔案無法撤銷雲端刪除或其他已完成的雲端操作。在未解決其互動問題的情況下，請勿在同一筆記庫上執行多個同步提供者。</p>
<h2 id="sign-in-and-connect-your-first-vault">登入並連接您的第一個筆記庫</h2>
<ol>
<li>打開 <strong>設定 → Smart Sync → 登入</strong>。選擇 Google、GitHub 或電子郵件。社群登入使用系統瀏覽器；電子郵件驗證使用插件對話方塊中的短期程式碼。</li>
<li>授權後返回Obsidian。自動檢查在臨時網路故障或返回應用程式後恢復。如果仍在等待，請使用 <strong>檢查登入狀況</strong> 在待處理的對話框中。如果請求過期，請重新登入。切勿共用登入代碼。</li>
<li>建立雲端筆記庫或選擇現有筆記庫，然後按照加密密碼提示進行操作。確保密碼安全：帳號登入無法恢復密碼。僅符合的筆記庫名稱並不能識別同一個雲端筆記庫。</li>
<li>在同步現有文件之前，請檢查同步方向、附件下載、排除和設定範圍。</li>
<li>運行 <strong>立即同步筆記庫</strong>, 打開 <strong>同步任務和歷史記錄</strong>，然後等待完成。在連接其他裝置之前，請檢查代表性註釋、附件和原始修改時間。</li>
</ol>
<p>如果筆記庫建立回應遺失，請使用待處理作業的復原訊息並檢查現有的雲端筆記庫。不要重複建立具有不同名稱的新筆記庫。</p>
<h2 id="add-another-device">增加另一個設備</h2>
<p>安裝相同的區域插件，登入相同的帳戶並選擇相同的雲端筆記庫。使用其原始加密密碼。設備管理流程還提供了一個六位數的配對代碼：在新設備上取得它，並使用已連接的設備批准它 <strong>新增設備</strong>，並比對顯示的指紋後批准。包括前導零。過期或使用過的程式碼必須重新產生。</p>
<p>查看每個裝置的本機篩選器和附件策略。一台裝置上完成的雲端上傳並不代表其他所有裝置都已下載。</p>
<h2 id="synchronization-attachments-and-offline-recovery">同步、附件和離線恢復</h2>
<p>使用雙向同步進行普通編輯。僅上傳、僅接收、更新現有和暫停模式有意限制哪些變更會移動；切換模式前請閱讀方向提示。停止一輪會暫停自動同步，直到您選擇 <strong>立即同步</strong> 或 <strong>重試</strong>.</p>
<p>在完整和增量正文傳輸期間，Markdown 註釋優先於附件。目錄、重新命名和刪除依賴項仍然遵循其安全順序，並且主動傳輸可以在新排隊的註釋之前完成。嵌入的圖像或 PDF 可能會稍後到達。在同步偏好設定中選擇附件下載策略；使用 <strong>下載待處理的附件</strong> 當需要時。元資料檢查和網路狀況仍然影響總時間。</p>
<p>本機編輯在離線狀態下仍保留在本機。當網路恢復時，重新開啟 Obsidian，恢復同步（如果暫停），並檢查剩餘任務。在手機和平板電腦上，將 Obsidian 保持在前台，直到重要變更完成。鎖定螢幕或將應用程式置於背景可以將其暫停；桌面托盤設定不提供行動後台執行。</p>
<p>當元資料可用時，同步會攜帶來源檔案的原始修改時間。缺少它的舊雲端版本不能被視為保留了原始時間；從保留它的來源重新同步。產生新內容的合併有新的修改時間。</p>
<p>LAN 加速是可選的。檢查其連線狀態；如果不支援直接連線或沒有可用的對等點，雲端同步仍然是後備方案。同一網路發現並不能保證直接連結能夠正常運作。</p>
<h2 id="recover-earlier-versions-and-deleted-notes">還原早期版本和刪除的註釋</h2>
<p>開啟同步筆記並選擇 <strong>查看筆記歷史記錄並恢復</strong> 從其上下文選單中，或 <strong>顯示活動筆記歷史記錄</strong> 從命令面板。恢復之前檢查修訂和差異。使用 <strong>顯示已刪除的筆記</strong> 查看可恢復的已刪除內容。可用性取決於筆記庫的保留政策；過期或清除的歷史記錄無法恢復。</p>
<p>使用 <strong>保留、使用和清理</strong> 查看歷史策略和雲端使用情況。清理和清除作業會永久刪除符合條件的歷史記錄；先備份並閱讀確認資訊。歷史並不能取代獨立的備份。</p>
<h2 id="sync-selected-obsidian-settings">同步選定的 Obsidian 設定</h2>
<p>展開同步首選項和配置類別。編輯器首選項、外觀、熱鍵、書籤、社群插件程式碼、外掛程式資料、外掛程式啟用、主題和片段具有單獨的控制項。在啟用類別之前查看個別排除項。插件啟用變更可能需要重新啟動 Obsidian。行動裝置上將跳過僅限桌面的插件；在啟用第三方插件的程式碼或資料之前檢查第三方插件的兼容性。</p>
<p>過濾器預設應用此設備的排除項、附件閾值和配置範圍。應用一個會暫停同步；審查並明確恢復。預設不會複製帳戶金鑰或綁定其他雲端筆記庫。使用 <strong>匯出加密配置恢復</strong> 為了受保護的恢復並單獨儲存其密碼；切勿一起共用恢復檔案和密碼。</p>
<h2 id="sorting-pins-recent-files-and-search">排序、固定、最近文件和搜索</h2>
<p>啟用排序並設定根規則；更深層可以繼承父規則或使用自訂規則。使用註釋的上下文選單 <strong>插銷</strong>, <strong>取消固定</strong>, <strong>移至底部</strong> 或 <strong>從底部取出</strong>。引腳變更等待同步到達其他設備。</p>
<p>啟用最近的文件以使用左側邊欄中的時鐘標籤或 <strong>最近的文件</strong> 命令；禁用它會停止記錄開啟的檔案。啟用筆記搜尋以搜尋本地可用的筆記。未下載的附件不是本地可用的內容。</p>
<h2 id="password-protect-a-note-or-selected-text">用密碼保護註釋或選定的文本</h2>
<p>開啟 Markdown 筆記，如果需要，在編輯模式下選擇文本，然後執行 <strong>加密選取的文本</strong> 或 <strong>加密整個筆記</strong>。設定並確認單獨的密碼，閱讀警告並儲存。點擊加密內容即可解鎖；其行動包括 <strong>編輯</strong>, <strong>鎖</strong>, <strong>更改密碼</strong> 和 <strong>永久解密</strong>。透過安全性編輯視窗進行編輯，使保存保持加密狀態。</p>
<p>標題仍然可見。链接的图像和附件不会使用所选文本自动加密。早期的歷史記錄和備份可能會保留明文。永久解密將普通明文寫入本地並正常同步。密碼提示未加密。密碼不可恢復。</p>
<p>使用 <strong>注意加密設定</strong> 選擇不活動鎖定逾時，或 <strong>立即鎖定所有加密內容</strong>。關閉筆記、離開筆記庫或將應用程式移到背景也會鎖定它。如果儲存失敗，請按照 <strong>恢復加密草稿</strong> 使用原始密碼恢復單獨的加密筆記；不要刪除原始檔案來修復錯誤。</p>
<h2 id="desktop-tray-and-windows-startup">桌面托盤和 Windows 啟動</h2>
<p>在支援的桌面主機上， <strong>進階 → 使用托盤圖示在背景運行</strong> 預設情況下處於開啟狀態。關閉筆記庫視窗可使其繼續運行；點擊其托盤圖示將其恢復。它的選單只能關閉這個筆記庫。不受支援的托盤主機保持正常關閉。行動裝置隱藏此選項。</p>
<p><strong>登入時啟動至托盤</strong> 僅適用於 Windows，預設為關閉。啟用它會在目前使用者的啟動資料夾中建立此筆記庫的捷徑並啟用後台托盤。普通的發布保持可見。自訂 Obsidian 設定檔無法啟用啟動，因為主機可能會將請求路由到另一個實例。在停用托盤、卸載或還原到不支援啟動的版本之前先停用登入啟動。 macOS、Linux、Android、iPhone 和 iPad 不顯示 Windows 啟動開關。</p>
<h2 id="storage-plans-and-payments">儲存計劃和付款</h2>
<p>在設定中開啟儲存套餐入口，查看目前套餐。行動裝置會嘗試直接開啟系統瀏覽器；若跳轉失敗或無法確認，請使用提供的連結。付款前請核對金額、幣別、計費週期及續費條款。結帳以美元（USD）進行，使用分配給帳戶的付款管道：預設為 Stripe，符合條件的帳戶也可能使用 Dodo Payments。重新開啟未付款的購買流程會繼續原訂單。現有訂單及訂閱保留原付款管道；結果不確定時，請勿再次付款。返回 Obsidian 後確認套餐已更新；再次付款前，先查詢狀態不確定的訂單。</p>
<p>免費方案包括 50 MB、1 個雲端筆記庫和無限設備。付費容量和當前條款顯示在 <a href="https://smartsync.cc/zh-TW/pricing/">計劃頁面</a>。儲存容量由帳戶下的所有雲端筆記庫共用。</p>
<h2 id="sign-out-revoke-a-device-or-delete-an-account">登出、撤銷設備或刪除帳戶</h2>
<p>註銷會保留本地註釋。如果離線登出無法確認遠端撤銷，請在需要立即刪除時從另一個連接的裝置撤銷該裝置。卸載不會刪除雲端帳戶。</p>
<p>雲端刪除具有破壞性：請先驗證獨立的本機備份。透過筆記庫管理刪除雲端筆記庫並等待清理。打開 <strong>帳戶 → 危險區域 → 刪除帳戶</strong>，出現提示時驗證相同帳戶，然後鍵入 <strong>DELETE</strong> 正是如此。付費服務時間並不能阻止刪除。這將刪除帳戶存取權限和連線的身份；保留本機註釋。閱讀 <a href="https://smartsync.cc/zh-TW/privacy/">保留政策</a>.</p>
<h2 id="troubleshooting-and-device-limits">故障排除和設備限制</h2>
<p>閱讀錯誤顯示的恢復操作。在設備或筆記庫限制下，連接現有筆記庫、撤銷未使用的設備或選擇適當的計畫。如果支援需要，手動匯出診斷資訊； Global 用戶端不會上傳診斷遙測資料。將可見錯誤、插件/Obsidian 版本和平台發送至 <a href="mailto:admin@smartsync.cc">admin@smartsync.cc</a>。刪除密碼、令牌、驗證碼和私人筆記內容。</p>
<h2 id="interface-language">介面語言</h2>
<p>本版本支援英語、簡體中文、繁體中文、日語、韓語、德語、法語、西班牙語、巴西葡萄牙語及俄語。</p>
<p>在 Smart Sync 設定頂部附近的介面語言中選擇遵循 Obsidian 或明確語言。此選擇僅適用於該裝置上的本機筆記庫。儲存它，完成任何活動同步，然後重新載入外掛程式或重新啟動 Obsidian 以一起更新設定、命令和選單。</p>
<p>這僅更改顯示文字。服務區域、帳戶、雲端庫、加密密碼、文件內容、同步進度不變。不同的設備可能使用不同的語言。</p>
