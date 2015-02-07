openstack-heat-apic
====================

Heat plugin for Cisco ACI




## Environment

Required

* Python 2.7+
* [acitoolkit](http://datacenter.github.io/acitoolkit/)


## Downloading

Clone the repository

     git clone https://github.com/kecorbin/openstack-heat-apic.git 


# Installation

Copy the plugin into heat plugin_dirs specified in /etc/heat/heat.conf
    
     cp plugin/apic_plugin.py /usr/lib/heat

Restart openstack-heat-engine (RHEL example)

    systemctl restart openstack-heat-engine
    


# Usage

sample HOT template in example directory


The following section needs to be added to heat.conf

    [apic_plugin]
    apic_system_id=openstack
    apic_host=1.1.1.1
    apic_username=admin
    apic_password=password

