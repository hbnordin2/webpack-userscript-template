# Purpose

This package is a template to allow you to start UserScript projects with live reload.

## Setup

1. Allow Tampermonkey's access to local file URIs: [tampermonkey/faq](https://tampermonkey.net/faq.php?ext=dhdg#Q204)
2. Run `npm --install`
3. Install and enable the following plugin: [LiveReload](https://chrome.google.com/webstore/detail/jnihajbhpnppcggbcgedagnkighmdlei)

## Usage

1. Run `npm run dev`
2. Install `webpack-userscript-template/dist/index.dev.user.js` on TamperMonkey (just copy/paste it)
3. Editing anything under source trigger hot-reloading
4. To confirm it works, go to <https://www.example.com/> and open the console, you should see it printing content.

## Deployment

```bash
npm run build
```

`dist/index.prod.user.js` is the final script.

To use it, copy and paste the result into TamperMonkey.

## Troubleshooting

If you are using Chrome, you may need to [go to your settings](chrome://flags/) and disable "Cookies without SameSite must be secure" for LiveReload to work.

Note that is a security feature, and you just disabled it for your entire browser, so be aware when browsing on Chrome while using this dev tool.
