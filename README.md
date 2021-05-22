
## About 

This is an example of how to use [NextAuth.js](https://next-auth.js.org) TypeScript library to add adenin DigitalAssistant localhost authentication to a [Next.js](https://nextjs.org) application.
   

`dev.cmd`  disables ssl validation (so that node will accept dev certificate for https://localhost:44367) and runs `next dev`


## Host Tenant

A new OAuth client needs to be registered:   
Client Name: spanext    
Title: nextjs spa    
Client Id: tt94cztgbzknvmgfdyfiqk9ah4ej79hq    
Return Url: http://localhost:3000/api/auth/callback/adenin    




## Start the application

To run site locally, use:

```
npm run dev
```

To run it it production mode, use:

```
npm build
npm start
```

## Configuring for production

You must set the `NEXTAUTH_URL` environment variable with the URL of your site, before deploying to production.

e.g. `NEXTAUTH_URL=https://example.com`

To do this in on Vercel, you can use the [Vercel project dashboard](https://vercel.com/dashboard) or the `vc env` command:

    vc env add NEXTAUTH_URL production

Be sure to also set environment variables for the Client ID and Client Secret values for all your authentication providers.
