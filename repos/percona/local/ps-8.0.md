# `percona:8.0.32-24-centos`

## Docker Metadata

- Image ID: `sha256:9b19a7e19813d6639c28cd1bb2a54a091ce21cec682d290dc1a65e5318392cc7`
- Created: `2023-04-12T11:08:35.321019842Z`
- Virtual Size: ~ 1.03 Gb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/docker-entrypoint.sh"]`
- Command: `["mysqld"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `PS_VERSION=8.0.32-24.1`
  - `MYSQL_SHELL_VERSION=8.0.32-1`
  - `OS_VER=el9`
  - `FULL_PERCONA_VERSION=8.0.32-24.1.el9`
  - `FULL_MYSQL_SHELL_VERSION=8.0.32-1.el9`
  - `PS_REPO=testing`
- Labels:
  - `org.opencontainers.image.authors=info@percona.com`

## `rpm` (`.rpm`-based packages)

### `rpm` package: `acl-2.3.1-3.el9.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url acl-2.3.1-3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/acl-2.3.1-3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/acl-2.3.1-3.el9.src.rpm
```

### `rpm` package: `alternatives-1.20-2.0.3.el9.x86_64`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ dnf --quiet download --source --url alternatives-1.20-2.0.3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/chkconfig-1.20-2.0.3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/chkconfig-1.20-2.0.3.el9.src.rpm
```

### `rpm` package: `audit-libs-3.0.7-103.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url audit-libs-3.0.7-103.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/audit-3.0.7-103.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/audit-3.0.7-103.el9.src.rpm
```

### `rpm` package: `basesystem-11-13.el9.noarch`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url basesystem-11-13.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/basesystem-11-13.el9.src.rpm
```

### `rpm` package: `bash-5.1.8-6.el9_1.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url bash-5.1.8-6.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/bash-5.1.8-6.el9_1.src.rpm
```

### `rpm` package: `bzip2-libs-1.0.8-8.el9.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url bzip2-libs-1.0.8-8.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/bzip2-1.0.8-8.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/bzip2-1.0.8-8.el9.src.rpm
```

### `rpm` package: `ca-certificates-2022.2.54-90.2.el9_0.noarch`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url ca-certificates-2022.2.54-90.2.el9_0.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/ca-certificates-2022.2.54-90.2.el9_0.src.rpm
```

### `rpm` package: `chkconfig-1.20-2.0.3.el9.x86_64`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ dnf --quiet download --source --url chkconfig-1.20-2.0.3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/chkconfig-1.20-2.0.3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/chkconfig-1.20-2.0.3.el9.src.rpm
```

### `rpm` package: `coreutils-8.32-32.0.1.el9.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url coreutils-8.32-32.0.1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/coreutils-8.32-32.0.1.el9.src.rpm
```

### `rpm` package: `coreutils-common-8.32-32.0.1.el9.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url coreutils-common-8.32-32.0.1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/coreutils-8.32-32.0.1.el9.src.rpm
```

### `rpm` package: `cracklib-2.9.6-27.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url cracklib-2.9.6-27.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/cracklib-2.9.6-27.el9.src.rpm
```

### `rpm` package: `cracklib-dicts-2.9.6-27.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url cracklib-dicts-2.9.6-27.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/cracklib-2.9.6-27.el9.src.rpm
```

### `rpm` package: `crypto-policies-20220815-1.git0fbe86f.el9.noarch`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url crypto-policies-20220815-1.git0fbe86f.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/crypto-policies-20220815-1.git0fbe86f.el9.src.rpm
```

### `rpm` package: `cryptsetup-libs-2.4.3-5.el9_1.1.x86_64`

Licenses (from `rpm --query`): GPLv2+ and LGPLv2+

Source:

```console
$ dnf --quiet download --source --url cryptsetup-libs-2.4.3-5.el9_1.1
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/cryptsetup-2.4.3-5.el9_1.1.src.rpm
```

### `rpm` package: `curl-7.76.1-19.el9_1.2.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url curl-7.76.1-19.el9_1.2
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/curl-7.76.1-19.el9_1.2.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/curl-7.76.1-19.el9_1.2.src.rpm
```

### `rpm` package: `cyrus-sasl-lib-2.1.27-20.el9.x86_64`

Licenses (from `rpm --query`): BSD with advertising

Source:

```console
$ dnf --quiet download --source --url cyrus-sasl-lib-2.1.27-20.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/cyrus-sasl-2.1.27-20.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/cyrus-sasl-2.1.27-20.el9.src.rpm
```

### `rpm` package: `dbus-1.12.20-7.0.1.el9_1.x86_64`

Licenses (from `rpm --query`): (GPLv2+ or AFL) and GPLv2+

Source:

```console
$ dnf --quiet download --source --url dbus-1.12.20-7.0.1.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/dbus-1.12.20-7.0.1.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/dbus-1.12.20-7.0.1.el9_1.src.rpm
```

### `rpm` package: `dbus-broker-28-7.el9.x86_64`

Licenses (from `rpm --query`): ASL 2.0

Source:

```console
$ dnf --quiet download --source --url dbus-broker-28-7.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/dbus-broker-28-7.el9.src.rpm
```

### `rpm` package: `dbus-common-1.12.20-7.0.1.el9_1.noarch`

Licenses (from `rpm --query`): (GPLv2+ or AFL) and GPLv2+

Source:

```console
$ dnf --quiet download --source --url dbus-common-1.12.20-7.0.1.el9_1.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/dbus-1.12.20-7.0.1.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/dbus-1.12.20-7.0.1.el9_1.src.rpm
```

### `rpm` package: `dbus-libs-1.12.20-7.0.1.el9_1.x86_64`

Licenses (from `rpm --query`): (GPLv2+ or AFL) and GPLv2+

Source:

```console
$ dnf --quiet download --source --url dbus-libs-1.12.20-7.0.1.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/dbus-1.12.20-7.0.1.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/dbus-1.12.20-7.0.1.el9_1.src.rpm
```

### `rpm` package: `device-mapper-1.02.185-3.el9.x86_64`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ dnf --quiet download --source --url device-mapper-1.02.185-3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/lvm2-2.03.16-3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/lvm2-2.03.16-3.el9.src.rpm
```

### `rpm` package: `device-mapper-libs-1.02.185-3.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2

Source:

```console
$ dnf --quiet download --source --url device-mapper-libs-1.02.185-3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/lvm2-2.03.16-3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/lvm2-2.03.16-3.el9.src.rpm
```

### `rpm` package: `dhcp-client-4.4.2-17.b1.el9.x86_64`

Licenses (from `rpm --query`): ISC

Source:

```console
$ dnf --quiet download --source --url dhcp-client-4.4.2-17.b1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/dhcp-4.4.2-17.b1.el9.src.rpm
```

### `rpm` package: `dhcp-common-4.4.2-17.b1.el9.noarch`

Licenses (from `rpm --query`): ISC

Source:

```console
$ dnf --quiet download --source --url dhcp-common-4.4.2-17.b1.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/dhcp-4.4.2-17.b1.el9.src.rpm
```

### `rpm` package: `diffutils-3.7-12.el9.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url diffutils-3.7-12.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/diffutils-3.7-12.el9.src.rpm
```

### `rpm` package: `dnf-4.12.0-4.0.1.el9.noarch`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url dnf-4.12.0-4.0.1.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/dnf-4.12.0-4.0.1.el9.src.rpm
```

### `rpm` package: `dnf-data-4.12.0-4.0.1.el9.noarch`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url dnf-data-4.12.0-4.0.1.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/dnf-4.12.0-4.0.1.el9.src.rpm
```

### `rpm` package: `dnf-plugins-core-4.1.0-3.0.1.el9.noarch`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url dnf-plugins-core-4.1.0-3.0.1.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/dnf-plugins-core-4.1.0-3.0.1.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/dnf-plugins-core-4.1.0-3.0.1.el9.src.rpm
```

### `rpm` package: `elfutils-default-yama-scope-0.187-5.el9.noarch`

Licenses (from `rpm --query`): GPLv2+ or LGPLv3+

