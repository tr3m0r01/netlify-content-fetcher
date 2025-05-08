# Netlify Content Fetcher

This is a simple content fetcher that mirrors content from https://content-c5v.pages.dev/ on a Netlify site.

## How it works

1. The index.html file contains embedded JavaScript that fetches content from the target domain
2. It preserves the path structure of the original site
3. The netlify.toml configuration ensures all routes are handled by the index.html file

## Deployment

1. Push this repository to GitHub
2. Connect your GitHub repository to Netlify
3. Deploy the site
4. Any path requested on your Netlify site will display the content from the corresponding path on https://content-c5v.pages.dev/

## Limitations

- CORS policies might prevent fetching content if the target site doesn't allow it
- Some dynamic content or JavaScript functionality from the original site might not work properly
- Relative links and resource paths may require additional handling 