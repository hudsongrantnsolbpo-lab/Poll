DEPLOY (needs the Netlify CLI or a Git repo, so the function's dependency installs)

Option A - Git: push this folder to GitHub, then in Netlify: Add new site > Import from Git.
Option B - CLI:  npm i -g netlify-cli && npm install && netlify deploy --prod

THEN: Site configuration > Environment variables > add ADMIN_PIN = (your secret PIN) and redeploy.
The PIN unlocks the "Organizer" link (close/reopen poll, reset votes).

NOTE: plain drag-and-drop of the folder will NOT run the voting function.
