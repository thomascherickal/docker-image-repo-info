<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `percona`

-	[`percona:5`](#percona5)
-	[`percona:5.6`](#percona56)
-	[`percona:5.6.51`](#percona5651)
-	[`percona:5.6.51-centos`](#percona5651-centos)
-	[`percona:5.6-centos`](#percona56-centos)
-	[`percona:5.7`](#percona57)
-	[`percona:5.7.32`](#percona5732)
-	[`percona:5.7.32-centos`](#percona5732-centos)
-	[`percona:5.7-centos`](#percona57-centos)
-	[`percona:5-centos`](#percona5-centos)
-	[`percona:8`](#percona8)
-	[`percona:8.0`](#percona80)
-	[`percona:8.0.22-13`](#percona8022-13)
-	[`percona:8.0.22-13-centos`](#percona8022-13-centos)
-	[`percona:8.0-centos`](#percona80-centos)
-	[`percona:8-centos`](#percona8-centos)
-	[`percona:centos`](#perconacentos)
-	[`percona:latest`](#perconalatest)
-	[`percona:ps-5`](#perconaps-5)
-	[`percona:ps-5.6`](#perconaps-56)
-	[`percona:ps-5.6.51`](#perconaps-5651)
-	[`percona:ps-5.7`](#perconaps-57)
-	[`percona:ps-5.7.32`](#perconaps-5732)
-	[`percona:ps-8`](#perconaps-8)
-	[`percona:ps-8.0`](#perconaps-80)
-	[`percona:ps-8.0.22-13`](#perconaps-8022-13)
-	[`percona:psmdb-3.6`](#perconapsmdb-36)
-	[`percona:psmdb-3.6.21`](#perconapsmdb-3621)
-	[`percona:psmdb-4.0`](#perconapsmdb-40)
-	[`percona:psmdb-4.0.22`](#perconapsmdb-4022)
-	[`percona:psmdb-4.2`](#perconapsmdb-42)
-	[`percona:psmdb-4.2.12`](#perconapsmdb-4212)
-	[`percona:psmdb-4.4`](#perconapsmdb-44)
-	[`percona:psmdb-4.4.3`](#perconapsmdb-443)

## `percona:5`

```console
$ docker pull percona@sha256:358eff0fa5115958da5e913c56f6420cfe5a2102dde63f8b06bbc24566893916
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5` - linux; amd64

```console
$ docker pull percona@sha256:00e206b1ddc71450a885624a9bfab84b4281b0d4b07699a22d4fc47bcfa44b52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.5 MB (220519463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41370b19b67aa296306b0172907bb8058e50086190a13b3390985c57bcbef8b9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:59 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Tue, 08 Dec 2020 00:49:15 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Tue, 08 Dec 2020 00:49:16 GMT
ENV PS_VERSION=5.7.32-35.1
# Tue, 08 Dec 2020 00:49:16 GMT
ENV OS_VER=el8
# Tue, 08 Dec 2020 00:49:17 GMT
ENV FULL_PERCONA_VERSION=5.7.32-35.1.el8
# Tue, 08 Dec 2020 00:49:43 GMT
RUN set -ex;     dnf install -y         dnf-utils         jemalloc         cracklib-dicts         which;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         selinux-policy             | xargs curl -Lf -o /tmp/selinux-policy.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm --nodeps;     rm -rf /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm;         dnf install -y         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf remove -y dnf-utils;     dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Tue, 08 Dec 2020 00:49:44 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 08 Dec 2020 00:49:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 08 Dec 2020 00:49:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 08 Dec 2020 00:49:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Dec 2020 00:49:45 GMT
USER mysql
# Tue, 08 Dec 2020 00:49:45 GMT
EXPOSE 3306
# Tue, 08 Dec 2020 00:49:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205beaf4be145d43ce7f738775ac25339927be11e45ec9d34fd8dd5538c9ef66`  
		Last Modified: Tue, 08 Dec 2020 00:53:46 GMT  
		Size: 1.5 KB (1541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be50bbff9088000f27631eb27c12dece641c44fc636f08d894c80cc2ce6e90f`  
		Last Modified: Tue, 08 Dec 2020 00:53:48 GMT  
		Size: 30.4 MB (30388488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560824284de3bdd0da4b80fca9717c986cc0bc3b7f2780096ab57bcbaf6cc7b1`  
		Last Modified: Tue, 08 Dec 2020 00:54:09 GMT  
		Size: 114.9 MB (114942980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbdf23842a16bd108ccb1cd247bbd06fec10094a7ac2236d4916bb1890e077c`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc7f9b3a007572a65eeb7d21136c59f339f5b505d1ffb5ee9b0575db9416de8`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6`

```console
$ docker pull percona@sha256:b6bc17e2a4572723e3fe86f9238afcfb7c6dd3d257d2db6b86f8b0938227ce52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.6` - linux; amd64

```console
$ docker pull percona@sha256:09ccce2f3d13b37c5cbdc75854c8ad6efbf35afdabd0dd2181f1859481cf9258
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.7 MB (140734318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3700cad0b44abb340f3f0a468fccfb8c4e273265179ead0894cb29dfd3eca3a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 14 Nov 2020 00:45:10 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 14 Nov 2020 00:45:42 GMT
RUN groupdel input && groupadd -g 999 mysql
# Sat, 14 Nov 2020 00:45:43 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Wed, 25 Nov 2020 22:23:27 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Thu, 26 Nov 2020 18:22:05 GMT
ENV PERCONA_VERSION=5.6.50-rel90.0.1.el7
# Thu, 26 Nov 2020 18:22:46 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 26 Nov 2020 18:22:47 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 26 Nov 2020 18:22:47 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 26 Nov 2020 18:22:47 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Thu, 26 Nov 2020 18:22:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 26 Nov 2020 18:22:47 GMT
USER mysql
# Thu, 26 Nov 2020 18:22:48 GMT
EXPOSE 3306
# Thu, 26 Nov 2020 18:22:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75e5924dc16b794b9dfe808be3f7a247acec59d0e0b5ba0e0007e86073e80d9`  
		Last Modified: Sat, 14 Nov 2020 00:47:52 GMT  
		Size: 541.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60550dc8778b2360245b3a4a2609bc9b2e1415c8795d27812232246892a8dba3`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebce5663c9fe5c45da8b16ddad68e6088d75046395dc267f948f8b3390b1efcf`  
		Last Modified: Thu, 26 Nov 2020 18:23:57 GMT  
		Size: 6.6 MB (6562458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140c3608c6243c53a4c59d253c86d1c5df95e005713600442016d48aaecc87a9`  
		Last Modified: Thu, 26 Nov 2020 18:24:06 GMT  
		Size: 58.1 MB (58064791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2f7710126bd9cb3df7dc98a6a7e6559f7e6617e9c63265c22dd342c40b6d14`  
		Last Modified: Thu, 26 Nov 2020 18:23:55 GMT  
		Size: 4.9 KB (4878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf0f791d44e94b8100317f9d42ac785f4421b4230301e34ffac891bb8579125`  
		Last Modified: Thu, 26 Nov 2020 18:23:55 GMT  
		Size: 2.9 KB (2940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6.51`

```console
$ docker pull percona@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `percona:5.6.51-centos`

```console
$ docker pull percona@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `percona:5.6-centos`

```console
$ docker pull percona@sha256:b6bc17e2a4572723e3fe86f9238afcfb7c6dd3d257d2db6b86f8b0938227ce52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.6-centos` - linux; amd64

```console
$ docker pull percona@sha256:09ccce2f3d13b37c5cbdc75854c8ad6efbf35afdabd0dd2181f1859481cf9258
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.7 MB (140734318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3700cad0b44abb340f3f0a468fccfb8c4e273265179ead0894cb29dfd3eca3a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 14 Nov 2020 00:45:10 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 14 Nov 2020 00:45:42 GMT
RUN groupdel input && groupadd -g 999 mysql
# Sat, 14 Nov 2020 00:45:43 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Wed, 25 Nov 2020 22:23:27 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Thu, 26 Nov 2020 18:22:05 GMT
ENV PERCONA_VERSION=5.6.50-rel90.0.1.el7
# Thu, 26 Nov 2020 18:22:46 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 26 Nov 2020 18:22:47 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 26 Nov 2020 18:22:47 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 26 Nov 2020 18:22:47 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Thu, 26 Nov 2020 18:22:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 26 Nov 2020 18:22:47 GMT
USER mysql
# Thu, 26 Nov 2020 18:22:48 GMT
EXPOSE 3306
# Thu, 26 Nov 2020 18:22:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75e5924dc16b794b9dfe808be3f7a247acec59d0e0b5ba0e0007e86073e80d9`  
		Last Modified: Sat, 14 Nov 2020 00:47:52 GMT  
		Size: 541.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60550dc8778b2360245b3a4a2609bc9b2e1415c8795d27812232246892a8dba3`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebce5663c9fe5c45da8b16ddad68e6088d75046395dc267f948f8b3390b1efcf`  
		Last Modified: Thu, 26 Nov 2020 18:23:57 GMT  
		Size: 6.6 MB (6562458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140c3608c6243c53a4c59d253c86d1c5df95e005713600442016d48aaecc87a9`  
		Last Modified: Thu, 26 Nov 2020 18:24:06 GMT  
		Size: 58.1 MB (58064791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2f7710126bd9cb3df7dc98a6a7e6559f7e6617e9c63265c22dd342c40b6d14`  
		Last Modified: Thu, 26 Nov 2020 18:23:55 GMT  
		Size: 4.9 KB (4878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf0f791d44e94b8100317f9d42ac785f4421b4230301e34ffac891bb8579125`  
		Last Modified: Thu, 26 Nov 2020 18:23:55 GMT  
		Size: 2.9 KB (2940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7`

```console
$ docker pull percona@sha256:358eff0fa5115958da5e913c56f6420cfe5a2102dde63f8b06bbc24566893916
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7` - linux; amd64

```console
$ docker pull percona@sha256:00e206b1ddc71450a885624a9bfab84b4281b0d4b07699a22d4fc47bcfa44b52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.5 MB (220519463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41370b19b67aa296306b0172907bb8058e50086190a13b3390985c57bcbef8b9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:59 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Tue, 08 Dec 2020 00:49:15 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Tue, 08 Dec 2020 00:49:16 GMT
ENV PS_VERSION=5.7.32-35.1
# Tue, 08 Dec 2020 00:49:16 GMT
ENV OS_VER=el8
# Tue, 08 Dec 2020 00:49:17 GMT
ENV FULL_PERCONA_VERSION=5.7.32-35.1.el8
# Tue, 08 Dec 2020 00:49:43 GMT
RUN set -ex;     dnf install -y         dnf-utils         jemalloc         cracklib-dicts         which;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         selinux-policy             | xargs curl -Lf -o /tmp/selinux-policy.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm --nodeps;     rm -rf /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm;         dnf install -y         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf remove -y dnf-utils;     dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Tue, 08 Dec 2020 00:49:44 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 08 Dec 2020 00:49:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 08 Dec 2020 00:49:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 08 Dec 2020 00:49:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Dec 2020 00:49:45 GMT
USER mysql
# Tue, 08 Dec 2020 00:49:45 GMT
EXPOSE 3306
# Tue, 08 Dec 2020 00:49:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205beaf4be145d43ce7f738775ac25339927be11e45ec9d34fd8dd5538c9ef66`  
		Last Modified: Tue, 08 Dec 2020 00:53:46 GMT  
		Size: 1.5 KB (1541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be50bbff9088000f27631eb27c12dece641c44fc636f08d894c80cc2ce6e90f`  
		Last Modified: Tue, 08 Dec 2020 00:53:48 GMT  
		Size: 30.4 MB (30388488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560824284de3bdd0da4b80fca9717c986cc0bc3b7f2780096ab57bcbaf6cc7b1`  
		Last Modified: Tue, 08 Dec 2020 00:54:09 GMT  
		Size: 114.9 MB (114942980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbdf23842a16bd108ccb1cd247bbd06fec10094a7ac2236d4916bb1890e077c`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc7f9b3a007572a65eeb7d21136c59f339f5b505d1ffb5ee9b0575db9416de8`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.32`

```console
$ docker pull percona@sha256:358eff0fa5115958da5e913c56f6420cfe5a2102dde63f8b06bbc24566893916
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7.32` - linux; amd64

```console
$ docker pull percona@sha256:00e206b1ddc71450a885624a9bfab84b4281b0d4b07699a22d4fc47bcfa44b52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.5 MB (220519463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41370b19b67aa296306b0172907bb8058e50086190a13b3390985c57bcbef8b9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:59 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Tue, 08 Dec 2020 00:49:15 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Tue, 08 Dec 2020 00:49:16 GMT
ENV PS_VERSION=5.7.32-35.1
# Tue, 08 Dec 2020 00:49:16 GMT
ENV OS_VER=el8
# Tue, 08 Dec 2020 00:49:17 GMT
ENV FULL_PERCONA_VERSION=5.7.32-35.1.el8
# Tue, 08 Dec 2020 00:49:43 GMT
RUN set -ex;     dnf install -y         dnf-utils         jemalloc         cracklib-dicts         which;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         selinux-policy             | xargs curl -Lf -o /tmp/selinux-policy.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm --nodeps;     rm -rf /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm;         dnf install -y         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf remove -y dnf-utils;     dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Tue, 08 Dec 2020 00:49:44 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 08 Dec 2020 00:49:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 08 Dec 2020 00:49:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 08 Dec 2020 00:49:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Dec 2020 00:49:45 GMT
USER mysql
# Tue, 08 Dec 2020 00:49:45 GMT
EXPOSE 3306
# Tue, 08 Dec 2020 00:49:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205beaf4be145d43ce7f738775ac25339927be11e45ec9d34fd8dd5538c9ef66`  
		Last Modified: Tue, 08 Dec 2020 00:53:46 GMT  
		Size: 1.5 KB (1541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be50bbff9088000f27631eb27c12dece641c44fc636f08d894c80cc2ce6e90f`  
		Last Modified: Tue, 08 Dec 2020 00:53:48 GMT  
		Size: 30.4 MB (30388488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560824284de3bdd0da4b80fca9717c986cc0bc3b7f2780096ab57bcbaf6cc7b1`  
		Last Modified: Tue, 08 Dec 2020 00:54:09 GMT  
		Size: 114.9 MB (114942980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbdf23842a16bd108ccb1cd247bbd06fec10094a7ac2236d4916bb1890e077c`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc7f9b3a007572a65eeb7d21136c59f339f5b505d1ffb5ee9b0575db9416de8`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.32-centos`

```console
$ docker pull percona@sha256:358eff0fa5115958da5e913c56f6420cfe5a2102dde63f8b06bbc24566893916
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7.32-centos` - linux; amd64

```console
$ docker pull percona@sha256:00e206b1ddc71450a885624a9bfab84b4281b0d4b07699a22d4fc47bcfa44b52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.5 MB (220519463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41370b19b67aa296306b0172907bb8058e50086190a13b3390985c57bcbef8b9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:59 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Tue, 08 Dec 2020 00:49:15 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Tue, 08 Dec 2020 00:49:16 GMT
ENV PS_VERSION=5.7.32-35.1
# Tue, 08 Dec 2020 00:49:16 GMT
ENV OS_VER=el8
# Tue, 08 Dec 2020 00:49:17 GMT
ENV FULL_PERCONA_VERSION=5.7.32-35.1.el8
# Tue, 08 Dec 2020 00:49:43 GMT
RUN set -ex;     dnf install -y         dnf-utils         jemalloc         cracklib-dicts         which;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         selinux-policy             | xargs curl -Lf -o /tmp/selinux-policy.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm --nodeps;     rm -rf /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm;         dnf install -y         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf remove -y dnf-utils;     dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Tue, 08 Dec 2020 00:49:44 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 08 Dec 2020 00:49:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 08 Dec 2020 00:49:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 08 Dec 2020 00:49:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Dec 2020 00:49:45 GMT
USER mysql
# Tue, 08 Dec 2020 00:49:45 GMT
EXPOSE 3306
# Tue, 08 Dec 2020 00:49:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205beaf4be145d43ce7f738775ac25339927be11e45ec9d34fd8dd5538c9ef66`  
		Last Modified: Tue, 08 Dec 2020 00:53:46 GMT  
		Size: 1.5 KB (1541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be50bbff9088000f27631eb27c12dece641c44fc636f08d894c80cc2ce6e90f`  
		Last Modified: Tue, 08 Dec 2020 00:53:48 GMT  
		Size: 30.4 MB (30388488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560824284de3bdd0da4b80fca9717c986cc0bc3b7f2780096ab57bcbaf6cc7b1`  
		Last Modified: Tue, 08 Dec 2020 00:54:09 GMT  
		Size: 114.9 MB (114942980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbdf23842a16bd108ccb1cd247bbd06fec10094a7ac2236d4916bb1890e077c`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc7f9b3a007572a65eeb7d21136c59f339f5b505d1ffb5ee9b0575db9416de8`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7-centos`

```console
$ docker pull percona@sha256:358eff0fa5115958da5e913c56f6420cfe5a2102dde63f8b06bbc24566893916
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7-centos` - linux; amd64

```console
$ docker pull percona@sha256:00e206b1ddc71450a885624a9bfab84b4281b0d4b07699a22d4fc47bcfa44b52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.5 MB (220519463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41370b19b67aa296306b0172907bb8058e50086190a13b3390985c57bcbef8b9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:59 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Tue, 08 Dec 2020 00:49:15 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Tue, 08 Dec 2020 00:49:16 GMT
ENV PS_VERSION=5.7.32-35.1
# Tue, 08 Dec 2020 00:49:16 GMT
ENV OS_VER=el8
# Tue, 08 Dec 2020 00:49:17 GMT
ENV FULL_PERCONA_VERSION=5.7.32-35.1.el8
# Tue, 08 Dec 2020 00:49:43 GMT
RUN set -ex;     dnf install -y         dnf-utils         jemalloc         cracklib-dicts         which;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         selinux-policy             | xargs curl -Lf -o /tmp/selinux-policy.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm --nodeps;     rm -rf /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm;         dnf install -y         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf remove -y dnf-utils;     dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Tue, 08 Dec 2020 00:49:44 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 08 Dec 2020 00:49:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 08 Dec 2020 00:49:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 08 Dec 2020 00:49:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Dec 2020 00:49:45 GMT
USER mysql
# Tue, 08 Dec 2020 00:49:45 GMT
EXPOSE 3306
# Tue, 08 Dec 2020 00:49:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205beaf4be145d43ce7f738775ac25339927be11e45ec9d34fd8dd5538c9ef66`  
		Last Modified: Tue, 08 Dec 2020 00:53:46 GMT  
		Size: 1.5 KB (1541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be50bbff9088000f27631eb27c12dece641c44fc636f08d894c80cc2ce6e90f`  
		Last Modified: Tue, 08 Dec 2020 00:53:48 GMT  
		Size: 30.4 MB (30388488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560824284de3bdd0da4b80fca9717c986cc0bc3b7f2780096ab57bcbaf6cc7b1`  
		Last Modified: Tue, 08 Dec 2020 00:54:09 GMT  
		Size: 114.9 MB (114942980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbdf23842a16bd108ccb1cd247bbd06fec10094a7ac2236d4916bb1890e077c`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc7f9b3a007572a65eeb7d21136c59f339f5b505d1ffb5ee9b0575db9416de8`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5-centos`

```console
$ docker pull percona@sha256:358eff0fa5115958da5e913c56f6420cfe5a2102dde63f8b06bbc24566893916
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5-centos` - linux; amd64

```console
$ docker pull percona@sha256:00e206b1ddc71450a885624a9bfab84b4281b0d4b07699a22d4fc47bcfa44b52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.5 MB (220519463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41370b19b67aa296306b0172907bb8058e50086190a13b3390985c57bcbef8b9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:59 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Tue, 08 Dec 2020 00:49:15 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Tue, 08 Dec 2020 00:49:16 GMT
ENV PS_VERSION=5.7.32-35.1
# Tue, 08 Dec 2020 00:49:16 GMT
ENV OS_VER=el8
# Tue, 08 Dec 2020 00:49:17 GMT
ENV FULL_PERCONA_VERSION=5.7.32-35.1.el8
# Tue, 08 Dec 2020 00:49:43 GMT
RUN set -ex;     dnf install -y         dnf-utils         jemalloc         cracklib-dicts         which;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         selinux-policy             | xargs curl -Lf -o /tmp/selinux-policy.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm --nodeps;     rm -rf /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm;         dnf install -y         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf remove -y dnf-utils;     dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Tue, 08 Dec 2020 00:49:44 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 08 Dec 2020 00:49:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 08 Dec 2020 00:49:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 08 Dec 2020 00:49:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Dec 2020 00:49:45 GMT
USER mysql
# Tue, 08 Dec 2020 00:49:45 GMT
EXPOSE 3306
# Tue, 08 Dec 2020 00:49:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205beaf4be145d43ce7f738775ac25339927be11e45ec9d34fd8dd5538c9ef66`  
		Last Modified: Tue, 08 Dec 2020 00:53:46 GMT  
		Size: 1.5 KB (1541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be50bbff9088000f27631eb27c12dece641c44fc636f08d894c80cc2ce6e90f`  
		Last Modified: Tue, 08 Dec 2020 00:53:48 GMT  
		Size: 30.4 MB (30388488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560824284de3bdd0da4b80fca9717c986cc0bc3b7f2780096ab57bcbaf6cc7b1`  
		Last Modified: Tue, 08 Dec 2020 00:54:09 GMT  
		Size: 114.9 MB (114942980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbdf23842a16bd108ccb1cd247bbd06fec10094a7ac2236d4916bb1890e077c`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc7f9b3a007572a65eeb7d21136c59f339f5b505d1ffb5ee9b0575db9416de8`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8`

```console
$ docker pull percona@sha256:d5d76334aa84c239fde43a2d2331d9bc268acec1702632d1741037a80419dda3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8` - linux; amd64

```console
$ docker pull percona@sha256:5bbb24c3ff580b9feebf71f4a2df037fa26adacc8cd73b52ff5911fd89fa2b6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.5 MB (239482162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef86f7cd16d0a330e95d544ac8d2972013aeea59202bf620660b1330103584f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:04 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 08 Dec 2020 00:48:12 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 14 Dec 2020 21:36:41 GMT
ENV PS_VERSION=8.0.22-13.1
# Mon, 14 Dec 2020 21:36:41 GMT
ENV OS_VER=el8
# Mon, 14 Dec 2020 21:36:41 GMT
ENV FULL_PERCONA_VERSION=8.0.22-13.1.el8
# Mon, 14 Dec 2020 21:37:14 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 14 Dec 2020 21:37:15 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 14 Dec 2020 21:37:15 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 14 Dec 2020 21:37:16 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 14 Dec 2020 21:37:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Dec 2020 21:37:16 GMT
USER mysql
# Mon, 14 Dec 2020 21:37:16 GMT
EXPOSE 3306 33060
# Mon, 14 Dec 2020 21:37:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ce9644bc2779e06cc0a9ac9a86e9f4981ba7c6f0274fb87a2d59b1e9f47f44`  
		Last Modified: Tue, 08 Dec 2020 00:53:09 GMT  
		Size: 1.6 KB (1568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980739941cb96072c34a82314491f555b66b9440b93eed4ef3b9c4b35a451b62`  
		Last Modified: Tue, 08 Dec 2020 00:53:13 GMT  
		Size: 19.3 MB (19323541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a089ee89f6043a60f32e44e5405ba3fdc61a0dd8403bc5082f7b188f6091cc`  
		Last Modified: Mon, 14 Dec 2020 21:38:38 GMT  
		Size: 145.0 MB (144970871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b068859f838cf3d9907c77ae252f18ac268163439c0de7e44867d7a5e68164a`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aec5f76445c9fd06a1652fcbf8d4cb0ae7924d1560149e5972c39eb39f3cff`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0`

```console
$ docker pull percona@sha256:d5d76334aa84c239fde43a2d2331d9bc268acec1702632d1741037a80419dda3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0` - linux; amd64

```console
$ docker pull percona@sha256:5bbb24c3ff580b9feebf71f4a2df037fa26adacc8cd73b52ff5911fd89fa2b6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.5 MB (239482162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef86f7cd16d0a330e95d544ac8d2972013aeea59202bf620660b1330103584f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:04 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 08 Dec 2020 00:48:12 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 14 Dec 2020 21:36:41 GMT
ENV PS_VERSION=8.0.22-13.1
# Mon, 14 Dec 2020 21:36:41 GMT
ENV OS_VER=el8
# Mon, 14 Dec 2020 21:36:41 GMT
ENV FULL_PERCONA_VERSION=8.0.22-13.1.el8
# Mon, 14 Dec 2020 21:37:14 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 14 Dec 2020 21:37:15 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 14 Dec 2020 21:37:15 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 14 Dec 2020 21:37:16 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 14 Dec 2020 21:37:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Dec 2020 21:37:16 GMT
USER mysql
# Mon, 14 Dec 2020 21:37:16 GMT
EXPOSE 3306 33060
# Mon, 14 Dec 2020 21:37:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ce9644bc2779e06cc0a9ac9a86e9f4981ba7c6f0274fb87a2d59b1e9f47f44`  
		Last Modified: Tue, 08 Dec 2020 00:53:09 GMT  
		Size: 1.6 KB (1568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980739941cb96072c34a82314491f555b66b9440b93eed4ef3b9c4b35a451b62`  
		Last Modified: Tue, 08 Dec 2020 00:53:13 GMT  
		Size: 19.3 MB (19323541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a089ee89f6043a60f32e44e5405ba3fdc61a0dd8403bc5082f7b188f6091cc`  
		Last Modified: Mon, 14 Dec 2020 21:38:38 GMT  
		Size: 145.0 MB (144970871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b068859f838cf3d9907c77ae252f18ac268163439c0de7e44867d7a5e68164a`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aec5f76445c9fd06a1652fcbf8d4cb0ae7924d1560149e5972c39eb39f3cff`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.22-13`

```console
$ docker pull percona@sha256:d5d76334aa84c239fde43a2d2331d9bc268acec1702632d1741037a80419dda3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0.22-13` - linux; amd64

```console
$ docker pull percona@sha256:5bbb24c3ff580b9feebf71f4a2df037fa26adacc8cd73b52ff5911fd89fa2b6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.5 MB (239482162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef86f7cd16d0a330e95d544ac8d2972013aeea59202bf620660b1330103584f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:04 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 08 Dec 2020 00:48:12 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 14 Dec 2020 21:36:41 GMT
ENV PS_VERSION=8.0.22-13.1
# Mon, 14 Dec 2020 21:36:41 GMT
ENV OS_VER=el8
# Mon, 14 Dec 2020 21:36:41 GMT
ENV FULL_PERCONA_VERSION=8.0.22-13.1.el8
# Mon, 14 Dec 2020 21:37:14 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 14 Dec 2020 21:37:15 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 14 Dec 2020 21:37:15 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 14 Dec 2020 21:37:16 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 14 Dec 2020 21:37:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Dec 2020 21:37:16 GMT
USER mysql
# Mon, 14 Dec 2020 21:37:16 GMT
EXPOSE 3306 33060
# Mon, 14 Dec 2020 21:37:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ce9644bc2779e06cc0a9ac9a86e9f4981ba7c6f0274fb87a2d59b1e9f47f44`  
		Last Modified: Tue, 08 Dec 2020 00:53:09 GMT  
		Size: 1.6 KB (1568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980739941cb96072c34a82314491f555b66b9440b93eed4ef3b9c4b35a451b62`  
		Last Modified: Tue, 08 Dec 2020 00:53:13 GMT  
		Size: 19.3 MB (19323541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a089ee89f6043a60f32e44e5405ba3fdc61a0dd8403bc5082f7b188f6091cc`  
		Last Modified: Mon, 14 Dec 2020 21:38:38 GMT  
		Size: 145.0 MB (144970871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b068859f838cf3d9907c77ae252f18ac268163439c0de7e44867d7a5e68164a`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aec5f76445c9fd06a1652fcbf8d4cb0ae7924d1560149e5972c39eb39f3cff`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.22-13-centos`

```console
$ docker pull percona@sha256:d5d76334aa84c239fde43a2d2331d9bc268acec1702632d1741037a80419dda3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0.22-13-centos` - linux; amd64

```console
$ docker pull percona@sha256:5bbb24c3ff580b9feebf71f4a2df037fa26adacc8cd73b52ff5911fd89fa2b6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.5 MB (239482162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef86f7cd16d0a330e95d544ac8d2972013aeea59202bf620660b1330103584f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:04 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 08 Dec 2020 00:48:12 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 14 Dec 2020 21:36:41 GMT
ENV PS_VERSION=8.0.22-13.1
# Mon, 14 Dec 2020 21:36:41 GMT
ENV OS_VER=el8
# Mon, 14 Dec 2020 21:36:41 GMT
ENV FULL_PERCONA_VERSION=8.0.22-13.1.el8
# Mon, 14 Dec 2020 21:37:14 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 14 Dec 2020 21:37:15 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 14 Dec 2020 21:37:15 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 14 Dec 2020 21:37:16 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 14 Dec 2020 21:37:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Dec 2020 21:37:16 GMT
USER mysql
# Mon, 14 Dec 2020 21:37:16 GMT
EXPOSE 3306 33060
# Mon, 14 Dec 2020 21:37:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ce9644bc2779e06cc0a9ac9a86e9f4981ba7c6f0274fb87a2d59b1e9f47f44`  
		Last Modified: Tue, 08 Dec 2020 00:53:09 GMT  
		Size: 1.6 KB (1568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980739941cb96072c34a82314491f555b66b9440b93eed4ef3b9c4b35a451b62`  
		Last Modified: Tue, 08 Dec 2020 00:53:13 GMT  
		Size: 19.3 MB (19323541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a089ee89f6043a60f32e44e5405ba3fdc61a0dd8403bc5082f7b188f6091cc`  
		Last Modified: Mon, 14 Dec 2020 21:38:38 GMT  
		Size: 145.0 MB (144970871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b068859f838cf3d9907c77ae252f18ac268163439c0de7e44867d7a5e68164a`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aec5f76445c9fd06a1652fcbf8d4cb0ae7924d1560149e5972c39eb39f3cff`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0-centos`

```console
$ docker pull percona@sha256:d5d76334aa84c239fde43a2d2331d9bc268acec1702632d1741037a80419dda3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0-centos` - linux; amd64

```console
$ docker pull percona@sha256:5bbb24c3ff580b9feebf71f4a2df037fa26adacc8cd73b52ff5911fd89fa2b6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.5 MB (239482162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef86f7cd16d0a330e95d544ac8d2972013aeea59202bf620660b1330103584f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:04 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 08 Dec 2020 00:48:12 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 14 Dec 2020 21:36:41 GMT
ENV PS_VERSION=8.0.22-13.1
# Mon, 14 Dec 2020 21:36:41 GMT
ENV OS_VER=el8
# Mon, 14 Dec 2020 21:36:41 GMT
ENV FULL_PERCONA_VERSION=8.0.22-13.1.el8
# Mon, 14 Dec 2020 21:37:14 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 14 Dec 2020 21:37:15 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 14 Dec 2020 21:37:15 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 14 Dec 2020 21:37:16 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 14 Dec 2020 21:37:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Dec 2020 21:37:16 GMT
USER mysql
# Mon, 14 Dec 2020 21:37:16 GMT
EXPOSE 3306 33060
# Mon, 14 Dec 2020 21:37:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ce9644bc2779e06cc0a9ac9a86e9f4981ba7c6f0274fb87a2d59b1e9f47f44`  
		Last Modified: Tue, 08 Dec 2020 00:53:09 GMT  
		Size: 1.6 KB (1568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980739941cb96072c34a82314491f555b66b9440b93eed4ef3b9c4b35a451b62`  
		Last Modified: Tue, 08 Dec 2020 00:53:13 GMT  
		Size: 19.3 MB (19323541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a089ee89f6043a60f32e44e5405ba3fdc61a0dd8403bc5082f7b188f6091cc`  
		Last Modified: Mon, 14 Dec 2020 21:38:38 GMT  
		Size: 145.0 MB (144970871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b068859f838cf3d9907c77ae252f18ac268163439c0de7e44867d7a5e68164a`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aec5f76445c9fd06a1652fcbf8d4cb0ae7924d1560149e5972c39eb39f3cff`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8-centos`

```console
$ docker pull percona@sha256:d5d76334aa84c239fde43a2d2331d9bc268acec1702632d1741037a80419dda3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8-centos` - linux; amd64

```console
$ docker pull percona@sha256:5bbb24c3ff580b9feebf71f4a2df037fa26adacc8cd73b52ff5911fd89fa2b6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.5 MB (239482162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef86f7cd16d0a330e95d544ac8d2972013aeea59202bf620660b1330103584f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:04 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 08 Dec 2020 00:48:12 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 14 Dec 2020 21:36:41 GMT
ENV PS_VERSION=8.0.22-13.1
# Mon, 14 Dec 2020 21:36:41 GMT
ENV OS_VER=el8
# Mon, 14 Dec 2020 21:36:41 GMT
ENV FULL_PERCONA_VERSION=8.0.22-13.1.el8
# Mon, 14 Dec 2020 21:37:14 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 14 Dec 2020 21:37:15 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 14 Dec 2020 21:37:15 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 14 Dec 2020 21:37:16 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 14 Dec 2020 21:37:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Dec 2020 21:37:16 GMT
USER mysql
# Mon, 14 Dec 2020 21:37:16 GMT
EXPOSE 3306 33060
# Mon, 14 Dec 2020 21:37:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ce9644bc2779e06cc0a9ac9a86e9f4981ba7c6f0274fb87a2d59b1e9f47f44`  
		Last Modified: Tue, 08 Dec 2020 00:53:09 GMT  
		Size: 1.6 KB (1568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980739941cb96072c34a82314491f555b66b9440b93eed4ef3b9c4b35a451b62`  
		Last Modified: Tue, 08 Dec 2020 00:53:13 GMT  
		Size: 19.3 MB (19323541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a089ee89f6043a60f32e44e5405ba3fdc61a0dd8403bc5082f7b188f6091cc`  
		Last Modified: Mon, 14 Dec 2020 21:38:38 GMT  
		Size: 145.0 MB (144970871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b068859f838cf3d9907c77ae252f18ac268163439c0de7e44867d7a5e68164a`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aec5f76445c9fd06a1652fcbf8d4cb0ae7924d1560149e5972c39eb39f3cff`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:centos`

```console
$ docker pull percona@sha256:358eff0fa5115958da5e913c56f6420cfe5a2102dde63f8b06bbc24566893916
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:centos` - linux; amd64

```console
$ docker pull percona@sha256:00e206b1ddc71450a885624a9bfab84b4281b0d4b07699a22d4fc47bcfa44b52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.5 MB (220519463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41370b19b67aa296306b0172907bb8058e50086190a13b3390985c57bcbef8b9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:59 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Tue, 08 Dec 2020 00:49:15 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Tue, 08 Dec 2020 00:49:16 GMT
ENV PS_VERSION=5.7.32-35.1
# Tue, 08 Dec 2020 00:49:16 GMT
ENV OS_VER=el8
# Tue, 08 Dec 2020 00:49:17 GMT
ENV FULL_PERCONA_VERSION=5.7.32-35.1.el8
# Tue, 08 Dec 2020 00:49:43 GMT
RUN set -ex;     dnf install -y         dnf-utils         jemalloc         cracklib-dicts         which;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         selinux-policy             | xargs curl -Lf -o /tmp/selinux-policy.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm --nodeps;     rm -rf /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm;         dnf install -y         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf remove -y dnf-utils;     dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Tue, 08 Dec 2020 00:49:44 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 08 Dec 2020 00:49:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 08 Dec 2020 00:49:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 08 Dec 2020 00:49:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Dec 2020 00:49:45 GMT
USER mysql
# Tue, 08 Dec 2020 00:49:45 GMT
EXPOSE 3306
# Tue, 08 Dec 2020 00:49:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205beaf4be145d43ce7f738775ac25339927be11e45ec9d34fd8dd5538c9ef66`  
		Last Modified: Tue, 08 Dec 2020 00:53:46 GMT  
		Size: 1.5 KB (1541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be50bbff9088000f27631eb27c12dece641c44fc636f08d894c80cc2ce6e90f`  
		Last Modified: Tue, 08 Dec 2020 00:53:48 GMT  
		Size: 30.4 MB (30388488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560824284de3bdd0da4b80fca9717c986cc0bc3b7f2780096ab57bcbaf6cc7b1`  
		Last Modified: Tue, 08 Dec 2020 00:54:09 GMT  
		Size: 114.9 MB (114942980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbdf23842a16bd108ccb1cd247bbd06fec10094a7ac2236d4916bb1890e077c`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc7f9b3a007572a65eeb7d21136c59f339f5b505d1ffb5ee9b0575db9416de8`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:latest`

```console
$ docker pull percona@sha256:358eff0fa5115958da5e913c56f6420cfe5a2102dde63f8b06bbc24566893916
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:latest` - linux; amd64

```console
$ docker pull percona@sha256:00e206b1ddc71450a885624a9bfab84b4281b0d4b07699a22d4fc47bcfa44b52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.5 MB (220519463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41370b19b67aa296306b0172907bb8058e50086190a13b3390985c57bcbef8b9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:59 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Tue, 08 Dec 2020 00:49:15 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Tue, 08 Dec 2020 00:49:16 GMT
ENV PS_VERSION=5.7.32-35.1
# Tue, 08 Dec 2020 00:49:16 GMT
ENV OS_VER=el8
# Tue, 08 Dec 2020 00:49:17 GMT
ENV FULL_PERCONA_VERSION=5.7.32-35.1.el8
# Tue, 08 Dec 2020 00:49:43 GMT
RUN set -ex;     dnf install -y         dnf-utils         jemalloc         cracklib-dicts         which;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         selinux-policy             | xargs curl -Lf -o /tmp/selinux-policy.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm --nodeps;     rm -rf /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm;         dnf install -y         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf remove -y dnf-utils;     dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Tue, 08 Dec 2020 00:49:44 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 08 Dec 2020 00:49:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 08 Dec 2020 00:49:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 08 Dec 2020 00:49:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Dec 2020 00:49:45 GMT
USER mysql
# Tue, 08 Dec 2020 00:49:45 GMT
EXPOSE 3306
# Tue, 08 Dec 2020 00:49:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205beaf4be145d43ce7f738775ac25339927be11e45ec9d34fd8dd5538c9ef66`  
		Last Modified: Tue, 08 Dec 2020 00:53:46 GMT  
		Size: 1.5 KB (1541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be50bbff9088000f27631eb27c12dece641c44fc636f08d894c80cc2ce6e90f`  
		Last Modified: Tue, 08 Dec 2020 00:53:48 GMT  
		Size: 30.4 MB (30388488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560824284de3bdd0da4b80fca9717c986cc0bc3b7f2780096ab57bcbaf6cc7b1`  
		Last Modified: Tue, 08 Dec 2020 00:54:09 GMT  
		Size: 114.9 MB (114942980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbdf23842a16bd108ccb1cd247bbd06fec10094a7ac2236d4916bb1890e077c`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc7f9b3a007572a65eeb7d21136c59f339f5b505d1ffb5ee9b0575db9416de8`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5`

```console
$ docker pull percona@sha256:358eff0fa5115958da5e913c56f6420cfe5a2102dde63f8b06bbc24566893916
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5` - linux; amd64

```console
$ docker pull percona@sha256:00e206b1ddc71450a885624a9bfab84b4281b0d4b07699a22d4fc47bcfa44b52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.5 MB (220519463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41370b19b67aa296306b0172907bb8058e50086190a13b3390985c57bcbef8b9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:59 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Tue, 08 Dec 2020 00:49:15 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Tue, 08 Dec 2020 00:49:16 GMT
ENV PS_VERSION=5.7.32-35.1
# Tue, 08 Dec 2020 00:49:16 GMT
ENV OS_VER=el8
# Tue, 08 Dec 2020 00:49:17 GMT
ENV FULL_PERCONA_VERSION=5.7.32-35.1.el8
# Tue, 08 Dec 2020 00:49:43 GMT
RUN set -ex;     dnf install -y         dnf-utils         jemalloc         cracklib-dicts         which;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         selinux-policy             | xargs curl -Lf -o /tmp/selinux-policy.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm --nodeps;     rm -rf /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm;         dnf install -y         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf remove -y dnf-utils;     dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Tue, 08 Dec 2020 00:49:44 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 08 Dec 2020 00:49:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 08 Dec 2020 00:49:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 08 Dec 2020 00:49:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Dec 2020 00:49:45 GMT
USER mysql
# Tue, 08 Dec 2020 00:49:45 GMT
EXPOSE 3306
# Tue, 08 Dec 2020 00:49:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205beaf4be145d43ce7f738775ac25339927be11e45ec9d34fd8dd5538c9ef66`  
		Last Modified: Tue, 08 Dec 2020 00:53:46 GMT  
		Size: 1.5 KB (1541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be50bbff9088000f27631eb27c12dece641c44fc636f08d894c80cc2ce6e90f`  
		Last Modified: Tue, 08 Dec 2020 00:53:48 GMT  
		Size: 30.4 MB (30388488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560824284de3bdd0da4b80fca9717c986cc0bc3b7f2780096ab57bcbaf6cc7b1`  
		Last Modified: Tue, 08 Dec 2020 00:54:09 GMT  
		Size: 114.9 MB (114942980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbdf23842a16bd108ccb1cd247bbd06fec10094a7ac2236d4916bb1890e077c`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc7f9b3a007572a65eeb7d21136c59f339f5b505d1ffb5ee9b0575db9416de8`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.6`

```console
$ docker pull percona@sha256:b6bc17e2a4572723e3fe86f9238afcfb7c6dd3d257d2db6b86f8b0938227ce52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.6` - linux; amd64

```console
$ docker pull percona@sha256:09ccce2f3d13b37c5cbdc75854c8ad6efbf35afdabd0dd2181f1859481cf9258
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.7 MB (140734318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3700cad0b44abb340f3f0a468fccfb8c4e273265179ead0894cb29dfd3eca3a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 14 Nov 2020 00:45:10 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 14 Nov 2020 00:45:42 GMT
RUN groupdel input && groupadd -g 999 mysql
# Sat, 14 Nov 2020 00:45:43 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Wed, 25 Nov 2020 22:23:27 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Thu, 26 Nov 2020 18:22:05 GMT
ENV PERCONA_VERSION=5.6.50-rel90.0.1.el7
# Thu, 26 Nov 2020 18:22:46 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 26 Nov 2020 18:22:47 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 26 Nov 2020 18:22:47 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 26 Nov 2020 18:22:47 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Thu, 26 Nov 2020 18:22:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 26 Nov 2020 18:22:47 GMT
USER mysql
# Thu, 26 Nov 2020 18:22:48 GMT
EXPOSE 3306
# Thu, 26 Nov 2020 18:22:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75e5924dc16b794b9dfe808be3f7a247acec59d0e0b5ba0e0007e86073e80d9`  
		Last Modified: Sat, 14 Nov 2020 00:47:52 GMT  
		Size: 541.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60550dc8778b2360245b3a4a2609bc9b2e1415c8795d27812232246892a8dba3`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebce5663c9fe5c45da8b16ddad68e6088d75046395dc267f948f8b3390b1efcf`  
		Last Modified: Thu, 26 Nov 2020 18:23:57 GMT  
		Size: 6.6 MB (6562458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140c3608c6243c53a4c59d253c86d1c5df95e005713600442016d48aaecc87a9`  
		Last Modified: Thu, 26 Nov 2020 18:24:06 GMT  
		Size: 58.1 MB (58064791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2f7710126bd9cb3df7dc98a6a7e6559f7e6617e9c63265c22dd342c40b6d14`  
		Last Modified: Thu, 26 Nov 2020 18:23:55 GMT  
		Size: 4.9 KB (4878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf0f791d44e94b8100317f9d42ac785f4421b4230301e34ffac891bb8579125`  
		Last Modified: Thu, 26 Nov 2020 18:23:55 GMT  
		Size: 2.9 KB (2940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.6.51`

```console
$ docker pull percona@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `percona:ps-5.7`

```console
$ docker pull percona@sha256:358eff0fa5115958da5e913c56f6420cfe5a2102dde63f8b06bbc24566893916
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.7` - linux; amd64

```console
$ docker pull percona@sha256:00e206b1ddc71450a885624a9bfab84b4281b0d4b07699a22d4fc47bcfa44b52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.5 MB (220519463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41370b19b67aa296306b0172907bb8058e50086190a13b3390985c57bcbef8b9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:59 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Tue, 08 Dec 2020 00:49:15 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Tue, 08 Dec 2020 00:49:16 GMT
ENV PS_VERSION=5.7.32-35.1
# Tue, 08 Dec 2020 00:49:16 GMT
ENV OS_VER=el8
# Tue, 08 Dec 2020 00:49:17 GMT
ENV FULL_PERCONA_VERSION=5.7.32-35.1.el8
# Tue, 08 Dec 2020 00:49:43 GMT
RUN set -ex;     dnf install -y         dnf-utils         jemalloc         cracklib-dicts         which;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         selinux-policy             | xargs curl -Lf -o /tmp/selinux-policy.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm --nodeps;     rm -rf /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm;         dnf install -y         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf remove -y dnf-utils;     dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Tue, 08 Dec 2020 00:49:44 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 08 Dec 2020 00:49:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 08 Dec 2020 00:49:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 08 Dec 2020 00:49:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Dec 2020 00:49:45 GMT
USER mysql
# Tue, 08 Dec 2020 00:49:45 GMT
EXPOSE 3306
# Tue, 08 Dec 2020 00:49:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205beaf4be145d43ce7f738775ac25339927be11e45ec9d34fd8dd5538c9ef66`  
		Last Modified: Tue, 08 Dec 2020 00:53:46 GMT  
		Size: 1.5 KB (1541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be50bbff9088000f27631eb27c12dece641c44fc636f08d894c80cc2ce6e90f`  
		Last Modified: Tue, 08 Dec 2020 00:53:48 GMT  
		Size: 30.4 MB (30388488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560824284de3bdd0da4b80fca9717c986cc0bc3b7f2780096ab57bcbaf6cc7b1`  
		Last Modified: Tue, 08 Dec 2020 00:54:09 GMT  
		Size: 114.9 MB (114942980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbdf23842a16bd108ccb1cd247bbd06fec10094a7ac2236d4916bb1890e077c`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc7f9b3a007572a65eeb7d21136c59f339f5b505d1ffb5ee9b0575db9416de8`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.7.32`

```console
$ docker pull percona@sha256:358eff0fa5115958da5e913c56f6420cfe5a2102dde63f8b06bbc24566893916
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.7.32` - linux; amd64

```console
$ docker pull percona@sha256:00e206b1ddc71450a885624a9bfab84b4281b0d4b07699a22d4fc47bcfa44b52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.5 MB (220519463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41370b19b67aa296306b0172907bb8058e50086190a13b3390985c57bcbef8b9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:59 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Tue, 08 Dec 2020 00:49:15 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Tue, 08 Dec 2020 00:49:16 GMT
ENV PS_VERSION=5.7.32-35.1
# Tue, 08 Dec 2020 00:49:16 GMT
ENV OS_VER=el8
# Tue, 08 Dec 2020 00:49:17 GMT
ENV FULL_PERCONA_VERSION=5.7.32-35.1.el8
# Tue, 08 Dec 2020 00:49:43 GMT
RUN set -ex;     dnf install -y         dnf-utils         jemalloc         cracklib-dicts         which;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         selinux-policy             | xargs curl -Lf -o /tmp/selinux-policy.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm --nodeps;     rm -rf /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm;         dnf install -y         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf remove -y dnf-utils;     dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Tue, 08 Dec 2020 00:49:44 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 08 Dec 2020 00:49:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 08 Dec 2020 00:49:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 08 Dec 2020 00:49:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Dec 2020 00:49:45 GMT
USER mysql
# Tue, 08 Dec 2020 00:49:45 GMT
EXPOSE 3306
# Tue, 08 Dec 2020 00:49:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205beaf4be145d43ce7f738775ac25339927be11e45ec9d34fd8dd5538c9ef66`  
		Last Modified: Tue, 08 Dec 2020 00:53:46 GMT  
		Size: 1.5 KB (1541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be50bbff9088000f27631eb27c12dece641c44fc636f08d894c80cc2ce6e90f`  
		Last Modified: Tue, 08 Dec 2020 00:53:48 GMT  
		Size: 30.4 MB (30388488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560824284de3bdd0da4b80fca9717c986cc0bc3b7f2780096ab57bcbaf6cc7b1`  
		Last Modified: Tue, 08 Dec 2020 00:54:09 GMT  
		Size: 114.9 MB (114942980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbdf23842a16bd108ccb1cd247bbd06fec10094a7ac2236d4916bb1890e077c`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc7f9b3a007572a65eeb7d21136c59f339f5b505d1ffb5ee9b0575db9416de8`  
		Last Modified: Tue, 08 Dec 2020 00:53:45 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8`

```console
$ docker pull percona@sha256:d5d76334aa84c239fde43a2d2331d9bc268acec1702632d1741037a80419dda3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8` - linux; amd64

```console
$ docker pull percona@sha256:5bbb24c3ff580b9feebf71f4a2df037fa26adacc8cd73b52ff5911fd89fa2b6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.5 MB (239482162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef86f7cd16d0a330e95d544ac8d2972013aeea59202bf620660b1330103584f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:04 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 08 Dec 2020 00:48:12 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 14 Dec 2020 21:36:41 GMT
ENV PS_VERSION=8.0.22-13.1
# Mon, 14 Dec 2020 21:36:41 GMT
ENV OS_VER=el8
# Mon, 14 Dec 2020 21:36:41 GMT
ENV FULL_PERCONA_VERSION=8.0.22-13.1.el8
# Mon, 14 Dec 2020 21:37:14 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 14 Dec 2020 21:37:15 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 14 Dec 2020 21:37:15 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 14 Dec 2020 21:37:16 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 14 Dec 2020 21:37:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Dec 2020 21:37:16 GMT
USER mysql
# Mon, 14 Dec 2020 21:37:16 GMT
EXPOSE 3306 33060
# Mon, 14 Dec 2020 21:37:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ce9644bc2779e06cc0a9ac9a86e9f4981ba7c6f0274fb87a2d59b1e9f47f44`  
		Last Modified: Tue, 08 Dec 2020 00:53:09 GMT  
		Size: 1.6 KB (1568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980739941cb96072c34a82314491f555b66b9440b93eed4ef3b9c4b35a451b62`  
		Last Modified: Tue, 08 Dec 2020 00:53:13 GMT  
		Size: 19.3 MB (19323541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a089ee89f6043a60f32e44e5405ba3fdc61a0dd8403bc5082f7b188f6091cc`  
		Last Modified: Mon, 14 Dec 2020 21:38:38 GMT  
		Size: 145.0 MB (144970871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b068859f838cf3d9907c77ae252f18ac268163439c0de7e44867d7a5e68164a`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aec5f76445c9fd06a1652fcbf8d4cb0ae7924d1560149e5972c39eb39f3cff`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0`

```console
$ docker pull percona@sha256:d5d76334aa84c239fde43a2d2331d9bc268acec1702632d1741037a80419dda3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8.0` - linux; amd64

```console
$ docker pull percona@sha256:5bbb24c3ff580b9feebf71f4a2df037fa26adacc8cd73b52ff5911fd89fa2b6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.5 MB (239482162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef86f7cd16d0a330e95d544ac8d2972013aeea59202bf620660b1330103584f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:04 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 08 Dec 2020 00:48:12 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 14 Dec 2020 21:36:41 GMT
ENV PS_VERSION=8.0.22-13.1
# Mon, 14 Dec 2020 21:36:41 GMT
ENV OS_VER=el8
# Mon, 14 Dec 2020 21:36:41 GMT
ENV FULL_PERCONA_VERSION=8.0.22-13.1.el8
# Mon, 14 Dec 2020 21:37:14 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 14 Dec 2020 21:37:15 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 14 Dec 2020 21:37:15 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 14 Dec 2020 21:37:16 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 14 Dec 2020 21:37:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Dec 2020 21:37:16 GMT
USER mysql
# Mon, 14 Dec 2020 21:37:16 GMT
EXPOSE 3306 33060
# Mon, 14 Dec 2020 21:37:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ce9644bc2779e06cc0a9ac9a86e9f4981ba7c6f0274fb87a2d59b1e9f47f44`  
		Last Modified: Tue, 08 Dec 2020 00:53:09 GMT  
		Size: 1.6 KB (1568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980739941cb96072c34a82314491f555b66b9440b93eed4ef3b9c4b35a451b62`  
		Last Modified: Tue, 08 Dec 2020 00:53:13 GMT  
		Size: 19.3 MB (19323541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a089ee89f6043a60f32e44e5405ba3fdc61a0dd8403bc5082f7b188f6091cc`  
		Last Modified: Mon, 14 Dec 2020 21:38:38 GMT  
		Size: 145.0 MB (144970871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b068859f838cf3d9907c77ae252f18ac268163439c0de7e44867d7a5e68164a`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aec5f76445c9fd06a1652fcbf8d4cb0ae7924d1560149e5972c39eb39f3cff`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0.22-13`

```console
$ docker pull percona@sha256:d5d76334aa84c239fde43a2d2331d9bc268acec1702632d1741037a80419dda3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8.0.22-13` - linux; amd64

```console
$ docker pull percona@sha256:5bbb24c3ff580b9feebf71f4a2df037fa26adacc8cd73b52ff5911fd89fa2b6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.5 MB (239482162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef86f7cd16d0a330e95d544ac8d2972013aeea59202bf620660b1330103584f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:04 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 08 Dec 2020 00:48:12 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 14 Dec 2020 21:36:41 GMT
ENV PS_VERSION=8.0.22-13.1
# Mon, 14 Dec 2020 21:36:41 GMT
ENV OS_VER=el8
# Mon, 14 Dec 2020 21:36:41 GMT
ENV FULL_PERCONA_VERSION=8.0.22-13.1.el8
# Mon, 14 Dec 2020 21:37:14 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 14 Dec 2020 21:37:15 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 14 Dec 2020 21:37:15 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 14 Dec 2020 21:37:16 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 14 Dec 2020 21:37:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Dec 2020 21:37:16 GMT
USER mysql
# Mon, 14 Dec 2020 21:37:16 GMT
EXPOSE 3306 33060
# Mon, 14 Dec 2020 21:37:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ce9644bc2779e06cc0a9ac9a86e9f4981ba7c6f0274fb87a2d59b1e9f47f44`  
		Last Modified: Tue, 08 Dec 2020 00:53:09 GMT  
		Size: 1.6 KB (1568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980739941cb96072c34a82314491f555b66b9440b93eed4ef3b9c4b35a451b62`  
		Last Modified: Tue, 08 Dec 2020 00:53:13 GMT  
		Size: 19.3 MB (19323541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a089ee89f6043a60f32e44e5405ba3fdc61a0dd8403bc5082f7b188f6091cc`  
		Last Modified: Mon, 14 Dec 2020 21:38:38 GMT  
		Size: 145.0 MB (144970871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b068859f838cf3d9907c77ae252f18ac268163439c0de7e44867d7a5e68164a`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aec5f76445c9fd06a1652fcbf8d4cb0ae7924d1560149e5972c39eb39f3cff`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-3.6`

```console
$ docker pull percona@sha256:5518f80fb62305e809f36463c086682da1ac1b54fcc26f2cea349bed47397f2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6` - linux; amd64

```console
$ docker pull percona@sha256:dfe21f5b7428d0fd01104245196b92730bc2295b2a7304c95160363a745c1bb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.1 MB (159091589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59125b14c3cd23ab35e736814197eb2e1360b8b0aa5b7b28c76ec2f74fbceed1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:52:23 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 30 Dec 2020 19:23:09 GMT
ENV PSMDB_VERSION=3.6.21-11.0
# Wed, 30 Dec 2020 19:23:09 GMT
ENV OS_VER=el8
# Wed, 30 Dec 2020 19:23:09 GMT
ENV FULL_PERCONA_VERSION=3.6.21-11.0.el8
# Wed, 30 Dec 2020 19:23:09 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 30 Dec 2020 19:23:29 GMT
RUN set -ex;     dnf install -y         dnf-utils         shadow-utils         curl         procps-ng         jq         oniguruma         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         dnf remove -y dnf-utils;         dnf clean all;         rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Wed, 30 Dec 2020 19:23:30 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 30 Dec 2020 19:23:30 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 30 Dec 2020 19:23:31 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 30 Dec 2020 19:23:33 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 30 Dec 2020 19:23:33 GMT
VOLUME [/data/db]
# Wed, 30 Dec 2020 19:23:33 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Wed, 30 Dec 2020 19:23:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 30 Dec 2020 19:23:34 GMT
EXPOSE 27017
# Wed, 30 Dec 2020 19:23:34 GMT
USER 1001
# Wed, 30 Dec 2020 19:23:34 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cbdf4c8d89f3c13b353d56e39e0bfb67c9a4d33f86a20850bca43ce4d6d04b`  
		Last Modified: Tue, 08 Dec 2020 00:55:23 GMT  
		Size: 19.3 MB (19312715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f9fd34dfab88b897f2511eb633bab4dbc3e73bb59c30adccedde0a0b696e95`  
		Last Modified: Wed, 30 Dec 2020 19:24:49 GMT  
		Size: 56.4 MB (56438251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997881db31567c1ce99d0dbdd9f8f2621925a008e4bf9fedd33f30441df1fbb1`  
		Last Modified: Wed, 30 Dec 2020 19:24:39 GMT  
		Size: 1.5 KB (1544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a218d438de71f86d41c6cbf77133fbb0742c3f63b22fa3055d74d7d8b6ac4123`  
		Last Modified: Wed, 30 Dec 2020 19:24:39 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3a78c8b8384fb03510ab4f92ded66724c96f63bf2d97d403cda4082a8d2029`  
		Last Modified: Wed, 30 Dec 2020 19:24:39 GMT  
		Size: 10.6 KB (10577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79285dbdeabb6cb0a339e44716a4b5bb3c8fd10aae526ec33133685109dced55`  
		Last Modified: Wed, 30 Dec 2020 19:24:41 GMT  
		Size: 8.1 MB (8137888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e07ef43f518421bf5ba7b849d088a31e8afc68e50c01963572e99d7602ef599`  
		Last Modified: Wed, 30 Dec 2020 19:24:39 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-3.6.21`

```console
$ docker pull percona@sha256:5518f80fb62305e809f36463c086682da1ac1b54fcc26f2cea349bed47397f2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6.21` - linux; amd64

```console
$ docker pull percona@sha256:dfe21f5b7428d0fd01104245196b92730bc2295b2a7304c95160363a745c1bb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.1 MB (159091589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59125b14c3cd23ab35e736814197eb2e1360b8b0aa5b7b28c76ec2f74fbceed1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:52:23 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 30 Dec 2020 19:23:09 GMT
ENV PSMDB_VERSION=3.6.21-11.0
# Wed, 30 Dec 2020 19:23:09 GMT
ENV OS_VER=el8
# Wed, 30 Dec 2020 19:23:09 GMT
ENV FULL_PERCONA_VERSION=3.6.21-11.0.el8
# Wed, 30 Dec 2020 19:23:09 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 30 Dec 2020 19:23:29 GMT
RUN set -ex;     dnf install -y         dnf-utils         shadow-utils         curl         procps-ng         jq         oniguruma         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         dnf remove -y dnf-utils;         dnf clean all;         rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Wed, 30 Dec 2020 19:23:30 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 30 Dec 2020 19:23:30 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 30 Dec 2020 19:23:31 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 30 Dec 2020 19:23:33 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 30 Dec 2020 19:23:33 GMT
VOLUME [/data/db]
# Wed, 30 Dec 2020 19:23:33 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Wed, 30 Dec 2020 19:23:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 30 Dec 2020 19:23:34 GMT
EXPOSE 27017
# Wed, 30 Dec 2020 19:23:34 GMT
USER 1001
# Wed, 30 Dec 2020 19:23:34 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cbdf4c8d89f3c13b353d56e39e0bfb67c9a4d33f86a20850bca43ce4d6d04b`  
		Last Modified: Tue, 08 Dec 2020 00:55:23 GMT  
		Size: 19.3 MB (19312715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f9fd34dfab88b897f2511eb633bab4dbc3e73bb59c30adccedde0a0b696e95`  
		Last Modified: Wed, 30 Dec 2020 19:24:49 GMT  
		Size: 56.4 MB (56438251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997881db31567c1ce99d0dbdd9f8f2621925a008e4bf9fedd33f30441df1fbb1`  
		Last Modified: Wed, 30 Dec 2020 19:24:39 GMT  
		Size: 1.5 KB (1544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a218d438de71f86d41c6cbf77133fbb0742c3f63b22fa3055d74d7d8b6ac4123`  
		Last Modified: Wed, 30 Dec 2020 19:24:39 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3a78c8b8384fb03510ab4f92ded66724c96f63bf2d97d403cda4082a8d2029`  
		Last Modified: Wed, 30 Dec 2020 19:24:39 GMT  
		Size: 10.6 KB (10577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79285dbdeabb6cb0a339e44716a4b5bb3c8fd10aae526ec33133685109dced55`  
		Last Modified: Wed, 30 Dec 2020 19:24:41 GMT  
		Size: 8.1 MB (8137888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e07ef43f518421bf5ba7b849d088a31e8afc68e50c01963572e99d7602ef599`  
		Last Modified: Wed, 30 Dec 2020 19:24:39 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.0`

```console
$ docker pull percona@sha256:a4cae12e9e3dcb8e91ba95a15fb536ca6224915ca392da98ef8a66e88b4af246
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0` - linux; amd64

```console
$ docker pull percona@sha256:bb24cef54cae1928b29b5c3b1a9af057980670db80fe2e01e0e58b4b17356e4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.7 MB (169672809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:809f4f0126f0de3468e2db57f22efd983f1c9f8cc4960b086c5fd088f6405fb9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:51:44 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-40 release
# Tue, 19 Jan 2021 22:21:16 GMT
ENV PSMDB_VERSION=4.0.22-17
# Tue, 19 Jan 2021 22:21:16 GMT
ENV OS_VER=el8
# Tue, 19 Jan 2021 22:21:16 GMT
ENV FULL_PERCONA_VERSION=4.0.22-17.el8
# Tue, 19 Jan 2021 22:21:16 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 19 Jan 2021 22:21:38 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Tue, 19 Jan 2021 22:21:39 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 19 Jan 2021 22:21:39 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 19 Jan 2021 22:21:40 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 19 Jan 2021 22:21:40 GMT
ENV GOSU_VERSION=1.11
# Tue, 19 Jan 2021 22:21:43 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Tue, 19 Jan 2021 22:21:45 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 19 Jan 2021 22:21:45 GMT
VOLUME [/data/db]
# Tue, 19 Jan 2021 22:21:46 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Tue, 19 Jan 2021 22:21:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Jan 2021 22:21:46 GMT
EXPOSE 27017
# Tue, 19 Jan 2021 22:21:46 GMT
USER 1001
# Tue, 19 Jan 2021 22:21:46 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87c43536e4dd825be5b2d7fd17dece2918488aad1465d7705a6f1f6881385ab`  
		Last Modified: Tue, 08 Dec 2020 00:55:08 GMT  
		Size: 19.3 MB (19312628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da07d458158604b556747c97b46ca3b94220598c8b5affa77df64a88f516e8b0`  
		Last Modified: Tue, 19 Jan 2021 22:23:00 GMT  
		Size: 66.1 MB (66104998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f629b4213fc30e9e7d83d4df23963c1ad2d80b18c35ed6558fbbbca2b1ebafb`  
		Last Modified: Tue, 19 Jan 2021 22:22:52 GMT  
		Size: 1.5 KB (1548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a942f2e5a252f9154decbbadbe78fe2466a587e99967271f2bd313f17f17bce5`  
		Last Modified: Tue, 19 Jan 2021 22:22:48 GMT  
		Size: 4.1 KB (4072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da160ec527545ff4dbe37740c18bff0e3dce3d86e3e8819df289d84e97d40594`  
		Last Modified: Tue, 19 Jan 2021 22:22:48 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808bd34d3a7178cbb92de2b7202d2ab863be7d506e67ced8bca08180bd7cd927`  
		Last Modified: Tue, 19 Jan 2021 22:22:48 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9b7c6020308bad1f3fc987caf2d5b185e8df1f910446bfcf82f07e274f2e4b`  
		Last Modified: Tue, 19 Jan 2021 22:22:49 GMT  
		Size: 8.1 MB (8137894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c10a37ecd85a8207a073170b747d5e90eb42a0f13ed60211e09179b9db03ed2`  
		Last Modified: Tue, 19 Jan 2021 22:22:48 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.0.22`

```console
$ docker pull percona@sha256:a4cae12e9e3dcb8e91ba95a15fb536ca6224915ca392da98ef8a66e88b4af246
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0.22` - linux; amd64

```console
$ docker pull percona@sha256:bb24cef54cae1928b29b5c3b1a9af057980670db80fe2e01e0e58b4b17356e4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.7 MB (169672809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:809f4f0126f0de3468e2db57f22efd983f1c9f8cc4960b086c5fd088f6405fb9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:51:44 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-40 release
# Tue, 19 Jan 2021 22:21:16 GMT
ENV PSMDB_VERSION=4.0.22-17
# Tue, 19 Jan 2021 22:21:16 GMT
ENV OS_VER=el8
# Tue, 19 Jan 2021 22:21:16 GMT
ENV FULL_PERCONA_VERSION=4.0.22-17.el8
# Tue, 19 Jan 2021 22:21:16 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 19 Jan 2021 22:21:38 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Tue, 19 Jan 2021 22:21:39 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 19 Jan 2021 22:21:39 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 19 Jan 2021 22:21:40 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 19 Jan 2021 22:21:40 GMT
ENV GOSU_VERSION=1.11
# Tue, 19 Jan 2021 22:21:43 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Tue, 19 Jan 2021 22:21:45 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 19 Jan 2021 22:21:45 GMT
VOLUME [/data/db]
# Tue, 19 Jan 2021 22:21:46 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Tue, 19 Jan 2021 22:21:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Jan 2021 22:21:46 GMT
EXPOSE 27017
# Tue, 19 Jan 2021 22:21:46 GMT
USER 1001
# Tue, 19 Jan 2021 22:21:46 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87c43536e4dd825be5b2d7fd17dece2918488aad1465d7705a6f1f6881385ab`  
		Last Modified: Tue, 08 Dec 2020 00:55:08 GMT  
		Size: 19.3 MB (19312628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da07d458158604b556747c97b46ca3b94220598c8b5affa77df64a88f516e8b0`  
		Last Modified: Tue, 19 Jan 2021 22:23:00 GMT  
		Size: 66.1 MB (66104998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f629b4213fc30e9e7d83d4df23963c1ad2d80b18c35ed6558fbbbca2b1ebafb`  
		Last Modified: Tue, 19 Jan 2021 22:22:52 GMT  
		Size: 1.5 KB (1548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a942f2e5a252f9154decbbadbe78fe2466a587e99967271f2bd313f17f17bce5`  
		Last Modified: Tue, 19 Jan 2021 22:22:48 GMT  
		Size: 4.1 KB (4072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da160ec527545ff4dbe37740c18bff0e3dce3d86e3e8819df289d84e97d40594`  
		Last Modified: Tue, 19 Jan 2021 22:22:48 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808bd34d3a7178cbb92de2b7202d2ab863be7d506e67ced8bca08180bd7cd927`  
		Last Modified: Tue, 19 Jan 2021 22:22:48 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9b7c6020308bad1f3fc987caf2d5b185e8df1f910446bfcf82f07e274f2e4b`  
		Last Modified: Tue, 19 Jan 2021 22:22:49 GMT  
		Size: 8.1 MB (8137894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c10a37ecd85a8207a073170b747d5e90eb42a0f13ed60211e09179b9db03ed2`  
		Last Modified: Tue, 19 Jan 2021 22:22:48 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:77e45ed05a5cf470df0b0acbbb8ea1af5507cafc900e1df91a1b986bbaa4575f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:207293b3dfd7414d994520fc64bba4998169b677125655b05dca17ce5324f74a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.5 MB (181461618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df3dab167c41b8b6bb91935e3a954c16f4f49291a65366b6f8091460d9981e51`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 21 Dec 2020 20:56:48 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Fri, 05 Feb 2021 03:51:37 GMT
ENV PSMDB_VERSION=4.2.12-13
# Fri, 05 Feb 2021 03:51:37 GMT
ENV OS_VER=el8
# Fri, 05 Feb 2021 03:51:37 GMT
ENV FULL_PERCONA_VERSION=4.2.12-13.el8
# Fri, 05 Feb 2021 03:51:38 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Fri, 05 Feb 2021 03:52:06 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Fri, 05 Feb 2021 03:52:07 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Fri, 05 Feb 2021 03:52:08 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Fri, 05 Feb 2021 03:52:09 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Fri, 05 Feb 2021 03:52:10 GMT
ENV GOSU_VERSION=1.11
# Fri, 05 Feb 2021 03:52:12 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Fri, 05 Feb 2021 03:52:15 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Fri, 05 Feb 2021 03:52:15 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Fri, 05 Feb 2021 03:52:16 GMT
VOLUME [/data/db]
# Fri, 05 Feb 2021 03:52:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 05 Feb 2021 03:52:16 GMT
EXPOSE 27017
# Fri, 05 Feb 2021 03:52:17 GMT
USER 1001
# Fri, 05 Feb 2021 03:52:18 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d01f42cbe2e951cb89ccb275a413326c4661a29bc539cd3017515834f3fde`  
		Last Modified: Mon, 21 Dec 2020 21:01:51 GMT  
		Size: 19.5 MB (19481154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e861403de0098a41e509199af4c37c45067caab6a6e5736f6df86a2719645d`  
		Last Modified: Fri, 05 Feb 2021 03:53:24 GMT  
		Size: 77.7 MB (77725285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20809edb7c6ce00b170ec16993d1ce67468cfb2d8735da4520208732440e0ae1`  
		Last Modified: Fri, 05 Feb 2021 03:53:09 GMT  
		Size: 1.5 KB (1546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0952a1f5e14f5381180e6ca88a5ec131be2fd417bc7ec31d07cd9f937b5a1cf`  
		Last Modified: Fri, 05 Feb 2021 03:53:08 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e76442d5e51ab9d3fd450da640c97268e9c9ef7d6955aac23370029574f5d78`  
		Last Modified: Fri, 05 Feb 2021 03:53:08 GMT  
		Size: 10.6 KB (10577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3383c6bedf30e852010c098f156580904915f3e9e8de9d41b2ebd7ae191beddc`  
		Last Modified: Fri, 05 Feb 2021 03:53:09 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d6324a1c0753fa03ad77c017a2694d8467a7e4430b7d610087b8a95ec5040b`  
		Last Modified: Fri, 05 Feb 2021 03:53:10 GMT  
		Size: 8.1 MB (8137891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9430755f7133c5f6af0f2d151f2a009661b11bdb3761bc00489e6c4f27ab3dea`  
		Last Modified: Fri, 05 Feb 2021 03:53:08 GMT  
		Size: 4.5 KB (4541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2.12`

```console
$ docker pull percona@sha256:77e45ed05a5cf470df0b0acbbb8ea1af5507cafc900e1df91a1b986bbaa4575f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.2.12` - linux; amd64

```console
$ docker pull percona@sha256:207293b3dfd7414d994520fc64bba4998169b677125655b05dca17ce5324f74a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.5 MB (181461618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df3dab167c41b8b6bb91935e3a954c16f4f49291a65366b6f8091460d9981e51`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 21 Dec 2020 20:56:48 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Fri, 05 Feb 2021 03:51:37 GMT
ENV PSMDB_VERSION=4.2.12-13
# Fri, 05 Feb 2021 03:51:37 GMT
ENV OS_VER=el8
# Fri, 05 Feb 2021 03:51:37 GMT
ENV FULL_PERCONA_VERSION=4.2.12-13.el8
# Fri, 05 Feb 2021 03:51:38 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Fri, 05 Feb 2021 03:52:06 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Fri, 05 Feb 2021 03:52:07 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Fri, 05 Feb 2021 03:52:08 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Fri, 05 Feb 2021 03:52:09 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Fri, 05 Feb 2021 03:52:10 GMT
ENV GOSU_VERSION=1.11
# Fri, 05 Feb 2021 03:52:12 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Fri, 05 Feb 2021 03:52:15 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Fri, 05 Feb 2021 03:52:15 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Fri, 05 Feb 2021 03:52:16 GMT
VOLUME [/data/db]
# Fri, 05 Feb 2021 03:52:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 05 Feb 2021 03:52:16 GMT
EXPOSE 27017
# Fri, 05 Feb 2021 03:52:17 GMT
USER 1001
# Fri, 05 Feb 2021 03:52:18 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d01f42cbe2e951cb89ccb275a413326c4661a29bc539cd3017515834f3fde`  
		Last Modified: Mon, 21 Dec 2020 21:01:51 GMT  
		Size: 19.5 MB (19481154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e861403de0098a41e509199af4c37c45067caab6a6e5736f6df86a2719645d`  
		Last Modified: Fri, 05 Feb 2021 03:53:24 GMT  
		Size: 77.7 MB (77725285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20809edb7c6ce00b170ec16993d1ce67468cfb2d8735da4520208732440e0ae1`  
		Last Modified: Fri, 05 Feb 2021 03:53:09 GMT  
		Size: 1.5 KB (1546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0952a1f5e14f5381180e6ca88a5ec131be2fd417bc7ec31d07cd9f937b5a1cf`  
		Last Modified: Fri, 05 Feb 2021 03:53:08 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e76442d5e51ab9d3fd450da640c97268e9c9ef7d6955aac23370029574f5d78`  
		Last Modified: Fri, 05 Feb 2021 03:53:08 GMT  
		Size: 10.6 KB (10577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3383c6bedf30e852010c098f156580904915f3e9e8de9d41b2ebd7ae191beddc`  
		Last Modified: Fri, 05 Feb 2021 03:53:09 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d6324a1c0753fa03ad77c017a2694d8467a7e4430b7d610087b8a95ec5040b`  
		Last Modified: Fri, 05 Feb 2021 03:53:10 GMT  
		Size: 8.1 MB (8137891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9430755f7133c5f6af0f2d151f2a009661b11bdb3761bc00489e6c4f27ab3dea`  
		Last Modified: Fri, 05 Feb 2021 03:53:08 GMT  
		Size: 4.5 KB (4541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.4`

```console
$ docker pull percona@sha256:a09c214c83518b975700a0fd2a27e770d5d4774a20e9b89fe969361964c396b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.4` - linux; amd64

```console
$ docker pull percona@sha256:30eb0671e148351c94d7c14f94979b7f615d6309d7dc4e62708840ed48c831c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.3 MB (200313722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d56f28a168f65096821f9493308543a1e404138fdefe6713d2004aed7077c1d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 21 Dec 2020 20:52:15 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Tue, 02 Feb 2021 02:17:01 GMT
ENV PSMDB_VERSION=4.4.3-5
# Tue, 02 Feb 2021 02:17:02 GMT
ENV OS_VER=el8
# Tue, 02 Feb 2021 02:17:02 GMT
ENV FULL_PERCONA_VERSION=4.4.3-5.el8
# Tue, 02 Feb 2021 02:17:02 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 02 Feb 2021 02:17:37 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Tue, 02 Feb 2021 02:17:38 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 02 Feb 2021 02:17:38 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 02 Feb 2021 02:17:39 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 02 Feb 2021 02:17:39 GMT
ENV GOSU_VERSION=1.11
# Tue, 02 Feb 2021 02:17:42 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Tue, 02 Feb 2021 02:17:44 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 02 Feb 2021 02:17:44 GMT
COPY file:1e164890dbc426ff0038117af76a47815ae534b64e95a15a83e6e5d7f79a4d77 in /entrypoint.sh 
# Tue, 02 Feb 2021 02:17:44 GMT
VOLUME [/data/db]
# Tue, 02 Feb 2021 02:17:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 Feb 2021 02:17:44 GMT
EXPOSE 27017
# Tue, 02 Feb 2021 02:17:45 GMT
USER 1001
# Tue, 02 Feb 2021 02:17:45 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2acf9799d0998bd2c0650b3450cdfa5c5a4dd09a53a5d2107305b0e99b208b8`  
		Last Modified: Mon, 21 Dec 2020 20:58:18 GMT  
		Size: 19.5 MB (19481136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be45162f63f6b96b82e92bd9872c6360d28e921c29089175b1ff5135de42f5d`  
		Last Modified: Tue, 02 Feb 2021 02:19:00 GMT  
		Size: 96.6 MB (96577404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb45148c3ae37f22062bdef25a3a38f7fb3fbd6644608c7701970424d424f64f`  
		Last Modified: Tue, 02 Feb 2021 02:18:45 GMT  
		Size: 1.5 KB (1546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf5ed8c5b1f23d8df2648229243e90ad020be2dc0df89f25dff07209503a1fc`  
		Last Modified: Tue, 02 Feb 2021 02:18:45 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75ada0f6c49845565be69dea6d0393a387a525ae3f66c527f498bd124ecf9fd`  
		Last Modified: Tue, 02 Feb 2021 02:18:46 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169c8e02832c39bebb549462da84ec7a49ffcf173611b8051e7c7b6a85f2d815`  
		Last Modified: Tue, 02 Feb 2021 02:18:45 GMT  
		Size: 914.6 KB (914552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97ad666fb33f6d96ddb8709395f7afc61d17c3b3189d2f567165284ef31b028`  
		Last Modified: Tue, 02 Feb 2021 02:18:56 GMT  
		Size: 8.1 MB (8137890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2ed30031fdabe29eaa40e1f6211ea4fcb8b2eb8b10288f61a1d4cfd83f3885`  
		Last Modified: Tue, 02 Feb 2021 02:18:44 GMT  
		Size: 4.5 KB (4544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.4.3`

```console
$ docker pull percona@sha256:a09c214c83518b975700a0fd2a27e770d5d4774a20e9b89fe969361964c396b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.4.3` - linux; amd64

```console
$ docker pull percona@sha256:30eb0671e148351c94d7c14f94979b7f615d6309d7dc4e62708840ed48c831c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.3 MB (200313722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d56f28a168f65096821f9493308543a1e404138fdefe6713d2004aed7077c1d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 21 Dec 2020 20:52:15 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Tue, 02 Feb 2021 02:17:01 GMT
ENV PSMDB_VERSION=4.4.3-5
# Tue, 02 Feb 2021 02:17:02 GMT
ENV OS_VER=el8
# Tue, 02 Feb 2021 02:17:02 GMT
ENV FULL_PERCONA_VERSION=4.4.3-5.el8
# Tue, 02 Feb 2021 02:17:02 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 02 Feb 2021 02:17:37 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Tue, 02 Feb 2021 02:17:38 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 02 Feb 2021 02:17:38 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 02 Feb 2021 02:17:39 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 02 Feb 2021 02:17:39 GMT
ENV GOSU_VERSION=1.11
# Tue, 02 Feb 2021 02:17:42 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Tue, 02 Feb 2021 02:17:44 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 02 Feb 2021 02:17:44 GMT
COPY file:1e164890dbc426ff0038117af76a47815ae534b64e95a15a83e6e5d7f79a4d77 in /entrypoint.sh 
# Tue, 02 Feb 2021 02:17:44 GMT
VOLUME [/data/db]
# Tue, 02 Feb 2021 02:17:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 Feb 2021 02:17:44 GMT
EXPOSE 27017
# Tue, 02 Feb 2021 02:17:45 GMT
USER 1001
# Tue, 02 Feb 2021 02:17:45 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2acf9799d0998bd2c0650b3450cdfa5c5a4dd09a53a5d2107305b0e99b208b8`  
		Last Modified: Mon, 21 Dec 2020 20:58:18 GMT  
		Size: 19.5 MB (19481136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be45162f63f6b96b82e92bd9872c6360d28e921c29089175b1ff5135de42f5d`  
		Last Modified: Tue, 02 Feb 2021 02:19:00 GMT  
		Size: 96.6 MB (96577404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb45148c3ae37f22062bdef25a3a38f7fb3fbd6644608c7701970424d424f64f`  
		Last Modified: Tue, 02 Feb 2021 02:18:45 GMT  
		Size: 1.5 KB (1546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf5ed8c5b1f23d8df2648229243e90ad020be2dc0df89f25dff07209503a1fc`  
		Last Modified: Tue, 02 Feb 2021 02:18:45 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75ada0f6c49845565be69dea6d0393a387a525ae3f66c527f498bd124ecf9fd`  
		Last Modified: Tue, 02 Feb 2021 02:18:46 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169c8e02832c39bebb549462da84ec7a49ffcf173611b8051e7c7b6a85f2d815`  
		Last Modified: Tue, 02 Feb 2021 02:18:45 GMT  
		Size: 914.6 KB (914552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97ad666fb33f6d96ddb8709395f7afc61d17c3b3189d2f567165284ef31b028`  
		Last Modified: Tue, 02 Feb 2021 02:18:56 GMT  
		Size: 8.1 MB (8137890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2ed30031fdabe29eaa40e1f6211ea4fcb8b2eb8b10288f61a1d4cfd83f3885`  
		Last Modified: Tue, 02 Feb 2021 02:18:44 GMT  
		Size: 4.5 KB (4544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
