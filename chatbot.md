---
clavier: true
gestionGrosMots: true
rechercheContenu: true
avatar: https://college-vincent-van-gogh.forge.apps.education.fr/chatbot_assistance_vvg/Documents/VVG-AVATAR-FT.png
avatarCercle: true
favicon: https://college-vincent-van-gogh.forge.apps.education.fr/chatbot_assistance_vvg/Documents/VVG-FAVICON40.png
footer: 'Outil construit avec ChatMD, outil libre & gratuit créé par Cédric Eyssette - Paramétrages et configuration : Adrien Magraner (Référent Numérique) & Nathalie Tregoat (ATI)'
contenuDynamique: true
typewriter: false
messageParDéfaut: ["Désolé, je suis encore en train d'apprendre et n'ai pas la réponse à votre question. Contactez l'établissement pour plus d'information.", "Je n'ai pas encore appris la réponse à cette question. Peut-être qu'en contactant directement l'établissement, vous pourrez obtenir plus d'informations ?"]
theme: bubbles
include: ['https://college-vincent-van-gogh.forge.apps.education.fr/chatbot_assistance_vvg/sans-profil.md', 'https://college-vincent-van-gogh.forge.apps.education.fr/chatbot_assistance_vvg/Aide-Pix-Eleves.md', 'https://college-vincent-van-gogh.forge.apps.education.fr/chatbot_assistance_vvg/Aide-Pix-Professeurs.md', 'https://college-vincent-van-gogh.forge.apps.education.fr/chatbot_assistance_vvg/Aide-Neo-Eleve.md' , https://github.com/ntregoat/VinceAssist/blob/main/Aide-Num-Prof.md , https://github.com/ntregoat/VinceAssist/blob/main/Aide-Num-Prof.md]
---

# Collège Vincent Van Gogh : Besoin d'aide ?

<center>![Logo-vvg](https://college-vincent-van-gogh.forge.apps.education.fr/chatbot_assistance_vvg/Documents/VVG-AVATAR-FT.jpg)</center>
<!-- Pas besoin d'entrée clavier ici, orientation principale du chatbot -->

`@KEYBOARD = false`

*****

Bonjour, je suis **Vincent**, un chatbot programmé pour répondre, ou du moins essayer de répondre, à vos questions concernant le collège.

:::warning collapsible *Important !*
Je suis en constante évolution et n'aurais probablement pas les réponses à toutes les questions. Dans ce cas, n'hésitez pas à contacter l'établissement.
:::
*****

Tout d'abord, faisons plus ample connaissance. Cela me permettra de mieux vous aider.

Qui êtes-vous ?

1. [Un élève](eleves_accueil)
2. [Un personnel de l'établissement](profs_accueil)
3. [Un parent d'élève](responsables_accueil) 
4. [Une personne extérieure à l'établissement](exterieurs_accueil)


<!-- Ici uniquement les pages d'accueil général en fonction des profils.
Le contenu est répartis dans les différents fichiers -->

## eleves_accueil

`@type_user = eleve`

**Comment puis-je t'aider ?**

******

Je suis ravi de pouvoir discuter avec toi. 
Laisse toi guider par les questions qui s'affichent ci-dessous ou écris directement ta question en bas de cette page.

Ma question concerne...

1. [...PIX](eleves_pix)
2. [...Néo](eleves_neo)
3. [...le brevet](dnb)
4. [...l'ASSR](assr)
5. [...les tablettes ou ordinateurs](eleves_emi)
6. [Aide moi à faire mon sac !](eleves_mon_cartable)

## profs_accueil

`@type_user = profs`

**Comment puis-je t'aider ?**

*****

Laisse toi guider par les questions qui s'affichent ci-dessous ou écris ta question directement en bas de cette page.

Ma question concerne...

1. [...le numérique](profs_numerique)
2. [Je veux contacter l'établissement](contact)

## responsables_accueil

`@type_user = parent`

**Comment puis-je vous aider ?**

*****

Je suis ravi de pouvoir discuter avec vous.
Laissez-vous guider par les questions qui s'affichent ci-dessous ou écrivez directement votre question en bas de cette page.

Ma question concerne...

1. [...Néo](responsables_neo)
2. [...le brevet](dnb)
3. [...l'ASSR](assr)
4. [Je veux aider mon enfant à faire son cartable !](eleves_mon_cartable)
5. [Je veux contacter l'établissement](contact)

## exterieurs_accueil

`@type_user = exterieur`

**Comment puis-je vous aider ?**

*****

Je suis ravi de pouvoir discuter avec vous.

1. [Je veux contacter l'établissement](contact)

## profs_numerique

`if @type_user==profs` 

:computer: **J'ai des questions concernant les outils numériques utilisés au collège.** :desktop_computer: 

*****

Pour lequel as-tu besoin d'aide ?

1. [PIX](profs_pix)
2. [Les outils numériques au collège VVG] (profs_num)


`endif`