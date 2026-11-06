<p><a href="../../../README.md">English</a> · <a href="../zh-CN/README.md">简体中文</a> · <a href="../zh-TW/README.md">繁體中文</a> · <a href="../ja/README.md">日本語</a> · <a href="../ko/README.md">한국어</a> · <a href="../de/README.md">Deutsch</a> · <a href="../fr/README.md">Français</a> · <a href="../es/README.md">Español</a> · <a href="../pt-BR/README.md">Português (Brasil)</a> · <a href="../ru/README.md">Русский</a></p>
<h1 id="smart-sync">Smart Sync</h1>
<p>Synchronisation cryptée de vos notes, pièces jointes et paramètres sélectionnés Obsidian. Préservez les heures de modification des fichiers d&#x27;origine, récupérez les versions conservées et gérez vos appareils.</p>
<p>Le serveur d&#x27;applications global s&#x27;exécute sur Oracle Cloud à Ashburn, aux États-Unis. Les données des objets chiffrés sont stockées de manière privée avec Cloudflare R2.</p>
<p>Nous accordons de l’importance à la sécurité et à la confidentialité des données. Les notes, pièces jointes et chemins de fichiers sont chiffrés sur votre appareil avec AES-256-GCM avant leur envoi. Le chiffrement et le déchiffrement ont lieu sur vos appareils ; le service stocke le contenu chiffré et votre mot de passe de chiffrement est distinct de vos identifiants de connexion.</p>
<p>Utiliser Obsidian <strong>1.12.7 ou version ultérieure</strong>.</p>
<p><a href="https://smartsync.cc/fr/">Site Web</a> · <a href="https://smartsync.cc/fr/download/">Télécharger / mettre à jour</a> · <a href="USER-GUIDE.md">Manuel d&#x27;utilisation</a> · <a href="https://smartsync.cc/fr/pricing/">Forfaits</a></p>
<h2 id="get-started">Commencez</h2>
<h3 id="install-from-obsidian-community-plugins">Installer depuis les plugins communautaires d’Obsidian</h3>
<p>Une fois Smart Sync référencé dans le répertoire communautaire d’Obsidian, vous pourrez l’installer directement dans Obsidian :</p>
<ol>
<li>Dans Obsidian, ouvrez Paramètres → Plugins communautaires.</li>
<li>Si les plugins communautaires sont désactivés, activez-les et lisez l’avertissement affiché par Obsidian.</li>
<li>Choisissez Parcourir, recherchez Smart Sync et ouvrez sa fiche (auteur : lihy).</li>
<li>Choisissez Installer, puis Activer.</li>
</ol>
<h3 id="wujie-hub-or-manual-download">Wujie Hub ou téléchargement manuel</h3>
<p>Dans Wujie Hub, sélectionnez <strong>Smart Sync → Stable</strong> pour obtenir la version stable actuelle.</p>
<p>Pour une installation manuelle, téléchargez <code>main.js</code>, <code>manifest.json</code> et <code>styles.css</code> de la correspondance <a href="https://github.com/adventurer2008/obsidian-smart-sync-release-global/releases">Sortie GitHub</a>. Vérifiez son <code>SHA256SUMS.txt</code>. Placez les trois fichiers dans <code>&lt;vault&gt;/.obsidian/plugins/smart-sync-global/</code> (ou celui de votre dossier de configuration personnalisé <code>plugins/smart-sync-global/</code>). Rechargez Obsidian, puis activez Smart Sync dans les plugins de la communauté après avoir examiné vous-même l&#x27;invite de confiance de l&#x27;hôte.</p>
<h2 id="sign-in-and-connect-your-first-vault">Connectez-vous et connectez votre premier coffre-fort</h2>
<ol>
<li>Ouvert <strong>Paramètres → Smart Sync → Connexion</strong>, choisissez Google, GitHub ou e-mail, puis créez ou sélectionnez un coffre-fort cloud. Conservez sa phrase secrète de cryptage en sécurité ; la connexion au compte ne peut pas le récupérer.</li>
<li>Vérifiez les préférences de synchronisation, exécutez la synchronisation et confirmez l&#x27;achèvement avant d&#x27;ajouter un autre appareil. Suivez le <a href="USER-GUIDE.md">manuel étape par étape</a> pour l&#x27;appairage, la récupération et le dépannage.</li>
</ol>
<h2 id="features">Caractéristiques</h2>
<ul>
<li>Synchronisation Notes-first, politiques de téléchargement de pièces jointes, exclusions, progression des tâches et accélération LAN en option avec repli sur le cloud.</li>
<li>Récupération de l&#x27;historique et des notes supprimées dans les limites de conservation, couplage/révocation d&#x27;appareils et récupération de configuration cryptée.</li>
<li>Paramètres Obsidian sélectionnés, plugins compatibles, thèmes et extraits synchronisés sur tous les appareils.</li>
<li>Tri au niveau des dossiers, notes épinglées/en bas, fichiers récents et recherche de notes locales.</li>
<li>Notes entières ou texte sélectionné protégés par mot de passe, édition sécurisée et récupération de brouillons cryptés. Les titres, les pièces jointes liées et l&#x27;historique antérieur en texte brut ont des limites de confidentialité distinctes.</li>
<li>Plateau de bureau pris en charge et lancement facultatif du Windows lors de la connexion. Les systèmes mobiles peuvent suspendre le travail en arrière-plan ; revenez à Obsidian et confirmez la fin des téléchargements.</li>
</ul>
<h2 id="account-payments-and-privacy">Compte, paiements et confidentialité</h2>
<p>La synchronisation hébergée nécessite un compte. Le forfait gratuit comprend actuellement 50 MB, un coffre-fort cloud et un nombre illimité d&#x27;appareils ; les forfaits payants ajoutent de la capacité.Les paiements sont en USD, via Stripe par défaut ; certains comptes peuvent utiliser Dodo Payments. Une commande impayée peut être reprise. Les commandes et abonnements existants conservent leur prestataire. Ne payez pas à nouveau si le résultat est incertain. Examen <a href="https://smartsync.cc/fr/pricing/">plans</a> et <a href="https://smartsync.cc/fr/terms/">termes</a> avant de payer.</p>
<p>Le contenu et les chemins sont cryptés sur l&#x27;appareil. L’identité du compte, les étiquettes du coffre-fort/appareil, l’utilisation et les métadonnées opérationnelles ne relèvent pas du cryptage du contenu. Le client Global conserve les diagnostics localement pour une exportation manuelle et ne télécharge pas la télémétrie de diagnostic. Le chiffrement et l&#x27;historique ne remplacent pas les sauvegardes indépendantes. Lire le <a href="https://smartsync.cc/fr/privacy/">politique de confidentialité</a>.</p>
<p>Pour supprimer un compte, supprimez d&#x27;abord les coffres-forts cloud et attendez le nettoyage, puis utilisez <strong>Compte → Zone de danger → Supprimer le compte</strong>, vérifiez la même identité et saisissez la confirmation demandée. Les notes locales demeurent.</p>
<p>Questions : <a href="mailto:admin@smartsync.cc">admin@smartsync.cc</a>. Incluez votre plate-forme et vos versions de plugin/Obsidian ; n’envoyez jamais de mots de passe, de jetons, de codes de courrier électronique ou de notes privées.</p>
