## What is CDN 
`CDN stands for Content Dlivery Network. A CDN is a system of distrubuted  servers that hosts resources such as images, CSS, JavaScript files etc`
`Companies like [Microsoft](https://www.microsoft.com/en-us/), [Google](https://www.google.com), [Yahoo](https://www.yahoo.com) etc have a free public CDN from which we can load jQuery instead of hosting it on our own web server`.
**Microsoft jquery CDN :**
https://docs.microsoft.com/en-us/aspnet/ajax/cdn/overview
**Google Jquery CDN :**
https://developers.google.com/speed/libraries
## Benifites of using CDN 
- Distributed CDN server: The jQuery file can be downloaded from the CDN server that is closest to the user.
- Browser Caching : jQuery is used on many popular websites. If a user has already visited a webpage that uses jQuery from a CDN, and then if he arrives at your page, the jQuery files has already been cached by browser so there is no need to download it again.
-Parallel Downloads: There is a browser limit on how many files can be concurrently downloaded from a given domain. This number varies from browser to browser. For example, if the browser allows only 2 concurrent downloads from a given domain, the 3rd downlaod is bloacked until one of the previous files has been fuly downloaded. Since the jQuery file is on a CDN, it is being downloaded from a different domain. So this means the browser allows another 2 parallel downloads from the CDN server.
- Reduced server load: The HTTP request for jQuery file is handled by CDN server, so the load on your webserver is reduced. This also means there is a saving on your website bandwidth consumption which in turn will reduce your hosting cost.
- Disadvantages : Your client firewalls may block the CDN. So you may have to request your clients to whitelist the CDN.
