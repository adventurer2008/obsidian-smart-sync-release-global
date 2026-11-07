<p><a href="../../../README.md">English</a> · <a href="../zh-CN/README.md">简体中文</a> · <a href="../zh-TW/README.md">繁體中文</a> · <a href="../ja/README.md">日本語</a> · <a href="../ko/README.md">한국어</a> · <a href="../de/README.md">Deutsch</a> · <a href="../fr/README.md">Français</a> · <a href="../es/README.md">Español</a> · <a href="../pt-BR/README.md">Português (Brasil)</a> · <a href="../ru/README.md">Русский</a></p>
<h1 id="smart-sync">Smart Sync</h1>
<p>Obsidian社区同步插件， <strong>多设备实时同步，同步速度更快，功能更强，超越Obsidian官方同步功能。</strong><br>
电脑、手机、平板，笔记、附件与所选设置保持同步。</p>
<p>Global 应用程序服务器在美国阿什本的 Oracle Cloud 上运行。 加密对象数据使用 Cloudflare R2 进行私有存储。</p>
<p>我们重视数据安全和数据隐私。笔记、附件和文件路径在上传前，会先在您的设备上使用 AES-256-GCM 加密。加密和解密均在您的设备上完成，服务端存储加密内容；加密密码与账户登录凭据相互独立。</p>
<p>使用Obsidian <strong>1.12.7 或更高版本</strong>.</p>
<p><a href="https://smartsync.cc/zh-CN/">网站</a> · <a href="https://smartsync.cc/zh-CN/download/">下载/更新</a> · <a href="USER-GUIDE.md">操作手册</a> · <a href="https://smartsync.cc/zh-CN/pricing/">计划</a></p>
<h2 id="get-started">开始使用</h2>
<h3 id="install-from-obsidian-community-plugins">通过 Obsidian 社区插件安装</h3>
<p>Smart Sync 在 Obsidian 社区插件目录上架后，即可直接在 Obsidian 中安装：</p>
<ol>
<li>在 Obsidian 中打开“设置 → 第三方插件”。</li>
<li>如果尚未启用第三方插件，点击“启用第三方插件”，并阅读 Obsidian 显示的提示。</li>
<li>点击“浏览”，搜索 Smart Sync，打开插件详情（作者：lihy）。</li>
<li>点击“安装”，安装完成后点击“启用”。</li>
</ol>
<h3 id="wujie-hub-or-manual-download">通过 Wujie Hub 或手动下载</h3>
<p>在 Wujie Hub 中选择 <strong>Smart Sync → 稳定</strong> 获取当前稳定版。</p>
<p>如需手动安装，请下载 <code>main.js</code>, <code>manifest.json</code> 和 <code>styles.css</code> 从匹配的 <a href="https://github.com/adventurer2008/obsidian-smart-sync-release-global/releases">GitHub 发布</a>。检查其 <code>SHA256SUMS.txt</code>。将三个文件放入 <code>&lt;vault&gt;/.obsidian/plugins/smart-sync-global/</code> （或者您的自定义配置文件夹的 <code>plugins/smart-sync-global/</code>）。重新加载 Obsidian，然后在亲自检查主机的信任提示后在社区插件中启用 Smart Sync。</p>
<h2 id="sign-in-and-connect-your-first-vault">登录并连接您的第一个笔记库</h2>
<ol>
<li>打开 <strong>设置 → Smart Sync → 登录</strong>，选择 Google、GitHub 或电子邮件，然后创建或选择云笔记库。确保其加密密码安全；帐户登录无法恢复。</li>
<li>在添加其他设备之前查看同步首选项、运行同步并确认完成。遵循 <a href="USER-GUIDE.md">分步手册</a> 用于配对、恢复和故障排除。</li>
</ol>
<h2 id="features">特点</h2>
<ul>
<li>笔记优先同步、附件下载策略、排除、任务进度以及带有云回退功能的可选 LAN 加速。</li>
<li>保留限制内的历史记录和已删除笔记恢复、设备配对/撤销以及加密配置恢复。</li>
<li>选定的 Obsidian 设置、兼容插件、主题和片段在设备之间同步。</li>
<li>文件夹级排序、固定/底部注释、最近的文件和本地注释搜索。</li>
<li>密码保护整个笔记或选定的文本，安全编辑和加密草稿恢复。标题、链接的附件和早期的纯文本历史记录具有单独的隐私边界。</li>
<li>支持的桌面托盘和可选的 Windows 在登录时启动。移动系统可以暂停后台工作；返回 Obsidian 并确认上传完成。</li>
</ul>
<h2 id="account-payments-and-privacy">账户、付款和隐私</h2>
<p>托管同步需要一个帐户。免费套餐包括 50 MB、1 个云笔记库和无限设备；付费计划增加了容量。支付币种为美元（USD），默认使用 Stripe，部分账号可分配 Dodo Payments。未付款时再次进入会继续原订单；已有订单和订阅保留原渠道，结果不确定时请勿重复付款。购买前请查看 <a href="https://smartsync.cc/zh-CN/pricing/">计划</a> 和 <a href="https://smartsync.cc/zh-CN/terms/">条款</a> ，然后再付款。</p>
<p>内容和路径在设备上加密。帐户身份、笔记库/设备标签、使用情况和操作元数据都在内容加密之外。全局客户端将诊断信息保留在本地以供手动导出，并且不会上传诊断遥测数据。加密和历史记录不会取代独立备份。阅读 <a href="https://smartsync.cc/zh-CN/privacy/">隐私政策</a>.</p>
<p>对于帐户删除，请先删除云笔记库并等待清理，然后使用 <strong>账户 → 危险区域 → 删除账户</strong>，验证相同的身份并输入请求的确认信息。本地注释仍然存在。</p>
<p>问题咨询： <a href="mailto:admin@smartsync.cc">admin@smartsync.cc</a>。包括您的平台和插件/Obsidian 版本；切勿发送密码、令牌、电子邮件代码或私人笔记。</p>
