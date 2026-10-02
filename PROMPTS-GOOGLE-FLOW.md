# FoxAir — Vidéo de mise en service · Prompts Google Flow / Veo

**Durée totale :** séquence 1 de 10 s + 6 séquences de 8 s = 58 s (montage final 45–60 s)
**Mode Flow recommandé :** *Frames to Video* (image de départ + image de fin quand indiqué). C'est le seul moyen fiable de garder la machine identique : Veo anime la photo au lieu de la réinventer.
**Format :** 16:9, 1080p. Prompts en anglais (Veo les suit mieux).

---

## 0. Ce que j'ai constaté sur les photos (à lire avant)

| Constat | Conséquence |
|---|---|
| **La machine n'est pas dans un carton** : elle est livrée **sous film étirable transparent**, avec des **panneaux blancs de protection** devant les pads arrière (photos 4, 9). | Le déballage = retrait du film, pas ouverture de carton. Je l'ai écrit ainsi. |
| Les « isolants arrière » sont en réalité les **pads d'évaporation verts en nid d'abeille** (photos 11, 14, 18, 30). | Leur rôle est **certain** grâce à votre schéma `schema-fonctionnement-evaporation` : l'eau ruisselle sur les pads, l'air chaud les traverse et ressort refroidi par le ventilateur. |
| Raccordement eau : platine inox avec **2 raccords laiton**, celui de gauche avec une **vanne à boisseau à poignée jaune**, 2 pictos bleus au-dessus (photo 29). Tuyau jaune branché sur l'un d'eux (photos 13, 14). | **Je ne sais pas lequel est l'arrivée d'eau et lequel est le trop-plein/vidange.** Les pictos ne sont pas lisibles. → voir « Infos manquantes ». |
| Bouchon de vidange blanc sous l'arrière, au centre (photo 28). | Non utilisé dans la vidéo (pas demandé), mais disponible. |
| Écran tactile : séquence de démarrage réelle visible : `Init. : Vanne position bypass` → `Init. : Amorçage de la pompe` → `Système Ok` (photos 19, 26, 27). Interface : ventilateur (10 / 100), goutte d'eau (0 / 20), Manu/Auto, 20.0 °C, bouton power. | On peut montrer la mise sous tension **sans rien inventer** en enchaînant ces vraies captures. |
| Câble d'alimentation noir sort en bas du flanc côté commandes (photos 21, 23). | Pas de photo de la prise ni d'un interrupteur général → on ne montre pas le branchement électrique. |

### Correspondance numéros ↔ fichiers
| # | Fichier | Contenu |
|---|---|---|
| 1 | 01-emballee-face-avant.jpg | Face avant sous film |
| 3 | 03-emballee-profil.jpg | Profil sous film |
| 9 | 09-emballee-arriere-panneau-blanc.jpg | Arrière sous film + panneau blanc |
| 10 | 10-emballee-base-roues.jpg | Base + roues sous film |
| 11 | 11-deballee-arriere-pads-evaporation.jpg | Arrière déballé, pads verts, face |
| 12 | 12-deballee-flanc-raccords-eau.jpg | Flanc côté raccords eau, sans tuyau |
| 13 | 13-deballee-trois-quart-tuyau-eau-branche.jpg | ¾ avant + tuyau jaune branché |
| 14 | 14-deballee-arriere-pads-tuyau-eau.jpg | ¾ arrière, pads + raccord + tuyau |
| 15 | 15-deballee-face-avant.jpg | Face avant déballée, tuyau jaune |
| 16 | 16-ecran-logo-foxair.jpg | Écran logo FoxAir |
| 17 | 17-ecran-eteint.jpg | Écran éteint |
| 18 | 18-deballee-arriere-pads-flanc-commandes.jpg | ¾ arrière côté commandes + pads |
| 20 | 20-deballee-trois-quart-avant-commandes.jpg | ¾ avant côté commandes |
| 21 | 21-deballee-flanc-commandes.jpg | Flanc commandes complet |
| 22 | 22-deballee-haut-ventilateur.jpg | Haut du ventilateur |
| 23 | 23-arret-urgence.jpg | Arrêt d'urgence |
| 25 | 25-ecran-interface-complete.jpg | Écran interface complète |
| 26 | 26-ecran-amorcage-pompe.jpg | Écran « Amorçage de la pompe » |
| 27 | 27-ecran-systeme-ok.jpg | Écran « Système Ok » |
| 29 | 29-raccords-eau-gros-plan.jpg | Gros plan raccords eau |
| 30 | 30-pads-evaporation-haut-rampe.jpg | Haut des pads + rampe |

