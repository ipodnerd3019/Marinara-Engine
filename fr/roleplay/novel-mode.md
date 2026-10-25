# Novel Mode : écrire une histoire à deux

Ce guide explique Novel Mode dans Marinara Engine. Novel Mode transforme un chat Roleplay en une seule page continue, comme un manuscrit, où toi et l'IA écrivez une histoire ensemble. Il explique comment commencer un roman, écrire et modifier des passages, orienter l'IA et écouter l'histoire.

## Ce qu'est Novel Mode

Novel Mode est un style d'affichage pour les chats Roleplay. L'histoire se lit comme une seule page plutôt que comme un chat : il n'y a ni avatars, ni noms, ni horodatages, ni bulles de message. Chaque fois que l'IA écrit, elle ajoute un passage à la page. Les paragraphes sont mis en retrait comme dans un livre imprimé, et les passages s'enchaînent sans coupure.

Contrairement à un Roleplay classique, l'IA écrit aussi ton protagoniste. Elle écrit ses actions, ses dialogues et ses pensées, si bien que l'histoire avance sans attendre ton tour. Tu l'orientes autrement : en écrivant tes propres passages, en modifiant ce qui est déjà sur la page et en donnant de courtes consignes pour le passage suivant.

Un roman reste un chat Roleplay sous la surface. Les lorebooks – des recueils de faits sur ton univers –, les résumés, la mémoire, les branches et les agents fonctionnent comme dans n'importe quel Roleplay.

Avec plusieurs personnages, un roman utilise toujours le mode de groupe **Merged** (fusionné) : l'IA écrit tous les personnages d'une seule voix, comme le ferait un romancier, il n'y a donc pas de tours à prendre. Pour les romans, **Chat Settings** (réglages du chat) masque les options de mode de groupe, d'ordre des réponses et de couleur des dialogues. Le **Scenario Override** (remplacement du scénario) du groupe s'applique toujours.

## Commencer un roman

1. Crée un nouveau chat Roleplay.
2. À la première étape de l'assistant de configuration, règle **Display style** (style d'affichage) sur **Novel** (roman).
3. Termine l'assistant. Les personnages et le persona sont facultatifs. N'ajoute des personnages que si tu veux que leurs fiches de personnage fassent partie du contexte de l'histoire.

Choisir **Novel** conserve tes agents, comme dans n'importe quel Roleplay. Les sprites, le HUD et les effets météo s'affichent quand les agents qui les produisent sont activés (Expression Engine, World State et les agents tracker) ; retire ces agents dans l'assistant ou dans **Chat Settings** pour obtenir une page nue. Les romans affichent une icône de livre dans la liste des chats.

Choisir **Novel** sélectionne aussi **Marinara's Novel Preset**, qui demande à l'IA d'écrire ton protagoniste (voir plus bas). Tu peux choisir un autre preset – un modèle de prompt enregistré – à l'étape **Preset** de l'assistant ou plus tard dans **Chat Settings**. Si tu reviens à un autre style d'affichage dans le même assistant, ton preset précédent revient, sauf si tu en as choisi un autre entre-temps.

## Écrire et modifier

