Ansible Role for Rbenv & Ruby
====================

[![Build Status](https://travis-ci.org/vitalied/ansible-role-ruby.svg?branch=master)](https://travis-ci.org/vitalied/ansible-role-ruby)
[![GitHub tag](https://img.shields.io/github/tag/vitalied/ansible-role-ruby.svg)](https://github.com/vitalied/ansible-role-ruby)
[![GitHub license](https://img.shields.io/github/license/vitalied/ansible-role-ruby.svg)](https://github.com/vitalied/ansible-role-ruby/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/ansible/role/8686.svg)](https://galaxy.ansible.com/detail#/role/8686)

Ansible Role for Rbenv & Ruby Management.

Requirements
------------

This role require Ansible 2.0 or higher.

This role was designed for Ubuntu Server 14.04+.

Role Variables
--------------

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">parameter</th>
<th align="left">required</th>
<th align="left">default</th>
<th align="left">choices</th>
<th align="left">comments</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left">ruby_version</td>
<td align="left">yes</td>
<td align="left">2.3.0</td>
<td align="left"></td>
<td align="left">Version of Ruby to install.</td>
</tr>
<tr class="even">
<td align="left">ruby_user</td>
<td align="left">yes</td>
<td align="left">deploy</td>
<td align="left"></td>
<td align="left">The user under which the Rbenv & ruby will be installed.</td>
</tr>
<tr class="odd">
<td align="left">ruby_gems</td>
<td align="left">yes</td>
<td align="left"><a href="https://github.com/vitalied/ansible-role-ruby/blob/master/defaults/main.yml">defaults/main.yml</a></td>
<td align="left"><ul>
<li>list</li>
</ul></td>
<td align="left">Ruby gems to install.</td>
</tr>
</tbody>
</table>

Dependencies
------------

No additional role dependencies.

Example Playbook
----------------

    - hosts: servers
      roles:
        - { role: vitalied.ruby }

License
-------

-   Code released under [MIT](https://github.com/vitalied/ansible-role-ruby/blob/master/LICENSE)
-   Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)
