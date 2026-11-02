# Jaya Player — guide d’utilisation

Jaya Player est un lecteur IPTV pour Android TV, box TV et smartphones.
L’application **ne fournit aucune chaîne TV ni contenu** : elle lit uniquement les playlists ajoutées par l’utilisateur.

---

## 1. Installation

1. Téléchargez l’application : **https://github.com/FirstRandomUser/jaya-player-releases/releases/latest/download/jaya-player.apk** (toujours la dernière version) ou depuis la page [Releases](https://github.com/FirstRandomUser/jaya-player-releases/releases/latest).
2. Sur une box TV, l’application **Downloader** ou une clé USB est pratique.
3. Lors de la première installation, Android demande d’autoriser l’installation depuis cette source — autorisez-la.
4. Android 6.0 ou plus récent est requis.

Ensuite, l’application télécharge et installe les mises à jour **toute seule** (voir section 10).

---

## 2. Premier lancement et playlist

Au premier lancement, les **Paramètres** s’ouvrent.

1. Appuyez sur **Playlists → Ajouter**.
2. Choisissez le type :
   - **lien M3U** — adresse de la playlist fournie par votre fournisseur ;
   - **Xtream Codes** — adresse du serveur, identifiant et mot de passe ;
   - **fichier** — playlist `.m3u` sur l’appareil ou une clé USB.
3. **EPG** (guide des programmes) — adresse XMLTV. Elle figure généralement déjà dans la playlist du fournisseur, le champ peut rester vide. S’il n’y a pas de guide, demandez l’adresse EPG à votre fournisseur et saisissez-la ici.
4. **Mettre à jour toutes les … h** — fréquence de mise à jour de la playlist et du guide.
5. Appuyez sur **Enregistrer**. Le chargement se fait en arrière-plan — vous pouvez reprendre le visionnage tout de suite.

Vous pouvez ajouter plusieurs playlists. Si une mise à jour échoue (par exemple sans internet), l’application réessaie d’elle-même au prochain lancement.

---

## 3. Télécommande

| Touche | Action |
|---|---|
| ▲ ▼ | chaîne précédente / suivante |
| ◀ | liste des chaînes |
| ◀ ◀ (plus à gauche) | liste des groupes |
| ▶ | Favoris |
| ▶ ▶ (deux fois vite) | statistiques du flux (on/off) |
| OK | panneau d’infos |
| OK à nouveau | pause |
| OK en pause | reprendre |
| OK long | menu d’actions (audio, sous-titres, format, paramètres) |
| chiffres | aller à une chaîne par son numéro |
| 0 | chaîne précédente |
| Retour deux fois | quitter |

**Dans la liste des chaînes :**
- ▶ — guide de la chaîne sélectionnée ;
- OK long — mode de marquage : ◀ ajouter/retirer des Favoris, ▶ supprimer la chaîne (les chaînes supprimées se restaurent dans le groupe « Supprimées »).

**Sur smartphone :** toucher — pause et panneau d’infos ; glisser vers le haut — panneau, vers le bas — le masquer ; glisser vers la droite sur la moitié gauche — liste des chaînes ; vers la gauche sur la moitié droite — Favoris ; appui long — paramètres.

---

## 4. Guide et archives

- Le guide est conservé **24 heures en arrière et 48 heures en avant**.
- Appuyez sur ▶ dans la liste des chaînes pour ouvrir le guide. Les émissions passées peuvent être regardées depuis les **archives** si votre fournisseur les propose.
- Dans les archives : **OK** — barre de navigation, ◀ ▶ — pas (s’accélère en maintenant), **Retour** — revenir au direct.

---

## 5. Pause du direct (Timeshift)

**Paramètres → Lecture → Pause du direct avec enregistrement.**

- **Désactivée :** la pause fige l’image ; à la reprise, on revient au direct.
- **Activée :** après la pause, la lecture reprend **au même moment**. Le retard sur le direct s’affiche en bas ; **Retour** — revenir au direct.

**Stockage de la pause :**
- **Mémoire interne** — l’enregistrement démarre au moment de la pause et est supprimé au changement de chaîne.
- **Disque externe (USB)** — l’enregistrement tourne en permanence pendant que vous regardez une chaîne, donc **en pause ◀ ▶ permettent de reculer** (autant que l’espace le permet). L’application crée un dossier `Timeshift` sur le disque et utilise au maximum 80 % de l’espace libre ; les anciens enregistrements sont supprimés automatiquement.

Clé USB : FAT32 ou exFAT (NTFS si votre appareil le gère).
Les flux DASH, les flux chiffrés et les flux à piste audio séparée ne sont pas pris en charge — la pause y fonctionne normalement.

---

