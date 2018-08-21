# Docs

This is a simple docs repository for maintaining LSC digital assets.

## Updating the website's Ghost installation

to log in with an ssh client to the AWS host. `ssh <username>@<server`

You should have full sudo privileges.  That means you can peform actions with ghost as the ubuntu user.  So you'd need to:
`sudo -i `
(this makes you root)
`su - ubuntu`
(now you are ubuntu -- the user who installed ghost, doing ghost cli things with any other user will break everything due to permissions.)

At this point, you should be able to run ghost commands like `ghost update` from `/var/www/ghost/` just like in the manual :)

If you need to update the Ghost-CLI itself, you can do so from the ubuntu user with `sudo npm install -g ghost-cli`
