# Kablun
Kablun is a moderation service for ER:LC on Roblox which has an aim of organising everything into one service. Lots of features will be provided and there will be one repository using both the frontend of the service, and the backend.

Note that some things stated here will only be meant for the main repository, not necessarily in this repo.

## Structure
### Repository
- ``/frontend``: Where all the frontend source code is found
- ``/frontend/README.md``: Information about the structure of frontend source
- ``/frontend/web``: Directory for the website files frontend
- ``/backend``: Where all the backend source code is found
- ``/backend/README.md``: Information about the structure of backend source
- ``/backend/api``: Directory for the API files backend
- ``/backend/api/src``: The code for the API

There may be additional directories not stated, this just provides the initial context.

### Website Structure
The entire website structure will be programmed in Next.js. However, there will be different subdomains for certain stuff. The directory of ``/frontend/web`` will look something like the following:
```
/frontend/web/
  subs/
    root/
      README.md
      src/
        ...
    panel/
      README.md
      src/
  packages/
    ...
```
You can see that each directory has a name, such as ``root`` or ``panel``. These are example names. The ``root`` signifies the URL path of ``kablun.com``, meanwhile ``panel`` will have a path of ``panel.kablun.com``. We'll use some sort of NPM module to organise it all.

The subdomain ``src/`` directory is the actual content of the subdomain.
The ``packages/`` directory is shared things across the subdomain source directories, such as components or index.css files. Things that should be shared.
