# jellyfin-for-plexguide
YML file for Jellyfin and Traefik in Plexguide

Plexguide allows you to add your own Docker containers that can be deployed through the Plexguide script and can be backed up.
The template s found in /opt/mycontainers and the template file is _template.yml

Easiest way to use this is simply create a file called "jellyfin.yml" (without the quotes) in that folder (so you would have /opt/mycontainers/jellyfin.yml) and just paste in the text from the jellyfin.yml file here.

Then run Plexguide, and go to the PG Box: App installer section.
There the jellyfin app shuld be in the list to deploy like any other prepared app (i.e. Plex, Netdata, etc/)

Choose to install it like any other app. It will allow for the cron job backups as desired and give you the URL and port needed to access the web front end of Jellyfin.

#Instructions for a more automated (not copy and paste into jellyfin.yml) approach

1. Go to the /opt/mycontainers directory (cd /opt/mycontainers)
2. Type the command: git init
3. Type the command: git remote rm origin
4. Type the command: git remote add origin https://github.com/timekills/jellyfin-for-plexguide.git
5. Type the command: git pull origin master
6. (Optional) rm -r README.md if you don't want the README file cluttering up your drectory
7. Run Plexguide

Deploy jellyfin app like any other app
