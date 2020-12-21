<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `percona`

-	[`percona:5`](#percona5)
-	[`percona:5.6`](#percona56)
-	[`percona:5.6.50`](#percona5650)
-	[`percona:5.6.50-centos`](#percona5650-centos)
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
-	[`percona:ps-5.6.50`](#perconaps-5650)
-	[`percona:ps-5.7`](#perconaps-57)
-	[`percona:ps-5.7.32`](#perconaps-5732)
-	[`percona:ps-8`](#perconaps-8)
-	[`percona:ps-8.0`](#perconaps-80)
-	[`percona:ps-8.0.22-13`](#perconaps-8022-13)
-	[`percona:psmdb-3.6`](#perconapsmdb-36)
-	[`percona:psmdb-3.6.21`](#perconapsmdb-3621)
-	[`percona:psmdb-4.0`](#perconapsmdb-40)
-	[`percona:psmdb-4.0.21`](#perconapsmdb-4021)
-	[`percona:psmdb-4.2`](#perconapsmdb-42)
-	[`percona:psmdb-4.2.11`](#perconapsmdb-4211)
-	[`percona:psmdb-4.4`](#perconapsmdb-44)
-	[`percona:psmdb-4.4.2`](#perconapsmdb-442)

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

## `percona:5.6.50`

```console
$ docker pull percona@sha256:b6bc17e2a4572723e3fe86f9238afcfb7c6dd3d257d2db6b86f8b0938227ce52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.6.50` - linux; amd64

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

## `percona:5.6.50-centos`

```console
$ docker pull percona@sha256:b6bc17e2a4572723e3fe86f9238afcfb7c6dd3d257d2db6b86f8b0938227ce52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.6.50-centos` - linux; amd64

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

## `percona:ps-5.6.50`

```console
$ docker pull percona@sha256:b6bc17e2a4572723e3fe86f9238afcfb7c6dd3d257d2db6b86f8b0938227ce52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.6.50` - linux; amd64

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
$ docker pull percona@sha256:2cfe7be10c7c235c80b1823e30cc464dbdbd1d01669778f7b5899aeaac0249f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6` - linux; amd64

```console
$ docker pull percona@sha256:e0b1772ca5316e73d7fd9d41df22e022f3c611bdae347bb29318720e8aaaa0df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.1 MB (159137498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98f2e7711382c9eb5288420a65eba6c6f6094c4538dea65e6f08bcb8eba8c577`
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
# Tue, 08 Dec 2020 00:52:24 GMT
ENV PSMDB_VERSION=3.6.21-10.0
# Tue, 08 Dec 2020 00:52:24 GMT
ENV OS_VER=el8
# Tue, 08 Dec 2020 00:52:24 GMT
ENV FULL_PERCONA_VERSION=3.6.21-10.0.el8
# Tue, 08 Dec 2020 00:52:24 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 08 Dec 2020 00:52:41 GMT
RUN set -ex;     dnf install -y         dnf-utils         shadow-utils         curl         procps-ng         jq         oniguruma         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         dnf remove -y dnf-utils;         dnf clean all;         rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Tue, 08 Dec 2020 00:52:42 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 08 Dec 2020 00:52:43 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 08 Dec 2020 00:52:43 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 08 Dec 2020 00:52:46 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 08 Dec 2020 00:52:46 GMT
VOLUME [/data/db]
# Tue, 08 Dec 2020 00:52:46 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Tue, 08 Dec 2020 00:52:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Dec 2020 00:52:46 GMT
EXPOSE 27017
# Tue, 08 Dec 2020 00:52:47 GMT
USER 1001
# Tue, 08 Dec 2020 00:52:47 GMT
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
	-	`sha256:c0da165138b104d3beea941fdf4c9b25b517a2084c441c075ffc0a1043390247`  
		Last Modified: Tue, 08 Dec 2020 00:55:30 GMT  
		Size: 56.5 MB (56484164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34386f4f91111324c674ab4dd614e8a856563facfd87cf837fde0ffa610515c`  
		Last Modified: Tue, 08 Dec 2020 00:55:19 GMT  
		Size: 1.5 KB (1542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aae57e9a7a9bfc979c195f4403ae3dc49bda5c5bf9135fb7b0dbd6a2da34dbe`  
		Last Modified: Tue, 08 Dec 2020 00:55:19 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d6369dc1c044571c9b21a40f8856f36b7d35a04c319d163a79952bfff42608`  
		Last Modified: Tue, 08 Dec 2020 00:55:19 GMT  
		Size: 10.6 KB (10577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b70698a843a6dff6c04d4b7b756bd0d1d3be0313e48d208df3099fe0d133b1`  
		Last Modified: Tue, 08 Dec 2020 00:55:20 GMT  
		Size: 8.1 MB (8137888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfbb18a7d279fefc06c7be04364eaf06dc7cbd108490e1dbf5f30892c7362d3`  
		Last Modified: Tue, 08 Dec 2020 00:55:19 GMT  
		Size: 4.5 KB (4540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-3.6.21`

```console
$ docker pull percona@sha256:2cfe7be10c7c235c80b1823e30cc464dbdbd1d01669778f7b5899aeaac0249f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6.21` - linux; amd64

```console
$ docker pull percona@sha256:e0b1772ca5316e73d7fd9d41df22e022f3c611bdae347bb29318720e8aaaa0df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.1 MB (159137498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98f2e7711382c9eb5288420a65eba6c6f6094c4538dea65e6f08bcb8eba8c577`
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
# Tue, 08 Dec 2020 00:52:24 GMT
ENV PSMDB_VERSION=3.6.21-10.0
# Tue, 08 Dec 2020 00:52:24 GMT
ENV OS_VER=el8
# Tue, 08 Dec 2020 00:52:24 GMT
ENV FULL_PERCONA_VERSION=3.6.21-10.0.el8
# Tue, 08 Dec 2020 00:52:24 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 08 Dec 2020 00:52:41 GMT
RUN set -ex;     dnf install -y         dnf-utils         shadow-utils         curl         procps-ng         jq         oniguruma         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         dnf remove -y dnf-utils;         dnf clean all;         rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Tue, 08 Dec 2020 00:52:42 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 08 Dec 2020 00:52:43 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 08 Dec 2020 00:52:43 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 08 Dec 2020 00:52:46 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 08 Dec 2020 00:52:46 GMT
VOLUME [/data/db]
# Tue, 08 Dec 2020 00:52:46 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Tue, 08 Dec 2020 00:52:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Dec 2020 00:52:46 GMT
EXPOSE 27017
# Tue, 08 Dec 2020 00:52:47 GMT
USER 1001
# Tue, 08 Dec 2020 00:52:47 GMT
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
	-	`sha256:c0da165138b104d3beea941fdf4c9b25b517a2084c441c075ffc0a1043390247`  
		Last Modified: Tue, 08 Dec 2020 00:55:30 GMT  
		Size: 56.5 MB (56484164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34386f4f91111324c674ab4dd614e8a856563facfd87cf837fde0ffa610515c`  
		Last Modified: Tue, 08 Dec 2020 00:55:19 GMT  
		Size: 1.5 KB (1542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aae57e9a7a9bfc979c195f4403ae3dc49bda5c5bf9135fb7b0dbd6a2da34dbe`  
		Last Modified: Tue, 08 Dec 2020 00:55:19 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d6369dc1c044571c9b21a40f8856f36b7d35a04c319d163a79952bfff42608`  
		Last Modified: Tue, 08 Dec 2020 00:55:19 GMT  
		Size: 10.6 KB (10577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b70698a843a6dff6c04d4b7b756bd0d1d3be0313e48d208df3099fe0d133b1`  
		Last Modified: Tue, 08 Dec 2020 00:55:20 GMT  
		Size: 8.1 MB (8137888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfbb18a7d279fefc06c7be04364eaf06dc7cbd108490e1dbf5f30892c7362d3`  
		Last Modified: Tue, 08 Dec 2020 00:55:19 GMT  
		Size: 4.5 KB (4540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.0`

```console
$ docker pull percona@sha256:757b4cfd71a236746f0bdabbe12d113c07903922140385262b3b4183bec426c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0` - linux; amd64

```console
$ docker pull percona@sha256:6686b754be4dc58daac9486cc7cd78bf0a5884ba06d50c6ef1783ab790b37991
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161645360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc0a9e365b49fc9194c60180b44dd1e05b22b1a6a176835d71c307a54b7c0d67`
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
# Tue, 08 Dec 2020 00:51:44 GMT
ENV PSMDB_VERSION=4.0.21-15
# Tue, 08 Dec 2020 00:51:44 GMT
ENV OS_VER=el8
# Tue, 08 Dec 2020 00:51:44 GMT
ENV FULL_PERCONA_VERSION=4.0.21-15.el8
# Tue, 08 Dec 2020 00:51:44 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 08 Dec 2020 00:52:05 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Tue, 08 Dec 2020 00:52:06 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 08 Dec 2020 00:52:07 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 08 Dec 2020 00:52:08 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 08 Dec 2020 00:52:08 GMT
ENV GOSU_VERSION=1.11
# Tue, 08 Dec 2020 00:52:10 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Tue, 08 Dec 2020 00:52:12 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 08 Dec 2020 00:52:12 GMT
VOLUME [/data/db]
# Tue, 08 Dec 2020 00:52:12 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Tue, 08 Dec 2020 00:52:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Dec 2020 00:52:12 GMT
EXPOSE 27017
# Tue, 08 Dec 2020 00:52:13 GMT
USER 1001
# Tue, 08 Dec 2020 00:52:13 GMT
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
	-	`sha256:c054ceae55f6381ed5b7fa4d40bf8474af2a9ffd00c4ed7189416981c30a495d`  
		Last Modified: Tue, 08 Dec 2020 00:55:14 GMT  
		Size: 58.1 MB (58077566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e815a5f9e8e38ec7677fef1026898fb92321f26972fee395ec06c1ff8dbc4c31`  
		Last Modified: Tue, 08 Dec 2020 00:55:03 GMT  
		Size: 1.5 KB (1540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74176ced44f98f483c8e9d5a5e6f316f8482bfa371d2fd0bfde4c21214aa1b9e`  
		Last Modified: Tue, 08 Dec 2020 00:55:02 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccce96a5e3e9493afba1221df36d8f6e55fe8dd23dcf86a5a638a9cd9c152db`  
		Last Modified: Tue, 08 Dec 2020 00:55:02 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2250ef6e725a8f51b4d35b77433dd5a32843f3963160b44c0b77fe8a3d615e36`  
		Last Modified: Tue, 08 Dec 2020 00:55:02 GMT  
		Size: 914.5 KB (914543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1789370336f1e1599ed2be59ef8c088b6547132a7e5a2ca9d824dd2a4f13479`  
		Last Modified: Tue, 08 Dec 2020 00:55:04 GMT  
		Size: 8.1 MB (8137893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbbfa721e23f6a0f31fef1e7a37f1b8b0863e945d8cbca29dc6cc8b96b1b633`  
		Last Modified: Tue, 08 Dec 2020 00:55:02 GMT  
		Size: 4.5 KB (4540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.0.21`

```console
$ docker pull percona@sha256:757b4cfd71a236746f0bdabbe12d113c07903922140385262b3b4183bec426c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0.21` - linux; amd64

```console
$ docker pull percona@sha256:6686b754be4dc58daac9486cc7cd78bf0a5884ba06d50c6ef1783ab790b37991
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161645360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc0a9e365b49fc9194c60180b44dd1e05b22b1a6a176835d71c307a54b7c0d67`
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
# Tue, 08 Dec 2020 00:51:44 GMT
ENV PSMDB_VERSION=4.0.21-15
# Tue, 08 Dec 2020 00:51:44 GMT
ENV OS_VER=el8
# Tue, 08 Dec 2020 00:51:44 GMT
ENV FULL_PERCONA_VERSION=4.0.21-15.el8
# Tue, 08 Dec 2020 00:51:44 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 08 Dec 2020 00:52:05 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Tue, 08 Dec 2020 00:52:06 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 08 Dec 2020 00:52:07 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 08 Dec 2020 00:52:08 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 08 Dec 2020 00:52:08 GMT
ENV GOSU_VERSION=1.11
# Tue, 08 Dec 2020 00:52:10 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Tue, 08 Dec 2020 00:52:12 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 08 Dec 2020 00:52:12 GMT
VOLUME [/data/db]
# Tue, 08 Dec 2020 00:52:12 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Tue, 08 Dec 2020 00:52:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Dec 2020 00:52:12 GMT
EXPOSE 27017
# Tue, 08 Dec 2020 00:52:13 GMT
USER 1001
# Tue, 08 Dec 2020 00:52:13 GMT
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
	-	`sha256:c054ceae55f6381ed5b7fa4d40bf8474af2a9ffd00c4ed7189416981c30a495d`  
		Last Modified: Tue, 08 Dec 2020 00:55:14 GMT  
		Size: 58.1 MB (58077566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e815a5f9e8e38ec7677fef1026898fb92321f26972fee395ec06c1ff8dbc4c31`  
		Last Modified: Tue, 08 Dec 2020 00:55:03 GMT  
		Size: 1.5 KB (1540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74176ced44f98f483c8e9d5a5e6f316f8482bfa371d2fd0bfde4c21214aa1b9e`  
		Last Modified: Tue, 08 Dec 2020 00:55:02 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccce96a5e3e9493afba1221df36d8f6e55fe8dd23dcf86a5a638a9cd9c152db`  
		Last Modified: Tue, 08 Dec 2020 00:55:02 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2250ef6e725a8f51b4d35b77433dd5a32843f3963160b44c0b77fe8a3d615e36`  
		Last Modified: Tue, 08 Dec 2020 00:55:02 GMT  
		Size: 914.5 KB (914543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1789370336f1e1599ed2be59ef8c088b6547132a7e5a2ca9d824dd2a4f13479`  
		Last Modified: Tue, 08 Dec 2020 00:55:04 GMT  
		Size: 8.1 MB (8137893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbbfa721e23f6a0f31fef1e7a37f1b8b0863e945d8cbca29dc6cc8b96b1b633`  
		Last Modified: Tue, 08 Dec 2020 00:55:02 GMT  
		Size: 4.5 KB (4540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:af17aad82d40a565b7d89f2b6b810700b1ace8051bb6613ba6a502cb13573f44
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:474022685cc8cf5bc4cde8f7d18f41e7e91e6208103d0ab8e4b72e487c046bc8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.3 MB (170345414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d811d4aeecf5879556f450cd36f6baaced7591d5e9e8ee0ec4971c167f1338a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:49:57 GMT
LABEL org.label-schema.schema-version=1.0
# Tue, 08 Dec 2020 00:49:57 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Tue, 08 Dec 2020 00:49:57 GMT
LABEL org.label-schema.vendor=Percona
# Tue, 08 Dec 2020 00:49:57 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Tue, 08 Dec 2020 00:49:57 GMT
LABEL org.label-schema.license=SSPLv1
# Tue, 08 Dec 2020 00:49:57 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Tue, 08 Dec 2020 00:49:58 GMT
LABEL org.opencontainers.image.vendor=Percona
# Tue, 08 Dec 2020 00:49:58 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Tue, 08 Dec 2020 00:49:58 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Tue, 08 Dec 2020 00:49:58 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:50:43 GMT
ENV PSMDB_VERSION=4.2.10-11
# Tue, 08 Dec 2020 00:50:43 GMT
ENV OS_VER=el8
# Tue, 08 Dec 2020 00:50:43 GMT
ENV FULL_PERCONA_VERSION=4.2.10-11.el8
# Tue, 08 Dec 2020 00:50:44 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 08 Dec 2020 00:50:44 GMT
LABEL org.label-schema.schema-version=4.2.10-11
# Tue, 08 Dec 2020 00:50:44 GMT
LABEL org.opencontainers.image.version=4.2.10-11
# Tue, 08 Dec 2020 00:50:51 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Tue, 08 Dec 2020 00:51:21 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Tue, 08 Dec 2020 00:51:22 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 08 Dec 2020 00:51:22 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 08 Dec 2020 00:51:23 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 08 Dec 2020 00:51:23 GMT
ENV GOSU_VERSION=1.11
# Tue, 08 Dec 2020 00:51:25 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Tue, 08 Dec 2020 00:51:28 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 08 Dec 2020 00:51:28 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Tue, 08 Dec 2020 00:51:28 GMT
VOLUME [/data/db]
# Tue, 08 Dec 2020 00:51:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Dec 2020 00:51:28 GMT
EXPOSE 27017
# Tue, 08 Dec 2020 00:51:29 GMT
USER 1001
# Tue, 08 Dec 2020 00:51:29 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5723d1df872fba296abf30e11965659cbfd5fa5e70b089b5f0425a15e6a5683b`  
		Last Modified: Tue, 08 Dec 2020 00:54:48 GMT  
		Size: 19.3 MB (19312686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f62f73716e00e46afb04c206753c5cd5a0a03dc8cd74ac38ae3740c4e00bbb`  
		Last Modified: Tue, 08 Dec 2020 00:54:56 GMT  
		Size: 66.8 MB (66777557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17022f63436b82a959074b329e8415bc67a9e611ade986cf30da8af1d7fe22f3`  
		Last Modified: Tue, 08 Dec 2020 00:54:44 GMT  
		Size: 1.5 KB (1544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bc955135f8961942d529eab9afedf3894d4fc901fe7620cbf9f9dd8c745453`  
		Last Modified: Tue, 08 Dec 2020 00:54:43 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32a8c7a3b2bbf01d478b8cd5ba29dbd2c22cee8a23e6e0b80e3ce1f8be93ac4`  
		Last Modified: Tue, 08 Dec 2020 00:54:43 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be69a7019d24de6c852b3c4845ece13b8a1d369f382f543a3fe08deb413543bd`  
		Last Modified: Tue, 08 Dec 2020 00:54:44 GMT  
		Size: 914.5 KB (914546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5d0fe2168a89ecdc3973ee96f915256c710134aca0264ac8c8ae2a6c0cc5b1`  
		Last Modified: Tue, 08 Dec 2020 00:54:45 GMT  
		Size: 8.1 MB (8137889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d071e8dee06e256f01de28f253e73a2ac897f4e6c7bdcb95d694446b1c4d108`  
		Last Modified: Tue, 08 Dec 2020 00:54:43 GMT  
		Size: 4.5 KB (4540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2.11`

**does not exist** (yet?)

## `percona:psmdb-4.4`

```console
$ docker pull percona@sha256:c405e40f772fe432b9fc07abeb634b68b7b80bc98cf984314034d3e8607535d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.4` - linux; amd64

```console
$ docker pull percona@sha256:a82f9094ac4313316b2d9e3f5dc2473d864ef3db985c4f141eaf7b062362135e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.8 MB (181833228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:213549748cf2b211d91755fb829bdd2d76bb2a27a2045f7734edd47335bccc3e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:49:57 GMT
LABEL org.label-schema.schema-version=1.0
# Tue, 08 Dec 2020 00:49:57 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Tue, 08 Dec 2020 00:49:57 GMT
LABEL org.label-schema.vendor=Percona
# Tue, 08 Dec 2020 00:49:57 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Tue, 08 Dec 2020 00:49:57 GMT
LABEL org.label-schema.license=SSPLv1
# Tue, 08 Dec 2020 00:49:57 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Tue, 08 Dec 2020 00:49:58 GMT
LABEL org.opencontainers.image.vendor=Percona
# Tue, 08 Dec 2020 00:49:58 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Tue, 08 Dec 2020 00:49:58 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Tue, 08 Dec 2020 00:49:58 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:49:58 GMT
ENV PSMDB_VERSION=4.4.1-3
# Tue, 08 Dec 2020 00:49:59 GMT
ENV OS_VER=el8
# Tue, 08 Dec 2020 00:49:59 GMT
ENV FULL_PERCONA_VERSION=4.4.1-3.el8
# Tue, 08 Dec 2020 00:49:59 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 08 Dec 2020 00:49:59 GMT
LABEL org.label-schema.schema-version=4.4.1-3
# Tue, 08 Dec 2020 00:49:59 GMT
LABEL org.opencontainers.image.version=4.4.1-3
# Tue, 08 Dec 2020 00:50:10 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Tue, 08 Dec 2020 00:50:29 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Tue, 08 Dec 2020 00:50:30 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 08 Dec 2020 00:50:30 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 08 Dec 2020 00:50:31 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 08 Dec 2020 00:50:31 GMT
ENV GOSU_VERSION=1.11
# Tue, 08 Dec 2020 00:50:34 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Tue, 08 Dec 2020 00:50:36 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 08 Dec 2020 00:50:36 GMT
COPY file:1e164890dbc426ff0038117af76a47815ae534b64e95a15a83e6e5d7f79a4d77 in /entrypoint.sh 
# Tue, 08 Dec 2020 00:50:36 GMT
VOLUME [/data/db]
# Tue, 08 Dec 2020 00:50:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Dec 2020 00:50:37 GMT
EXPOSE 27017
# Tue, 08 Dec 2020 00:50:37 GMT
USER 1001
# Tue, 08 Dec 2020 00:50:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d626aa99fae5a6d007be9acdd14fec57b0cf8cc02cb7feaedab9a1fd45f40b`  
		Last Modified: Tue, 08 Dec 2020 00:54:31 GMT  
		Size: 19.3 MB (19312630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389bd89b605e2a1ec72f4eeb864e971413cad83ba9d6225da304b1efdbbabb6b`  
		Last Modified: Tue, 08 Dec 2020 00:54:37 GMT  
		Size: 78.3 MB (78265419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc76837ef87dc4247bf2a2e9d1d474bcdaaf97fb6e79f27417a9a390de0b0e3`  
		Last Modified: Tue, 08 Dec 2020 00:54:25 GMT  
		Size: 1.5 KB (1543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc30d91a61866ca448d60682c2353dee760cd4ca0419bfcd9eba00b94407119d`  
		Last Modified: Tue, 08 Dec 2020 00:54:23 GMT  
		Size: 4.1 KB (4071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe008bf9496a5b462774354c3dd4c99b8fed5e1c675ef667823e4c0a1382149e`  
		Last Modified: Tue, 08 Dec 2020 00:54:24 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d977079d3aa2594d193acf398b38b61155c278f449490134dc8438de06c0d7`  
		Last Modified: Tue, 08 Dec 2020 00:54:23 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904262524fbb419c032ad192d972fb3535b89b51cecf5e5e50c39aa0fe7237cf`  
		Last Modified: Tue, 08 Dec 2020 00:54:26 GMT  
		Size: 8.1 MB (8137894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5953048d1690331934521c94e24711187734c85e8dcff0d5e28e8dd11684c7`  
		Last Modified: Tue, 08 Dec 2020 00:54:24 GMT  
		Size: 4.5 KB (4545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.4.2`

**does not exist** (yet?)
