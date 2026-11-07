# 1. Où sont stockées les mesures de qualité de l'air ?

Elles sont stockées localement dans la base de données `environnement.db`, appartenant au laboratoire environnemental.

# 2. Où sont stockées les admissions hospitalières ?

Elles sont stockées localement dans la base de données `hopital.db`, appartenant à l'hôpital.

# 3. Les deux jeux de données sont-ils dans une même base ?

Non, ils sont stockés dans deux bases SQLite distinctes afin de préserver la séparation et l'autonomie des deux organisations.

# 4. Comment le laboratoire pourrait-il découvrir les données disponibles sans centraliser les fichiers ?

Grâce à un système fédéré qui permet de rechercher et de consulter les données disponibles auprès de chaque organisation, sans transférer ni centraliser leurs bases de données.