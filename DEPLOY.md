# Publish Salat Sa'ah on GitHub Pages

This is a standalone static website. No build, installation, backend, analytics or paid service is required. Nothing has been published automatically.

## Before uploading

Review `PRIVACY_AUDIT.md`. The privacy page is explicitly a pre-release review copy: complete the support-mailbox routine below and confirm the intended audience, update the relevant passages and replace the review notice before using it as the final policy for Google Play/OAuth. A public draft is not verification-ready. Do not remove uncertainty labels without resolving the underlying questions.

## Upload and enable Pages

1. Sign in to your GitHub account. Create a **public** repository named `salatsaah` (public repositories support Pages on GitHub Free). If it already exists, inspect its contents before replacing anything.
2. Upload the **contents** of `salatsaah-website`, not the enclosing folder, to the repository's `main` branch. `index.html` and `privacy.html` must be at the repository root; keep `assets/` alongside them. Include `.nojekyll` (a dotfile, sometimes hidden). The Markdown documents are safe deployment notes, but only the HTML, CSS, icon and `.nojekyll` are needed to serve the site. Do not upload any of the Android project or parent folder.
3. In **Settings → Pages → Build and deployment**, select **Deploy from a branch**, then **main** and **/ (root)**. Save. Do not set a custom domain.
4. Wait for GitHub's Pages deployment to finish. Replace `YOUR-USERNAME` below with the actual repository owner. Open both URLs in a signed-out/private browser:
   - `https://YOUR-USERNAME.github.io/salatsaah/`
   - `https://YOUR-USERNAME.github.io/salatsaah/privacy.html`
5. Confirm both return public pages without login, the icon/styles load, and the homepage Privacy link works. Check a phone-sized viewport. There is intentionally no store-download link until the app is published.

[GitHub's publishing-source instructions](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## Google Auth Platform → Branding

After the policy blockers are resolved and the pages are public, select the existing app project in Google Cloud → **Google Auth Platform → Branding**. Enter the homepage and privacy-policy URLs above in their respective fields. Use Salat Sa'ah and the supplied support contact consistently. Keep the existing OAuth clients and signing configuration unchanged. Review the Console's authorized-domain requirements and verification status; saving URLs alone does not verify ownership or publish verified branding.

## Attempt Search Console ownership verification

1. Use the Google account that owns or edits the OAuth project. In [Google Search Console](https://search.google.com/search-console), add a **URL-prefix** property for `https://YOUR-USERNAME.github.io/salatsaah/`.
2. Select HTML-file verification if offered. Download Google's exact verification file and upload it to the `salatsaah` repository root unchanged. After Pages deploys, check its exact required URL is publicly accessible, then click Verify. Alternatively use the supplied HTML meta tag in the homepage `<head>` if that method is offered. No tracking script is needed. Keep the verification file/tag after verification.
3. Follow the precise URL Search Console requests. If it requests a file at `https://YOUR-USERNAME.github.io/` rather than under `/salatsaah/`, the project repository cannot supply that root path. Do not claim success; an account-level Pages site or another supported method would be a separate setup decision.

**Shared-domain limitation:** you control your Pages content, not the DNS for `github.io`. A DNS-based Domain property for `github.io` cannot be verified by uploading project files. A successful URL-prefix verification proves control of that URL prefix; it does not establish ownership of all `github.io`, guarantee acceptance of an OAuth authorized domain, or complete OAuth brand/scope verification. Use only the hostname/domain the Console actually accepts and that you can demonstrate control over. Do not enter a URL path as an authorized domain or claim ownership of `github.io`.

If Google's OAuth flow rejects the shared Pages hostname or requires domain ownership you cannot establish, record the exact requirement and ask Google verification support about acceptable hosting. This package promises free website hosting, **not** guaranteed OAuth domain acceptance. No custom domain or paid hosting has been configured.

[Search Console verification methods](https://support.google.com/webmasters/answer/9008080) · [OAuth brand verification](https://developers.google.com/identity/protocols/oauth2/production-readiness/brand-verification) · [Sensitive-scope verification](https://developers.google.com/identity/protocols/oauth2/production-readiness/sensitive-scope-verification).

Calendar permissions may require sensitive-scope review, scope justification and a demonstration of the consent/user flow. Complete whatever the current Console requests. Website publication, domain ownership, brand verification and scope review are separate milestones. The published policy also needs an accessible link inside the app and consistent Play Data safety disclosures; this task does not modify the app or Console.

## Support-mailbox routine before final policy publication

The developer confirmed Calendar-only use of Google data and authorized selecting a minimal support-retention policy. The policy now commits to deleting support messages and attachments within 90 days after a request is resolved. This does not change the app's on-device account-email storage.

- Restrict mailbox access to people handling support; protect the account with two-step verification. Do not create a mailing list from correspondents.
- When a request is resolved, record its resolution date in a private support log or dated label. Do not put that log in the public repository.
- Review resolved requests weekly. Permanently delete the full thread, sent replies and downloaded attachments before the 90-day deadline; empty the relevant items from Trash. Do not use message age alone when a thread remained open for a long time.
- Process earlier deletion requests promptly. Keep only what a specific legal obligation requires, recording the reason and end date privately.
- Do not ask users to send Calendar data or authentication credentials to support. The policy's prohibition on staff access to Google API data remains in force.
- No mailbox configuration or deletion has been performed by this website task. Provider-controlled copies/backups remain subject to the provider's policies.
