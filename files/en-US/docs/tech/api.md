# API

To develop some advanced functions, MDx has reserved some API while developing. These APIs are reserved for program calls and are not directly exposed to theme users. This page will list all APIs and the their usages.

## Recently Commented

If a visitor has just submitted a comment, it will carry a Cookie named `mdx_recently_commented` with a value `true` for identification. The Cookie is valid for 15 minutes.

This API can take effect without configure.

## Offline Mode

If your site has enabled Service Worker, it can be accessed offline. However, due to offline, the search and comment functions are not available at this time. MDx provides an offline mode that can gracefully disable the search and comment functions and displays a notice when activated.

The offline mode must be activated manually. It can be activated by setting the Javascript variable `offlineMode` to `true` before `js.js`, `post.js` or `page.js` is loaded in the end of the page.

```JavaScript
var offlineMode = true;
```

## Disable Cookie Consent

If you have enabled the Cookie consent function, you may wish to disable the prompt for visitors from non-EU regions. MDx provides an API to disable it, **but that only provides a method of direct disabling. Specific judgment logic needs to be designed separately.**

To disable cookie consent, you have to set the Javascript variable `displayCookie` to `false` before `js.js`, `post.js` or `page.js` is loaded in the end of the page.

```JavaScript
var displayCookie = false;
```
