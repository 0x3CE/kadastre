# Decisions

1 : /dbinfo renvoie en JSON les métadonnées des logs publics : identifiant, date, durée, type d'engin (mav_type), cadre, version du firmware, matériel, étiquettes d'erreur posées par l'utilisateur (1 Other, 2 Vibration… 8 External conditions). /download?log=<id> renvoie le fichier. Limite : 10 requêtes par minute, sinon blocage d'IP.
Selon moi, log_date renvoie la date du téléversement. En effet la date de vol correspond au nom du fichier (date antérieur), et log date est postérieur. Donc j'en déduis cela. 