Source:

```console
$ dnf --quiet download --source --url elfutils-default-yama-scope-0.187-5.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/elfutils-0.187-5.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/elfutils-0.187-5.el9.src.rpm
```

### `rpm` package: `elfutils-libelf-0.187-5.el9.x86_64`

Licenses (from `rpm --query`): GPLv2+ or LGPLv3+

Source:

```console
$ dnf --quiet download --source --url elfutils-libelf-0.187-5.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/elfutils-0.187-5.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/elfutils-0.187-5.el9.src.rpm
```

### `rpm` package: `elfutils-libs-0.187-5.el9.x86_64`

Licenses (from `rpm --query`): GPLv2+ or LGPLv3+

Source:

```console
$ dnf --quiet download --source --url elfutils-libs-0.187-5.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/elfutils-0.187-5.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/elfutils-0.187-5.el9.src.rpm
```

### `rpm` package: `expat-2.4.9-1.el9_1.1.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url expat-2.4.9-1.el9_1.1
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/expat-2.4.9-1.el9_1.1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/expat-2.4.9-1.el9_1.1.src.rpm
```

### `rpm` package: `file-libs-5.39-10.el9.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url file-libs-5.39-10.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/file-5.39-10.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/file-5.39-10.el9.src.rpm
```

### `rpm` package: `filesystem-3.16-2.el9.x86_64`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url filesystem-3.16-2.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/filesystem-3.16-2.el9.src.rpm
```

### `rpm` package: `findutils-4.8.0-5.el9.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url findutils-4.8.0-5.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/findutils-4.8.0-5.el9.src.rpm
```

### `rpm` package: `gawk-5.1.0-6.el9.x86_64`

Licenses (from `rpm --query`): GPLv3+ and GPLv2+ and LGPLv2+ and BSD

Source:

```console
$ dnf --quiet download --source --url gawk-5.1.0-6.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/gawk-5.1.0-6.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/gawk-5.1.0-6.el9.src.rpm
```

### `rpm` package: `gdbm-libs-1.19-4.el9.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url gdbm-libs-1.19-4.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/gdbm-1.19-4.el9.src.rpm
```

### `rpm` package: `glib2-2.68.4-5.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url glib2-2.68.4-5.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/glib2-2.68.4-5.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/glib2-2.68.4-5.el9.src.rpm
```

### `rpm` package: `glibc-2.34-40.0.1.el9_1.1.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and LGPLv2+ with exceptions and GPLv2+ and GPLv2+ with exceptions and BSD and Inner-Net and ISC and Public Domain and GFDL

Source:

```console
$ dnf --quiet download --source --url glibc-2.34-40.0.1.el9_1.1
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/glibc-2.34-40.0.1.el9_1.1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/glibc-2.34-40.0.1.el9_1.1.src.rpm
```

### `rpm` package: `glibc-common-2.34-40.0.1.el9_1.1.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and LGPLv2+ with exceptions and GPLv2+ and GPLv2+ with exceptions and BSD and Inner-Net and ISC and Public Domain and GFDL

Source:

```console
$ dnf --quiet download --source --url glibc-common-2.34-40.0.1.el9_1.1
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/glibc-2.34-40.0.1.el9_1.1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/glibc-2.34-40.0.1.el9_1.1.src.rpm
```

### `rpm` package: `glibc-langpack-en-2.34-40.0.1.el9_1.1.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and LGPLv2+ with exceptions and GPLv2+ and GPLv2+ with exceptions and BSD and Inner-Net and ISC and Public Domain and GFDL

Source:

```console
$ dnf --quiet download --source --url glibc-langpack-en-2.34-40.0.1.el9_1.1
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/glibc-2.34-40.0.1.el9_1.1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/glibc-2.34-40.0.1.el9_1.1.src.rpm
```

### `rpm` package: `gmp-6.2.0-10.el9.x86_64`

Licenses (from `rpm --query`): LGPLv3+ or GPLv2+

Source:

```console
$ dnf --quiet download --source --url gmp-6.2.0-10.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/gmp-6.2.0-10.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/gmp-6.2.0-10.el9.src.rpm
```

### `rpm` package: `gnupg2-2.3.3-2.el9_0.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url gnupg2-2.3.3-2.el9_0
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/gnupg2-2.3.3-2.el9_0.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/gnupg2-2.3.3-2.el9_0.src.rpm
```

### `rpm` package: `gnutls-3.7.6-18.el9_1.x86_64`

Licenses (from `rpm --query`): GPLv3+ and LGPLv2+

Source:

```console
$ dnf --quiet download --source --url gnutls-3.7.6-18.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/gnutls-3.7.6-18.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/gnutls-3.7.6-18.el9_1.src.rpm
```

### `rpm` package: `gpg-pubkey-8483c65d-5ccc5b19`

Licenses (from `rpm --query`): pubkey

**WARNING:** unable to find source (`dnf download` failed or returned no results)!

### `rpm` package: `gpg-pubkey-8507efa5-5b02c2fb`

Licenses (from `rpm --query`): pubkey

**WARNING:** unable to find source (`dnf download` failed or returned no results)!

### `rpm` package: `gpg-pubkey-8b4efbe6-629ec292`

Licenses (from `rpm --query`): pubkey

**WARNING:** unable to find source (`dnf download` failed or returned no results)!

### `rpm` package: `gpg-pubkey-8d8b756f-629e59ec`

Licenses (from `rpm --query`): pubkey

**WARNING:** unable to find source (`dnf download` failed or returned no results)!

### `rpm` package: `gpg-pubkey-cd2efd2a-4b26dda1`

Licenses (from `rpm --query`): pubkey

**WARNING:** unable to find source (`dnf download` failed or returned no results)!

### `rpm` package: `gpgme-1.15.1-6.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and GPLv3+

Source:

```console
$ dnf --quiet download --source --url gpgme-1.15.1-6.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/gpgme-1.15.1-6.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/gpgme-1.15.1-6.el9.src.rpm
```

### `rpm` package: `grep-3.6-5.el9.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url grep-3.6-5.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/grep-3.6-5.el9.src.rpm
```

### `rpm` package: `groff-base-1.22.4-10.el9.x86_64`

Licenses (from `rpm --query`): GPLv3+ and GFDL and BSD and MIT

Source:

```console
$ dnf --quiet download --source --url groff-base-1.22.4-10.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/groff-1.22.4-10.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/groff-1.22.4-10.el9.src.rpm
```

### `rpm` package: `gzip-1.12-1.el9.x86_64`

Licenses (from `rpm --query`): GPLv3+ and GFDL

Source:

```console
$ dnf --quiet download --source --url gzip-1.12-1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/gzip-1.12-1.el9.src.rpm
```

### `rpm` package: `hostname-3.23-6.el9.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url hostname-3.23-6.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/hostname-3.23-6.el9.src.rpm
```

### `rpm` package: `ima-evm-utils-1.4-4.el9.x86_64`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ dnf --quiet download --source --url ima-evm-utils-1.4-4.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/ima-evm-utils-1.4-4.el9.src.rpm
```

### `rpm` package: `initscripts-10.11.5-1.el9.x86_64`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ dnf --quiet download --source --url initscripts-10.11.5-1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/initscripts-10.11.5-1.el9.src.rpm
```

### `rpm` package: `initscripts-rename-device-10.11.5-1.el9.x86_64`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ dnf --quiet download --source --url initscripts-rename-device-10.11.5-1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/initscripts-10.11.5-1.el9.src.rpm
```

