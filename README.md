# LPU-CLIENT

**NurseBeacon Ward Admin**, the web dashboard for the NurseBeacon + Reassure nurse-call system.

Live site: https://haziaintsht.github.io/LPU-CLIENT/

This repository holds only the built website, a Flutter web build of `lib/admin_main.dart`, served by GitHub Pages
from the `main` branch. The data lives in Supabase; the site connects to it with the project's publishable key.

To update the site:

1. Rebuild it from the app folder:

   ```bash
   flutter build web --release -t lib/admin_main.dart --dart-define-from-file=env.json --base-href /LPU-CLIENT/
   ```

2. Copy `build/web` over the files here, keeping this README and `.nojekyll`.
3. Commit and push.

> The admin has no login of its own, so anyone with the link can view and change ward data. Use made-up patients only.