---

## Bloc de cohérence (déjà intégré dans chaque prompt)
> Exact same FoxAir evaporative air cooler as in the reference image: matte warm-grey rotomoulded plastic body with deep rectangular ribbed recesses, large black round fan grille with four black brackets on the front, blue FoxAir badge below the fan, black swivel casters and black side handles. Do not alter shape, proportions, colors, components or labels.

**Negative prompt commun** (à ajouter à chaque scène) :
`text overlay, subtitles, captions, titles, watermark, logo animation, extra buttons, extra components, redesigned machine, different color, glossy plastic, chrome, neon, glow, particles, sparks, smoke, lens flare, sci-fi, futuristic HUD, hologram, CGI look, cartoon, warped geometry, melting shapes, morphing, flicker, distorted text, gibberish text, extra fingers, deformed hands, people's faces, fast camera, shaky handheld, whip pan, dutch angle`

---

## SÉQUENCE 1 — TOUR À 360° DE LA MACHINE EMBALLÉE, PUIS DÉBALLAGE
- **Durée :** 10 s (0–7 s : tour complet à 360° ; 7–10 s : début du déballage)
- **Références :** mode Flow **« Ingredients to Video »** (jusqu'à 3 images) pour que Veo connaisse toutes les faces :
  1. `01-emballee-face-avant.jpg` (face avant)
  2. `05-emballee-flanc-commandes.jpg` (flanc côté écran / arrêt d'urgence)
  3. `09-emballee-arriere-panneau-blanc.jpg` (arrière avec panneau blanc)
  Appui si besoin de remplacer une image : `03-emballee-profil.jpg` (flanc côté raccords), `10-emballee-base-roues.jpg`.
- **À l'image :** la machine reste immobile, filmée sous son film étirable. La caméra en fait le tour complet : face avant → flanc côté commandes → arrière avec panneau blanc → flanc côté raccords → retour face avant. Une fois revenue face avant, deux mains gantées entrent dans le champ, tranchent le film au cutter et commencent à le dérouler.
- **Caméra :** orbite à 360° lente, constante, à hauteur de poitrine, distance fixe, puis arrêt en face avant avec un léger dolly-in.
- **Éléments :** la machine ne bouge pas. Pendant le tour, rien ne bouge. Dans les 3 dernières secondes, seuls le film et les mains bougent.
- **Transition :** ouverture, fondu depuis le noir au montage. La séquence 2 reprend sur la machine déballée en face avant (`15-deballee-face-avant.jpg`).

> ⚠️ **Risque Veo :** un 360° est le mouvement le plus difficile pour garder la machine identique. Les faces non fournies en référence (flanc côté raccords) risquent d'être inventées. Générez 3 à 4 variantes. Si le résultat dérive, découpez en 2 plans : **1a** = tour à 360° seul (8 s), **1b** = déballage seul avec l'ancien prompt (départ `01-emballee-face-avant.jpg`).

**Prompt :**
```
Photorealistic industrial product video, 16:9, 10 seconds. A large FoxAir evaporative air cooler stands perfectly still on its black casters in the middle of a clean bright warehouse with a corrugated metal roof and pale concrete floor, fully wrapped in clear plastic stretch film exactly as in the reference images. Seconds 0 to 7: the camera performs one slow, smooth, continuous 360-degree orbit around the wrapped machine at chest height and constant distance, starting on the front with the large round black fan grille visible under the film, passing the side with the small control panel and red emergency stop, then the rear with the large white protective panel under the film, then the opposite side, and returning exactly to the front view. Seconds 7 to 10: the camera stops on the front view with a very slow subtle dolly-in; two gloved hands enter from the right, a utility knife cleanly slits the stretch film vertically along the side edge, and the hands begin peeling the transparent film away from the front. Only arms and gloves visible, no faces. The machine never moves or changes. Soft natural daylight from roof skylights, neutral white balance, realistic reflections on the plastic film, crisp detail, gimbal-stabilized motion, premium industrial commercial look, 35mm lens. Exact same machine as in the reference images on every side: do not alter shape, proportions, colors, components or labels. No text on screen.
```
**À éviter (spécifique) :** `cardboard box, carton, machine rotating on itself, turntable, machine moving or rolling, inconsistent sides, extra fan on the back, missing white rear panel, camera speeding up, jerky orbit, plastic flying in the air, film turning into smoke, fan spinning` + negative commun.

---

## SÉQUENCE 2 — INSTALLATION (version corrigée)
- **Durée :** 8 s
- **Pourquoi la version précédente ratait :** (1) elle donnait à Veo une seule image et lui demandait de faire rouler la machine et de tourner autour, donc il devait **inventer** les côtés et redessinait la machine ; (2) le prompt redécrivait la machine en détail, et Veo s'en sert pour en fabriquer une nouvelle au lieu de garder la photo ; (3) rien ne fixait la taille.
- **Correctifs :**
  1. Mode Flow **« Frames to Video »** avec **image de départ ET image de fin réelles** : Veo n'a plus qu'à interpoler entre deux vraies photos.
     - Départ : `15-deballee-face-avant.jpg`
     - Fin : `20-deballee-trois-quart-avant-commandes.jpg`
  2. **Plus de machine qui roule.** Seule la caméra bouge (le déplacement sur roulettes est ce qui déformait le plus).
  3. **Prompt court**, qui décrit le mouvement et l'échelle, pas le design (le design vient des photos).
  4. **Échelle donnée par le décor :** la machine dépasse nettement le garde-corps de la mezzanine visible derrière elle (photo 15).
- **À l'image :** la machine déballée, immobile. La caméra passe lentement de la face avant au ¾ avant côté commandes.
- **Caméra :** arc lent d'environ 35°, hauteur et distance constantes.
- **Transition :** la séquence 1 se termine face avant pendant le déballage → la 2 démarre face avant, machine nue.

> ⚠️ **Infos manquantes :**
> - **Dimensions réelles** (hauteur × largeur × profondeur) : elles ne figurent sur aucune photo. Donnez-les-moi et je les ajoute au prompt (ex. *« about 1.8 m tall »*), ça aide Veo à garder l'échelle.
> - Sur `15-deballee-face-avant.jpg`, le **tuyau jaune est déjà branché** et un câble est au sol. Je n'ai aucune photo de la machine déballée **sans** tuyau. Si ça vous gêne dans l'ordre du récit (l'eau est branchée en séquence 3), il faut une photo de la face avant sans tuyau.

**Prompt :**
```
Slow cinematic camera move around the exact machine shown in the start frame, ending exactly on the end frame. The machine is completely static and keeps its exact real size, shape, proportions, colors and every detail from the two reference photos; it is a large floor-standing unit, clearly taller than the mezzanine safety railing behind it. Camera: smooth gimbal-stabilized arc of about 35 degrees from the straight front view to the three-quarter front view of the control side, constant height and distance, steady speed. The fan does not spin. Keep the same warehouse, same daylight and same floor as the photos. Photorealistic, industrial commercial look. No text on screen.
```
**À éviter :** `new machine design, redesigned body, smaller machine, miniature, desk fan, different fan grille, extra handles, extra wheels, wheels changing number, machine moving, rolling, sliding, floating, wobbling, warping, morphing between frames, fan spinning, different background, people` + negative commun.

**Si le résultat dérive encore :** passez à un simple **dolly-in frontal** (départ et fin = `15-deballee-face-avant.jpg`, prompt : *« Very slow straight push-in toward the static machine, nothing else moves »*). C'est le mouvement le plus fidèle possible avec Veo.

---

## SÉQUENCE 3 — RACCORDEMENT À L'EAU
- **Durée :** 8 s
- **Références :** départ = photo **29** (gros plan raccords). Fin (optionnelle) = photo **13** ou **14** (tuyau jaune branché). Appui : 12.
- **À l'image :** gros plan de la platine inox aux 2 raccords laiton. Une main amène le tuyau d'arrosage jaune, l'emboîte sur le raccord, puis tourne la poignée jaune de la vanne d'un quart de tour pour l'ouvrir.
- **Caméra :** macro, léger glissement latéral + léger dolly-in vers les raccords.
- **Éléments :** tuyau jaune, main, poignée jaune (¼ de tour).
- **Transition :** cut sur le flanc — on passe du plan large ¾ (fin séq. 2) au gros plan du raccord, même côté de la machine.

> ⚠️ **Info manquante bloquante :** sur les photos 13/14 le tuyau est branché sur le raccord **avec** la vanne jaune, mais je ne peux pas confirmer que c'est l'arrivée d'eau, ni le type d'embout (raccord rapide type Gardena ? filetage ?), ni la pression requise. Le prompt ci-dessous reproduit **exactement ce que montrent les photos 13/14** (tuyau sur le raccord à vanne). Si c'est faux, dites-le-moi.

**Prompt :**
```
Photorealistic industrial macro product video, 16:9. Close-up of the lower side panel of the FoxAir evaporative air cooler, exactly as in the reference image: a small brushed stainless steel plate with two blue pictograms, below it two brass hose fittings, the left one with a yellow lever ball valve. A gloved hand brings in a flexible yellow garden hose with its connector and pushes it firmly onto the RIGHT brass fitting, the plain one without a valve. The left fitting with the yellow valve is not touched. Precise, calm, instructional movement. Camera: macro lens, slow lateral slide combined with a gentle push-in toward the fittings, shallow depth of field, focus locked on the brass fittings. Soft even studio-like light, realistic metal reflections on brass and stainless steel, matte warm-grey plastic texture. Exact same panel, fittings and valve as in the reference image: do not add, remove or move any component. No text on screen.
```
**À éviter :** `water spraying, leaking water, splashes, extra fittings, third valve, red valve, copper pipe, plumbing tools, wrench, valve changing color, hose on the left fitting, hose on the yellow valve, hand touching the yellow valve, readable fake text on the plate` + commun.

---

## SÉQUENCE 4 — ARRIÈRE : PADS D'ÉVAPORATION
- **Durée :** 8 s
- **Références :** départ = photo **9** (arrière sous film + panneau blanc) **ou**, plus sûr, photo **11** (pads à nu). Appui : 30, 14, 18. Schéma de fonctionnement pour le rôle.
- **À l'image :** l'arrière de la machine : le grand cadre gris et les pads verts en nid d'abeille. Option A : une main retire le panneau blanc de protection et découvre les pads. Option B (recommandée, moins risquée) : simple révélation lente des pads.
- **Rôle (certain, d'après votre schéma) :** l'eau humidifie les pads, l'air chaud aspiré les traverse et se refroidit par évaporation. → à mettre **en texte au montage**, pas dans la vidéo.
- **Caméra :** travelling vertical lent de bas en haut le long des pads jusqu'à la rampe métallique supérieure (photo 30), puis léger recul.
- **Éléments :** aucun (ou panneau blanc retiré en option A). Pas d'eau visible : je n'ai pas de photo des pads mouillés.
- **Transition :** le tuyau jaune de la séq. 3 est visible au sol au premier plan (comme photo 14), ce qui relie les deux plans.

**Prompt (option B) :**
```
Photorealistic industrial product video, 16:9. Rear view of the FoxAir evaporative air cooler, exactly as in the reference image: a large rectangular warm-grey rotomoulded plastic frame holding wide green honeycomb cellulose evaporative cooling pads, made of three vertical panels, topped by a horizontal brushed metal water distribution rail with small bolts, and a row of rectangular recesses along the base. A yellow garden hose lies on the floor in the foreground. Camera: slow vertical crane-up starting low at the base, gliding upward along the textured green honeycomb pads to the metal rail at the top, then a gentle pull-back to reveal the whole rear face. Soft natural daylight from roof skylights grazing the pad texture to show the fine wave pattern, crisp detail, premium industrial commercial look. Pads stay dry and still. Exact same machine as in the reference image: do not alter shape, proportions, colors, components or labels. No text on screen.
```
**À éviter :** `water flowing, dripping, blue glowing water, animated airflow arrows, mist, steam, pads changing color, brown pads, different pad pattern, pads moving, frame deforming` + commun.

---

## SÉQUENCE 5 — ARRÊT D'URGENCE
- **Durée :** 8 s
- **Références :** départ = photo **23** (bouton seul). Appui : 21 (position sur le flanc).
- **À l'image :** la platine grise vissée (4 vis) avec le bouton coup-de-poing rouge sur collerette jaune « EMERGENCY ». On l'identifie clairement. Aucune pression sur le bouton (on ne déclenche pas d'arrêt en pleine mise en service).
- **Caméra :** dolly-in lent et très léger arc de 10°, finissant en plan rapproché centré, le bouton net.
- **Éléments :** aucun.
- **Transition :** coupe vers le flanc côté commandes — la séq. 4 finit sur l'arrière, on contourne vers la face latérale.

**Prompt :**
```
Photorealistic industrial close-up product video, 16:9. The emergency stop on the side of the FoxAir evaporative air cooler, exactly as in the reference image: a light grey square metal plate fixed with four black screws, set into a recess of the matte warm-grey rotomoulded plastic body, with a red mushroom-head emergency stop button on a yellow circular collar printed with the word EMERGENCY. Camera: slow smooth dolly-in with a very subtle 10-degree arc, ending on a centered close-up with the red button and yellow collar in sharp focus, background softly blurred. Soft directional studio light creating a gentle highlight on the red button dome. Nothing moves except the camera. Exact same button, collar, plate and screws as in the reference image; the printed word stays sharp and unchanged. No added text on screen.
```
**À éviter :** `button being pressed, hand, button glowing, light-up button, alarm light, rotating beacon, different button shape, square button, green button, misspelled EMERGENCY, extra labels` + commun.

---

## SÉQUENCE 6 — ÉCRAN DE CONTRÔLE & MISE SOUS TENSION
- **Durée :** 2 × 8 s possible, ou 1 × 8 s.
- **Références :** **6a** départ = photo **17** (écran éteint), fin = photo **16** (logo FoxAir). **6b** départ = photo **26** (« Amorçage de la pompe »), fin = photo **27** (« Système Ok »). Appui : 25, 19.
- **À l'image :** l'écran tactile s'allume sur le logo FoxAir (6a), puis l'interface réelle affiche l'initialisation et passe à « Système Ok » (6b).
- **Caméra :** dolly-in lent vers la platine, frontal, puis fixe.
- **Éléments :** uniquement le contenu de l'écran.
- **Transition :** l'écran est juste au-dessus de l'arrêt d'urgence sur le même flanc (photo 21) → léger tilt-up implicite entre 5 et 6.

> ⚠️ **Risque Veo :** la génération de texte d'écran est souvent illisible. **Conseil d'agence :** générer uniquement le mouvement caméra sur l'écran éteint (6a), puis **incruster au montage les vraies captures 16 → 19 → 26 → 27** sur l'écran (tracking 4 coins). C'est ce qui garantit des textes exacts. Je ne sais pas comment l'écran s'allume (interrupteur ? automatique au branchement ?) → on ne montre aucune main.

**Prompt 6a :**
```
Photorealistic industrial product video, 16:9. Close-up of the control panel on the side of the FoxAir evaporative air cooler, exactly as in the reference image: a light grey metal plate fixed with black screws around its edge, a black-framed rectangular touchscreen, and below it the green and blue FoxAir logo with the words evaporative technology. The screen is dark, then softly powers on and fades in to the FoxAir logo on a white background, exactly as in the end frame. Camera: slow frontal dolly-in toward the panel, perfectly stable, ending centered on the screen. Soft neutral light, realistic glass reflection on the screen. Exact same panel, logo and screws as in the reference image. No added text on screen.
```
**Prompt 6b :**
```
Photorealistic industrial product video, 16:9. Static frontal close-up of the FoxAir touchscreen exactly as in the reference image, showing the real interface: a green status bar at the top, temperature and humidity readings on the left, a fan icon and a water drop icon in two circles, a Manu/Auto toggle, a 20.0 °C setpoint and a power icon. The status bar changes from the pump priming message to the system OK message exactly as in the end frame, the water drop value rises smoothly. Camera: locked-off, almost imperceptible slow push-in. Soft neutral light. Keep every icon, number and layout identical to the reference images; no new interface elements. No added text on screen.
```
**À éviter :** `invented UI, new icons, menus sliding, holographic display, glowing screen edges, scrolling gibberish text, finger tapping, cursor, screen changing size, different logo` + commun.

---

## SÉQUENCE 7 — MISE EN SERVICE FINALE
- **Durée :** 8 s
- **Références :** départ = photo **20** (¾ avant côté commandes). Appui : 15, 22, 13.
- **À l'image :** la machine installée, tuyau jaune et câble branchés, ventilateur en rotation régulière. Plan héros.
- **Caméra :** orbite lente de 45° autour de la machine, légère montée de caméra, finit en ¾ avant héroïque. Plan de fin tenu 2 s (pour votre carton titre au montage).
- **Éléments :** **seulement les pales du ventilateur tournent**, régulièrement.
- **Transition :** depuis l'écran « Système Ok », recul / coupe sur le plan large → la machine démarre.

**Prompt :**
```
Photorealistic premium industrial hero shot, 16:9. The fully installed FoxAir evaporative air cooler, exactly as in the reference image, stands on its casters in a clean bright warehouse: matte warm-grey rotomoulded plastic body, large black round fan grille with four black brackets, blue FoxAir badge, side control panel with lit touchscreen and red emergency stop, yellow water hose and black power cable connected and lying neatly on the floor. The fan blades behind the grille spin at a steady realistic speed, nothing else moves. Camera: slow smooth 45-degree orbit from the front toward a three-quarter front view on the control side, with a subtle rise in height, ending on a stable heroic composition held for the last two seconds. Soft natural daylight from roof skylights, neutral tones, clean premium industrial commercial look, 35mm lens, high detail. Exact same machine as in the reference image: do not alter shape, proportions, colors, components or labels. No text on screen.
```
**À éviter :** `wind effects, flying papers, visible air streams, mist, cold vapor, blue tint, motion blur on body, grille rotating, fan spinning backwards or erratically, machine moving, people` + commun.

---

## Infos manquantes — à me fournir pour être 100 % fidèle
1. **Raccordement eau :** quel raccord est l'arrivée (celui à vanne jaune ?), à quoi sert l'autre (trop-plein ? vidange ?), type d'embout, pression/débit requis. Une photo nette des 2 pictos bleus suffirait.
2. **Électrique :** photo de la prise / du connecteur et indication de la tension (230 V mono ?). Y a-t-il un interrupteur général, ou l'écran s'allume-t-il au branchement ?
3. **Roulettes :** ont-elles un frein ?
4. **Pads en eau :** pas de photo des pads mouillés → je n'ai pas montré l'eau ruisseler. Une photo/vidéo de la machine en fonctionnement réel permettrait de l'ajouter.
5. **Panneaux blancs (photos 4, 9) :** confirmez qu'il s'agit bien de protections de transport à retirer.

## Conseils de montage
- Ordre des fichiers : 1 → 2 → 3 → 4 → 5 → 6a → 6b → 7 (≈ 56 s ; coupez 0,5–1 s en tête/queue de chaque plan pour descendre à ~50 s).
- Transitions : coupes franches ou fondus courts (6–8 images). Pas d'effets.
- Étalonnage : unifiez la balance des blancs (neutre, légèrement chaude) sur tous les plans.
- Générez 2–4 variantes par séquence et gardez celle où la machine dérive le moins de la photo.