### `rpm` package: `initscripts-service-10.11.5-1.el9.noarch`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ dnf --quiet download --source --url initscripts-service-10.11.5-1.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/initscripts-10.11.5-1.el9.src.rpm
```

### `rpm` package: `ipcalc-1.0.0-5.el9.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url ipcalc-1.0.0-5.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/ipcalc-1.0.0-5.el9.src.rpm
```

### `rpm` package: `iproute-5.18.0-1.0.1.el9.x86_64`

Licenses (from `rpm --query`): GPLv2+ and Public Domain

Source:

```console
$ dnf --quiet download --source --url iproute-5.18.0-1.0.1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/iproute-5.18.0-1.0.1.el9.src.rpm
```

### `rpm` package: `iputils-20210202-8.el9_1.1.x86_64`

Licenses (from `rpm --query`): BSD and GPLv2+

Source:

```console
$ dnf --quiet download --source --url iputils-20210202-8.el9_1.1
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/iputils-20210202-8.el9_1.1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/iputils-20210202-8.el9_1.1.src.rpm
```

### `rpm` package: `jemalloc-5.2.1-2.el9.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url jemalloc-5.2.1-2.el9
https://yum.oracle.com/repo/OracleLinux/OL9/developer/EPEL/x86_64/getPackageSource/jemalloc-5.2.1-2.el9.src.rpm
```

### `rpm` package: `json-c-0.14-11.el9.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url json-c-0.14-11.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/json-c-0.14-11.el9.src.rpm
```

### `rpm` package: `keyutils-libs-1.6.1-4.el9.x86_64`

Licenses (from `rpm --query`): GPLv2+ and LGPLv2+

Source:

```console
$ dnf --quiet download --source --url keyutils-libs-1.6.1-4.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/keyutils-1.6.1-4.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/keyutils-1.6.1-4.el9.src.rpm
```

### `rpm` package: `kmod-libs-28-7.0.1.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url kmod-libs-28-7.0.1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/kmod-28-7.0.1.el9.src.rpm
```

### `rpm` package: `krb5-libs-1.19.1-24.0.1.el9_1.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url krb5-libs-1.19.1-24.0.1.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/krb5-1.19.1-24.0.1.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/krb5-1.19.1-24.0.1.el9_1.src.rpm
```

### `rpm` package: `libacl-2.3.1-3.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libacl-2.3.1-3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/acl-2.3.1-3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/acl-2.3.1-3.el9.src.rpm
```

### `rpm` package: `libaio-0.3.111-13.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libaio-0.3.111-13.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libaio-0.3.111-13.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libaio-0.3.111-13.el9.src.rpm
```

### `rpm` package: `libarchive-3.5.3-3.el9.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url libarchive-3.5.3-3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libarchive-3.5.3-3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libarchive-3.5.3-3.el9.src.rpm
```

### `rpm` package: `libassuan-2.5.5-3.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and GPLv3+

Source:

```console
$ dnf --quiet download --source --url libassuan-2.5.5-3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libassuan-2.5.5-3.el9.src.rpm
```

### `rpm` package: `libattr-2.5.1-3.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libattr-2.5.1-3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/attr-2.5.1-3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/attr-2.5.1-3.el9.src.rpm
```

### `rpm` package: `libblkid-2.37.4-9.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libblkid-2.37.4-9.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/util-linux-2.37.4-9.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/util-linux-2.37.4-9.el9.src.rpm
```

### `rpm` package: `libbpf-0.6.0-1.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2 or BSD

Source:

```console
$ dnf --quiet download --source --url libbpf-0.6.0-1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libbpf-0.6.0-1.el9.src.rpm
```

### `rpm` package: `libbrotli-1.0.9-6.el9.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libbrotli-1.0.9-6.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/brotli-1.0.9-6.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/brotli-1.0.9-6.el9.src.rpm
```

### `rpm` package: `libcap-2.48-8.el9.x86_64`

Licenses (from `rpm --query`): BSD or GPLv2

Source:

```console
$ dnf --quiet download --source --url libcap-2.48-8.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libcap-2.48-8.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libcap-2.48-8.el9.src.rpm
```

### `rpm` package: `libcap-ng-0.8.2-7.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libcap-ng-0.8.2-7.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libcap-ng-0.8.2-7.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libcap-ng-0.8.2-7.el9.src.rpm
```

### `rpm` package: `libcbor-0.7.0-5.el9.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libcbor-0.7.0-5.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libcbor-0.7.0-5.el9.src.rpm
```

### `rpm` package: `libcom_err-1.46.5-3.el9.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libcom_err-1.46.5-3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/e2fsprogs-1.46.5-3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/e2fsprogs-1.46.5-3.el9.src.rpm
```

### `rpm` package: `libcomps-0.1.18-1.el9.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url libcomps-0.1.18-1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libcomps-0.1.18-1.el9.src.rpm
```

### `rpm` package: `libcurl-7.76.1-19.el9_1.2.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libcurl-7.76.1-19.el9_1.2
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/curl-7.76.1-19.el9_1.2.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/curl-7.76.1-19.el9_1.2.src.rpm
```

### `rpm` package: `libdb-5.3.28-53.el9.x86_64`

Licenses (from `rpm --query`): BSD and LGPLv2 and Sleepycat

Source:

```console
$ dnf --quiet download --source --url libdb-5.3.28-53.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libdb-5.3.28-53.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libdb-5.3.28-53.el9.src.rpm
```

### `rpm` package: `libdnf-0.67.0-3.0.1.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libdnf-0.67.0-3.0.1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libdnf-0.67.0-3.0.1.el9.src.rpm
```

### `rpm` package: `libeconf-0.4.1-2.el9.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libeconf-0.4.1-2.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libeconf-0.4.1-2.el9.src.rpm
```

### `rpm` package: `libedit-3.1-37.20210216cvs.el9.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url libedit-3.1-37.20210216cvs.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libedit-3.1-37.20210216cvs.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libedit-3.1-37.20210216cvs.el9.src.rpm
```

### `rpm` package: `libestr-0.1.11-4.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libestr-0.1.11-4.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libestr-0.1.11-4.el9.src.rpm
```

### `rpm` package: `libevent-2.1.12-6.el9.x86_64`

Licenses (from `rpm --query`): BSD and ISC

Source:

```console
$ dnf --quiet download --source --url libevent-2.1.12-6.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libevent-2.1.12-6.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libevent-2.1.12-6.el9.src.rpm
```

### `rpm` package: `libfastjson-0.99.9-3.el9.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libfastjson-0.99.9-3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libfastjson-0.99.9-3.el9.src.rpm
```

### `rpm` package: `libfdisk-2.37.4-9.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libfdisk-2.37.4-9.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/util-linux-2.37.4-9.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/util-linux-2.37.4-9.el9.src.rpm
```

### `rpm` package: `libffi-3.4.2-7.el9.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libffi-3.4.2-7.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libffi-3.4.2-7.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libffi-3.4.2-7.el9.src.rpm
```

### `rpm` package: `libfido2-1.6.0-7.el9.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url libfido2-1.6.0-7.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libfido2-1.6.0-7.el9.src.rpm
```

### `rpm` package: `libgcc-11.3.1-2.1.0.2.el9.x86_64`

Licenses (from `rpm --query`): GPLv3+ and GPLv3+ with exceptions and GPLv2+ with exceptions and LGPLv2+ and BSD

Source:

```console
$ dnf --quiet download --source --url libgcc-11.3.1-2.1.0.2.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/gcc-11.3.1-2.1.0.2.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/gcc-11.3.1-2.1.0.2.el9.src.rpm
```

### `rpm` package: `libgcrypt-1.10.0-10.el9_1.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libgcrypt-1.10.0-10.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libgcrypt-1.10.0-10.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libgcrypt-1.10.0-10.el9_1.src.rpm
```

### `rpm` package: `libgomp-11.3.1-2.1.0.2.el9.x86_64`

Licenses (from `rpm --query`): GPLv3+ and GPLv3+ with exceptions and GPLv2+ with exceptions and LGPLv2+ and BSD

Source:

```console
$ dnf --quiet download --source --url libgomp-11.3.1-2.1.0.2.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/gcc-11.3.1-2.1.0.2.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/gcc-11.3.1-2.1.0.2.el9.src.rpm
```

### `rpm` package: `libgpg-error-1.42-5.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libgpg-error-1.42-5.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libgpg-error-1.42-5.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libgpg-error-1.42-5.el9.src.rpm
```

### `rpm` package: `libicu-67.1-9.el9.x86_64`

Licenses (from `rpm --query`): MIT and UCD and Public Domain

Source:

```console
$ dnf --quiet download --source --url libicu-67.1-9.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/icu-67.1-9.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/icu-67.1-9.el9.src.rpm
```

### `rpm` package: `libidn2-2.3.0-7.el9.x86_64`

Licenses (from `rpm --query`): (GPLv2+ or LGPLv3+) and GPLv3+

Source:

```console
$ dnf --quiet download --source --url libidn2-2.3.0-7.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libidn2-2.3.0-7.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libidn2-2.3.0-7.el9.src.rpm
```

### `rpm` package: `libksba-1.5.1-6.el9_1.x86_64`

Licenses (from `rpm --query`): (LGPLv3+ or GPLv2+) and GPLv3+

Source:

```console
$ dnf --quiet download --source --url libksba-1.5.1-6.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libksba-1.5.1-6.el9_1.src.rpm
```

### `rpm` package: `libmnl-1.0.4-15.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libmnl-1.0.4-15.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libmnl-1.0.4-15.el9.src.rpm
```

### `rpm` package: `libmodulemd-2.13.0-2.el9.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libmodulemd-2.13.0-2.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libmodulemd-2.13.0-2.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libmodulemd-2.13.0-2.el9.src.rpm
```

### `rpm` package: `libmount-2.37.4-9.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libmount-2.37.4-9.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/util-linux-2.37.4-9.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/util-linux-2.37.4-9.el9.src.rpm
```

### `rpm` package: `libnghttp2-1.43.0-5.el9.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libnghttp2-1.43.0-5.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/nghttp2-1.43.0-5.el9.src.rpm
```

### `rpm` package: `libpkgconf-1.7.3-9.el9.x86_64`

Licenses (from `rpm --query`): ISC

Source:

```console
$ dnf --quiet download --source --url libpkgconf-1.7.3-9.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/pkgconf-1.7.3-9.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/pkgconf-1.7.3-9.el9.src.rpm
```

### `rpm` package: `libpsl-0.21.1-5.el9.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libpsl-0.21.1-5.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libpsl-0.21.1-5.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libpsl-0.21.1-5.el9.src.rpm
```

### `rpm` package: `libpwquality-1.4.4-8.el9.x86_64`

Licenses (from `rpm --query`): BSD or GPLv2+

Source:

```console
$ dnf --quiet download --source --url libpwquality-1.4.4-8.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libpwquality-1.4.4-8.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libpwquality-1.4.4-8.el9.src.rpm
```

### `rpm` package: `librepo-1.14.2-3.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url librepo-1.14.2-3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/librepo-1.14.2-3.el9.src.rpm
```

### `rpm` package: `libreport-filesystem-2.15.2-6.0.3.el9.noarch`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url libreport-filesystem-2.15.2-6.0.3.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libreport-2.15.2-6.0.3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libreport-2.15.2-6.0.3.el9.src.rpm
```

