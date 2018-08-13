ansible-role-grpc-swift
=======================

[![GitHub license](https://img.shields.io/github/license/bluk/ansible-role-grpc-swift.svg)](https://github.com/bluk/ansible-role-grpc-swift/blob/master/LICENSE) [![Build Status](https://travis-ci.org/bluk/ansible-role-grpc-swift.svg?branch=master)](https://travis-ci.org/bluk/ansible-role-grpc-swift)

An [Ansible](https://www.ansible.com) role to build and install [grpc-swift](https://github.com/grpc/grpc-swift).

Requirements
------------

1. Install the `protoc` binaries. You can download the release from
   [google/protobuf](https://github.com/google/protobuf/releases) or use
   `brew install protobuf`.

2. It is assumed that your system has Xcode CLI / Swift Package Manager
   installed.

Role Variables
--------------

* `grpc_swift_install_path` - The path to clone the `grpc-swift` repository.

* `grpc_swift_git_url` - The git URL to clone `grpc-swift` from.

* `grpc_swift_git_update` - If the cloned `grpc-swift` git repository should be updated.

* `grpc_swift_binary_install_path` - The path to install the built binaries.

Dependencies
------------

No dependencies.

Example Playbook
----------------

```
- hosts: servers
  roles:
     - { role: bluk.grpc_swift }
```

License
-------

Apache 2.0
