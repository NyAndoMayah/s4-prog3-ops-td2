# s4-prog3-ops-td2

Stack de stockage
Dans ce premier exercice, vous allez créer des ressources de stockage, en suivant les instructions suivantes :
Créer une instance RDS de type postgres

Choisissez la plus petite instance de base de données, et le minimum possible pour les configurations. Pour l’identifiant et le mot de passe pour les accès à la base de données, stockez les dans SSM Parameter Store et invoquez les depuis celui-ci afin de ne pas les exposer.
Stocker les valeurs de retour dans SSM Parameter
Utilisez les fonctions approprié pour que dans une variable SSM, que vous allez créer à partir de votre template cloudformation, la valeur stockée serait du type : “jdbc:postgresql://”+${Database endpoint address}+”:”+${Database endpoint port}+”/”+${Database name}
Montrez le nom de la base de données en Output

Et ensuite il va falloir déployer notre infrastructure. Pour ce faire, veuillez suivre les instructions suivantes :
créer un workflow git qui va servir à déployer notre template
veillez à bien configurer vos secrets dans Settings>Secrets and variables > Actions

NB : n’exposez pas publiquement vos accès AWS
