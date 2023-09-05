# 📷 Photo Blog

_This template is in `BETA`._

_Optimizations are still being made around auth and cache behavior._

_Database schema changes are expected._

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?demo-title=Photo+Blog&demo-description=Store+photos+with+original+camera+data&demo-url=https%3A%2F%2Fphotos.sambecker.com&demo-image=https%3A%2F%2Fphotos.sambecker.com%2Fdeploy-image&project-name=Photo+Blog&repository-name=photo-blog&repository-url=https%3A%2F%2Fgithub.com%2Fsambecker%2Fphoto-blog&from=templates&skippable-integrations=1&env-description=Configure+your+photo+blog+meta&env-link=BLANK&env=NEXT_PUBLIC_SITE_TITLE%2CNEXT_PUBLIC_SITE_DOMAIN&teamCreateStatus=hidden&stores=%5B%7B%22type%22%3A%22postgres%22%7D%2C%7B%22type%22%3A%22blob%22%7D%5D)

### 1. Deploy to Vercel

1. Click Deploy
2. Add required storage ([Vercel Postgres](https://vercel.com/docs/storage/vercel-postgres) + [Vercel Blob](https://vercel.com/docs/storage/vercel-blob))
3. Add environment variables
- `NEXT_PUBLIC_SITE_TITLE` (e.g., My Photos)
- `NEXT_PUBLIC_SITE_DOMAIN` (e.g., photos.domain.com)
- `NEXT_PUBLIC_SITE_DESCRIPTION` (optional—mainly used for OG meta)

### 2. Setup Auth

1. Create a Clerk account
2. Add Clerk environment variables to your project
3. Create an admin user
4. Add standard environment variables:
- `NEXT_PUBLIC_CLERK_SIGN_IN_URL`
- `CLERK_SECRET_KEY`
- `CLERK_ADMIN_USER_ID`
4. Add your admin user id to environment variables:
- `CLERK_ADMIN_USER_ID` 

### 3. Develop locally

1. Clone code
2. Install dependencies `pnpm i`
3. Run `vc dev` to utilize Vercel-stored environment variables
