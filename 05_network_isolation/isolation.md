# Étape 7 – Isolation réseau avec Docker Compose

Tests effectués :

- ✅ Depuis `app` :
  - ping `web` → OK
  - ping `db` → OK

- ❌ Depuis `web` :
  - ping `db` → échoue (pas dans le même réseau)

Les réseaux définis :
- `frontend` : web + app
- `backend` : app + db

Conclusion : app agit comme un pont entre les deux réseaux, mais web et db sont isolés.

