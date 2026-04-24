# venera-configs

Configuration file repository for venera

## Using a fork with jsDelivr

If you are using your own fork as the source repository, you can access files through jsDelivr without setting up a separate CDN.

Example URLs:

- `https://cdn.jsdelivr.net/gh/<your-github-name>/venera-configs@main/index.json`
- `https://cdn.jsdelivr.net/gh/<your-github-name>/venera-configs@main/your_config_name.js`

Notes:

- The repository must be public for jsDelivr GitHub URLs to work.
- If this repository is a fork, GitHub Actions are disabled by default after forking.
- Enable Actions in the forked repository if you want `.github/workflows/purge_cdn.yml` to automatically purge jsDelivr cache after pushing to `main`.
- jsDelivr may still serve cached content for a short time. If needed, manually purge a file with:
  `https://purge.jsdelivr.net/gh/<your-github-name>/venera-configs@main/<file>`

## Create a new configuration

1. Download `_template_.js`, `_venera_.js`, put them in the same directory
2. Rename `_template_.js` to `your_config_name.js`
3. Edit `your_config_name.js` to your needs. 
   - The `_template_.js` file contains comments to help you with that. 
   - The `_venera_.js` is used for code completion in your IDE.
