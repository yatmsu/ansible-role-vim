# Ansible Role: Vim

[![Join the chat at https://gitter.im/yatmsu/ansible-role-vim](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/yatmsu/ansible-role-vim?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Ansible Role that installs Vim on RetHat/CentOS

## Requirements

None.

## Role Variables

  vim_url: ftp://ftp.vim.org/pub/vim/unix/vim-7.4.tar.bz2

  vimrc_url: https://raw.githubusercontent.com/vim/vim/master/runtime/vimrc_example.vim

  download_dir: /usr/local/src/vim

  unarchived_dir: /usr/local/src/vim/vim74

  configure_options: --enable-multibyte --with-features=huge --disable-selinux --enable-luainterp --enable-perlinterp --enable-pythoninterp --enable-rubyinterp --enable-tclinterp

## Dependencies

None.

## Example Playbook

  - hosts: all
    roles:
       - { role: yatmsu.vim }

## License

BSD

## Author Information

https://github.com/yatmsu
