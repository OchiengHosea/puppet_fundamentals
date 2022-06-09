##Introduction to Puppet

Puppet is a language for describing the desired state of your infrastructure
and a set of tools to enforce that state

Puppet can generate reports to be used in inventory audits

###Specific terms in Puppet

Node - an individual server or device managed by Puppet
Resources - individual units of configuration in Puppet like files and system user
Class - a collection of Puppet code that makes sense as a logical group
Manifest - a text file for holding Puppet code
Profile - A class that defines a specific set of configuration
Role - a class that defines the business role of a node

to start a vagrant file, run vagrant up

puppet code can be packaged into modules and shared in puppet forge

to write your own modules,you can put them into a directory called site in the root of control repo

Facter
This is the tool that puppet uses to gather information about nodes on what needs to be done on them

Facter runs at the begining of a puppet run and gathers all the facts to be submitted to the master. Then the master uses those data and other data to generate a catalogue 
that will be applied to that node.

Module

