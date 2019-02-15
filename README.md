Changes from information listed below
-------------------------------------
In this repository, I've made a few adjustments.
1. Integration of lastpass-cli to enable the Ansible lastpass lookup plugin
2. Setting Nginx to listen on ports 80 and 443 (with mounted ssl certificates)

To use these features, you need to set the following variables in `installer/inventory.yml`
* `host_port=80` - HTTP Port for Nginx
* `ssl_host_port=443` - HTTPS Port for Nginx
* `lastpass_username=` - Lastpass username/email address
* `lastpass_password=` - Lastpass password
* `ssl_cert_local_dir=` - Local directory on the system running AWX where your SSL Certificate and key reside
* `ssl_cert_file=` - Name of the SSL Certificate file (in Nginx format) - this is not the full path, just the file name
* `ssl_key_file=` - Name of the SSL Key file (in Nginx format) - this is not the full path, just the file name



Default AWX Readme
------------------

<img src="https://raw.githubusercontent.com/ansible/awx-logos/master/awx/ui/client/assets/logo-login.svg?sanitize=true" width=200 alt="AWX" />

AWX provides a web-based user interface, REST API, and task engine built on top of [Ansible](https://github.com/ansible/ansible). It is the upstream project for [Tower](https://www.ansible.com/tower), a commercial derivative of AWX.  

To install AWX, please view the [Install guide](./INSTALL.md).

To learn more about using AWX, and Tower, view the [Tower docs site](http://docs.ansible.com/ansible-tower/index.html).

The AWX Project Frequently Asked Questions can be found [here](https://www.ansible.com/awx-project-faq).

The AWX logos and branding assets are covered by [our trademark guidelines](https://github.com/ansible/awx-logos/blob/master/TRADEMARKS.md).

Contributing
------------

- Refer to the [Contributing guide](./CONTRIBUTING.md) to get started developing, testing, and building AWX.
- All code submissions are done through pull requests against the `devel` branch.
- All contributors must use git commit --signoff for any commit to be merged, and agree that usage of --signoff constitutes agreement with the terms of [DCO 1.1](./DCO_1_1.md)
- Take care to make sure no merge commits are in the submission, and use `git rebase` vs `git merge` for this reason.
- If submitting a large code change, it's a good idea to join the `#ansible-awx` channel on irc.freenode.net, and talk about what you would like to do or add first. This not only helps everyone know what's going on, it also helps save time and effort, if the community decides some changes are needed.

Reporting Issues
----------------

If you're experiencing a problem that you feel is a bug in AWX, or have ideas for how to improve AWX, we encourage you to open an issue, and share your feedback. But before opening a new issue, we ask that you please take a look at our [Issues guide](./ISSUES.md).

Code of Conduct
---------------

We ask all of our community members and contributors to adhere to the [Ansible code of conduct](http://docs.ansible.com/ansible/latest/community/code_of_conduct.html). If you have questions, or need assistance, please reach out to our community team at [codeofconduct@ansible.com](mailto:codeofconduct@ansible.com)   

Get Involved
------------

We welcome your feedback and ideas. Here's how to reach us with feedback and questions:

- Join the `#ansible-awx` channel on irc.freenode.net
- Join the [mailing list](https://groups.google.com/forum/#!forum/awx-project)

License
-------

[Apache v2](./LICENSE.md)
