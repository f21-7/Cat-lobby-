# CatLobby public website starter pack

This folder contains a simple landing page and the current policy-page drafts from the Revision 229 Store Edition project.

Files:
- `index.html` — simple CatLobby landing page
- `privacy-policy.html` — policy draft; NOT ready to publish until every bracketed placeholder is completed and every statement is checked against the actual service
- `community-guidelines.html` — guidelines draft; NOT ready to publish until the responsible moderator and realistic review schedule are confirmed

## Required before publishing

1. Complete every `[[...]]` placeholder in `privacy-policy.html`.
2. Confirm the actual Supabase retention/log/backup settings and how account deletion and related data deletion are performed. Do not promise deletion timelines that have not been implemented and tested.
3. Confirm who operates CatLobby and who checks the moderation queue, how often it is reviewed, what response target can genuinely be met, and how appeals are handled.
4. Apply and test the Store Catalog and UGC Reporting migration in a staging Supabase project; verify profile/Love Note report submission and private queue review before claiming the report process is live.
5. Confirm the support mailbox is monitored by the responsible operator.
6. Publish these files on a public HTTPS static host. The site URL and the exact `privacy-policy.html` URL must remain stable.
7. Put the Privacy Policy URL in Partner Center. Link Community Guidelines from inside CatLobby and provide the public page URL.

## Simple hosting with GitHub Pages

GitHub Pages can host static HTML. On GitHub Free the repository must be public, so upload ONLY these website files—never the game source, Supabase credentials, service-role keys, webhook secrets, or personal documents.

1. Have the adult account owner/administrator create a public repository named `catlobby-site` (or another suitable name).
2. Upload `index.html`, `privacy-policy.html`, and `community-guidelines.html` to the repository root. Keep this README optional; it does not need to be public.
3. Open repository Settings → Pages.
4. Under Build and deployment, choose Deploy from a branch, select `main` and `/ (root)`, then Save.
5. Wait for GitHub Pages to publish, then open the site URL shown on the Pages settings screen.
6. Test both policy links in a private browser window and confirm they load over HTTPS.

The project-site URL normally has the form `https://OWNER.github.io/REPOSITORY/`; the privacy URL is that URL plus `privacy-policy.html`. Use the exact URLs GitHub displays, not an assumed URL.

GitHub Pages is only one hosting option. A domain name is not required for the page URLs to work.
