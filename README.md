**1. Cloner les sources du portefeuille**

```
git clone https://github.com/cryptonotefoundation/cryptonotewallet.git
```

**2. Modifier `CryptoNoteWallet.cmake`**
 
```
set(CN_PROJECT_NAME "gallion")
set(CN_CURRENCY_DISPLAY_NAME "Gallion")
set(CN_CURRENCY_TICKER "GMT")
```

**3. Définissez un lien symbolique vers les sources de pièces au même niveau que `src`. Par exemple:**

```
ln -s ../cryptonote cryptonote
```

Une autre façon est de créer un sous-module git:
```
git submodule add https://github.com/cryptonotefoundation/cryptonote.git cryptonote
```

Remplacez l'URL par le dépôt distant git de votre pièce.

**4. Construire**

```
mkdir build && cd build && cmake .. && make
```
