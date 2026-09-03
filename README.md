# Aspire Connect — Fixed GitHub + Vercel Package

This version fixes the navigation issue by using explicit `.html` page links.
It is intentionally flat and requires no framework/build process.

Repository root should contain:
- index.html
- services.html
- industries.html
- about.html
- contact.html
- styles.css
- vercel.json
- robots.txt
- sitemap.xml

## Replace your current GitHub files

1. Open your GitHub `aspire-connect` repository.
2. Replace the old files with the files from this package.
3. Keep the filenames exactly as shown.
4. Commit the changes.
5. Vercel should automatically redeploy the new commit.
6. Open the Vercel deployment URL and hard-refresh the browser (Ctrl+F5).
7. Test:
   - /
   - /services.html
   - /industries.html
   - /about.html
   - /contact.html

If Vercel is connected to the GitHub repository, you do not need to manually redeploy after committing.

## Why this version

The previous version used folders such as `/services/index.html` and relied on directory/index URL routing. Depending on how the files were uploaded and how the deployment was being tested, those routes can return 404s. This version uses explicit HTML filenames, which is the most straightforward and robust setup for a simple static GitHub/Vercel site.

The visual design and content are unchanged.
