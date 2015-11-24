# Harry skin for roundcube

![screenshot](https://raw.githubusercontent.com/beliys/harry/master/screenshots/main.png)

[Look more screenshot...](https://github.com/beliys/harry/blob/master/SCREENSHOTS.md "Look more screenshot...")

Instruction for install:
=====

```bash
git clone https://github.com/beliys/harry /tmp/harry
cp -rf /tmp/harry/skins/harry /var/www/html/roundcube/skins/harry
cp -rf /tmp/harry/plugins/* /var/www/html/roundcube/plugins
chown -R webapps:webapps /var/www/html/roundcube
rm -rf /tmp/harry
```
NOTE: 
1) change /var/www/html/roundcube/ to valid path to roundcube
2) change webapps:webapps for valid USEROWNER:GROUPOWNER

Instruction for install on directadmin:
=====

```bash
git clone https://github.com/beliys/harry /tmp/harry
cp -rf /tmp/harry/skins/harry /var/www/html/roundcube/skins/harry
cp -rf /tmp/harry/plugins/* /var/www/html/roundcube/plugins
chown -R webapps:webapps /var/www/html/roundcube
mkdir -p /usr/local/directadmin/custombuild/custom/roundcube/plugins
mkdir -p /usr/local/directadmin/custombuild/custom/roundcube/skins
cp -rf /tmp/harry/skins/harry /usr/local/directadmin/custombuild/custom/roundcube/skins/harry
cp -rf /tmp/harry/plugins/* /usr/local/directadmin/custombuild/custom/roundcube/plugins
rm -rf /tmp/harry
```