### `rpm` package: `libseccomp-2.5.2-2.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2

Source:

```console
$ dnf --quiet download --source --url libseccomp-2.5.2-2.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libseccomp-2.5.2-2.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libseccomp-2.5.2-2.el9.src.rpm
```

### `rpm` package: `libselinux-3.4-3.el9.x86_64`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url libselinux-3.4-3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libselinux-3.4-3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libselinux-3.4-3.el9.src.rpm
```

### `rpm` package: `libselinux-utils-3.4-3.el9.x86_64`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url libselinux-utils-3.4-3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libselinux-3.4-3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libselinux-3.4-3.el9.src.rpm
```

### `rpm` package: `libsemanage-3.4-2.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libsemanage-3.4-2.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libsemanage-3.4-2.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libsemanage-3.4-2.el9.src.rpm
```

### `rpm` package: `libsepol-3.4-1.1.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libsepol-3.4-1.1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libsepol-3.4-1.1.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libsepol-3.4-1.1.el9.src.rpm
```

### `rpm` package: `libsigsegv-2.13-4.el9.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url libsigsegv-2.13-4.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libsigsegv-2.13-4.el9.src.rpm
```

### `rpm` package: `libsmartcols-2.37.4-9.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libsmartcols-2.37.4-9.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/util-linux-2.37.4-9.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/util-linux-2.37.4-9.el9.src.rpm
```

### `rpm` package: `libsolv-0.7.22-1.el9.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url libsolv-0.7.22-1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libsolv-0.7.22-1.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libsolv-0.7.22-1.el9.src.rpm
```

### `rpm` package: `libssh-0.9.6-3.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libssh-0.9.6-3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libssh-0.9.6-3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libssh-0.9.6-3.el9.src.rpm
```

### `rpm` package: `libssh-config-0.9.6-3.el9.noarch`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libssh-config-0.9.6-3.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libssh-0.9.6-3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libssh-0.9.6-3.el9.src.rpm
```

### `rpm` package: `libstdc++-11.3.1-2.1.0.2.el9.x86_64`

Licenses (from `rpm --query`): GPLv3+ and GPLv3+ with exceptions and GPLv2+ with exceptions and LGPLv2+ and BSD

Source:

```console
$ dnf --quiet download --source --url libstdc++-11.3.1-2.1.0.2.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/gcc-11.3.1-2.1.0.2.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/gcc-11.3.1-2.1.0.2.el9.src.rpm
```

### `rpm` package: `libtasn1-4.16.0-8.el9_1.x86_64`

Licenses (from `rpm --query`): GPLv3+ and LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libtasn1-4.16.0-8.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libtasn1-4.16.0-8.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libtasn1-4.16.0-8.el9_1.src.rpm
```

### `rpm` package: `libtirpc-1.3.3-0.el9.x86_64`

Licenses (from `rpm --query`): SISSL and BSD

Source:

```console
$ dnf --quiet download --source --url libtirpc-1.3.3-0.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libtirpc-1.3.3-0.el9.src.rpm
```

### `rpm` package: `libunistring-0.9.10-15.el9.x86_64`

Licenses (from `rpm --query`): GPLv2+ or LGPLv3+

Source:

```console
$ dnf --quiet download --source --url libunistring-0.9.10-15.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libunistring-0.9.10-15.el9.src.rpm
```

### `rpm` package: `libuser-0.63-11.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libuser-0.63-11.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libuser-0.63-11.el9.src.rpm
```

### `rpm` package: `libutempter-1.2.1-6.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libutempter-1.2.1-6.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libutempter-1.2.1-6.el9.src.rpm
```

### `rpm` package: `libuuid-2.37.4-9.el9.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url libuuid-2.37.4-9.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/util-linux-2.37.4-9.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/util-linux-2.37.4-9.el9.src.rpm
```

### `rpm` package: `libverto-0.3.2-3.el9.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libverto-0.3.2-3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libverto-0.3.2-3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libverto-0.3.2-3.el9.src.rpm
```

### `rpm` package: `libxcrypt-4.4.18-3.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and BSD and Public Domain

Source:

```console
$ dnf --quiet download --source --url libxcrypt-4.4.18-3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libxcrypt-4.4.18-3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libxcrypt-4.4.18-3.el9.src.rpm
```

### `rpm` package: `libxml2-2.9.13-3.el9_1.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libxml2-2.9.13-3.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libxml2-2.9.13-3.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/libxml2-2.9.13-3.el9_1.src.rpm
```

### `rpm` package: `libyaml-0.2.5-7.el9.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libyaml-0.2.5-7.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libyaml-0.2.5-7.el9.src.rpm
```

### `rpm` package: `libzstd-1.5.1-2.el9.x86_64`

Licenses (from `rpm --query`): BSD and GPLv2

Source:

```console
$ dnf --quiet download --source --url libzstd-1.5.1-2.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/zstd-1.5.1-2.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/zstd-1.5.1-2.el9.src.rpm
```

### `rpm` package: `lua-libs-5.4.4-2.el9_1.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url lua-libs-5.4.4-2.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/lua-5.4.4-2.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/lua-5.4.4-2.el9_1.src.rpm
```

### `rpm` package: `lz4-libs-1.9.3-5.el9.x86_64`

Licenses (from `rpm --query`): GPLv2+ and BSD

Source:

```console
$ dnf --quiet download --source --url lz4-libs-1.9.3-5.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/lz4-1.9.3-5.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/lz4-1.9.3-5.el9.src.rpm
```

### `rpm` package: `mpfr-4.1.0-7.el9.x86_64`

Licenses (from `rpm --query`): LGPLv3+

Source:

```console
$ dnf --quiet download --source --url mpfr-4.1.0-7.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/mpfr-4.1.0-7.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/mpfr-4.1.0-7.el9.src.rpm
```

### `rpm` package: `ncurses-6.2-8.20210508.el9.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url ncurses-6.2-8.20210508.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/ncurses-6.2-8.20210508.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/ncurses-6.2-8.20210508.el9.src.rpm
```

### `rpm` package: `ncurses-base-6.2-8.20210508.el9.noarch`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url ncurses-base-6.2-8.20210508.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/ncurses-6.2-8.20210508.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/ncurses-6.2-8.20210508.el9.src.rpm
```

