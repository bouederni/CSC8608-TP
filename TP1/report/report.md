# Exercice 1 : Initialisation du dépôt, réservation GPU, et lancement de la UI via SSH

## Question 1.c.

- Lien du dépôt : https://github.com/bouederni/CSC8608-TP
- Endroit d'exécution du TP : Sur le SLURM de l'école
- Arborescence : ![1a.png](img/1a.png)

Commandes d'activation : 
```bash
(conda-tp) bouederni1@arcadia-slurm-controller:~/CSC8608-TP$ srun --gres=gpu:1 --time=01:30:00 --cpus-per-task=4 --mem=16G --pty bash
(base) bouederni1@arcadia-slurm-node-2:~/CSC8608-TP$ conda activate conda-tp
```

## Question 1.e.
![img/1e](img/1e.png)

## Question 1.g.
![img/1g](img/1g.png)

## Question 1.i.
- Port choisi : `1234`

ssh -L 1234:localhost:1234 node2-tsp