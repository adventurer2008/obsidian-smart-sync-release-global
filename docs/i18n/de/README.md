<p><a href="../../../README.md">English</a> · <a href="../zh-CN/README.md">简体中文</a> · <a href="../zh-TW/README.md">繁體中文</a> · <a href="../ja/README.md">日本語</a> · <a href="../ko/README.md">한국어</a> · <a href="../de/README.md">Deutsch</a> · <a href="../fr/README.md">Français</a> · <a href="../es/README.md">Español</a> · <a href="../pt-BR/README.md">Português (Brasil)</a> · <a href="../ru/README.md">Русский</a></p>
<h1 id="smart-sync">Smart Sync</h1>
<p>Verschlüsselte Synchronisierung für Ihre Obsidian-Notizen, Anhänge und ausgewählten Einstellungen. Behalten Sie die Änderungszeiten der ursprünglichen Dateien bei, stellen Sie beibehaltene Versionen wieder her und verwalten Sie Ihre Geräte.</p>
<p>Der globale Anwendungsserver läuft auf Oracle Cloud in Ashburn, USA. Verschlüsselte Objektdaten werden privat mit Cloudflare R2 gespeichert.</p>
<p>Datensicherheit und Datenschutz sind uns wichtig. Notizen, Anhänge und Dateipfade werden vor dem Hochladen auf Ihrem Gerät mit AES-256-GCM verschlüsselt. Ver- und Entschlüsselung erfolgen auf Ihren Geräten. Der Dienst speichert verschlüsselte Inhalte; Ihr Verschlüsselungspasswort ist von Ihrer Kontoanmeldung getrennt.</p>
<p><strong>Aktuelle Version: 1.1.5</strong> · Obsidian <strong>1.12.7+</strong> · Plugin-ID: <code>smart-sync-global</code>.</p>
<p><a href="https://smartsync.cc/de/">Website</a> · <a href="https://smartsync.cc/de/download/">Herunterladen/aktualisieren</a> · <a href="USER-GUIDE.md">Bedienungsanleitung</a> · <a href="https://smartsync.cc/de/pricing/">Pläne</a></p>
<h2 id="get-started">Fangen Sie an</h2>
<ol>
<li>Sichern Sie Ihre Notizen und versuchen Sie es zunächst mit einem separaten Tresor. Wählen Sie in Wujie Hub <strong>Smart Sync → Stabil</strong>, oder laden Sie die drei Plugin-Dateien herunter von <a href="https://github.com/adventurer2008/obsidian-smart-sync-release-global/releases">Veröffentlichungen</a>.</li>
<li>Installieren <code>main.js</code>, <code>manifest.json</code> und <code>styles.css</code> in deinem Tresor <code>.obsidian/plugins/smart-sync-global/</code> Ordner. Laden Sie Obsidian neu und überprüfen Sie die Vertrauensaufforderung, bevor Sie das Plugin aktivieren. Updates ersetzen nur diese drei Dateien; Bewahren Sie Einstellungen, geheime Speicherung, Kontrollpunkte und Notizen auf.</li>
<li>Offen <strong>Einstellungen → Smart Sync → Anmelden</strong>, wählen Sie Google, GitHub oder E-Mail und erstellen Sie dann einen Cloud-Tresor oder wählen Sie ihn aus. Bewahren Sie die Verschlüsselungspassphrase sicher auf; Die Kontoanmeldung kann nicht wiederhergestellt werden.</li>
<li>Überprüfen Sie die Synchronisierungseinstellungen, führen Sie die Synchronisierung durch und bestätigen Sie den Abschluss, bevor Sie ein weiteres Gerät hinzufügen. Folgen Sie dem <a href="USER-GUIDE.md">Schritt-für-Schritt-Anleitung</a> zur Kopplung, Wiederherstellung und Fehlerbehebung.</li>
</ol>
<h2 id="features">Funktionen</h2>
<ul>
<li>Notes-First-Synchronisierung, Richtlinien zum Herunterladen von Anhängen, Ausschlüsse, Aufgabenfortschritt und optionale LAN-Beschleunigung mit Cloud-Fallback.</li>
<li>Verlauf und Wiederherstellung gelöschter Notizen innerhalb der Aufbewahrungsgrenzen, Gerätekopplung/-widerruf und Wiederherstellung verschlüsselter Konfigurationen.</li>
<li>Ausgewählte Obsidian-Einstellungen, kompatible Plugins, Themes und Snippets werden geräteübergreifend synchronisiert.</li>
<li>Sortierung auf Ordnerebene, angeheftete/unterste Notizen, zuletzt verwendete Dateien und lokale Notizensuche.</li>
<li>Passwortgeschützte ganze Notizen oder ausgewählter Text, sichere Bearbeitung und verschlüsselte Entwurfswiederherstellung. Für Titel, verknüpfte Anhänge und den früheren Klartextverlauf gelten separate Datenschutzgrenzen.</li>
<li>Desktop-Tray, sofern unterstützt, und optionaler Windows-Start beim Anmelden. Mobile Systeme können die Hintergrundarbeit unterbrechen; Kehren Sie zu Obsidian zurück und bestätigen Sie, dass der Upload abgeschlossen ist.</li>
</ul>
<p>Smart Sync 1.1.5 unterstützt zehn Oberflächensprachen. Die Sprache kann in den Plugin-Einstellungen gewählt werden.</p>
<h2 id="account-payments-and-privacy">Konto, Zahlungen und Datenschutz</h2>
<p>Für die gehostete Synchronisierung ist ein Konto erforderlich. Der kostenlose Plan umfasst derzeit 50 MB, einen Cloud-Tresor und unbegrenzte Geräte; Bezahlte Pläne erhöhen die Kapazität.Zahlungen erfolgen in USD, standardmäßig über Stripe; einigen Konten kann Dodo Payments zugewiesen werden. Unbezahlte Bestellungen werden fortgesetzt. Bestehende Bestellungen und Abonnements behalten ihren Zahlungsanbieter. Zahlen Sie bei unklarem Status nicht erneut. Rezension <a href="https://smartsync.cc/de/pricing/">Pläne</a> und <a href="https://smartsync.cc/de/terms/">Begriffe</a> vor der Zahlung.</p>
<p>Inhalte und Pfade werden auf dem Gerät verschlüsselt. Kontoidentität, Tresor-/Gerätebezeichnungen, Nutzungs- und Betriebsmetadaten liegen außerhalb der Inhaltsverschlüsselung. Der globale Client speichert die Diagnosen lokal für den manuellen Export und lädt keine Diagnosetelemetriedaten hoch. Verschlüsselung und Verlauf ersetzen keine unabhängigen Backups. Lesen Sie die <a href="https://smartsync.cc/de/privacy/">Datenschutzrichtlinie</a>.</p>
<p>Zum Löschen eines Kontos löschen Sie zunächst die Cloud-Tresore, warten Sie auf die Bereinigung und verwenden Sie sie dann <strong>Konto → Gefahrenzone → Konto löschen</strong>, überprüfen Sie dieselbe Identität und geben Sie die angeforderte Bestätigung ein. Lokale Notizen bleiben erhalten.</p>
<p>Fragen: <a href="mailto:admin@smartsync.cc">admin@smartsync.cc</a>. Geben Sie Ihre Plattform- und Plugin-/Obsidian-Versionen an; Senden Sie niemals Passwörter, Token, E-Mail-Codes oder private Notizen.</p>
