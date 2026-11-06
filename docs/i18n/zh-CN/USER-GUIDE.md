<p><a href="../../../USER-GUIDE.md">English</a> · <a href="../zh-CN/USER-GUIDE.md">简体中文</a> · <a href="../zh-TW/USER-GUIDE.md">繁體中文</a> · <a href="../ja/USER-GUIDE.md">日本語</a> · <a href="../ko/USER-GUIDE.md">한국어</a> · <a href="../de/USER-GUIDE.md">Deutsch</a> · <a href="../fr/USER-GUIDE.md">Français</a> · <a href="../es/USER-GUIDE.md">Español</a> · <a href="../pt-BR/USER-GUIDE.md">Português (Brasil)</a> · <a href="../ru/USER-GUIDE.md">Русский</a></p>
<h1 id="smart-sync-user-guide">Smart Sync 用户指南</h1>
<p>适用于 Smart Sync 1.1.5 (<code>smart-sync-global</code>). <a href="https://smartsync.cc/zh-CN/">网站</a> · <a href="https://smartsync.cc/zh-CN/download/">下载</a> · <a href="https://smartsync.cc/zh-CN/privacy/">隐私</a>.</p>
<h2 id="install-or-update">安装或更新</h2>
<p>使用Obsidian <strong>1.12.7 或更高版本</strong>。备份您的笔记库并首先尝试单独的测试笔记库。在Wujie Hub中，选择 <strong>Smart Sync → 稳定</strong> 对于当前的稳定包。 Alpha 是一个独立的测试通道。</p>
<p>如需手动安装，请下载 <code>main.js</code>, <code>manifest.json</code> 和 <code>styles.css</code> 从匹配的 <a href="https://github.com/adventurer2008/obsidian-smart-sync-release-global/releases">GitHub 发布</a>。检查其 <code>SHA256SUMS.txt</code>。将三个文件放入 <code>&lt;vault&gt;/.obsidian/plugins/smart-sync-global/</code> （或者您的自定义配置文件夹的 <code>plugins/smart-sync-global/</code>）。重新加载 Obsidian，然后在亲自检查主机的信任提示后在社区插件中启用 Smart Sync。</p>
<p>对于更新，禁用插件，替换 <strong>只有这三个程序文件</strong>，然后重新加载并启用它。保存 <code>data.json</code>、秘密存储、同步检查点和所有注释。请勿将其他设备的插件设置或凭据复制到此笔记库中。保留以前的程序文件并独立备份；降级程序文件无法撤消云删除或其他已完成的云操作。在未解决其交互问题的情况下，请勿在同一笔记库上运行多个同步提供程序。</p>
<h2 id="sign-in-and-connect-your-first-vault">登录并连接您的第一个笔记库</h2>
<ol>
<li>打开 <strong>设置 → Smart Sync → 登录</strong>。选择 Google、GitHub 或电子邮件。社交登录使用系统浏览器；电子邮件验证使用插件对话框中的短期代码。</li>
<li>授权后返回Obsidian。自动检查在临时网络故障或返回应用程序后恢复。如果仍在等待，请使用 <strong>检查登录情况</strong> 在待处理的对话框中。如果请求过期，请重新登录。切勿共享登录代码。</li>
<li>创建云笔记库或选择现有笔记库，然后按照加密密码提示进行操作。确保密码安全：帐户登录无法恢复密码。仅匹配的笔记库名称并不能标识同一个云笔记库。</li>
<li>在同步现有文件之前，请检查同步方向、附件下载、排除和配置范围。</li>
<li>运行 <strong>立即同步笔记库</strong>, 打开 <strong>同步任务和历史记录</strong>，然后等待完成。连接其他设备之前，请检查代表性注释、附件和原始修改时间。</li>
</ol>
<p>如果笔记库创建回复丢失，请使用待处理操作的恢复消息并检查现有的云笔记库。不要重复创建具有不同名称的新笔记库。</p>
<h2 id="add-another-device">添加另一个设备</h2>
<p>安装相同的区域插件，登录相同的帐户并选择相同的云笔记库。使用其原始加密密码。设备管理流程还提供了一个六位数的配对代码：在新设备上获取它，使用已连接的设备批准它 <strong>添加设备</strong>，并比对显示的指纹后再批准。包括前导零。过期或使用过的代码必须重新生成。</p>
<p>查看每个设备的本地过滤器和附件策略。一台设备上完成的云上传并不意味着其他所有设备都已下载。</p>
<h2 id="synchronization-attachments-and-offline-recovery">同步、附件和离线恢复</h2>
<p>使用双向同步进行普通编辑。仅上传、仅接收、更新现有和暂停模式有意限制哪些更改会移动；切换模式前请阅读方向提示。停止一轮会暂停自动同步，直到您选择 <strong>立即同步</strong> 或 <strong>重试</strong>.</p>
<p>在完整和增量正文传输期间，Markdown 注释优先于附件。目录、重命名和删除依赖项仍然遵循其安全顺序，并且主动传输可以在新排队的注释之前完成。嵌入的图像或 PDF 可能会稍后到达。在同步偏好设置中选择附件下载策略；使用 <strong>下载待处理的附件</strong> 当需要时。元数据检查和网络状况仍然影响总时间。</p>
<p>本地编辑在离线状态下仍保留在本地。当网络恢复时，重新打开 Obsidian，恢复同步（如果暂停），并检查剩余任务。在手机和平​​板电脑上，将 Obsidian 保持在前台，直到重要更改完成。锁定屏幕或将应用程序置于后台可以将其暂停；桌面托盘设置不提供移动后台执行。</p>
<p>当元数据可用时，同步会携带源文件的原始修改时间。缺少它的旧云版本不能被视为保留了原始时间；从保留它的源重新同步。产生新内容的合并具有新的修改时间。</p>
<p>LAN 加速是可选的。检查其连接状态；如果不支持直接连接或没有可用的对等点，云同步仍然是后备方案。同一网络发现并不能保证直接链路能够正常工作。</p>
<h2 id="recover-earlier-versions-and-deleted-notes">恢复早期版本和删除的注释</h2>
<p>打开同步笔记并选择 <strong>查看笔记历史记录并恢复</strong> 从其上下文菜单中，或 <strong>显示活动笔记历史记录</strong> 从命令面板。恢复之前检查修订和差异。使用 <strong>显示已删除的笔记</strong> 查看可恢复的已删除内容。可用性取决于笔记库的保留政策；过期或清除的历史记录无法恢复。</p>
<p>使用 <strong>保留、使用和清理</strong> 查看历史策略和云使用情况。清理和清除操作会永久删除符合条件的历史记录；首先备份并阅读确认信息。历史并不能替代独立的备份。</p>
<h2 id="sync-selected-obsidian-settings">同步选定的 Obsidian 设置</h2>
<p>展开同步首选项和配置类别。编辑器首选项、外观、热键、书签、社区插件代码、插件数据、插件启用、主题和片段具有单独的控件。在启用类别之前查看个别排除项。插件启用更改可能需要重新启动 Obsidian。移动设备上将跳过仅限桌面的插件；在启用第三方插件的代码或数据之前检查第三方插件的兼容性。</p>
<p>过滤器预设应用此设备的排除项、附件阈值和配置范围。应用一个会暂停同步；审查并明确恢复。预设不会复制帐户密钥或绑定其他云笔记库。使用 <strong>导出加密配置恢复</strong> 为了受保护的恢复并单独存储其密码；切勿一起共享恢复文件和密码。</p>
<h2 id="sorting-pins-recent-files-and-search">排序、固定、最近文件和搜索</h2>
<p>启用排序并设置根规则；更深层次可以继承父规则或使用自定义规则。使用注释的上下文菜单 <strong>销</strong>, <strong>取消固定</strong>, <strong>移至底部</strong> 或 <strong>从底部取出</strong>。引脚更改等待同步到达其他设备。</p>
<p>启用最近的文件以使用左侧边栏中的时钟选项卡或 <strong>最近的文件</strong> 命令；禁用它会停止记录打开的文件。启用笔记搜索以搜索本地可用的笔记。未下载的附件不是本地可用的内容。</p>
<h2 id="password-protect-a-note-or-selected-text">用密码保护注释或选定的文本</h2>
<p>打开 Markdown 笔记，如果需要，在编辑模式下选择文本，然后运行 <strong>加密选定的文本</strong> 或 <strong>加密整个笔记</strong>。设置并确认单独的密码，阅读警告并保存。点击加密内容即可解锁；其行动包括 <strong>编辑</strong>, <strong>锁</strong>, <strong>更改密码</strong> 和 <strong>永久解密</strong>。通过安全编辑窗口进行编辑，使保存保持加密状态。</p>
<p>标题仍然可见。链接的图像和附件不会使用所选文本自动加密。早期的历史记录和备份可能会保留明文。永久解密将普通明文写入本地并正常同步。密码提示未加密。密码不可恢复。</p>
<p>使用 <strong>注意加密设置</strong> 选择不活动锁定超时，或 <strong>立即锁定所有加密内容</strong>。关闭笔记、离开笔记库或将应用程序移动到后台也会锁定它。如果保存失败，请按照 <strong>恢复加密草稿</strong> 使用原始密码恢复单独的加密笔记；不要删除原始文件来修复错误。</p>
<h2 id="desktop-tray-and-windows-startup">桌面托盘和 Windows 启动</h2>
<p>在支持的桌面主机上， <strong>高级 → 使用托盘图标在后台运行</strong> 默认情况下处于打开状态。关闭笔记库窗口可使其继续运行；单击其托盘图标将其恢复。它的菜单只能关闭这个笔记库。不受支持的托盘主机保持正常关闭。移动设备隐藏此选项。</p>
<p><strong>登录时启动至托盘</strong> 仅限 Windows，默认情况下处于关闭状态。启用它会在当前用户的启动文件夹中创建此笔记库的快捷方式并启用后台托盘。普通的发布保持可见。自定义 Obsidian 配置文件无法启用启动，因为主机可能会将请求路由到另一个实例。在禁用托盘、卸载或恢复到不支持启动的版本之前先禁用登录启动。 macOS、Linux、Android、iPhone 和 iPad 不显示 Windows 启动开关。</p>
<h2 id="storage-plans-and-payments">存储计划和付款</h2>
<p>打开设置中的存储计划条目以查看当前计划。手机尝试直接打开系统浏览器；如果切换失败或无法确认，请使用提供的链接。付款前查看金额、货币、间隔和续订条款。支付币种为美元（USD），默认使用 Stripe，部分账号可分配 Dodo Payments。未付款时再次进入会继续原订单；已有订单和订阅保留原渠道，结果不确定时请勿重复付款。返回应用程序并验证计划更新；在再次付款之前检查不确定的订单。</p>
<p>免费计划目前包括 50 个 MB、1 个云笔记库和无限设备。付费容量和当前条款显示在 <a href="https://smartsync.cc/zh-CN/pricing/">计划页面</a>。存储容量由账户下的所有云笔记库共享。</p>
<h2 id="sign-out-revoke-a-device-or-delete-an-account">注销、撤销设备或删除帐户</h2>
<p>注销会保留本地注释。如果离线注销无法确认远程撤销，请在需要立即删除时从另一个连接的设备撤销该设备。卸载不会删除云帐户。</p>
<p>云删除具有破坏性：请先验证独立的本地备份。通过笔记库管理删除云笔记库并等待清理。打开 <strong>账户 → 危险区域 → 删除账户</strong>，出现提示时验证同一帐户，然后键入 <strong>DELETE</strong> 正是如此。付费服务时间并不能阻止删除。这将删除帐户访问权限和连接的身份；保留本地注释。阅读 <a href="https://smartsync.cc/zh-CN/privacy/">保留政策</a>.</p>
<h2 id="troubleshooting-and-device-limits">故障排除和设备限制</h2>
<p>阅读错误显示的恢复操作。在设备或笔记库限制下，连接现有笔记库、撤销未使用的设备或选择合适的计划。如果支持需要，手动导出诊断信息； Global 客户端不上传诊断遥测数据。将可见错误、插件/Obsidian 版本和平台发送至 <a href="mailto:admin@smartsync.cc">admin@smartsync.cc</a>。删除密码、令牌、验证码和私人笔记内容。</p>
<p>Windows、macOS、桌面 Linux、Android、iPhone/iOS 和 iPad/iPadOS 共享受保护的同步 UI。桌面本机功能和移动生命周期限制有所不同，如上所述。早期用户报告的普通 Windows/iOS/Android 流保留其特定的接受范围；这并不是新鲜事，物理设备完全接受所有六个平台系列上的所有功能。重新启动、锁定、分割视图、浏览器返回和混合版本行为需要检查您使用的实际设备。在升级期间保留每台设备的设置和备份。</p>
<h2 id="interface-language">界面语言</h2>
<p>多语言候选客户端支持英语、简体中文、繁体中文、日语、韩语、德语、法语、西班牙语、巴西葡萄牙语和俄语。在该更新发布之前，现有的稳定版 1.1.5 二进制文件仍保留英文版本。</p>
<p>在 Smart Sync 设置顶部附近的界面语言中选择遵循 Obsidian 或显式语言。该选择仅适用于该设备上的本地笔记库。保存它，完成任何活动同步，然后重新加载插件或重新启动 Obsidian 以一起更新设置、命令和菜单。</p>
<p>这仅更改显示文本。服务区域、账户、云库、加密密码、文件内容、同步进度不变。不同的设备可能使用不同的语言。</p>
