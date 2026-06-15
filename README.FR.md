<p align="center"><img width="210" height="164" alt="dubformbanner" src="https://github.com/user-attachments/assets/33318e27-2958-4e98-a061-d375c6bdd379" /></p>

**_<p align="center">Sampler 12-bit & Tape Delay Dub Techno.</p>_**

---

![Version](https://img.shields.io/badge/Version-1.1.0-brightgreen?style=flat-square)
![macOS Support](https://img.shields.io/badge/macOS-Sonoma%20%7C%20Sequoia%20%7C%20Tahoe-000000?style=flat-square&logo=apple&logoColor=white)
![Architecture](https://img.shields.io/badge/Architecture-Universal-black?labelColor=606060&style=flat-square&logo=apple&logoColor=white)
![Format](https://img.shields.io/badge/Format-Standalone-00CED1?style=flat-square)
![DAW](https://img.shields.io/badge/DAW-Ableton%20Live%2012%2B-000000?style=flat-square&logo=abletonlive&logoColor=white)

---

<img width="996" height="788" alt="dubformpreview" src="https://github.com/user-attachments/assets/23bcf855-2c19-4dda-9864-75de009603ac" />

---

## 𝐅𝐨𝐧𝐜𝐭𝐢𝐨𝐧𝐧𝐚𝐥𝐢𝐭é𝐬

- **Sampler à résolution variable** : Réduit la résolution en bits du signal entrant de 16 bits jusqu'à 2, introduisant du bruit de quantification numérique, du crunch et la texture caractéristique des samplers vintage et du hardware numérique d'époque.
- **Sous-échantillonnage Clock Rate** : Diminue la fréquence d'échantillonnage effective de 44.1 kHz jusqu'à 6 kHz, produisant des artefacts d'aliasing et le caractère lo-fi granuleux associé au SP-1200 et au hardware Akai classique.
- **Filter Multi-Mode** : Un filtre biquad avec quatre modes: Lowpass, Bandpass, Highpass et Notch; avec contrôle de résonance et un étage de Drive à soft-clipping de style analogique. La compensation de gain est appliquée automatiquement pour éviter les sauts de volume lorsque le drive augmente.
- **Tape Echo** : Une unité de délai avec temps de délai et intensité de feedback ajustables, plus un LFO de Wow/Flutter qui module le temps de délai pour simuler l'instabilité de hauteur des machines à écho à bande vintage comme le Roland RE-201.
- **8 Presets Dub Techno** : Configurations nommées couvrant une gamme de traitements classiques du dub et de la dub techno, allant d'un écho spatial propre à des textures lo-fi lourdement dégradées.
- **Enregistrement de sortie en direct** : Capture la sortie master traitée directement dans un fichier WAV stéréo 16 bits, horodaté et téléchargé automatiquement via le bouton **Record**.
- **VU Meter** : Appareil de mesure analogique de style vintage avec simulation balistique mécanique; attaque rapide, relâchement pondéré; pour surveiller les niveaux de sortie.
- **Waveform Display** : Représentation visuelle de l'audio chargé avec une tête de lecture en temps réel. Cliquez ou faites glisser pour naviguer vers n'importe quelle position dans le sample.
- **Utilisation hors ligne** : Tous les traitements s'exécutent localement. Aucune connexion réseau n'est requise pendant l'utilisation.

---

## 𝐂𝐨𝐧𝐟𝐢𝐠𝐮𝐫𝐚𝐭𝐢𝐨𝐧 𝐑𝐞𝐪𝐮𝐢𝐬𝐞

- **macOS** : 14.0 (Sonoma), 15.0 (Sequoia) ou 16.0 (Tahoe)
- **Architecture** : Intel (x64), Apple Silicon (Arm64) ou Universal (U2B)
- **RAM** : 256 MB minimum
- **DAW (mode Plugin)** : Ableton Live 12 ou 11, Logic Pro, Reason avec le pilote audio virtuel [BlackHole](https://github.com/ExistentialAudio/BlackHole) pour le routage DAW en mode standalone.
> Les formats de plugins Audio Unit (AU) & VST3 sont actuellement en cours de développement.

---

## 𝐈𝐧𝐬𝐭𝐚𝐥𝐥𝐚𝐭𝐢𝐨𝐧

### 𝐒𝐭𝐚𝐧𝐝𝐚𝐥𝐨𝐧𝐞

1. Téléchargez la dernière version de [`Dub Stabs`](https://github.com/KouseiMusic/Dubform/releases/download/Dubform_1.1.0/Dubform.1.1.0.macOS.Universal.zip).
2. Extrayez et glissez `Dub Stabs` vers votre dossier `Applications`.
3. Si macOS affiche un avertissement Gatekeeper au premier lancement, faites un clic droit sur l'application et choisissez `Ouvrir`, puis confirmez.

### 𝐀𝐮𝐝𝐢𝐨 𝐔𝐧𝐢𝐭 (𝐀𝐔)

> 𝐄𝐧 𝐜𝐨𝐮𝐫𝐬 𝐝𝐞 𝐝é𝐯𝐞𝐥𝐨𝐩𝐩𝐞𝐦𝐞𝐧𝐭

### 𝐕𝐒𝐓𝟑

> 𝐄𝐧 𝐜𝐨𝐮𝐫𝐬 𝐝𝐞 𝐝é𝐯𝐞𝐥𝐨𝐩𝐩𝐞𝐦𝐞𝐧𝐭

## 𝐔𝐭𝐢𝐥𝐢𝐬𝐚𝐭𝐢𝐨𝐧 𝐞𝐧 𝐃𝐀𝐖

1. Installez [`BlackHole`](https://github.com/ExistentialAudio/BlackHole), un pilote audio virtuel gratuit pour macOS.
2. Ouvrez `Configuration audio et MIDI` (dans `/Applications/Utilitaires/`).
3. Créez un `Appareil à sorties multiples` incluant votre `Interface Audio` et `BlackHole`.
4. Définissez cet `Appareil à sorties multiples` comme sortie système dans `Réglages Système` > `Son`.
5. Dans votre `DAW`, créez une piste d'entrée audio et réglez sa source d'entrée sur `BlackHole`.
6. Vous pouvez maintenant enregistrer ou surveiller la sortie de `Dubform` en temps réel.

---

## 𝐂𝐨𝐧𝐭𝐫ô𝐥𝐞𝐬

### 𝐒𝐚𝐦𝐩𝐥𝐞𝐫

La section sampler dégrade l'audio entrant pour simuler le hardware numérique vintage. Les deux contrôles affectent directement le moteur de lecture et se mettent à jour en temps réel.

| Contrôle | Description | Plage |
| :--- | :--- | :--- |
| **Bit Depth** | Réduit la résolution du signal audio. Les valeurs basses introduisent un bruit de quantification prononcé et un crunch texturé. Les valeurs au-dessus de 12 sont relativement propres ; en dessous de 8, la dégradation devient un élément de caractère fort. | 2 à 16 bit |
| **Clock** | Réduit la fréquence d'échantillonnage effective en ralentissant la lecture et en modifiant le pitch. Les valeurs basses produisent de l'aliasing, des artefacts et la texture distinctive des machines à faible vitesse d'horloge. 44.1 kHz est non traité ; 6 kHz correspond à la dégradation maximale. | 6 kHz à 44.1 kHz |

### 𝐅𝐢𝐥𝐭𝐞𝐫

| Contrôle | Description | Plage |
| :--- | :--- | :--- |
| **Cutoff** | La fréquence à laquelle le filtre commence à atténuer le signal. En mode Lowpass, cela coupe les hautes fréquences ; en Highpass, cela atténue les basses ; en Bandpass, cela isole une région fréquentielle autour de ce point. | 20 Hz à 20 000 Hz |
| **Resonance** | Booste le signal au niveau et autour de la fréquence de coupure, ajoutant de l'emphase et, à des réglages élevés, un sifflement ou une résonance caractéristique. La compensation de gain réduit le niveau global à mesure que la résonance augmente pour éviter les pics agressifs. | 0.0 à 1.0 |
| **Drive** | Pousse le signal à travers un waveshaper de type soft-clipping avant d'entrer dans le filtre. Ajoute de la saturation harmonique et une chaleur de style analogique. Une compensation de gain automatique est appliquée pour que le volume perçu reste constant. | 1x à 10x |
| **Mode** | Sélectionne la topologie du filtre. **LP** (Lowpass) laisse passer les fréquences sous le cutoff et est le mode le plus courant pour le filtrage sombre typique du dub. **BP** (Bandpass) isole une bande de fréquences. **HP** (Highpass) supprime les basses fréquences. **NOTCH** crée un creux étroit au cutoff, produisant un effet de balayage type phaser lorsqu'il est automatisé. | LP / BP / HP / NOTCH |

### 𝐄𝐜𝐡𝐨

La section echo modélise une unité de délai à bande.

| Contrôle | Description | Plage |
| :--- | :--- | :--- |
| **Rate** | Le temps entre le signal original et sa première répétition. Les temps courts (sous 200 ms) produisent un slap-back et un doublage rythmique. Les temps longs (400 ms et plus) produisent l'écho dub classique et des effets de nappe spatiale. | 0.01 s à 2.0 s |
| **Intensity** | Définit la quantité de signal retardé réinjectée dans l'entrée du délai, contrôlant le nombre de répétitions audibles. À des valeurs faibles, l'écho s'estompe rapidement ; à des valeurs élevées, il se maintient en une longue queue de sifflement. La valeur maximale (0.93) approche mais n'atteint jamais le feedback infini. | 0.0 à 0.93 |
| **Wow / Flutter** | Applique un LFO lent au temps de délai, simulant l'instabilité de hauteur causée par les irrégularités du moteur et les variations de vitesse de bande des machines analogiques. Ajoute de la chaleur et du mouvement. | 0.0 à 1.0 |

### 𝐆𝐥𝐨𝐛𝐚𝐥 𝐂𝐨𝐧𝐭𝐫𝐨𝐥𝐬

| Contrôle | Description |
| :--- | :--- |
| **Load** | Ouvre une boîte de dialogue pour sélectionner et charger un fichier audio. La lecture commence automatiquement une fois le fichier décodé. |
| **Presets** | Menu déroulant avec 8 configurations couvrant une gamme d'approches de traitement dub et dub techno. La sélection d'un preset applique tous les paramètres simultanément avec une brève transition fluide pour éviter les clics. |
| **Volume** | Gain de sortie master, contrôlant le niveau du signal final. Le réglage par défaut est 80%. Les valeurs supérieures à 100% offrent un gain supplémentaire pour les sources plus calmes. |
| **Record** | Démarre et arrête l'enregistrement en direct de la sortie master. Une fois arrêté, l'audio capturé est écrit dans un fichier WAV stéréo 16 bits et téléchargé automatiquement. Le nom du fichier inclut la date et l'heure. |
| **Play** | Lance la lecture du sample chargé à partir de la position actuelle de la tête de lecture. |
| **Pause** | Interrompt la lecture et maintient la tête de lecture à sa position actuelle. Appuyer sur Play reprend la lecture là où elle s'était arrêtée. |
| **Stop** | Arrête la lecture et ramène la tête de lecture au début du sample. |
| **Waveform** | Le panneau waveform en bas de l'interface affiche l'audio chargé. Cliquez n'importe où sur le panneau pour sauter à cette position ou cliquez et faites glisser pour naviguer dans le sample en temps réel. |

---

## 𝐏𝐫𝐞𝐬𝐞𝐭𝐬

| Preset | Caractère |
| :--- | :--- |
| **Classic Dub** | Dégradation 12-bit chaleureuse, écho court avec feedback modéré. Évoque le traitement classique Roland Space Echo des productions dub jamaïcaines. |
| **Deepchord Space** | Signal 16-bit propre, long délai sombre, filtrage lowpass profond. Caractéristique des textures vastes et océaniques de la dub techno de Détroit du milieu des années 2000. |
| **Submerged** | Écrasement 8-bit lourd et faible fréquence d'horloge, filtre profond sous 100 Hz, délai moyen. Dense et claustrophobique. |
| **Resonant Drift** | Signal 12-bit à travers un filtre bandpass avec résonance contrôlée. La bande de fréquence étroite et l'écho dérivant produisent une texture hypnotique et cyclique. |
| **Infinite Wash** | Source 16-bit propre à travers un lowpass brillant avec un feedback élevé. Crée une nappe ambiante qui monte lentement. Le feedback est maintenu juste en dessous du seuil d'auto-oscillation. |
| **Basic Channel** | Signal 12-bit, lowpass serré, délai moyen avec feedback soutenu. Référence l'esthétique minimale et épurée de Maurizio et des premières sorties Basic Channel. |
| **Night Drive** | Signal 24-bit propre à travers un filtre doux avec un écho court et discret. Transparent — utile comme point de départ ou pour un traitement subtil. |
| **Echospace Tape** | Dégradation 10-bit, lowpass medium, long écho à bande avec wow/flutter prononcé. Lourd et usé, référençant l'esthétique de bande saturée des labels Echospace et Intrusion. |

---

## 𝐄𝐧𝐫𝐞𝐠𝐢𝐬𝐭𝐫𝐞𝐦𝐞𝐧𝐭

Appuyez sur le bouton `Rec` pour commencer la capture audio. Appuyez de nouveau pour l'arrêter. Un fichier `.wav` est exporté automatiquement et nommé en utilisant l'abréviation du preset actif ainsi que la date et l'heure actuelles (ex: `dubform_260609143022.wav`). L'enregistrement capture l'intégralité du signal traité, incluant le délai, la réverbération et le limiteur master.

---

## 𝐂𝐡𝐚î𝐧𝐞 𝐝𝐞 𝐒𝐢𝐠𝐧𝐚𝐥

```
┌─────────────────────────────────────────────────────────────────────────┐
│                           DUBFORM SIGNAL PATH                           │
└─────────────────────────────────────────────────────────────────────────┘

  AUDIO FILE
  (WAV / AIFF / MP3 / AAC / FLAC)
       │
       ▼
┌─────────────┐
│   SAMPLER   │  Bit Depth (2–16 bit) - reduces resolution / adds crunch
│             │  Clock Rate (6–44.1kHz) - slows the clock / adds aliasing
└──────┬──────┘
       │
       ▼
┌─────────────┐
│    DRIVE    │  Soft-clipping saturation stage before the filter.
│ (pre-filter │  Pushes the signal into harmonic warmth without hard
│ saturation) │  Distortion. Gain compensation applied automatically.
└──────┬──────┘
       │
       ▼
┌─────────────┐
│   FILTER    │  Mode: LP / BP / HP / NOTCH
│             │  Cutoff (20 Hz - 20 kHz) - sets the Frequency point.
│             │  Resonance (0.0 - 1.0) - emphasises the Cutoff peak.
└──────┬──────┘
       │
       ├──────────────────────────────────────┐
       │                                      │
       ▼                                      ▼
  (Dry Path)                        ┌─────────────────────────────────┐
       │                            │     TAPE ECHO                   │
       │                            │  Rate (delay time)              │
       │                            │  Intensity (feedback, max 0.93) │
       │                            │ Wow/Flutter (tape pitch wobble) │
       │                            │        ┌────────────────────────┘
       │                            │        │
       │                            │        │
       │                            │    ┌───┴────┐
       │                            │    │FEEDBACK│ ◄── Self-Loop
       │                            │    │  LOOP  │    (Hard-Limited
       │                            └────┤        │     below 1.0)
       │                                 └───┬────┘
       │                                     │
       ▼                                     ▼
┌─────────────────────────────────────────────────┐
│                  MASTER OUTPUT                  │
│              Volume (0-200%)                    │
└───────────────────────┬─────────────────────────┘
                        │
           ┌────────────┼──────────────┐
           ▼            ▼              ▼
     AUDIO OUTPUT   VU METER       RECORDER
                 
```

---

_Ce logiciel est gratuit. Si vous le trouvez utile, une ⭐️ sur GitHub aiderait d'autres personnes à le découvrir._

---

<p align="center"><code>Kousei</code></p>
<p align="center">2026</p>
