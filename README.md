# FPC Autos — Site Vitrine

**Maquette de démonstration** réalisée par Nexvia Digital  
Stack : HTML5 · Tailwind CSS (CDN) · JavaScript Vanilla

---

## Lancer le site localement

Le site est un fichier unique `index.html` — ouvrez-le directement dans votre navigateur.

**Méthode recommandée (serveur local) :**
```bash
# Python 3
cd /Users/ilocal/Desktop/FPC_AUTOS
python3 -m http.server 8080
# → ouvrir http://localhost:8080
```

Ou avec Node.js (si installé) :
```bash
npx serve .
```

---

## Publier en ligne (statique)

### Netlify Drop (le plus simple)
1. Allez sur [app.netlify.com/drop](https://app.netlify.com/drop)
2. Glissez-déposez le **dossier FPC_AUTOS** (contenant `index.html` + `images/`)
3. Le site est en ligne en quelques secondes

### Vercel
```bash
npm i -g vercel
cd /Users/ilocal/Desktop/FPC_AUTOS
vercel --name fpc-autos
```

---

## Structure du projet

```
FPC_AUTOS/
├── index.html                        ← site complet (une page)
├── images/
│   ├── 00_Logo_original_FPC_Autos.png
│   ├── 01_Photo_accueil_page_accueil.png
│   ├── 02_Photo_technicien_prestations.png
│   ├── 03_Photo_echange_client_accompagnement.png
│   ├── 04_Photo_exterieur_garage_centres.png
│   ├── 05_Photo_groupe_equipe.png
│   ├── 06_Portrait_illustratif_Fabrice.png
│   ├── 07_Portrait_illustratif_Karine.png
│   └── 09_Photo_controle_technique_atelier.png
└── README.md
```

---

## Comment personnaliser le site

### Remplacer une image
Remplacez simplement le fichier dans `images/` en conservant **exactement le même nom**.  
Exemple : remplacez `06_Portrait_illustratif_Fabrice.png` par le vrai portrait de Fabrice Pommier.

### Modifier les coordonnées (téléphone, email, horaires)
Dans `index.html`, cherchez les mentions :
- `Téléphone : à compléter`
- `Email : à compléter`
- `Horaires : à compléter`

Et remplacez-les par les vraies informations.

### Modifier les tarifs
Cherchez `85 €` et `55 €` dans le fichier HTML.

### Activer la réservation réelle
Le formulaire de rendez-vous est actuellement en mode simulation. Pour le connecter à un vrai système :
- Calendly, Doctolib, ou tout autre service de réservation
- API backend maison
- Remplacez la gestion du `submit` dans la section `// ── RDV form`

### Ajouter de vrais avis
La section `#avis` contient des exemples fictifs clairement étiquetés. Remplacez-les par de vraies citations de clients (avec leur accord écrit).

### Ouvrir le centre de Rezé
Quand l'ouverture est confirmée :
1. Retirez le badge « Ouverture à venir »
2. Ajoutez l'adresse définitive
3. Activez la réservation pour Rezé dans le formulaire

---

## Avant une publication commerciale réelle

- [ ] Remplacer toutes les photos illustratives par de vraies photos
- [ ] Ajouter les vrais portraits de Fabrice et Karine
- [ ] Compléter téléphone, email, horaires
- [ ] Ajouter des mentions légales conformes (RGPD, éditeur, hébergeur)
- [ ] Connecter le formulaire de rendez-vous à un vrai système
- [ ] Remplacer les avis fictifs par de vrais avis clients
- [ ] Vérifier les tarifs et activer/désactiver l'affichage selon la décision commerciale
- [ ] Supprimer les mentions « Maquette de démonstration »
