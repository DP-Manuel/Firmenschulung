# Website

Astro workspace for the public website.

## Current Preview

The first page is now a focused stakeholder prototype based on the preferred modern Variant B direction.

Included routes:

- `/` - homepage story
- `/unternehmen` - company-facing offer
- `/seminare` - seminar focus
- `/qualifizierung` - qualification and placement story
- `/system` - future-system outlook
- `/login` - non-functional login demo
- `/kontakt` - contact demo

The login and contact flows are visual only. They do not authenticate, submit data, or connect to a database.

## Local Commands

Use the portable Node.js runtime from the repository root:

```powershell
$env:PATH = "$PWD\tools\node-v22.16.0-win-x64;$env:PATH"
cd apps\website
npm install
npm run dev
```

If Astro's dev server is blocked by the Windows sandbox, build and serve the static output:

```powershell
$env:PATH = "$PWD\tools\node-v22.16.0-win-x64;$env:PATH"
cd apps\website
$env:ASTRO_TELEMETRY_DISABLED = "1"
npm run build
node .\scripts\serve-dist.mjs
```

Static preview URL:

```text
http://127.0.0.1:4321/Firmenschulung/
```
