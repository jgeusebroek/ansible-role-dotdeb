# Ansible role: dotdeb

An Ansible Role that adds the dotdeb repositor(y)(ies) to Debian hosts

## Requirements

None

## Dependencies

None

## Example Playbook

    ---
    - hosts: all
      sudo: yes

      roles:
         - { role: jgeusebroek.dotdeb, tags: ["dotdeb"] }

## Example Variables

    # You can optionally add extra repo's beside the main repo
    dotdeb_extra_repos: [ "wheezy-php56-zts" ]

    # You can optionally change the URL where the gpg key can be found
    dotdeb_gpg_key: 'https://www.dotdeb.org/dotdeb.gpg'

## License

MIT / BSD

## Author Information

This role was created in 2015 by [Jeroen Geusebroek](http://jeroengeusebroek.nl/).