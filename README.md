### Name

Yilong Chen

No partner this time



https://Oshima-Hina.github.io/Lab8_Starter/

### Graceful Degradation and Service Workers

Service workers are a practical implementation of the concept of graceful degradation in modern web applications. Graceful degradation is a development philosophy where we build an application assuming ideal conditions—such as a modern browser, stable network connection, and good device performance—but we also design fallback mechanisms to ensure that the application remains usable when those ideal conditions are not met. Rather than failing completely, the application "degrades gracefully," offering a simplified or limited version of itself that still allows the user to achieve essential tasks.

When we incorporate service workers into a web app, we're essentially building with these fallback scenarios in mind, especially in the context of network availability. A service worker operates independently of the main thread and has the ability to intercept and respond to network requests. This means that, even in the absence of a live internet connection, the service worker can serve cached responses to the user. Initially, we assume that the user has a working internet connection, and we fetch data and assets over the network. But after those resources have been successfully retrieved, the service worker can store them in a cache. If the user later revisits the site without an internet connection, the service worker steps in, intercepts the failed network requests, and responds with cached data instead. In this way, service workers help bridge the gap between ideal and non-ideal environments, allowing the web application to degrade, but do so with grace.

### pwa.png

[pwa.png](pwa.png)
