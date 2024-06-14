# hiddenplaya-site
Burning Man Hidden Playa Site

To make changes, clone the repo to your laptop and make whatever changes are needed. Commit your changes to your local repo then push back to Github's main branch for site to be published.

```
$git clone git@github.com:timothydlister/hiddenplaya-site.git
<make changes to site>
$git add .
$git commit
$git push origin main
```

# What's where?
* DNS is hosted on CloudFlare with a CNAME record pointing to DigitalOcean under Tim's personal account.
* Site Code is this repo on GitHub
* Site Hosting is through Digital Ocean 'App' under Tim's personal account.
* Digital Ocean connects to this repo and pulls the code as it's updated then publishes it on a webserver. TLS certificates are automatically generated through 'Let's Encrypt' courtesy of DigitalOcean.
* DigitalOcean web server app will load index.html (and possibly other well known root files but I'm not sure). 
This is currently a no cost solution to hosting a static site.

# What if it breaks?
Digital Ocean goes down occasionally. Just wait.
* If the site doesn't automatically update after pushing changes to this repo, the integration between DigitalOcean and this repo may have broken. In the past, I have to login to DigitalOcean and reauthorize the app to connect to my GitHub account. It's like the token expires or something....


