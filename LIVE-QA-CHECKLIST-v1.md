# TrustPress AI Hub Update QA Checklist v1

## Upload checklist

Upload to the TrustPress AI repo root:

- [ ] `index.html`
- [ ] `book-invisible-expert-os.jpg`
- [ ] `book-trust-orchestration.jpg`

## Live URL

Check:

`https://ivandimitry.github.io/trustpress-ai/`

## QA checks

- [ ] Page loads.
- [ ] Existing cards still display.
- [ ] New Invisible Expert OS card displays.
- [ ] Stars display on Invisible Expert OS card only.
- [ ] Invisible Expert OS has no download link.
- [ ] New Trust Orchestration card displays.
- [ ] Trust Orchestration card links to `../trust-orchestration/`.
- [ ] All images load.
- [ ] Mobile layout works.
- [ ] No broken paths.
- [ ] No old/incorrect filenames.
- [ ] No accidental changes to root site.

## Automated local checks

```json
{
  "sheza_image_ref": true,
  "trust_image_ref": true,
  "trust_link": true,
  "stars_once": true,
  "no_sheza_download_link_in_card": true,
  "no_local_paths": true,
  "no_sandbox": true,
  "existing_cards_kept": true
}
```

## Rollback

Use GitHub commit history and revert the latest commit if anything breaks.
