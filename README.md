# Netlify CMS - HUGO Module

## Configuration

```YAML
# config.yaml
Params:
  netlifyIdentity:
    enabled: true # enable if you are authenticating a new user with netlify identity
                  # disable to speed up page load and remove the external JS script
    bootstrap: true # enable to include CSS for bootstrap compatible z-index for modal
    dir: admin # defaults to admin. Set to the dir inside /static where your netlify
               # index.html is stored. 