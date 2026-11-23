# Deploy on Cloudflare Pages (free)

Upload the whole `noor-atelier` folder (the one containing `index.html` and `images`).
Do NOT upload the `docs` or `single-file` folders if you want a clean site; they are harmless but not needed.

## Steps

1. **Prepare the folder.** Copy `index.html` and the `images` folder into a new folder named `noor-site`.
2. **Create an account.** Go to https://dash.cloudflare.com and sign up with your email. Confirm the verification email.
3. **Open Pages.** In the left menu click **Workers & Pages**, then **Create**, then the **Pages** tab.
4. **Choose Direct Upload.** Click **Upload assets** (not "Connect to Git").
5. **Name the project.** For example `noor-atelier`. Your address will be `noor-atelier.pages.dev`.
6. **Upload.** Drag the `noor-site` folder into the upload box. Check that you can see `index.html` and `images`.
7. **Deploy.** Click **Deploy site**. Wait a few seconds.
8. **Open your link.** Click the `.pages.dev` link. Your store is live.
9. **Update later.** Open the project, click **Create new deployment**, and upload the updated folder.

## Optional: your own domain (e.g. nooratelier.com)

1. Buy the domain from Namecheap, GoDaddy or Cloudflare Registrar (about $10 to $15 a year).
2. In your Pages project open **Custom domains**, then **Set up a domain**.
3. Enter the domain and follow the on-screen steps. HTTPS is added automatically.

## Troubleshooting

- **Page opens but photos are missing:** the `images` folder was not uploaded, or its name changed.
- **WhatsApp opens the wrong number:** you have not replaced the dummy number yet.
- **Blank or old page after an update:** refresh with Ctrl+Shift+R (Cmd+Shift+R on Mac).
