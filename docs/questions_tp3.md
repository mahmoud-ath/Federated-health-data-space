## TP 3 — Réponses aux 7 questions

1. **Quelles données le laboratoire reçoit-il dans le TP 2 ? Et dans le TP 3 ?**

   Dans le TP 2, le laboratoire reçoit les données brutes : concentrations PM2.5 et admissions hospitalières. Dans le TP 3, il reçoit uniquement les catégories de pollution et les statistiques agrégées.

2. **Pourquoi l'hôpital effectue-t-il les calculs dans son propre environnement ?**

   Pour conserver la maîtrise de ses données et éviter de transférer les admissions individuelles vers le laboratoire.

3. **Quelles informations sont encore transmises à l'hôpital ?**

   Les dates et les catégories de pollution (`elevee` et `non_elevee`), envoyées par le laboratoire au format JSON.

4. **Une statistique agrégée garantit-elle toujours la confidentialité ?**

   Non. L'attaque par différence montre qu'une demande portant sur un seul jour peut révéler le nombre exact d'admissions.

5. **Une clé API suffit-elle pour garantir la souveraineté des données ?**

   Non. Elle contrôle l'accès, mais ne garantit pas la souveraineté. Il faut également des règles de gouvernance, des autorisations et un contrôle de l'utilisation des données.

6. **Comment limiter les demandes d'analyse aux opérations autorisées ?**

   En définissant des règles d'accès, des opérations autorisées, un nombre minimal d'observations et des limites sur les requêtes.

7. **Quels composants supplémentaires faut-il pour un véritable espace de données ?**

   Un catalogue de données, une gestion des identités et des accès, des contrats d'utilisation, une traçabilité des échanges et des mécanismes de sécurité et de gouvernance.