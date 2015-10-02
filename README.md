# Ansible Role: Vim

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