## 6. Groupes masqués (contrôle parental)

1. Ouvrez la liste des groupes (◀ ◀), sélectionnez un groupe et **maintenez OK** — la sélection de groupes s’active.
2. Marquez les groupes avec OK et appuyez sur **Retour**.
3. Saisissez le mot de passe avec les flèches et appuyez sur OK. Mot de passe par défaut : **▶ ▶ ▶ ▶**.
4. Après le premier masquage, l’application propose de créer votre propre mot de passe en flèches (ex. ▲ ▲ ◀ ▶) — retenez-le.

Pour réafficher les groupes masqués, dans la liste des groupes **appuyez trois fois vite sur ◀** et saisissez le mot de passe. Les groupes sont de nouveau masqués quand l’application est réduite.

---

## 7. Image dans l’image et arrière-plan (smartphone)

- **Image dans l’image :** en revenant à l’écran d’accueil, la vidéo continue dans une petite fenêtre.
- **Son en arrière-plan :** le son continue écran verrouillé ; contrôles dans le volet des notifications.

---

## 8. Paramètres

- **Écran :** fréquence d’images automatique, 120 Hz, durée du panneau d’infos, défilement des listes, **écran OLED** (protection contre le marquage : décalage des éléments, horloge masquée, économiseur d’écran en pause, assombrissement des menus).
- **Horloge :** position à l’écran.
- **Lecture :** image dans l’image, son en arrière-plan, nivellement du volume, statistiques, pause du direct, préchargement des chaînes voisines, tampon, User-Agent.
- **Thèmes** (bouton « Thèmes » séparé dans les paramètres) : thèmes prêts (Classique, Noir OLED, Océan, Chaud, Verre) ou vos propres couleurs de panneaux, sélection, texte, panneau d’infos, horloge et transparence.
- **Administration :** mot de passe et verrouillage d’options (les options verrouillées sont masquées).

**User-Agent** est la façon dont le lecteur se « présente » au serveur du fournisseur. Si la playlist se charge mais que les chaînes ne s’ouvrent pas, essayez **VLC**.

---

## 9. Sauvegarde

**Paramètres → À propos → Exporter** enregistre playlists, Favoris, groupes masqués et paramètres dans un fichier. **Importer** les restaure — par exemple sur un nouvel appareil.

---

## 10. Mises à jour

- L’application recherche, télécharge et installe les mises à jour elle-même (désactivable dans **À propos**).
- La signature est vérifiée avant l’installation — une mise à jour ne peut pas être falsifiée.
- Si l’application n’a pas pu vérifier les mises à jour pendant **90 jours**, un mode restreint s’active (sans guide ni archives, 5 chaînes en Favoris). Il suffit de se connecter à internet — tout revient.

---

## 11. Version Pro

Pour l’instant toutes les fonctions sont **gratuites**. À l’arrivée de Pro, chacun bénéficiera encore de **3 mois** d’accès complet.

| | Gratuit | Pro |
|---|---|---|
| Qualité | jusqu’à 1080p (4K/HDR — 3 minutes) | 4K, HDR |
| Favoris | 20 chaînes | illimité |
| Groupes masqués | 1 | illimité |
| Archives | 3 dernières heures | autant que le fournisseur |
| Nivellement du volume, fréquence automatique, 120 Hz, AC3/DTS vers l’ampli | — | ✓ |
| Pause du direct avec enregistrement, thèmes | — | ✓ |
| Image dans l’image et son en arrière-plan (smartphone) | — | ✓ |

---

## 12. Dépannage

- **Une chaîne ne s’ouvre pas** — changez le User-Agent (VLC) ; testez la playlist sur un autre appareil.
- **Pas de guide** — vérifiez l’adresse EPG de la playlist ; ouvrez **Playlists** — l’erreur de chargement y est affichée.
- **Son qui grésille sur smartphone avec le nivellement** — désactivez le nivellement.
- **La 4K saccade sur une box peu puissante** — choisissez le tampon « Grand » ou regardez en HD.

---

## 13. Connexion des appareils et qualité

- **Connecter des appareils** (Paramètres → Connecter des appareils) : associez le téléphone au téléviseur par un code qui s’affiche tout seul sur la TV. Envoyez playlists et paramètres, ajoutez une playlist depuis un navigateur via QR code, diffusez du téléphone vers la TV (📺, le téléphone devient télécommande) et reprenez la lecture.
- **Qualité** (panneau d’infos) : « Auto » baisse la qualité sur réseau lent ; « Meilleure » utilise toujours la plus haute. Mémorisé par chaîne.
- **Tampon « Auto »** : s’agrandit tout seul en cas de coupures fréquentes.

---

© 2026 Ruslan G. Tous droits réservés.