### `rpm` package: `ncurses-libs-6.2-8.20210508.el9.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url ncurses-libs-6.2-8.20210508.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/ncurses-6.2-8.20210508.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/ncurses-6.2-8.20210508.el9.src.rpm
```

### `rpm` package: `net-tools-2.0-0.62.20160912git.el9.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url net-tools-2.0-0.62.20160912git.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/net-tools-2.0-0.62.20160912git.el9.src.rpm
```

### `rpm` package: `nettle-3.8-3.el9_0.x86_64`

Licenses (from `rpm --query`): LGPLv3+ or GPLv2+

Source:

```console
$ dnf --quiet download --source --url nettle-3.8-3.el9_0
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/nettle-3.8-3.el9_0.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/nettle-3.8-3.el9_0.src.rpm
```

### `rpm` package: `npth-1.6-8.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url npth-1.6-8.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/npth-1.6-8.el9.src.rpm
```

### `rpm` package: `numactl-libs-2.0.14-8.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2 and GPLv2

Source:

```console
$ dnf --quiet download --source --url numactl-libs-2.0.14-8.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/numactl-2.0.14-8.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/numactl-2.0.14-8.el9.src.rpm
```

### `rpm` package: `openldap-2.6.2-3.el9.x86_64`

Licenses (from `rpm --query`): OpenLDAP

Source:

```console
$ dnf --quiet download --source --url openldap-2.6.2-3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/openldap-2.6.2-3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/openldap-2.6.2-3.el9.src.rpm
```

### `rpm` package: `openssh-8.7p1-24.el9_1.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url openssh-8.7p1-24.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/openssh-8.7p1-24.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/openssh-8.7p1-24.el9_1.src.rpm
```

### `rpm` package: `openssh-clients-8.7p1-24.el9_1.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url openssh-clients-8.7p1-24.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/openssh-8.7p1-24.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/openssh-8.7p1-24.el9_1.src.rpm
```

### `rpm` package: `openssh-server-8.7p1-24.el9_1.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url openssh-server-8.7p1-24.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/openssh-8.7p1-24.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/openssh-8.7p1-24.el9_1.src.rpm
```

### `rpm` package: `openssl-3.0.1-47.0.1.el9_1.x86_64`

Licenses (from `rpm --query`): ASL 2.0

Source:

```console
$ dnf --quiet download --source --url openssl-3.0.1-47.0.1.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/openssl-3.0.1-47.0.1.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/openssl-3.0.1-47.0.1.el9_1.src.rpm
```

### `rpm` package: `openssl-devel-3.0.1-47.0.1.el9_1.x86_64`

Licenses (from `rpm --query`): ASL 2.0

Source:

```console
$ dnf --quiet download --source --url openssl-devel-3.0.1-47.0.1.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/openssl-3.0.1-47.0.1.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/openssl-3.0.1-47.0.1.el9_1.src.rpm
```

### `rpm` package: `openssl-libs-3.0.1-47.0.1.el9_1.x86_64`

Licenses (from `rpm --query`): ASL 2.0

Source:

```console
$ dnf --quiet download --source --url openssl-libs-3.0.1-47.0.1.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/openssl-3.0.1-47.0.1.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/openssl-3.0.1-47.0.1.el9_1.src.rpm
```

### `rpm` package: `oracle-epel-release-el9-1.0-1.el9.x86_64`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ dnf --quiet download --source --url oracle-epel-release-el9-1.0-1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/oracle-epel-release-el9-1.0-1.el9.src.rpm
```

### `rpm` package: `oraclelinux-release-9.1-1.0.6.el9.x86_64`

Licenses (from `rpm --query`): GPL

Source:

```console
$ dnf --quiet download --source --url oraclelinux-release-9.1-1.0.6.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/oraclelinux-release-9.1-1.0.6.el9.src.rpm
```

### `rpm` package: `oraclelinux-release-el9-1.0-8.el9.x86_64`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ dnf --quiet download --source --url oraclelinux-release-el9-1.0-8.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/oraclelinux-release-el9-1.0-8.el9.src.rpm
```

### `rpm` package: `p11-kit-0.24.1-2.el9.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url p11-kit-0.24.1-2.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/p11-kit-0.24.1-2.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/p11-kit-0.24.1-2.el9.src.rpm
```

### `rpm` package: `p11-kit-trust-0.24.1-2.el9.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url p11-kit-trust-0.24.1-2.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/p11-kit-0.24.1-2.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/p11-kit-0.24.1-2.el9.src.rpm
```

### `rpm` package: `pam-1.5.1-12.el9.x86_64`

Licenses (from `rpm --query`): BSD and GPLv2+

Source:

```console
$ dnf --quiet download --source --url pam-1.5.1-12.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/pam-1.5.1-12.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/pam-1.5.1-12.el9.src.rpm
```

### `rpm` package: `passwd-0.80-12.el9.x86_64`

Licenses (from `rpm --query`): BSD or GPL+

Source:

```console
$ dnf --quiet download --source --url passwd-0.80-12.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/passwd-0.80-12.el9.src.rpm
```

### `rpm` package: `pcre-8.44-3.el9.3.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url pcre-8.44-3.el9.3
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/pcre-8.44-3.el9.3.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/pcre-8.44-3.el9.3.src.rpm
```

### `rpm` package: `pcre2-10.40-2.0.2.el9.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url pcre2-10.40-2.0.2.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/pcre2-10.40-2.0.2.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/pcre2-10.40-2.0.2.el9.src.rpm
```

### `rpm` package: `pcre2-syntax-10.40-2.0.2.el9.noarch`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url pcre2-syntax-10.40-2.0.2.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/pcre2-10.40-2.0.2.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/pcre2-10.40-2.0.2.el9.src.rpm
```

### `rpm` package: `percona-icu-data-files-8.0.32-24.1.el9.x86_64`

Licenses (from `rpm --query`): Copyright (c) 2000, 2018, Oracle and/or its affiliates. All rights reserved. Under GPLv2 license as shown in the Description field..

**WARNING:** unable to find source (`dnf download` failed or returned no results)!

### `rpm` package: `percona-mysql-shell-8.0.32-1.el9.x86_64`

Licenses (from `rpm --query`): GPLv2

**WARNING:** unable to find source (`dnf download` failed or returned no results)!

### `rpm` package: `percona-release-1.0-27.noarch`

Licenses (from `rpm --query`): GPL-3.0+

**WARNING:** unable to find source (`dnf download` failed or returned no results)!

### `rpm` package: `percona-server-client-8.0.32-24.1.el9.x86_64`

Licenses (from `rpm --query`): Copyright (c) 2000, 2018, Oracle and/or its affiliates. All rights reserved. Under GPLv2 license as shown in the Description field..

**WARNING:** unable to find source (`dnf download` failed or returned no results)!

### `rpm` package: `percona-server-devel-8.0.32-24.1.el9.x86_64`

Licenses (from `rpm --query`): Copyright (c) 2000, 2018, Oracle and/or its affiliates. All rights reserved. Under GPLv2 license as shown in the Description field..

**WARNING:** unable to find source (`dnf download` failed or returned no results)!