- **Ajouter ton propre texte :** écris sur la ligne en bas de la page, qui affiche **Keep writing, or press Send…** (continue d'écrire ou appuie sur Send). Quand tu quittes la ligne ou que tu appuies sur **Send** (envoyer), ton texte devient le passage suivant de l'histoire.
- **Modifier n'importe quoi sur la page :** toute la page est un seul éditeur. Clique n'importe où et tape, comme dans un traitement de texte. Tes modifications s'enregistrent d'elles-mêmes un instant après que tu as arrêté de taper, et **Ctrl+Z** les annule.
- **Mise en forme :** le texte d'un passage peut être en *italique* ou en **gras**. Sélectionne-le et appuie sur **Ctrl+I** ou **Ctrl+B** (**Cmd** sur Mac). Il est enregistré en markdown, sous la forme `*italic*` et `**bold**`, et les `*text*`, `_text_`, `**text**` et `__text__` déjà présents dans un passage s'affichent en italique et en gras. Tout autre balisage, comme les titres, les listes, les liens et le HTML, s'affiche en texte brut et ne reçoit aucun traitement particulier. Les retours à la ligne sont conservés : un passage dont les paragraphes tiennent sur des lignes simples les garde ainsi quand tu le modifies.
- **Sélectionner sur plusieurs passages :** tu peux sélectionner, copier et supprimer du texte qui s'étend sur plusieurs passages. Chaque passage reste une partie distincte de l'histoire : supprimer à cheval sur plusieurs passages retire du texte de chacun, jamais les passages eux-mêmes. Si tu vides complètement un passage et que tu passes à autre chose, Marinara te demande s'il faut le supprimer.
- **Actions d'un passage :** passe le pointeur sur un passage, ou place le curseur dedans, pour voir ses actions dans la marge : copier, traduire, régénérer, signet, épingler ou note, **Mark as new start** (marquer comme nouveau départ), masquer à l'IA, créer une branche et supprimer, plus **Speak** (lire à voix haute) quand la synthèse vocale est activée. Le dernier passage a aussi **Peek prompt** (voir le prompt), et un passage écrit avec une consigne a **Stored guidance** (consigne enregistrée), qui montre la direction qui lui a été donnée. Sur un téléphone, touche le passage, ou place le curseur dedans, pour les afficher.

## Demander la suite à l'IA

La barre de message sous la page fonctionne comme dans n'importe quel Roleplay, à une différence près : ce que tu y tapes ne devient jamais un message. Cela oriente seulement le passage suivant.

- **Send** avec une barre vide écrit les quelques paragraphes suivants de l'histoire.
- Tape une courte direction, comme `a storm arrives` ("une tempête arrive"), et appuie sur **Send**. L'IA oriente le passage suivant dans ce sens sans l'écrire dans l'histoire.
- Les commandes slash, la dictée et les sélecteurs de connexion et de persona fonctionnent comme d'habitude. Les pièces jointes et les réponses rapides **Post only** (publier seulement) et **Guide reply** (réponse guidée) ne sont pas proposées : rien de ce que tu publies ne devient un message, et **Send** envoie déjà ton texte comme consigne.
- Impersonate n'est pas proposé dans un roman : tu n'as pas de tour à écrire, puisque l'IA écrit déjà ton protagoniste. La commande `/impersonate`, la réponse rapide Impersonate et les réglages Impersonate du chat sont masqués.
- Avec l'agent CYOA activé, choisir l'une de ses options oriente le passage suivant dans ce sens, comme une consigne. Elle ne devient jamais un message de ta part, l'interrupteur Impersonate des choix est donc masqué. Avec **Add CYOA choices to the message box instead of sending them** (ajouter les choix CYOA à la zone de saisie au lieu de les envoyer) activé, le choix va plutôt dans la barre de message, où tu peux le combiner avec ta propre consigne.
- Pour réécrire un passage, utilise régénérer (**Regenerate**) dans ses actions. Tes modifications sont enregistrées d'abord. Avec **Guide swipes/regens with chat input** (guider les swipes et régénérations avec la zone de saisie) activé dans **Settings** (Paramètres) et du texte dans la barre de message, le bouton affiche **Regenerate (guided)** et oriente la nouvelle version vers ce texte, comme le fait **Send**. Dès qu'un passage a plus d'une version, des flèches sous lui permettent de passer de l'une à l'autre, et toute modification en cours de frappe est enregistrée dans la version sur laquelle tu l'as tapée.
- Pendant que l'IA écrit, **Send** devient **Stop** (arrêter).

## Comment l'IA est guidée pour écrire un roman

**Marinara's Novel Preset** est un preset intégré écrit pour les romans. Il indique à l'IA qu'elle coécrit un seul manuscrit avec toi, qu'elle écrit tous les personnages, y compris ton protagoniste, et qu'elle écrit de la prose de livre : des paragraphes, des dialogues entre guillemets, de l'*italique* seulement pour les pensées et l'insistance, et aucun autre markdown. Chaque passage reprend là où la page s'arrête et s'interrompt sur une pause naturelle, jamais sur une question qui t'est adressée. Elle suit la consigne que tu tapes dans la barre de message sans la citer ni écrire de notes à son sujet dans le passage.

L'identité du protagoniste dépend de la façon dont tu configures le roman :

| Configuration | Protagoniste | Distribution |
| --- | --- | --- |
| Ni persona ni personnages | Le protagoniste que le manuscrit suit déjà. Sur une page vide, l'IA en établit un, avec un nom, une voix et un désir, et le garde cohérent. | Pas de distribution préparée. L'IA introduit des personnages selon les besoins de l'histoire. |
| Un persona et des personnages | Ton persona. Son profil fait partie de la bible de l'histoire. | Tes personnages, chacun fidèle à sa fiche. |
| Des personnages mais pas de persona | Le protagoniste que le manuscrit suit déjà. Sinon, avec un seul personnage, ce personnage, sauf si sa fiche décrit quelqu'un d'autre, auquel cas l'IA crée cette personne. Avec plusieurs, l'IA choisit l'un d'eux, ou un nouveau personnage si les fiches désignent quelqu'un d'autre. | Tes personnages. |
| Un persona mais pas de personnages | Ton persona. | Pas de distribution préparée. |

Un persona compte quand il a une description ou un autre texte. Un persona qui n'a qu'un nom compte comme l'absence de persona, puisque l'IA ne voit jamais son nom. Sans persona, une fiche qui mentionne `{{user}}` se lit "User" ; les fiches écrites pour un roman sans persona se lisent donc mieux quand elles nomment le protagoniste ou ne mentionnent pas `{{user}}`.

Le preset pose quelques questions quand tu commences le roman : la classification du contenu (**NSFW** ou **SFW**), le point de vue (troisième, première ou deuxième personne), le style de narration (proche du protagoniste, alternant entre personnages-points de vue aux changements de scène, ou omniscient), le temps du récit, la longueur des passages (**Length**, longueur) et la langue. La première option de chaque question est celle par défaut.

Comme Marinara's Universal Preset, le preset Novel est en lecture seule et ne peut pas être supprimé. Ouvre-le dans **Presets** et crée une copie modifiable pour changer sa formulation. Il utilise tes réglages de génération de connexion et de chat plutôt que les siens. Voir [Éditeur de presets et gestionnaire de prompts](../prompts/presets.md).

Quelques points à connaître :

- Dans les chats Roleplay, une connexion avec son propre remplacement de preset utilise ce preset à la place, dans les romans aussi.
- Passer plus tard un roman en Visual Novel ou Classic avec l'interrupteur **Visual Novel display** (affichage Visual Novel) dans **Settings > Appearance** (Paramètres > apparence) conserve le preset Novel. Choisis un autre preset dans **Chat Settings** si tu ne veux plus que l'IA écrive ton protagoniste. L'interrupteur change aussi ton style d'affichage par défaut pour les chats Roleplay sans style enregistré, pas seulement le roman ouvert.
- Un autre preset fonctionne aussi dans un roman, mais la plupart des presets de Roleplay demandent à l'IA de ne jamais écrire ton personnage. C'est le cas de Marinara's Universal Preset : avec lui, l'IA te laisse ton protagoniste.

## Écouter l'histoire

Quand la synthèse vocale est activée, les actions de chaque passage incluent **Speak**. Avec **Only read dialogues** (ne lire que les dialogues) désactivé, la narration est lue aussi, avec la voix du narrateur quand **Use separate narrator voice** (utiliser une voix de narrateur distincte) est activé. Avec **Only read dialogues** activé, seuls les dialogues entre guillemets sont lus.
