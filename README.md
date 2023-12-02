
![image](https://user-images.githubusercontent.com/108534539/218347565-ebebee5e-3de3-427a-8370-cef5e44c3591.png)


Français:

L'empreinte en ligne de Digital Rogue Wave se fait principalement via son site web, que les clients consultent à l'aide de divers appareils tels que des ordinateurs portables, des téléphones mobiles et des tablettes.
Toutes les données de catalogue des produits sont stockées dans le serveur NoSQL MongoDB.
Toutes les données transactionnelles telles que l'inventaire et les ventes sont stockées dans le serveur de base de données MySQL.
Le serveur web de Digital Rogue Wave est entièrement alimenté par ces deux bases de données.
Les données sont extraites périodiquement de ces deux bases de données et placées dans l'entrepôt de données de pré-production fonctionnant sur PostgreSQL.
L'entrepôt de données de production est sur l'instance cloud du serveur IBM DB2.
Les équipes de BI se connectent au serveur IBM DB2 pour la création de tableaux de bord opérationnels. IBM Cognos Analytics est utilisé pour créer des tableaux de bord.
Digital Rogue Wave utilise un cluster Hadoop comme plateforme big data où toutes les données sont collectées à des fins d'analyse.
Spark est utilisé pour analyser les données sur le cluster Hadoop.
Pour déplacer les données entre OLTP, NoSQL et l'entrepôt de données, des pipelines ETL sont utilisés, et ceux-ci s'exécutent sur Apache Airflow.
Anglais:

Digital Rogue Wave's online presence is primarily through its website, which customers access using a variety of devices like laptops, mobiles, and tablets.
All product catalog data is stored in the MongoDB NoSQL server.
All transactional data like inventory and sales are stored in the MySQL database server.
Digital Rogue Wave's webserver is driven entirely by these two databases.
Data is periodically extracted from these two databases and put into the staging data warehouse running on PostgreSQL.
Production data warehouse is on the cloud instance of IBM DB2 server.
BI teams connect to the IBM DB2 for operational dashboard creation. IBM Cognos Analytics is used to create dashboards.
Digital Rogue Wave uses Hadoop cluster as its big data platform where all the data collected for analytics purposes.
Spark is used to analyze the data on the Hadoop cluster.
To move data between OLTP, NoSQL, and the data warehouse, ETL pipelines are used, and these run on Apache Airflow.
