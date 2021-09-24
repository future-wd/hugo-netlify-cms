# Netlify CMS - HUGO Module

## Configuration

```YAML
# config.yaml
Params:
  netlifyIdentity:
    enabled: true # enable if you are authenticating a new user with netlify identity
                  # disable to speed up page load and remove the external JS script
    bootstrap: true # enable to include CSS for bootstrap compatible z-index for modal

    # dir: admin # defaults to admin. Set to the dir inside /static where your netlify
               # index.html is stored. 
    # this may have to be moved to a higher level if the index.html file is copied to this dir on run.
```

## INSTALLATION

```HTML
# /layouts/index.html 
{{ define "main }}
...

{{ partial "netlify-cms/index" . }}
{{ end }}
```

create your config.yml file in /static/admin
see <https://www.netlifycms.org/docs/configuration-options/>

/static/admin/index.html is created by the module 

navigate to site.com/admin to use netlify CMS