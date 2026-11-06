<p><a href="../../../README.md">English</a> · <a href="../zh-CN/README.md">简体中文</a> · <a href="../zh-TW/README.md">繁體中文</a> · <a href="../ja/README.md">日本語</a> · <a href="../ko/README.md">한국어</a> · <a href="../de/README.md">Deutsch</a> · <a href="../fr/README.md">Français</a> · <a href="../es/README.md">Español</a> · <a href="../pt-BR/README.md">Português (Brasil)</a> · <a href="../ru/README.md">Русский</a></p>
<h1 id="smart-sync">Smart Sync</h1>
<p>Un plugin de sincronización de la comunidad para Obsidian. <strong>Sincronización en tiempo real entre dispositivos, mayor velocidad y funciones más potentes que van más allá del servicio oficial Obsidian Sync.</strong><br>
Mantén sincronizadas tus notas, archivos adjuntos y ajustes seleccionados en ordenadores, teléfonos y tabletas.</p>
<p>El servidor de aplicaciones global se ejecuta en Oracle Cloud en Ashburn, Estados Unidos. Los datos de objetos cifrados se almacenan de forma privada con Cloudflare R2.</p>
<p>Valoramos la seguridad y la privacidad de los datos. Las notas, los adjuntos y las rutas de archivos se cifran en su dispositivo con AES-256-GCM antes de subirlos. El cifrado y descifrado se realizan en sus dispositivos; el servicio almacena contenido cifrado y la contraseña de cifrado es independiente del inicio de sesión de la cuenta.</p>
<p>Utilice Obsidian <strong>1.12.7 o más reciente</strong>.</p>
<p><a href="https://smartsync.cc/es/">Sitio web</a> · <a href="https://smartsync.cc/es/download/">Descargar / actualizar</a> · <a href="USER-GUIDE.md">Manual de operación</a> · <a href="https://smartsync.cc/es/pricing/">Planes</a></p>
<h2 id="get-started">empezar</h2>
<h3 id="install-from-obsidian-community-plugins">Instalar desde los plugins de la comunidad de Obsidian</h3>
<p>Cuando Smart Sync figure en el directorio de la comunidad de Obsidian, podrá instalarlo directamente en Obsidian:</p>
<ol>
<li>En Obsidian, abra Ajustes → Plugins de la comunidad.</li>
<li>Si están desactivados, active los plugins de la comunidad y lea el aviso de Obsidian.</li>
<li>Seleccione Explorar, busque Smart Sync y abra su ficha (autor: lihy).</li>
<li>Seleccione Instalar y, después, Activar.</li>
</ol>
<h3 id="wujie-hub-or-manual-download">Wujie Hub o descarga manual</h3>
<p>En Wujie Hub, seleccione <strong>Smart Sync → Estable</strong> para obtener la versión estable actual.</p>
<p>Para instalación manual, descargue <code>main.js</code>, <code>manifest.json</code> y <code>styles.css</code> de la coincidencia <a href="https://github.com/adventurer2008/obsidian-smart-sync-release-global/releases">Lanzamiento GitHub</a>. Comprueba su <code>SHA256SUMS.txt</code>. Coloque los tres archivos en <code>&lt;vault&gt;/.obsidian/plugins/smart-sync-global/</code> (o la carpeta de configuración personalizada <code>plugins/smart-sync-global/</code>). Vuelva a cargar Obsidian, luego habilite Smart Sync en los complementos de la comunidad después de revisar usted mismo el indicador de confianza del host.</p>
<h2 id="sign-in-and-connect-your-first-vault">Inicia sesión y conecta tu primera bóveda</h2>
<ol>
<li>Abierto <strong>Configuración → Smart Sync → Iniciar sesión</strong>, elija Google, GitHub o envíe un correo electrónico y luego cree o seleccione una bóveda en la nube. Mantenga segura su contraseña de cifrado; El inicio de sesión de la cuenta no puede recuperarlo.</li>
<li>Revise las preferencias de sincronización, ejecute la sincronización y confirme la finalización antes de agregar otro dispositivo. Sigue el <a href="USER-GUIDE.md">manual paso a paso</a> para emparejamiento, recuperación y solución de problemas.</li>
</ol>
<h2 id="features">Características</h2>
<ul>
<li>Sincronización de notas primero, políticas de descarga de archivos adjuntos, exclusiones, progreso de tareas y aceleración LAN opcional con respaldo en la nube.</li>
<li>Recuperación de historial y notas eliminadas dentro de los límites de retención, emparejamiento/revocación de dispositivos y recuperación de configuración cifrada.</li>
<li>Configuraciones Obsidian seleccionadas, complementos compatibles, temas y fragmentos sincronizados entre dispositivos.</li>
<li>Clasificación a nivel de carpeta, notas fijadas/inferiores, archivos recientes y búsqueda de notas locales.</li>
<li>Notas completas o texto seleccionado protegido con contraseña, edición segura y recuperación de borradores cifrados. Los títulos, los archivos adjuntos vinculados y el historial de texto plano anterior tienen límites de privacidad separados.</li>
<li>Bandeja de escritorio donde se admite y se inicia el Windows opcional al iniciar sesión. Los sistemas móviles pueden suspender el trabajo en segundo plano; Regrese a Obsidian y confirme que las cargas finalizaron.</li>
</ul>
<h2 id="account-payments-and-privacy">Cuenta, pagos y privacidad</h2>
<p>La sincronización alojada requiere una cuenta. El plan gratuito actualmente incluye 50 MB, una bóveda en la nube y dispositivos ilimitados; Los planes pagos agregan capacidad.Los pagos se realizan en USD con Stripe de forma predeterminada; algunas cuentas pueden usar Dodo Payments. Se reanuda el pedido pendiente y los pedidos y suscripciones existentes conservan su proveedor. No vuelva a pagar si el resultado es incierto. Revisión <a href="https://smartsync.cc/es/pricing/">planes</a> y <a href="https://smartsync.cc/es/terms/">términos</a> antes de pagar.</p>
<p>El contenido y las rutas están cifrados en el dispositivo. La identidad de la cuenta, las etiquetas de la bóveda/dispositivo, el uso y los metadatos operativos están fuera del cifrado de contenido. El cliente global mantiene los diagnósticos localmente para exportarlos manualmente y no carga telemetría de diagnóstico. El cifrado y el historial no reemplazan las copias de seguridad independientes. Lea el <a href="https://smartsync.cc/es/privacy/">política de privacidad</a>.</p>
<p>Para eliminar una cuenta, primero elimine las bóvedas en la nube y espere a que se limpien, luego use <strong>Cuenta → Zona de peligro → Eliminar cuenta</strong>, verificar la misma identidad e ingresar la confirmación solicitada. Los billetes locales permanecen.</p>
<p>Consultas: <a href="mailto:admin@smartsync.cc">admin@smartsync.cc</a>. Incluya su plataforma y versiones del complemento/Obsidian; nunca envíe contraseñas, tokens, códigos de correo electrónico o notas privadas.</p>