### `rpm` package: `percona-server-rocksdb-8.0.32-24.1.el9.x86_64`

Licenses (from `rpm --query`): Copyright (c) 2000, 2018, Oracle and/or its affiliates. All rights reserved. Under GPLv2 license as shown in the Description field..

**WARNING:** unable to find source (`dnf download` failed or returned no results)!

### `rpm` package: `percona-server-server-8.0.32-24.1.el9.x86_64`

Licenses (from `rpm --query`): Copyright (c) 2000, 2018, Oracle and/or its affiliates. All rights reserved. Under GPLv2 license as shown in the Description field..

**WARNING:** unable to find source (`dnf download` failed or returned no results)!

### `rpm` package: `percona-server-shared-8.0.32-24.1.el9.x86_64`

Licenses (from `rpm --query`): Copyright (c) 2000, 2018, Oracle and/or its affiliates. All rights reserved. Under GPLv2 license as shown in the Description field..

**WARNING:** unable to find source (`dnf download` failed or returned no results)!

### `rpm` package: `perl-AutoLoader-5.74-479.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-AutoLoader-5.74-479.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-B-1.80-479.el9.x86_64`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-B-1.80-479.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-Carp-1.50-460.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Carp-1.50-460.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Carp-1.50-460.el9.src.rpm
```

### `rpm` package: `perl-Class-Struct-0.66-479.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Class-Struct-0.66-479.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-Data-Dumper-2.174-462.el9.x86_64`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Data-Dumper-2.174-462.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Data-Dumper-2.174-462.el9.src.rpm
```

### `rpm` package: `perl-Digest-1.19-4.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Digest-1.19-4.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Digest-1.19-4.el9.src.rpm
```

### `rpm` package: `perl-Digest-MD5-2.58-4.el9.x86_64`

Licenses (from `rpm --query`): (GPL+ or Artistic) and RSA

Source:

```console
$ dnf --quiet download --source --url perl-Digest-MD5-2.58-4.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Digest-MD5-2.58-4.el9.src.rpm
```

### `rpm` package: `perl-Encode-3.08-462.el9.x86_64`

Licenses (from `rpm --query`): (GPL+ or Artistic) and Artistic 2.0 and UCD

Source:

```console
$ dnf --quiet download --source --url perl-Encode-3.08-462.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Encode-3.08-462.el9.src.rpm
```

### `rpm` package: `perl-Errno-1.30-479.el9.x86_64`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Errno-1.30-479.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-Exporter-5.74-461.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Exporter-5.74-461.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Exporter-5.74-461.el9.src.rpm
```

### `rpm` package: `perl-Fcntl-1.13-479.el9.x86_64`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Fcntl-1.13-479.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-File-Basename-2.85-479.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-File-Basename-2.85-479.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-File-Path-2.18-4.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-File-Path-2.18-4.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-File-Path-2.18-4.el9.src.rpm
```

### `rpm` package: `perl-File-Temp-0.231.100-4.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-File-Temp-0.231.100-4.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-File-Temp-0.231.100-4.el9.src.rpm
```

### `rpm` package: `perl-File-stat-1.09-479.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-File-stat-1.09-479.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-FileHandle-2.03-479.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-FileHandle-2.03-479.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-Getopt-Long-2.52-4.el9.noarch`

Licenses (from `rpm --query`): GPLv2+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Getopt-Long-2.52-4.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Getopt-Long-2.52-4.el9.src.rpm
```

### `rpm` package: `perl-Getopt-Std-1.12-479.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Getopt-Std-1.12-479.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-HTTP-Tiny-0.076-460.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-HTTP-Tiny-0.076-460.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-HTTP-Tiny-0.076-460.el9.src.rpm
```

### `rpm` package: `perl-IO-1.43-479.el9.x86_64`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-IO-1.43-479.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-IO-Socket-IP-0.41-5.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-IO-Socket-IP-0.41-5.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-IO-Socket-IP-0.41-5.el9.src.rpm
```

### `rpm` package: `perl-IO-Socket-SSL-2.073-1.el9.noarch`

Licenses (from `rpm --query`): (GPL+ or Artistic) and MPLv2.0

Source:

```console
$ dnf --quiet download --source --url perl-IO-Socket-SSL-2.073-1.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-IO-Socket-SSL-2.073-1.el9.src.rpm
```

### `rpm` package: `perl-IPC-Open3-1.21-479.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-IPC-Open3-1.21-479.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-MIME-Base64-3.16-4.el9.x86_64`

Licenses (from `rpm --query`): (GPL+ or Artistic) and MIT

Source:

```console
$ dnf --quiet download --source --url perl-MIME-Base64-3.16-4.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-MIME-Base64-3.16-4.el9.src.rpm
```

### `rpm` package: `perl-Mozilla-CA-20200520-6.el9.noarch`

Licenses (from `rpm --query`): MPLv2.0

Source:

```console
$ dnf --quiet download --source --url perl-Mozilla-CA-20200520-6.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Mozilla-CA-20200520-6.el9.src.rpm
```

### `rpm` package: `perl-NDBM_File-1.15-479.el9.x86_64`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-NDBM_File-1.15-479.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-Net-SSLeay-1.92-2.el9.x86_64`

Licenses (from `rpm --query`): Artistic 2.0

Source:

```console
$ dnf --quiet download --source --url perl-Net-SSLeay-1.92-2.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Net-SSLeay-1.92-2.el9.src.rpm
```

### `rpm` package: `perl-POSIX-1.94-479.el9.x86_64`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-POSIX-1.94-479.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-PathTools-3.78-461.el9.x86_64`

Licenses (from `rpm --query`): (GPL+ or Artistic) and BSD

Source:

```console
$ dnf --quiet download --source --url perl-PathTools-3.78-461.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-PathTools-3.78-461.el9.src.rpm
```

### `rpm` package: `perl-Pod-Escapes-1.07-460.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Pod-Escapes-1.07-460.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Pod-Escapes-1.07-460.el9.src.rpm
```

### `rpm` package: `perl-Pod-Perldoc-3.28.01-461.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Pod-Perldoc-3.28.01-461.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Pod-Perldoc-3.28.01-461.el9.src.rpm
```

### `rpm` package: `perl-Pod-Simple-3.42-4.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Pod-Simple-3.42-4.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Pod-Simple-3.42-4.el9.src.rpm
```

### `rpm` package: `perl-Pod-Usage-2.01-4.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Pod-Usage-2.01-4.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Pod-Usage-2.01-4.el9.src.rpm
```

### `rpm` package: `perl-Scalar-List-Utils-1.56-461.el9.x86_64`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Scalar-List-Utils-1.56-461.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Scalar-List-Utils-1.56-461.el9.src.rpm
```

### `rpm` package: `perl-SelectSaver-1.02-479.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-SelectSaver-1.02-479.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-Socket-2.031-4.el9.x86_64`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Socket-2.031-4.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Socket-2.031-4.el9.src.rpm
```

### `rpm` package: `perl-Storable-3.21-460.el9.x86_64`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Storable-3.21-460.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Storable-3.21-460.el9.src.rpm
```

### `rpm` package: `perl-Symbol-1.08-479.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Symbol-1.08-479.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-Term-ANSIColor-5.01-461.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Term-ANSIColor-5.01-461.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Term-ANSIColor-5.01-461.el9.src.rpm
```

### `rpm` package: `perl-Term-Cap-1.17-460.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Term-Cap-1.17-460.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Term-Cap-1.17-460.el9.src.rpm
```

### `rpm` package: `perl-Text-ParseWords-3.30-460.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Text-ParseWords-3.30-460.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Text-ParseWords-3.30-460.el9.src.rpm
```

### `rpm` package: `perl-Text-Tabs+Wrap-2013.0523-460.el9.noarch`

Licenses (from `rpm --query`): TTWL

Source:

```console
$ dnf --quiet download --source --url perl-Text-Tabs+Wrap-2013.0523-460.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Text-Tabs+Wrap-2013.0523-460.el9.src.rpm
```

### `rpm` package: `perl-Time-Local-1.300-7.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-Time-Local-1.300-7.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-Time-Local-1.300-7.el9.src.rpm
```

### `rpm` package: `perl-URI-5.09-3.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-URI-5.09-3.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-URI-5.09-3.el9.src.rpm
```

### `rpm` package: `perl-base-2.27-479.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-base-2.27-479.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-constant-1.33-461.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-constant-1.33-461.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-constant-1.33-461.el9.src.rpm
```

### `rpm` package: `perl-if-0.60.800-479.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-if-0.60.800-479.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-interpreter-5.32.1-479.el9.x86_64`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-interpreter-5.32.1-479.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-libnet-3.13-4.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-libnet-3.13-4.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-libnet-3.13-4.el9.src.rpm
```

