<p><a href="../../../README.md">English</a> · <a href="../zh-CN/README.md">简体中文</a> · <a href="../zh-TW/README.md">繁體中文</a> · <a href="../ja/README.md">日本語</a> · <a href="../ko/README.md">한국어</a> · <a href="../de/README.md">Deutsch</a> · <a href="../fr/README.md">Français</a> · <a href="../es/README.md">Español</a> · <a href="../pt-BR/README.md">Português (Brasil)</a> · <a href="../ru/README.md">Русский</a></p>
<h1 id="smart-sync">Smart Sync</h1>
<p>Obsidian 메모, 첨부 파일 및 선택한 설정에 대한 암호화된 동기화입니다. 원본 파일 수정 시간을 보존하고, 보존된 버전을 복구하고, 장치를 관리하세요.</p>
<p>글로벌 애플리케이션 서버는 미국 Ashburn의 Oracle Cloud에서 실행됩니다. 암호화된 객체 데이터는 Cloudflare R2에 비공개로 저장됩니다.</p>
<p><strong>현재 버전: 1.1.5</strong> · Obsidian <strong>1.12.7+</strong> · 플러그인 ID: <code>smart-sync-global</code>.</p>
<p><a href="https://smartsync.cc/ko/">웹사이트</a> · <a href="https://smartsync.cc/ko/download/">다운로드/업데이트</a> · <a href="USER-GUIDE.md">사용 설명서</a> · <a href="https://smartsync.cc/ko/pricing/">계획</a></p>
<h2 id="get-started">시작하기</h2>
<ol>
<li>메모를 백업하고 먼저 별도의 볼트를 사용해 보세요. Wujie Hub에서 다음을 선택합니다. <strong>Smart Sync → 안정</strong>, 또는 다음에서 세 가지 플러그인 파일을 다운로드하세요. <a href="https://github.com/adventurer2008/obsidian-smart-sync-release-global/releases">릴리스</a>.</li>
<li>설치 <code>main.js</code>, <code>manifest.json</code> 그리고 <code>styles.css</code> 네 금고에 <code>.obsidian/plugins/smart-sync-global/</code> 폴더. 플러그인을 활성화하기 전에 Obsidian를 다시 로드하고 신뢰 프롬프트를 검토하세요. 업데이트는 이 세 가지 파일만 대체합니다. 설정, 비밀 저장소, 체크포인트 및 메모를 보존합니다.</li>
<li>열기 <strong>설정 → Smart Sync → 로그인</strong>, Google, GitHub 또는 이메일을 선택한 다음 클라우드 볼트를 생성하거나 선택하세요. 암호화 암호를 안전하게 유지하세요. 계정 로그인으로 복구할 수 없습니다.</li>
<li>다른 장치를 추가하기 전에 동기화 기본 설정을 검토하고 동기화를 실행하고 완료를 확인하세요. 따라가다 <a href="USER-GUIDE.md">단계별 매뉴얼</a> 페어링, 복구 및 문제 해결을 위해.</li>
</ol>
<h2 id="features">특징</h2>
<ul>
<li>Notes 우선 동기화, 첨부 파일 다운로드 정책, 제외, 작업 진행 및 클라우드 폴백을 통한 선택적 LAN 가속.</li>
<li>보존 한도 내 기록 및 삭제된 메모 복구, 장치 페어링/해지 및 암호화된 구성 복구.</li>
<li>선택된 Obsidian 설정, 호환 플러그인, 테마 및 스니펫이 여러 장치에서 동기화됩니다.</li>
<li>폴더 수준 정렬, 고정/하단 노트, 최근 파일 및 로컬 노트 검색.</li>
<li>비밀번호로 보호된 전체 메모 또는 선택한 텍스트, 안전한 편집 및 암호화된 초안 복구. 제목, 연결된 첨부 파일 및 이전 일반 텍스트 기록에는 별도의 개인 정보 보호 범위가 있습니다.</li>
<li>로그인 시 지원되고 선택적인 Windows가 실행되는 데스크탑 트레이. 모바일 시스템은 백그라운드 작업을 일시 중단할 수 있습니다. Obsidian로 돌아가서 업로드가 완료되었는지 확인하세요.</li>
</ul>
<p>Smart Sync 1.1.5은 10개 인터페이스 언어를 지원합니다. 플러그인 설정에서 언어를 선택할 수 있습니다.</p>
<h2 id="account-payments-and-privacy">계정, 결제 및 개인정보 보호</h2>
<p>호스팅된 동기화에는 계정이 필요합니다. 무료 플랜에는 현재 50개의 MB, 1개의 클라우드 볼트 및 무제한 장치가 포함되어 있습니다. 유료 요금제는 용량을 추가합니다.결제 통화는 USD이며 기본 서비스는 Stripe입니다. 일부 계정에는 Dodo Payments가 할당됩니다. 미결제 주문은 다시 열어 계속할 수 있고 기존 주문과 구독은 원래 결제 서비스를 유지합니다. 결과가 불확실하면 다시 결제하지 마세요. 검토 <a href="https://smartsync.cc/ko/pricing/">계획</a> 그리고 <a href="https://smartsync.cc/ko/terms/">용어</a> 을 결제 전에 확인하세요.</p>
<p>콘텐츠와 경로는 장치에서 암호화됩니다. 계정 ID, 저장소/장치 레이블, 사용량 및 운영 메타데이터는 콘텐츠 암호화 외부에 있습니다. 글로벌 클라이언트는 수동 내보내기를 위해 진단을 로컬로 유지하고 진단 원격 측정을 업로드하지 않습니다. 암호화 및 기록은 독립 백업을 대체하지 않습니다. 읽기 <a href="https://smartsync.cc/ko/privacy/">개인 정보 보호 정책</a>.</p>
<p>계정 삭제를 위해서는 먼저 클라우드 볼트를 삭제하고 정리를 기다린 후 사용하세요. <strong>계정 → 위험지대 → 계정 삭제</strong>, 동일한 신원을 확인하고 요청된 확인을 입력하십시오. 로컬 메모가 남아 있습니다.</p>
<p>문의: <a href="mailto:admin@smartsync.cc">admin@smartsync.cc</a>. 플랫폼과 플러그인/Obsidian 버전을 포함하세요. 비밀번호, 토큰, 이메일 코드 또는 개인 메모를 절대 보내지 마십시오.</p>
