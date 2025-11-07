# Admin-Poste-Exercice-1-Intermediaire

Pour cet exercice, j’ai fait les manipulations depuis PowerShell sur ma machine Windows, après m’être connectée en SSH sur ma machine Linux distante. Le but était d’afficher les processus, modifier la priorité d’un processus et terminer un processus via son PID.

# 1) Afficher la liste des processus et repérer celui qui utilise le plus de RAM

<img width="1919" height="253" alt="image" src="https://github.com/user-attachments/assets/5a1982c4-ea17-40da-a35a-83d22755c2b9" />

Le processus qui consommait le plus de RAM chez moi était gnome-shell, avec le PID 2587, à environ 11.3% de RAM.

# 2) Modifier la priorité d’un processus avec nice

<img width="958" height="90" alt="image" src="https://github.com/user-attachments/assets/aa5f8d7b-51e5-4a24-80ea-c9f4b2613489" />

Le PID du processus lancé était 3540.

Ensuite, j’ai vérifié la valeur NICE :

<img width="958" height="69" alt="image" src="https://github.com/user-attachments/assets/e4b2a091-0eb3-4970-8fd9-f4b285a9661b" />

La valeur NICE affichée était 10. Donc la modification de priorité via nice a bien été appliquée.

# 3) Terminer un processus avec son PID

<img width="958" height="117" alt="image" src="https://github.com/user-attachments/assets/9f25b3d7-8f8c-4870-b123-ec6e7754fa13" />

Le processus a été correctement stoppé.

# Conclusion

J’ai affiché la liste complète des processus et identifié celui qui consommait le plus de mémoire. Ensuite, j’ai changé la priorité d’un processus grâce à nice, puis je l’ai terminé avec son PID. Cela m’a permis de manipuler concrètement la gestion des processus depuis mon PowerShell, connecté en SSH à ma machine Linux.