### `rpm` package: `perl-libs-5.32.1-479.el9.x86_64`

Licenses (from `rpm --query`): (GPL+ or Artistic) and BSD and HSRL and MIT and UCD and Public domain

Source:

```console
$ dnf --quiet download --source --url perl-libs-5.32.1-479.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-mro-1.23-479.el9.x86_64`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-mro-1.23-479.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-overload-1.31-479.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-overload-1.31-479.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-overloading-0.02-479.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-overloading-0.02-479.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-parent-0.238-460.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-parent-0.238-460.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-parent-0.238-460.el9.src.rpm
```

### `rpm` package: `perl-podlators-4.14-460.el9.noarch`

Licenses (from `rpm --query`): (GPL+ or Artistic) and FSFAP

Source:

```console
$ dnf --quiet download --source --url perl-podlators-4.14-460.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-podlators-4.14-460.el9.src.rpm
```

### `rpm` package: `perl-subs-1.03-479.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-subs-1.03-479.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `perl-vars-1.05-479.el9.noarch`

Licenses (from `rpm --query`): GPL+ or Artistic

Source:

```console
$ dnf --quiet download --source --url perl-vars-1.05-479.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/perl-5.32.1-479.el9.src.rpm
```

### `rpm` package: `pkgconf-1.7.3-9.el9.x86_64`

Licenses (from `rpm --query`): ISC

Source:

```console
$ dnf --quiet download --source --url pkgconf-1.7.3-9.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/pkgconf-1.7.3-9.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/pkgconf-1.7.3-9.el9.src.rpm
```

### `rpm` package: `pkgconf-m4-1.7.3-9.el9.noarch`

Licenses (from `rpm --query`): GPLv2+ with exceptions

Source:

```console
$ dnf --quiet download --source --url pkgconf-m4-1.7.3-9.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/pkgconf-1.7.3-9.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/pkgconf-1.7.3-9.el9.src.rpm
```

### `rpm` package: `pkgconf-pkg-config-1.7.3-9.el9.x86_64`

Licenses (from `rpm --query`): ISC

Source:

```console
$ dnf --quiet download --source --url pkgconf-pkg-config-1.7.3-9.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/pkgconf-1.7.3-9.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/pkgconf-1.7.3-9.el9.src.rpm
```

### `rpm` package: `policycoreutils-3.4-4.el9.x86_64`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ dnf --quiet download --source --url policycoreutils-3.4-4.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/policycoreutils-3.4-4.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/policycoreutils-3.4-4.el9.src.rpm
```

### `rpm` package: `popt-1.18-8.el9.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url popt-1.18-8.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/popt-1.18-8.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/popt-1.18-8.el9.src.rpm
```

### `rpm` package: `procps-ng-3.3.17-8.el9.x86_64`

Licenses (from `rpm --query`): GPL+ and GPLv2 and GPLv2+ and GPLv3+ and LGPLv2+

Source:

```console
$ dnf --quiet download --source --url procps-ng-3.3.17-8.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/procps-ng-3.3.17-8.el9.src.rpm
```

### `rpm` package: `psmisc-23.4-3.el9.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url psmisc-23.4-3.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/psmisc-23.4-3.el9.src.rpm
```

### `rpm` package: `publicsuffix-list-dafsa-20210518-3.el9.noarch`

Licenses (from `rpm --query`): MPLv2.0

Source:

```console
$ dnf --quiet download --source --url publicsuffix-list-dafsa-20210518-3.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/publicsuffix-list-20210518-3.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/publicsuffix-list-20210518-3.el9.src.rpm
```

### `rpm` package: `python3-3.9.14-1.el9_1.2.x86_64`

Licenses (from `rpm --query`): Python

Source:

```console
$ dnf --quiet download --source --url python3-3.9.14-1.el9_1.2
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/python3.9-3.9.14-1.el9_1.2.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/python3.9-3.9.14-1.el9_1.2.src.rpm
```

### `rpm` package: `python3-dateutil-2.8.1-6.el9.noarch`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url python3-dateutil-2.8.1-6.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/python-dateutil-2.8.1-6.el9.src.rpm
```

### `rpm` package: `python3-dbus-1.2.18-2.el9.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url python3-dbus-1.2.18-2.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/dbus-python-1.2.18-2.el9.src.rpm
```

### `rpm` package: `python3-dnf-4.12.0-4.0.1.el9.noarch`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url python3-dnf-4.12.0-4.0.1.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/dnf-4.12.0-4.0.1.el9.src.rpm
```

### `rpm` package: `python3-dnf-plugins-core-4.1.0-3.0.1.el9.noarch`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url python3-dnf-plugins-core-4.1.0-3.0.1.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/dnf-plugins-core-4.1.0-3.0.1.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/dnf-plugins-core-4.1.0-3.0.1.el9.src.rpm
```

### `rpm` package: `python3-gpg-1.15.1-6.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and GPLv3+

Source:

```console
$ dnf --quiet download --source --url python3-gpg-1.15.1-6.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/gpgme-1.15.1-6.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/gpgme-1.15.1-6.el9.src.rpm
```

### `rpm` package: `python3-hawkey-0.67.0-3.0.1.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url python3-hawkey-0.67.0-3.0.1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libdnf-0.67.0-3.0.1.el9.src.rpm
```

### `rpm` package: `python3-libcomps-0.1.18-1.el9.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url python3-libcomps-0.1.18-1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libcomps-0.1.18-1.el9.src.rpm
```

### `rpm` package: `python3-libdnf-0.67.0-3.0.1.el9.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url python3-libdnf-0.67.0-3.0.1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/libdnf-0.67.0-3.0.1.el9.src.rpm
```

### `rpm` package: `python3-libs-3.9.14-1.el9_1.2.x86_64`

Licenses (from `rpm --query`): Python

Source:

```console
$ dnf --quiet download --source --url python3-libs-3.9.14-1.el9_1.2
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/python3.9-3.9.14-1.el9_1.2.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/python3.9-3.9.14-1.el9_1.2.src.rpm
```

### `rpm` package: `python3-pip-wheel-21.2.3-6.el9.noarch`

Licenses (from `rpm --query`): MIT and Python and ASL 2.0 and BSD and ISC and LGPLv2 and MPLv2.0 and (ASL 2.0 or BSD)

Source:

```console
$ dnf --quiet download --source --url python3-pip-wheel-21.2.3-6.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/python-pip-21.2.3-6.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/python-pip-21.2.3-6.el9.src.rpm
```

### `rpm` package: `python3-rpm-4.16.1.3-19.0.1.el9_1.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url python3-rpm-4.16.1.3-19.0.1.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/rpm-4.16.1.3-19.0.1.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/rpm-4.16.1.3-19.0.1.el9_1.src.rpm
```

### `rpm` package: `python3-setuptools-wheel-53.0.0-10.el9_1.1.noarch`

Licenses (from `rpm --query`): MIT and (BSD or ASL 2.0)

Source:

```console
$ dnf --quiet download --source --url python3-setuptools-wheel-53.0.0-10.el9_1.1.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/python-setuptools-53.0.0-10.el9_1.1.src.rpm
```

### `rpm` package: `python3-six-1.15.0-9.0.1.el9.noarch`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url python3-six-1.15.0-9.0.1.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/python-six-1.15.0-9.0.1.el9.src.rpm
```

