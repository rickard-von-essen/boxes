# boxes

Build [Vagrant] boxes with [Packer]. Hosted [on Atlas].

## Build a box

You need to change the working directory

    cd freebsd/

Validate

    packer validate template.json

Build

    packer build template.json

Import the box so you can test it with some existing Vagrantfile

    vagrant box add --name "test/freebsd-10.1-amd64" packer_freebsd-10.1-amd64_virtualbox.box

Upload the box [to Atlas].

## Getting started

Install Packer using Homebrew:

    brew install packer

## Credits

* The FreeBSD box is based on [nickchappell/packer-templates].
* The OpenBSD box is based on [tmatilai/packer-openbsd].

[Vagrant]: https://www.vagrantup.com/
[Packer]: https://www.packer.io/
[nickchappell/packer-templates]: https://github.com/nickchappell/packer-templates
[tmatilai/packer-openbsd]: https://github.com/tmatilai/packer-openbsd
[on Atlas]: https://atlas.hashicorp.com/twingly
[to Atlas]: https://atlas.hashicorp.com/vagrant
