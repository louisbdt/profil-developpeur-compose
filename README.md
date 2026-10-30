# Profil développeur Compose

## Description
Cette application affiche une fiche de profil développeur sous forme de composants Jetpack Compose réutilisables : un en-tête (nom, rôle), une description, une liste de compétences, une information de contact et un bouton d’action. Les données affichées peuvent être modifiées en changeant simplement les paramètres passés aux composables, comme le montrent les deux previews

## Notions utilisées
- composables
- paramètres
- modifiers
- padding externe / interne
- callbacks
- previews

## Explication
1. **Quels composables avez-vous créés ?**
   ProfileHeader, SkillItem, ContactButton, ProfileCard, ProfileScreen
2. **Quel composable représente l'écran principal ?**
   ProfileScreen.
3. **Où utilisez-vous un padding externe ?**
   Dans ProfileScreen, sur le modifier donné à ProfileCard (padding(24.dp)).
4. **Où utilisez-vous un padding interne ?**
   Dans ProfileCard, sur la Column du contenu (padding(16.dp)).
5. **Quel composant reçoit un callback ?**
   ContactButton, via onClick.
6. **Quelle information d'accessibilité avez-vous ajoutée (ou pourquoi pas) ?**
   Aucune information personnalisée : la seule action est un Button Material, qui expose déjà son rôle de bouton par défaut.
7. **Pourquoi vos composants peuvent-ils être considérés comme réutilisables ?**
   Ils reçoivent leurs données et leur modifier en paramètres, au lieu de les coder en dur.

## Captures d'écran
![Previews](screenshot/previews.png)