### `rpm` package: `readline-8.1-4.el9.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url readline-8.1-4.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/readline-8.1-4.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/readline-8.1-4.el9.src.rpm
```

### `rpm` package: `redhat-release-9.1-1.9.0.1.el9.x86_64`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ dnf --quiet download --source --url redhat-release-9.1-1.9.0.1.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/redhat-release-9.1-1.9.0.1.el9.src.rpm
```

### `rpm` package: `rootfiles-8.1-31.el9.noarch`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url rootfiles-8.1-31.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/rootfiles-8.1-31.el9.src.rpm
```

### `rpm` package: `rpm-4.16.1.3-19.0.1.el9_1.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url rpm-4.16.1.3-19.0.1.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/rpm-4.16.1.3-19.0.1.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/rpm-4.16.1.3-19.0.1.el9_1.src.rpm
```

### `rpm` package: `rpm-build-libs-4.16.1.3-19.0.1.el9_1.x86_64`

Licenses (from `rpm --query`): GPLv2+ and LGPLv2+ with exceptions

Source:

```console
$ dnf --quiet download --source --url rpm-build-libs-4.16.1.3-19.0.1.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/rpm-4.16.1.3-19.0.1.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/rpm-4.16.1.3-19.0.1.el9_1.src.rpm
```

### `rpm` package: `rpm-libs-4.16.1.3-19.0.1.el9_1.x86_64`

Licenses (from `rpm --query`): GPLv2+ and LGPLv2+ with exceptions

Source:

```console
$ dnf --quiet download --source --url rpm-libs-4.16.1.3-19.0.1.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/rpm-4.16.1.3-19.0.1.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/rpm-4.16.1.3-19.0.1.el9_1.src.rpm
```

### `rpm` package: `rpm-sign-libs-4.16.1.3-19.0.1.el9_1.x86_64`

Licenses (from `rpm --query`): GPLv2+ and LGPLv2+ with exceptions

Source:

```console
$ dnf --quiet download --source --url rpm-sign-libs-4.16.1.3-19.0.1.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/rpm-4.16.1.3-19.0.1.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/rpm-4.16.1.3-19.0.1.el9_1.src.rpm
```

### `rpm` package: `rsyslog-8.2102.0-105.el9.x86_64`

Licenses (from `rpm --query`): (GPLv3+ and ASL 2.0)

Source:

```console
$ dnf --quiet download --source --url rsyslog-8.2102.0-105.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/rsyslog-8.2102.0-105.el9.src.rpm
```

### `rpm` package: `sed-4.8-9.el9.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url sed-4.8-9.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/sed-4.8-9.el9.src.rpm
```

### `rpm` package: `setup-2.13.7-7.el9.noarch`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url setup-2.13.7-7.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/setup-2.13.7-7.el9.src.rpm
```

### `rpm` package: `shadow-utils-4.9-5.el9.x86_64`

Licenses (from `rpm --query`): BSD and GPLv2+

Source:

```console
$ dnf --quiet download --source --url shadow-utils-4.9-5.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/shadow-utils-4.9-5.el9.src.rpm
```

### `rpm` package: `sqlite-libs-3.34.1-6.el9_1.x86_64`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url sqlite-libs-3.34.1-6.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/sqlite-3.34.1-6.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/sqlite-3.34.1-6.el9_1.src.rpm
```

### `rpm` package: `systemd-250-12.0.2.el9_1.3.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and MIT and GPLv2+

Source:

```console
$ dnf --quiet download --source --url systemd-250-12.0.2.el9_1.3
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/systemd-250-12.0.2.el9_1.3.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/systemd-250-12.0.2.el9_1.3.src.rpm
```

### `rpm` package: `systemd-libs-250-12.0.2.el9_1.3.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and MIT

Source:

```console
$ dnf --quiet download --source --url systemd-libs-250-12.0.2.el9_1.3
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/systemd-250-12.0.2.el9_1.3.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/systemd-250-12.0.2.el9_1.3.src.rpm
```

### `rpm` package: `systemd-pam-250-12.0.2.el9_1.3.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and MIT and GPLv2+

Source:

```console
$ dnf --quiet download --source --url systemd-pam-250-12.0.2.el9_1.3
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/systemd-250-12.0.2.el9_1.3.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/systemd-250-12.0.2.el9_1.3.src.rpm
```

### `rpm` package: `systemd-rpm-macros-250-12.0.2.el9_1.3.noarch`

Licenses (from `rpm --query`): LGPLv2+ and MIT and GPLv2+

Source:

```console
$ dnf --quiet download --source --url systemd-rpm-macros-250-12.0.2.el9_1.3.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/systemd-250-12.0.2.el9_1.3.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/systemd-250-12.0.2.el9_1.3.src.rpm
```

### `rpm` package: `tar-1.34-6.el9_1.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url tar-1.34-6.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/tar-1.34-6.el9_1.src.rpm
```

### `rpm` package: `tpm2-tss-3.0.3-8.el9.x86_64`

Licenses (from `rpm --query`): BSD and TCGL

Source:

```console
$ dnf --quiet download --source --url tpm2-tss-3.0.3-8.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/tpm2-tss-3.0.3-8.el9.src.rpm
```

### `rpm` package: `tzdata-2023c-1.el9.noarch`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url tzdata-2023c-1.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/tzdata-2023c-1.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/tzdata-2023c-1.el9.src.rpm
```

### `rpm` package: `util-linux-2.37.4-9.el9.x86_64`

Licenses (from `rpm --query`): GPLv2 and GPLv2+ and LGPLv2+ and BSD with advertising and Public Domain

Source:

```console
$ dnf --quiet download --source --url util-linux-2.37.4-9.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/util-linux-2.37.4-9.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/util-linux-2.37.4-9.el9.src.rpm
```

### `rpm` package: `util-linux-core-2.37.4-9.el9.x86_64`

Licenses (from `rpm --query`): GPLv2 and GPLv2+ and LGPLv2+ and BSD with advertising and Public Domain

Source:

```console
$ dnf --quiet download --source --url util-linux-core-2.37.4-9.el9
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/util-linux-2.37.4-9.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/util-linux-2.37.4-9.el9.src.rpm
```

### `rpm` package: `vim-minimal-8.2.2637-20.0.1.el9_1.x86_64`

Licenses (from `rpm --query`): Vim and MIT

Source:

```console
$ dnf --quiet download --source --url vim-minimal-8.2.2637-20.0.1.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/vim-8.2.2637-20.0.1.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/vim-8.2.2637-20.0.1.el9_1.src.rpm
```

### `rpm` package: `which-2.21-28.el9.x86_64`

Licenses (from `rpm --query`): GPLv3

Source:

```console
$ dnf --quiet download --source --url which-2.21-28.el9
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/which-2.21-28.el9.src.rpm
```

### `rpm` package: `xz-libs-5.2.5-8.el9_0.x86_64`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url xz-libs-5.2.5-8.el9_0
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/xz-5.2.5-8.el9_0.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/xz-5.2.5-8.el9_0.src.rpm
```

### `rpm` package: `yum-4.12.0-4.0.1.el9.noarch`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url yum-4.12.0-4.0.1.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/dnf-4.12.0-4.0.1.el9.src.rpm
```

### `rpm` package: `yum-utils-4.1.0-3.0.1.el9.noarch`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url yum-utils-4.1.0-3.0.1.el9.noarch
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/dnf-plugins-core-4.1.0-3.0.1.el9.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/dnf-plugins-core-4.1.0-3.0.1.el9.src.rpm
```

### `rpm` package: `zlib-1.2.11-35.el9_1.x86_64`

Licenses (from `rpm --query`): zlib and Boost

Source:

```console
$ dnf --quiet download --source --url zlib-1.2.11-35.el9_1
https://yum.oracle.com/repo/OracleLinux/OL9/appstream/x86_64/getPackageSource/zlib-1.2.11-35.el9_1.src.rpm
https://yum.oracle.com/repo/OracleLinux/OL9/baseos/latest/x86_64/getPackageSource/zlib-1.2.11-35.el9_1.src.rpm
```
