# jellyfin-for-plexguide
YML file for Jellyfin and Traefik in Plexguide

Plexguide allows you to add your own Docker containers that can be deployed through the Plexguide script and can be backed up.
The template s found in /opt/mycontainers and the template file is _template.yml

Easiest way to use this is simply create a file called "jellyfin.yml" (without the quotes) in that folder (so you wouls have /opt/mycontainers/jellyfin.yml).

Then run Plexguide, and go to the PG Box: App installer section.
There the jellyfin app shuld be in the list to deploy like any other prepared app (i.e. Plex, Netdata, etc/)

Choose to install it like any other app. It will allow for the cron job backups as desired and give you the URL and port needed to access the web front end of Jellyfin.
