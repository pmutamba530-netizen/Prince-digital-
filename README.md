# Prince Digital V1 — Supabase

## 1. Préparer Supabase
1. Créer/ouvrir le projet Supabase.
2. Ouvrir SQL Editor.
3. Copier le contenu de `supabase/schema.sql`.
4. Exécuter le script.

## 2. Configuration locale
Créer `.env.local` à partir de `.env.example` et renseigner :
- NEXT_PUBLIC_SUPABASE_URL
- NEXT_PUBLIC_SUPABASE_ANON_KEY (Publishable/anon public key)
- NEXT_PUBLIC_WHATSAPP_NUMBER

Ne jamais mettre une `service_role` ou une `secret key` dans ces variables publiques.

## 3. Lancer
npm install
npm run dev

## 4. Déploiement Netlify
- Importer le projet depuis GitHub.
- Build command: `npm run build`
- Publish directory: laisser Netlify gérer Next.js.
- Ajouter les mêmes variables d'environnement dans Netlify.
- Redéployer.

## Ce que cette V1 fait réellement
- charge les services depuis Supabase;
- inscription et connexion e-mail/mot de passe;
- RLS de base pour protéger profils/commandes;
- bouton WhatsApp prérempli pour une demande de service;
- structure de base pour commandes et fichiers.

## Étapes suivantes
Paiement réel, stockage de fichiers, création de commande depuis l'interface, tableau de bord client, administration, notifications, intégrations fournisseurs et IA côté serveur nécessitent des modules supplémentaires et des comptes/API correspondants.
