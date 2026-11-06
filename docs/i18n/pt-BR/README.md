<p><a href="../../../README.md">English</a> · <a href="../zh-CN/README.md">简体中文</a> · <a href="../zh-TW/README.md">繁體中文</a> · <a href="../ja/README.md">日本語</a> · <a href="../ko/README.md">한국어</a> · <a href="../de/README.md">Deutsch</a> · <a href="../fr/README.md">Français</a> · <a href="../es/README.md">Español</a> · <a href="../pt-BR/README.md">Português (Brasil)</a> · <a href="../ru/README.md">Русский</a></p>
<h1 id="smart-sync">Smart Sync</h1>
<p>Sincronização criptografada para suas notas, anexos e configurações selecionadas do Obsidian. Preserve os tempos de modificação dos arquivos originais, recupere versões retidas e gerencie seus dispositivos.</p>
<p>O servidor de aplicativos Global é executado no Oracle Cloud em Ashburn, Estados Unidos. Os dados de objetos criptografados são armazenados de forma privada no Cloudflare R2.</p>
<p>Valorizamos a segurança e a privacidade dos dados. Notas, anexos e caminhos de arquivos são criptografados no seu dispositivo com AES-256-GCM antes do envio. A criptografia e a descriptografia ocorrem nos seus dispositivos; o serviço armazena conteúdo criptografado e a senha de criptografia é separada das credenciais de acesso à conta.</p>
<p>Usar Obsidian <strong>1.12.7 ou mais recente</strong>.</p>
<p><a href="https://smartsync.cc/pt-BR/">Site</a> · <a href="https://smartsync.cc/pt-BR/download/">Baixar / atualizar</a> · <a href="USER-GUIDE.md">Manual de operação</a> · <a href="https://smartsync.cc/pt-BR/pricing/">Planos</a></p>
<h2 id="get-started">Comece</h2>
<h3 id="install-from-obsidian-community-plugins">Instalar pelos plugins da comunidade do Obsidian</h3>
<p>Quando o Smart Sync estiver listado no diretório da comunidade do Obsidian, você poderá instalá-lo diretamente no Obsidian:</p>
<ol>
<li>No Obsidian, abra Configurações → Plugins da comunidade.</li>
<li>Se estiverem desativados, ative os plugins da comunidade e leia o aviso exibido pelo Obsidian.</li>
<li>Selecione Explorar, pesquise Smart Sync e abra a página do plugin (autor: lihy).</li>
<li>Selecione Instalar e, em seguida, Ativar.</li>
</ol>
<h3 id="wujie-hub-or-manual-download">Wujie Hub ou download manual</h3>
<p>No Wujie Hub, selecione <strong>Smart Sync → Estável</strong> para obter a versão estável atual.</p>
<p>Para instalação manual, baixe <code>main.js</code>, <code>manifest.json</code> e <code>styles.css</code> da correspondência <a href="https://github.com/adventurer2008/obsidian-smart-sync-release-global/releases">Versão GitHub</a>. Verifique seu <code>SHA256SUMS.txt</code>. Coloque os três arquivos em <code>&lt;vault&gt;/.obsidian/plugins/smart-sync-global/</code> (ou sua pasta de configuração personalizada <code>plugins/smart-sync-global/</code>). Recarregue Obsidian e ative Smart Sync nos plug-ins da comunidade depois de revisar você mesmo o prompt de confiança do host.</p>
<h2 id="sign-in-and-connect-your-first-vault">Faça login e conecte seu primeiro cofre</h2>
<ol>
<li>Abrir <strong>Configurações → Smart Sync → Entrar</strong>, escolha Google, GitHub ou e-mail e crie ou selecione um cofre na nuvem. Mantenha sua senha de criptografia segura; o login da conta não pode recuperá-lo.</li>
<li>Revise as preferências de sincronização, execute a sincronização e confirme a conclusão antes de adicionar outro dispositivo. Siga o <a href="USER-GUIDE.md">manual passo a passo</a> para emparelhamento, recuperação e solução de problemas.</li>
</ol>
<h2 id="features">Recursos</h2>
<ul>
<li>Sincronização de notas, políticas de download de anexos, exclusões, progresso de tarefas e aceleração de LAN opcional com fallback na nuvem.</li>
<li>Recuperação de histórico e notas excluídas dentro dos limites de retenção, emparelhamento/revogação de dispositivos e recuperação de configuração criptografada.</li>
<li>Configurações Obsidian selecionadas, plug-ins compatíveis, temas e snippets sincronizados entre dispositivos.</li>
<li>Classificação em nível de pasta, notas fixadas/inferiores, arquivos recentes e pesquisa de notas locais.</li>
<li>Notas inteiras ou texto selecionado protegidos por senha, edição segura e recuperação de rascunhos criptografados. Títulos, anexos vinculados e histórico anterior de texto simples têm limites de privacidade separados.</li>
<li>Bandeja de desktop onde há suporte e inicialização opcional do Windows no login. Os sistemas móveis podem suspender o trabalho em segundo plano; retorne para Obsidian e confirme o término dos uploads.</li>
</ul>
<h2 id="account-payments-and-privacy">Conta, pagamentos e privacidade</h2>
<p>A sincronização hospedada requer uma conta. O plano Gratuito inclui atualmente 50 MB, um cofre na nuvem e dispositivos ilimitados; planos pagos adicionam capacidade.Os pagamentos são em USD, com Stripe por padrão; algumas contas podem usar Dodo Payments. Pedidos não pagos podem ser retomados. Pedidos e assinaturas existentes mantêm o provedor original. Não pague novamente se o resultado estiver incerto. Revisão <a href="https://smartsync.cc/pt-BR/pricing/">planos</a> e <a href="https://smartsync.cc/pt-BR/terms/">termos</a> antes de pagar.</p>
<p>O conteúdo e os caminhos são criptografados no dispositivo. A identidade da conta, os rótulos do cofre/dispositivo, o uso e os metadados operacionais estão fora da criptografia de conteúdo. O cliente Global mantém diagnósticos localmente para exportação manual e não carrega telemetria de diagnóstico. A criptografia e o histórico não substituem os backups independentes. Leia o <a href="https://smartsync.cc/pt-BR/privacy/">política de privacidade</a>.</p>
<p>Para exclusão da conta, primeiro exclua os cofres na nuvem e aguarde a limpeza, depois use <strong>Conta → Zona de perigo → Excluir conta</strong>, verifique a mesma identidade e insira a confirmação solicitada. As notas locais permanecem.</p>
<p>Dúvidas: <a href="mailto:admin@smartsync.cc">admin@smartsync.cc</a>. Inclua sua plataforma e versões do plugin/Obsidian; nunca envie senhas, tokens, códigos de e-mail ou notas privadas.</p>
