## TP 4 — Réponses aux 7 questions

1. **Quelles informations permettent au laboratoire de découvrir et de comprendre le jeu de données ?**

   Les métadonnées du catalogue : identifiant, titre, description, organisation propriétaire, période couverte, unité de mesure et conditions d'accès.

2. **Qu'est-ce que DCAT et pourquoi le catalogue est-il une simplification inspirée de DCAT ?**

   DCAT est un vocabulaire standard permettant de décrire et de découvrir des jeux de données. Le catalogue du TP reprend certains de ses principes sans implémenter toutes ses fonctionnalités.

3. **Pourquoi contrôler la finalité avant d'autoriser l'accès ? Différence entre un catalogue, une politique d'usage et un contrôle d'accès.**

   Le contrôle de la finalité permet de vérifier que les données sont utilisées pour un objectif autorisé.
   - **Catalogue** : décrit les données disponibles.
   - **Politique d'usage** : définit les conditions d'utilisation des données.
   - **Contrôle d'accès** : vérifie et autorise ou refuse les demandes d'accès.

4. **Quelles informations circulent entre les trois nœuds ? Que reste-t-il dans la base hospitalière ? Pourquoi la conservation locale ne suffit-elle pas à garantir la confidentialité ?**

   Le catalogue, les demandes de contrat, les classifications signées et les statistiques agrégées circulent entre les organisations. Les admissions individuelles restent dans la base hospitalière.

   Cependant, la conservation locale ne garantit pas une confidentialité totale, car les classifications et les résultats statistiques transmis peuvent révéler certaines informations.

5. **Pourquoi ne pas publier une statistique calculée sur un groupe trop petit ? Pourquoi un seuil de trois jours n'est-il pas une preuve de k-anonymat ? Comment la signature limite-t-elle l'attaque du TP 3 ?**

   On masque les statistiques des petits groupes pour éviter de révéler des informations sensibles. Le seuil de 3 jours ne garantit pas le k-anonymat. La signature HMAC empêche la modification des classifications et bloque les requêtes falsifiées.

6. **Comparez les résultats avec et sans bruit. Expliquez le compromis précision / protection. Pourquoi ce code n'est-il pas une implémentation complète de confidentialité différentielle ?**

   Sans bruit, les résultats sont plus précis, mais moins confidentiels. Avec bruit, la protection augmente au détriment de la précision. Le code est une simulation pédagogique, car la gestion du bruit et du budget de confidentialité est simplifiée.

7. **La différence observée permet-elle de conclure que la pollution provoque les admissions ? Quelles variables faudrait-il considérer ?**

   Non, la différence observée ne prouve pas que la pollution provoque les admissions. Il faut considérer d'autres variables : température, humidité, âge, tabagisme, maladies préexistantes et infections respiratoires.