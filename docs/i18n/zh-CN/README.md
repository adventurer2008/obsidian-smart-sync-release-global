<p><a href="../../../README.md">English</a> · <a href="../zh-CN/README.md">简体中文</a> · <a href="../zh-TW/README.md">繁體中文</a> · <a href="../ja/README.md">日本語</a> · <a href="../ko/README.md">한국어</a> · <a href="../de/README.md">Deutsch</a> · <a href="../fr/README.md">Français</a> · <a href="../es/README.md">Español</a> · <a href="../pt-BR/README.md">Português (Brasil)</a> · <a href="../ru/README.md">Русский</a></p>
<h1 id="smart-sync">Smart Sync</h1>
<p>Obsidian 笔记、附件和选定设置的加密同步。保留原始文件修改时间、恢复保留版本并管理您的设备。</p>
<p>Global 应用程序服务器在美国阿什本的 Oracle Cloud 上运行。 加密对象数据使用 Cloudflare R2 进行私有存储。</p>
<p>我们重视数据安全和数据隐私。笔记、附件和文件路径在上传前，会先在您的设备上使用 AES-256-GCM 加密。加密和解密均在您的设备上完成，服务端存储加密内容；加密密码与账户登录凭据相互独立。</p>
<p><strong>当前版本：1.1.5</strong> ·Obsidian <strong>1.12.7+</strong> · 插件ID： <code>smart-sync-global</code>.</p>
<p><a href="https://smartsync.cc/zh-CN/">网站</a> · <a href="https://smartsync.cc/zh-CN/download/">下载/更新</a> · <a href="USER-GUIDE.md">操作手册</a> · <a href="https://smartsync.cc/zh-CN/pricing/">计划</a></p>
<h2 id="get-started">开始使用</h2>
<ol>
<li>备份您的笔记并首先尝试使用单独的笔记库。在Wujie Hub中，选择 <strong>Smart Sync → 稳定</strong>，或从下载三个插件文件 <a href="https://github.com/adventurer2008/obsidian-smart-sync-release-global/releases">发布</a>.</li>
<li>安装 <code>main.js</code>, <code>manifest.json</code> 和 <code>styles.css</code> 在你的笔记库里 <code>.obsidian/plugins/smart-sync-global/</code> 文件夹。在启用插件之前，重新加载 Obsidian 并查看其信任提示。更新仅替换这三个文件；保留设置、秘密存储、检查点和注释。</li>
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
<p>Smart Sync 1.1.5 支持十种界面语言，可在插件设置中选择。</p>
<h2 id="account-payments-and-privacy">账户、付款和隐私</h2>
<p>托管同步需要一个帐户。免费套餐目前包括 50 个 MB、1 个云笔记库和无限设备；付费计划增加了容量。支付币种为美元（USD），默认使用 Stripe，部分账号可分配 Dodo Payments。未付款时再次进入会继续原订单；已有订单和订阅保留原渠道，结果不确定时请勿重复付款。评论 <a href="https://smartsync.cc/zh-CN/pricing/">计划</a> 和 <a href="https://smartsync.cc/zh-CN/terms/">条款</a> ，然后再付款。</p>
<p>内容和路径在设备上加密。帐户身份、笔记库/设备标签、使用情况和操作元数据都在内容加密之外。全局客户端将诊断信息保留在本地以供手动导出，并且不会上传诊断遥测数据。加密和历史记录不会取代独立备份。阅读 <a href="https://smartsync.cc/zh-CN/privacy/">隐私政策</a>.</p>
<p>对于帐户删除，请先删除云笔记库并等待清理，然后使用 <strong>账户 → 危险区域 → 删除账户</strong>，验证相同的身份并输入请求的确认信息。本地注释仍然存在。</p>
<p>问题咨询： <a href="mailto:admin@smartsync.cc">admin@smartsync.cc</a>。包括您的平台和插件/Obsidian 版本；切勿发送密码、令牌、电子邮件代码或私人笔记。</p>
