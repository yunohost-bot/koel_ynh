# Packaging an app, starting from this example

* Copy this app before working on it, using the ['Use this template'](https://github.com/YunoHost/example_ynh/generate) button on the Github repo.
* Edit the `manifest.toml` with app specific info.
* Edit the `install`, `upgrade`, `remove`, `backup` and `restore` scripts, and any relevant conf files in `conf/`.
  * Using the [script helpers documentation.](https://yunohost.org/packaging_apps_helpers)
* Edit the `change_url` and `config` scripts too, or remove them if you have no use of them
* Add a `LICENSE` file for the package. NB: this LICENSE file is not meant to necessarily be the LICENSE of the upstream app - it is only the LICENSE you want this package's code to published with ;). We recommend to use [the AGPL-3](https://www.gnu.org/licenses/agpl-3.0.txt).
* Edit `doc/DISCLAIMER*.md`
* The `README.md` files are to be automatically generated by https://github.com/YunoHost/apps/tree/master/tools/README-generator

---
<!--
N.B.: This README was automatically generated by https://github.com/YunoHost/apps/tree/master/tools/README-generator
It shall NOT be edited by hand.
-->

# Example app for YunoHost

[![Integration level](https://dash.yunohost.org/integration/example.svg)](https://dash.yunohost.org/appci/app/example) ![Working status](https://ci-apps.yunohost.org/ci/badges/example.status.svg) ![Maintenance status](https://ci-apps.yunohost.org/ci/badges/example.maintain.svg)  
[![Install Example app with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=example)

*[Lire ce readme en français.](./README_fr.md)*

> *This package allows you to install Example app quickly and simply on a YunoHost server.
If you don't have YunoHost, please consult [the guide](https://yunohost.org/#/install) to learn how to install it.*

## Overview

Some long and extensive description of what the app is and does, lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

### Features

- Ut enim ad minim veniam, quis nostrud exercitation ullamco ;
- Laboris nisi ut aliquip ex ea commodo consequat ;
- Duis aute irure dolor in reprehenderit in voluptate ;
- Velit esse cillum dolore eu fugiat nulla pariatur ;
- Excepteur sint occaecat cupidatat non proident, sunt in culpa."


**Shipped version:** 1.0~ynh1

**Demo:** https://demo.example.com

## Screenshots

![Screenshot of Example app](./doc/screenshots/example.jpg)

## Disclaimers / important information

* Any known limitations, constrains or stuff not working, such as (but not limited to):
    * requiring a full dedicated domain ?
    * architectures not supported ?
    * not-working single-sign on or LDAP integration ?
    * the app requires an important amount of RAM / disk / .. to install or to work properly
    * etc...

* Other infos that people should be aware of, such as:
    * any specific step to perform after installing (such as manually finishing the install, specific admin credentials, ...)
    * how to configure / administrate the application if it ain't obvious
    * upgrade process / specificities / things to be aware of ?
    * security considerations ?

## Documentation and resources

* Official app website: <https://example.com>
* Official user documentation: <https://yunohost.org/apps>
* Official admin documentation: <https://yunohost.org/packaging_apps>
* Upstream app code repository: <https://some.forge.com/example/example>
* YunoHost documentation for this app: <https://yunohost.org/app_example>
* Report a bug: <https://github.com/YunoHost-Apps/example_ynh/issues>

## Developer info

Please send your pull request to the [testing branch](https://github.com/YunoHost-Apps/example_ynh/tree/testing).

To try the testing branch, please proceed like that.

``` bash
sudo yunohost app install https://github.com/YunoHost-Apps/example_ynh/tree/testing --debug
or
sudo yunohost app upgrade example -u https://github.com/YunoHost-Apps/example_ynh/tree/testing --debug
```

**More info regarding app packaging:** <https://yunohost.org/packaging_apps>