
Rkhunter Salt Formula
=====================


.. image:: https://travis-ci.org/saltstack-formulas/rkhunter-formula.svg?branch=master
   :target: https://travis-ci.org/saltstack-formulas/rkhunter-formula
   :alt: Build Status


Install and configure `rkhunter <http://rkhunter.sourceforge.net/>`_ directly with SaltStack.

Available states
----------------


* ``rkhunter.package`` : Installs ``rkhunter`` package
* ``rkhunter.config`` : Configures ``rkhunter`` package
* ``rkhunter`` : Installs and configures ``rkhunter`` package

Available pillars
-----------------

You can take a loot at `\ ``pillar.example`` <https://github.com/saltstack-formulas/rkhunter-formula/blob/master/pillar.example>`_ to configure Rkhunter with pillars.


* ``rkhunter:default:*`` is to configure ``/etc/default/rkhunter`` file (on Debian OS Family) or ``/etc/sysconfig/rkhunter`` file (on RedHat/Suse OS Family)
* ``rkhunter:config:*`` is to configure ``/etc/rkhunter.conf`` file

Run tests
---------

This formula is tested with `Kitchen <https://kitchen.ci/>`_ and `Inspec <https://www.inspec.io/>`_ in a Docker container.

To run tests you need to


* install Ruby dependencies : ``bundle install``
* run Kitchen : ``kitchen test``
