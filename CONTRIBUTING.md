# 🌍 Guide de Contribution - Wyrmcraft Core Lang

Bienvenue dans le dépôt de traduction de Wyrmcraft Core ! Ce guide vous explique comment contribuer correctement aux fichiers de langue.

## 📋 Structure du Projet

```
wyrmcraft-core-lang/
├── README.md
├── CONTRIBUTING.md
├── LICENSE
└── lang/
    ├── fr_FR.yml
    ├── en_US.yml
    ├── es_ES.yml
    └── ...
```

## ✅ Ce qu'il FAUT faire

### 1. **Respecter la structure et l'indentation**
- Conservez exactement la même structure YAML que le fichier original
- Gardez la même indentation (2 espaces par niveau)
- Préservez tous les commentaires (lignes commençant par `#`)

### 2. **Traduire uniquement les valeurs**
```yaml
# ✅ CORRECT
server_tpa_demande_envoyee: "Teleportation request sent to"

# ❌ INCORRECT - Ne jamais traduire les clés
server_tpa_request_sent: "Teleportation request sent to"
```

### 3. **Respecter le ton et le style du serveur**
- Maintenez un ton cohérent avec l'univers médiéval-fantastique de Wyrmcraft
- Utilisez un langage immersif et approprié au contexte RPG
- Conservez le niveau de formalité du texte original

### 4. **Préserver les séparations et commentaires**
```yaml
# > TPA >
  server_tpa_demande_envoyee: "..."
  
# > BACK >
  server_back_action_teleportation_en_cours: "..."
```

### 5. **Vérifier votre traduction**
- Relisez plusieurs fois votre traduction
- Testez si possible dans le jeu
- Demandez une relecture par un natif de la langue cible

## ❌ Ce qu'il ne FAUT PAS faire

### 1. **Ne JAMAIS inclure de codes couleur**
```yaml
# ❌ INCORRECT
server_tpa_demande_envoyee: "&aDemande de téléportation envoyée"

# ✅ CORRECT
server_tpa_demande_envoyee: "Demande de téléportation envoyée"
```
**Pourquoi ?** Les couleurs sont gérées automatiquement dans les fichiers de configuration du serveur.

### 2. **Ne PAS traduire les clés (keys)**
```yaml
# ❌ INCORRECT
serveur_tpa_demande_envoyee: "Teleportation request sent"

# ✅ CORRECT
server_tpa_demande_envoyee: "Teleportation request sent"
```
Les clés doivent rester identiques dans tous les fichiers de langue.

### 3. **Ne PAS utiliser de traductions automatiques sans vérification**
- Google Translate et autres outils automatiques produisent souvent des erreurs
- Vérifiez toujours le contexte et la cohérence
- Adaptez la traduction au style du serveur

### 4. **Ne PAS modifier l'indentation ou la structure**
```yaml
# ❌ INCORRECT
server_tpa_demande_envoyee:"Teleportation request sent"

# ✅ CORRECT
  server_tpa_demande_envoyee: "Teleportation request sent"
```

### 5. **Ne PAS supprimer ou ajouter des espaces inutiles**
```yaml
# ❌ INCORRECT
server_tpa_demande_envoyee:    "Teleportation request sent"   

# ✅ CORRECT
server_tpa_demande_envoyee: "Teleportation request sent"
```

## 🔤 Convention de Nommage des Fichiers

Utilisez le format standard de locale :
- `fr_FR.yml` (Français - France)
- `en_US.yml` (Anglais - États-Unis)
- `es_ES.yml` (Espagnol - Espagne)
- `de_DE.yml` (Allemand - Allemagne)
- `pt_BR.yml` (Portugais - Brésil)
- etc.

## 📝 Processus de Contribution

1. **Fork** le dépôt
2. **Créez** ou modifiez le fichier de langue approprié
3. **Suivez** toutes les règles ci-dessus
4. **Testez** votre traduction si possible
5. **Soumettez** une Pull Request avec une description claire

## 🎯 Exemple de Traduction Correcte

### Fichier original (fr_FR.yml)
```yaml
fr_fr:
# > TPA >
  server_tpa_demande_envoyee: "Demande de téléportation envoyée à"
  server_tpa_erreur_joueur_introuvable: "est introuvable."
```

### Traduction en anglais (en_US.yml)
```yaml
en_us:
# > TPA >
  server_tpa_demande_envoyee: "Teleportation request sent to"
  server_tpa_erreur_joueur_introuvable: "cannot be found."
```

## ⚠️ Points d'Attention

- Certains messages sont des fragments qui seront assemblés avec d'autres textes
- Respectez la ponctuation et les espaces en fin de phrase
- Les messages d'erreur doivent rester clairs et informatifs
- Les titres de PNJ doivent respecter l'univers médiéval-fantastique

## 📞 Questions ?

Si vous avez des questions sur la traduction ou des doutes sur une formulation, n'hésitez pas à ouvrir une Issue sur le dépôt.

---

**Merci de contribuer à Wyrmcraft Core ! 🐉**
