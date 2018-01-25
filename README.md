android-sdk
=========

Ansible role to install the Android SDK.

Requirements
------------

Ubuntu 14.04
Ubuntu 16.04
MacOSX 10.12

Role Variables
--------------

tools_path: destination path where to install the Android SDK.
android_sdk_packages: list of packages to install

Dependencies
------------

JulianArevalo.oracle-java

Example Playbook
----------------

Here a playbook example to install the Android SDK with some packages

    - hosts: all
      roles:
         - role: JulianArevalo.android-sdk
           tools_path: "~/tools"
           android_sdk_packages:
             - name: platforms
               version: android-19
             - name: build-tools
               version: 22.0.1
             - name: platform-tools

License
-------

MIT
