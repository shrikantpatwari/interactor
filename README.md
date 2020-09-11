# Interactor.js

A simple, light-weight (< 5KB minified), no dependency, front-end website interaction tracker. 

Collects usage data and submits it to a user-defined server endpoint on the beforeunload event. 

Great for creating a database to drive analytics, inform A/B testing, and guide other site optimization decisions.

This data can help you analyze:
* How your users navigate your website
* Engagement levels on a per-page and site-wide basis
* What platforms, language settings, and browser dimensions your users have
* Bounce rates, page and site bottle-necks, impressions, and conversions


```
<script>
    (function(y,u,k,t,a,o,n,e) {
            y['YuktaOneAnalyticsPixel'] = a;
            y[a]=y[a]||function(){(y[a].q=y[a].q||[]).push(arguments)};
            o=u.createElement(k),
            n=u.getElementsByTagName(k)[0];o.async=1;o.src=t;n.parentNode.insertBefore(o,n)
    })(window,document,'script','//analytics.yuktamedia.com/api/static/js/ymanalytics.min.js','yo');
    yo('apiKey', 'eyJhbGciOiJIUzI1NiJ9.eyJzdWIiOiIxIiwiaWF0IjoxNTg5OTgwMjg3LCJpc3MiOiJZdWt0YU1lZGlhIn0.NCMx4SH99b-mfaSfg7Rw4uPrkMYZm0ww6i7dS8VvvfE');
    yo('interactionElementsArray', ["load_more_posts cta","cta"]);
</script>
```
Use command to minify interactor js
uglifyjs interactor.js -c -o ymAnalytic.min.js
