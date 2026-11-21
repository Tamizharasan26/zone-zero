ZONE ZERO — RENDER DEPLOYMENT

Files:
- index.html: the complete single-file game. Keep this filename so the site opens at the root URL.
- render.yaml: optional Render Blueprint configuration for a static site.

EASIEST DEPLOY (GitHub + Render Dashboard)
1. Extract this ZIP.
2. Create a new GitHub repository, for example: zone-zero.
3. Upload index.html and render.yaml to the repository root (not inside another folder).
4. Open https://dashboard.render.com/ and sign in.
5. Choose New > Static Site.
6. Connect the zone-zero GitHub repository and select the main branch.
7. Set:
   Build Command: echo 'No build step required'
   Publish Directory: .
8. Click Create Static Site and wait for the deploy to finish.
9. Open the *.onrender.com URL shown in the Render dashboard.

You can alternatively use Render's Blueprint flow with render.yaml.

NOTES
- This is a static HTML game; do not create a Node/Web Service.
- No npm install, package.json, or server start command is required for this version.
- The game can load in a browser, but online multiplayer depends on its PeerJS/network setup and is a prototype; static hosting does not create a multiplayer game server.
