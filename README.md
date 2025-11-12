# TP React Débutant - Gestion de l'état et structuration des composants

Ce projet React démontre les concepts fondamentaux de la gestion d'état et de la structuration des composants React.

## 📋 Prérequis

- Node.js installé sur votre machine
- npm (généralement inclus avec Node.js)

## 🚀 Comment démarrer le projet

### Étape 1 : Ouvrir un terminal

Ouvrez votre terminal (Terminal sur Mac, PowerShell ou CMD sur Windows).

### Étape 2 : Aller dans le dossier du projet

```bash
cd tp-react-debutant
```

### Étape 3 : Démarrer le serveur de développement

```bash
npm start
```

**Note :** Si le port 3000 est déjà utilisé (par exemple par Grafana), vous pouvez utiliser un autre port :

```bash
PORT=3001 npm start
```

### Étape 4 : Ouvrir dans le navigateur

L'application s'ouvrira automatiquement dans votre navigateur à l'adresse :
- **http://localhost:3000** (par défaut)
- **http://localhost:3001** (si vous avez utilisé PORT=3001)

Si le navigateur ne s'ouvre pas automatiquement, copiez l'une de ces adresses dans votre navigateur.

## 🛑 Arrêter le serveur

Pour arrêter le serveur de développement, appuyez sur **Ctrl + C** dans le terminal.

## 📚 Ce que vous allez apprendre

Ce TP couvre les concepts suivants :

### 1. Formulaire Contrôlé (`FormulaireControle.js`)
- Utilisation de `useState` pour gérer l'état des champs
- Les valeurs sont contrôlées par React
- Chaque modification met à jour l'état immédiatement

### 2. Formulaire Non-Contrôlé (`FormulaireNonControle.js`)
- Utilisation de `useRef` pour accéder aux valeurs
- Les valeurs sont gérées par le DOM
- Accès aux valeurs uniquement lors de la soumission

### 3. Lifting State Up (`TemperatureInput.js` et `TemperatureConvertor.js`)
- Partage d'état entre composant parent et enfant
- Le parent gère l'état, l'enfant reçoit les props
- Communication via les fonctions de callback

### 4. Contexte React (`UtilisateurContext.js` et `Profil.js`)
- Partage de données globales sans passer par les props
- Utilisation de `createContext` et `useContext`
- Provider pour rendre les données disponibles partout

## 🎯 Structure du projet

```
src/
├── App.js                    # Composant principal avec Provider
├── FormulaireControle.js     # Formulaire contrôlé
├── FormulaireNonControle.js  # Formulaire non-contrôlé
├── TemperatureInput.js       # Composant enfant pour température
├── TemperatureConvertor.js   # Composant parent pour température
├── UtilisateurContext.js     # Contexte utilisateur
└── Profil.js                 # Composant utilisant le contexte
```

## 🧪 Tester l'application

Une fois l'application lancée, vous pouvez tester :

1. **Formulaire Contrôlé** : Saisissez un nom et un email, puis cliquez sur "Envoyer"
2. **Formulaire Non-Contrôlé** : Faites de même avec le deuxième formulaire
3. **Température** : Saisissez une température en degrés Celsius et voyez-la s'afficher
4. **Profil** : Cliquez sur "Se déconnecter" pour voir le changement d'état global

## 🔧 Commandes disponibles

Dans le dossier du projet, vous pouvez exécuter :

### `npm start`
Démarre le serveur de développement. La page se rechargera automatiquement quand vous modifiez le code.

### `npm test`
Lance le test runner en mode interactif.

### `npm run build`
Crée une version de production optimisée dans le dossier `build`.

## 📖 Ressources

- [Documentation React](https://reactjs.org/)
- [Create React App](https://create-react-app.dev/)

## 💡 Exercices supplémentaires (facultatifs)

Si vous voulez aller plus loin :

1. Ajoutez un formulaire d'inscription avec Nom, Email, Mot de passe
2. Créez un deuxième champ synchronisé pour convertir une température en Fahrenheit
3. Ajoutez un bouton pour reconnecter l'utilisateur dans le composant Profil

---

**Bon apprentissage ! 🎉**
