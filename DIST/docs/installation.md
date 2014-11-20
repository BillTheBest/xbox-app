End-User-Manual
============


##Installation

1. Download from https://raw.githubusercontent.com/mc007/xbox-app/master/DIST/xbox.zip
2. extract the zip on your in any folder
3. Adjust permissions to 755 if needed
4. Open http://localhost/xbox/

##Configuration
 
### Permissions 

All allowed user actions can adjusted in xbox-app/index.php in the static array "ALLOWED_ACTIONS"

Allowed plugins can be adjusted in xbox-app/index.php in the variable "$XF_PROHIBITED_PLUGINS"


### Adjusting the folder location 

In xbox-app/index.php adjust variable "$XF_PATH" : This must be an absolute path with a trailing slash! Notice that this path can be outside of your web-server folder.

###Configuration through URL parameters 

Open the file manaager in different layout modes, append the entry URL by: 

index.php?**layout=single**: Single panel

index.php?**layout=dual**: Dual panel

index.php?**layout=preview**:  Preview layout (split view with media preview)

index.php?**layout=preview&theme=dot-luv**: Preview layout in dark theme (split view with media preview)

index.php?**layout=preview&open=Pictures**: Auto open picture folder in preview mode (split view with media preview)

index.php?**layout=gallery&open=BurningMan&minimal=true&theme=dot-luv**: Auto open picture folder in gallery mode (split view with cover flow view)

index.php?**layout=browser&open=Pictures**: Auto open picture folder in browser mode (Dual view with tree for navigation, classics!)

###Users

The file manager has an ACL & user system but it is not fully implemented. At the moment you can only adjust the password in xbox-app/xapp/Commander/Users.php:
search for the segment "value": "asdasd" and change it to your needs!

###Remote servers

1. You can add remote servers to the file manager in the interface, or you 
2. edit the file xbox-xapp/commander/vfs.php (must be writeable for the interface). See also xbox-xapp/commander/vfs_example.php. In any case it needs the special mount "root"

###More information 

1. Check the development repository at https://github.com/mc007/xbox-app/



 