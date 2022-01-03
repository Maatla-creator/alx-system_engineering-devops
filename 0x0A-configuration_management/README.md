0x0A. Configuration management

File: 0-create_a_file.pp:

Using Puppet, create a file in /tmp.

Requirements:

File path is /tmp/school

File permission is 0744

File owner is www-data

File group is www-data

File contains I love Puppet.

File: 1-install_a_package.pp:

Using Puppet, install puppet-lint.

Requirements:

Install puppet-lint

Version must be 2.5.0

File: 2-execute_a_command.pp:

Using Puppet, create a manifest that kills a process named killmenow.

Requirements:

Must use the exec Puppet resource

Must use pkill.