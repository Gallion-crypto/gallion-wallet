**1. Cloner les sources du portefeuille**

```
git clone https://github.com/Gallion-crypto/gallion-wallet.git
```

**2. Définissez un lien symbolique vers les sources de pièces au même niveau que `src`. Par exemple:**

```
ln -s ../gallion cryptonote
```

Une autre façon est de créer un sous-module git:
```
git submodule add https://github.com/Gallion-crypto/gallion.git cryptonote
```

Remplacez l'URL par le dépôt distant git de votre pièce.

**3. Construire**

```
mkdir build && cd build && cmake .. && make
```
