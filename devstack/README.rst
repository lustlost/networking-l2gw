======================
 Enabling in Devstack
======================

1. Download DevStack

2. Add this repo as an external repository:

     > cat local.conf
     [[local|localrc]]
     enable_plugin networking-l2gw https://github.com/stackforge/networking-l2gw
     enable_service l2gw-plugin l2gw-agent
     OVSDB_HOSTS=<ovsdb_name>:<ip address>:<port>



3. run ``stack.sh``