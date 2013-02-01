# Overview

This charm provides gitlab from http://http://gitlab.org. Gitlab is a self hosted git management software based on gitolite and rails. It provides a neat source code repository management interface in the likes of github.

# Installation

To install this charm, first edit config.yaml to suite your needs and schedule the following juju actions:

    juju deploy mysql
    juju deploy gitlab

You can then add a relation between joomla and mysql with:

    juju add-relation gitlab mysql

Finally you need to expose your joomla instance:

    juju expose gitlab

Note that the mysql reation addition will create the database and populated it with the admin user. 

# Configuration

admin_password sets the admin password for the gitlab unit

# Contact Information

Author: Helio L Mota
Report bugs at: http://bugs.launchpad.net/charms/+source/gitlab
Location: http://jujucharms.com/charms/precise/gitlab
