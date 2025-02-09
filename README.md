# vault
Vault is a collection of configuration files aimed at building hardened images of common Operating Systems.

Installation:

Taking advantage of cloud-init, modify the following boot parameter: `linux /casper/vmlinuz  ---` to be:

`linux /casper/vmlinuz quiet autoinstall ds=nocloud-net\;s=https://raw.githubusercontent.com/<username>/<repo>/<branch>/ ---`

_Note: The backslash escapes the semi-colon._

