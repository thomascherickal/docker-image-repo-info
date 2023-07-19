<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `percona`

-	[`percona:5`](#percona5)
-	[`percona:5-centos`](#percona5-centos)
-	[`percona:5.6`](#percona56)
-	[`percona:5.6-centos`](#percona56-centos)
-	[`percona:5.6.51-2`](#percona5651-2)
-	[`percona:5.6.51-2-centos`](#percona5651-2-centos)
-	[`percona:5.7`](#percona57)
-	[`percona:5.7-centos`](#percona57-centos)
-	[`percona:5.7.39`](#percona5739)
-	[`percona:5.7.39-centos`](#percona5739-centos)
-	[`percona:8`](#percona8)
-	[`percona:8-centos`](#percona8-centos)
-	[`percona:8.0`](#percona80)
-	[`percona:8.0-centos`](#percona80-centos)
-	[`percona:8.0.33-25`](#percona8033-25)
-	[`percona:8.0.33-25-centos`](#percona8033-25-centos)
-	[`percona:centos`](#perconacentos)
-	[`percona:ps-5`](#perconaps-5)
-	[`percona:ps-5.6`](#perconaps-56)
-	[`percona:ps-5.6.51-2`](#perconaps-5651-2)
-	[`percona:ps-5.7`](#perconaps-57)
-	[`percona:ps-5.7.39`](#perconaps-5739)
-	[`percona:ps-8`](#perconaps-8)
-	[`percona:ps-8.0`](#perconaps-80)
-	[`percona:ps-8.0.33-25`](#perconaps-8033-25)
-	[`percona:psmdb-4.2`](#perconapsmdb-42)
-	[`percona:psmdb-4.2.24`](#perconapsmdb-4224)
-	[`percona:psmdb-4.4`](#perconapsmdb-44)
-	[`percona:psmdb-4.4.22`](#perconapsmdb-4422)
-	[`percona:psmdb-5.0`](#perconapsmdb-50)
-	[`percona:psmdb-5.0.18`](#perconapsmdb-5018)
-	[`percona:psmdb-6.0`](#perconapsmdb-60)
-	[`percona:psmdb-6.0.6`](#perconapsmdb-606)

## `percona:5`

```console
$ docker pull percona@sha256:152551a63255c5e252858b5ca632082b275c048a086b1355c70925af64250f63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5` - linux; amd64

```console
$ docker pull percona@sha256:37dd6744679dc7ed62bd1f4929469530a06eaf7f15de88e8de10a01782eb784f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.8 MB (416792246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a7406e542f53a3e7a9855b461e71ebe566606461b004e7e4720502acdb26ac`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:54:56 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Wed, 19 Jul 2023 20:55:38 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Wed, 19 Jul 2023 20:55:39 GMT
ENV PS_VERSION=5.7.39-42.1
# Wed, 19 Jul 2023 20:55:39 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:55:39 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Wed, 19 Jul 2023 20:56:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Wed, 19 Jul 2023 20:56:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 19 Jul 2023 20:56:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 19 Jul 2023 20:56:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 19 Jul 2023 20:56:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:56:26 GMT
USER mysql
# Wed, 19 Jul 2023 20:56:26 GMT
EXPOSE 3306
# Wed, 19 Jul 2023 20:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461daf9f83a293e04611358beed29d44d873ea2c8e8ec5d7ff861c5880530150`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e369e7c761b19ce864cbdb8eee412673d760ff8011cea3da197a062340b1a1`  
		Last Modified: Wed, 19 Jul 2023 21:02:05 GMT  
		Size: 190.4 MB (190392071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b521a644912a1d8f52b9c4b16a66da3f8b381b9c5ebb2a6ed6dc01de15fe00`  
		Last Modified: Wed, 19 Jul 2023 21:02:12 GMT  
		Size: 137.5 MB (137526118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b84cf62dae1737678206fcf51e9eb2b62c3f15fe6a7b5807b8d64c62dc9224`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649ef554e0e53bb5da6b9b155236875e9e0670f1be9c6904f4d79fdbd82a6f98`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5-centos`

```console
$ docker pull percona@sha256:152551a63255c5e252858b5ca632082b275c048a086b1355c70925af64250f63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5-centos` - linux; amd64

```console
$ docker pull percona@sha256:37dd6744679dc7ed62bd1f4929469530a06eaf7f15de88e8de10a01782eb784f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.8 MB (416792246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a7406e542f53a3e7a9855b461e71ebe566606461b004e7e4720502acdb26ac`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:54:56 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Wed, 19 Jul 2023 20:55:38 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Wed, 19 Jul 2023 20:55:39 GMT
ENV PS_VERSION=5.7.39-42.1
# Wed, 19 Jul 2023 20:55:39 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:55:39 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Wed, 19 Jul 2023 20:56:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Wed, 19 Jul 2023 20:56:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 19 Jul 2023 20:56:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 19 Jul 2023 20:56:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 19 Jul 2023 20:56:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:56:26 GMT
USER mysql
# Wed, 19 Jul 2023 20:56:26 GMT
EXPOSE 3306
# Wed, 19 Jul 2023 20:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461daf9f83a293e04611358beed29d44d873ea2c8e8ec5d7ff861c5880530150`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e369e7c761b19ce864cbdb8eee412673d760ff8011cea3da197a062340b1a1`  
		Last Modified: Wed, 19 Jul 2023 21:02:05 GMT  
		Size: 190.4 MB (190392071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b521a644912a1d8f52b9c4b16a66da3f8b381b9c5ebb2a6ed6dc01de15fe00`  
		Last Modified: Wed, 19 Jul 2023 21:02:12 GMT  
		Size: 137.5 MB (137526118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b84cf62dae1737678206fcf51e9eb2b62c3f15fe6a7b5807b8d64c62dc9224`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649ef554e0e53bb5da6b9b155236875e9e0670f1be9c6904f4d79fdbd82a6f98`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6`

```console
$ docker pull percona@sha256:8c915f6fff3a43383938b4015ee3740dc1886fd5016a1404ff45b55de71e49cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5.6` - linux; amd64

```console
$ docker pull percona@sha256:a865615cf007e34fc520a72786a807909f8c75fd233388a0a0445fa82b5319cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.3 MB (195312192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56b1d76c933806bd31b1a5833d091c41c5bc6c9d0953c4a2c764668d37c6f79e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 18:58:17 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 15 Sep 2021 18:58:18 GMT
RUN groupdel input && groupadd -g 999 mysql
# Wed, 15 Sep 2021 18:58:19 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Dec 2021 19:25:24 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         curl -Lf -o /tmp/nss.rpm http://mirror.centos.org/centos/7/updates/x86_64/Packages/nss-3.67.0-4.el7_9.x86_64.rpm;     rpmkeys --checksig /tmp/nss.rpm;     yum install -y /tmp/nss.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Thu, 30 Dec 2021 19:25:25 GMT
ENV PERCONA_VERSION=5.6.51-rel91.0.1.el7
# Thu, 30 Dec 2021 19:36:53 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Thu, 30 Dec 2021 19:36:55 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Dec 2021 19:36:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Dec 2021 19:36:55 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Thu, 30 Dec 2021 19:36:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Dec 2021 19:36:56 GMT
USER mysql
# Thu, 30 Dec 2021 19:36:56 GMT
EXPOSE 3306
# Thu, 30 Dec 2021 19:36:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd68507e31292f16aa2d29907b401abd6ab53be7b485f2bdea2a7182e63d1af`  
		Last Modified: Wed, 15 Sep 2021 19:05:51 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ee280aea028899106d471852f72f47591667f5edf38214be74a6121932ea56`  
		Last Modified: Wed, 15 Sep 2021 19:05:49 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729721338aa7f33aa759726ffa7b1c50288e2dcae602d0323eecab0ff98c9c26`  
		Last Modified: Thu, 30 Dec 2021 19:38:06 GMT  
		Size: 59.7 MB (59728568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d8b9873953ce124f23ca0f1406a9518ca744b77cfbebdd6d9f79a785fa7a09`  
		Last Modified: Thu, 30 Dec 2021 19:38:08 GMT  
		Size: 59.5 MB (59476470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927c076538b02993035990718d78a0b06fe3a6fc95b571ce334ae270c2cd4cc8`  
		Last Modified: Thu, 30 Dec 2021 19:37:58 GMT  
		Size: 5.0 KB (4956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1806011b64a9860267de7f898bd25bd33c0a6a69901dc7f8319e855bea3c1303`  
		Last Modified: Thu, 30 Dec 2021 19:37:58 GMT  
		Size: 2.9 KB (2942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6-centos`

```console
$ docker pull percona@sha256:8c915f6fff3a43383938b4015ee3740dc1886fd5016a1404ff45b55de71e49cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5.6-centos` - linux; amd64

```console
$ docker pull percona@sha256:a865615cf007e34fc520a72786a807909f8c75fd233388a0a0445fa82b5319cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.3 MB (195312192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56b1d76c933806bd31b1a5833d091c41c5bc6c9d0953c4a2c764668d37c6f79e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 18:58:17 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 15 Sep 2021 18:58:18 GMT
RUN groupdel input && groupadd -g 999 mysql
# Wed, 15 Sep 2021 18:58:19 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Dec 2021 19:25:24 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         curl -Lf -o /tmp/nss.rpm http://mirror.centos.org/centos/7/updates/x86_64/Packages/nss-3.67.0-4.el7_9.x86_64.rpm;     rpmkeys --checksig /tmp/nss.rpm;     yum install -y /tmp/nss.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Thu, 30 Dec 2021 19:25:25 GMT
ENV PERCONA_VERSION=5.6.51-rel91.0.1.el7
# Thu, 30 Dec 2021 19:36:53 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Thu, 30 Dec 2021 19:36:55 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Dec 2021 19:36:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Dec 2021 19:36:55 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Thu, 30 Dec 2021 19:36:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Dec 2021 19:36:56 GMT
USER mysql
# Thu, 30 Dec 2021 19:36:56 GMT
EXPOSE 3306
# Thu, 30 Dec 2021 19:36:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd68507e31292f16aa2d29907b401abd6ab53be7b485f2bdea2a7182e63d1af`  
		Last Modified: Wed, 15 Sep 2021 19:05:51 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ee280aea028899106d471852f72f47591667f5edf38214be74a6121932ea56`  
		Last Modified: Wed, 15 Sep 2021 19:05:49 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729721338aa7f33aa759726ffa7b1c50288e2dcae602d0323eecab0ff98c9c26`  
		Last Modified: Thu, 30 Dec 2021 19:38:06 GMT  
		Size: 59.7 MB (59728568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d8b9873953ce124f23ca0f1406a9518ca744b77cfbebdd6d9f79a785fa7a09`  
		Last Modified: Thu, 30 Dec 2021 19:38:08 GMT  
		Size: 59.5 MB (59476470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927c076538b02993035990718d78a0b06fe3a6fc95b571ce334ae270c2cd4cc8`  
		Last Modified: Thu, 30 Dec 2021 19:37:58 GMT  
		Size: 5.0 KB (4956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1806011b64a9860267de7f898bd25bd33c0a6a69901dc7f8319e855bea3c1303`  
		Last Modified: Thu, 30 Dec 2021 19:37:58 GMT  
		Size: 2.9 KB (2942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6.51-2`

```console
$ docker pull percona@sha256:8c915f6fff3a43383938b4015ee3740dc1886fd5016a1404ff45b55de71e49cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5.6.51-2` - linux; amd64

```console
$ docker pull percona@sha256:a865615cf007e34fc520a72786a807909f8c75fd233388a0a0445fa82b5319cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.3 MB (195312192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56b1d76c933806bd31b1a5833d091c41c5bc6c9d0953c4a2c764668d37c6f79e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 18:58:17 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 15 Sep 2021 18:58:18 GMT
RUN groupdel input && groupadd -g 999 mysql
# Wed, 15 Sep 2021 18:58:19 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Dec 2021 19:25:24 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         curl -Lf -o /tmp/nss.rpm http://mirror.centos.org/centos/7/updates/x86_64/Packages/nss-3.67.0-4.el7_9.x86_64.rpm;     rpmkeys --checksig /tmp/nss.rpm;     yum install -y /tmp/nss.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Thu, 30 Dec 2021 19:25:25 GMT
ENV PERCONA_VERSION=5.6.51-rel91.0.1.el7
# Thu, 30 Dec 2021 19:36:53 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Thu, 30 Dec 2021 19:36:55 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Dec 2021 19:36:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Dec 2021 19:36:55 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Thu, 30 Dec 2021 19:36:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Dec 2021 19:36:56 GMT
USER mysql
# Thu, 30 Dec 2021 19:36:56 GMT
EXPOSE 3306
# Thu, 30 Dec 2021 19:36:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd68507e31292f16aa2d29907b401abd6ab53be7b485f2bdea2a7182e63d1af`  
		Last Modified: Wed, 15 Sep 2021 19:05:51 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ee280aea028899106d471852f72f47591667f5edf38214be74a6121932ea56`  
		Last Modified: Wed, 15 Sep 2021 19:05:49 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729721338aa7f33aa759726ffa7b1c50288e2dcae602d0323eecab0ff98c9c26`  
		Last Modified: Thu, 30 Dec 2021 19:38:06 GMT  
		Size: 59.7 MB (59728568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d8b9873953ce124f23ca0f1406a9518ca744b77cfbebdd6d9f79a785fa7a09`  
		Last Modified: Thu, 30 Dec 2021 19:38:08 GMT  
		Size: 59.5 MB (59476470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927c076538b02993035990718d78a0b06fe3a6fc95b571ce334ae270c2cd4cc8`  
		Last Modified: Thu, 30 Dec 2021 19:37:58 GMT  
		Size: 5.0 KB (4956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1806011b64a9860267de7f898bd25bd33c0a6a69901dc7f8319e855bea3c1303`  
		Last Modified: Thu, 30 Dec 2021 19:37:58 GMT  
		Size: 2.9 KB (2942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6.51-2-centos`

```console
$ docker pull percona@sha256:8c915f6fff3a43383938b4015ee3740dc1886fd5016a1404ff45b55de71e49cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5.6.51-2-centos` - linux; amd64

```console
$ docker pull percona@sha256:a865615cf007e34fc520a72786a807909f8c75fd233388a0a0445fa82b5319cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.3 MB (195312192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56b1d76c933806bd31b1a5833d091c41c5bc6c9d0953c4a2c764668d37c6f79e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 18:58:17 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 15 Sep 2021 18:58:18 GMT
RUN groupdel input && groupadd -g 999 mysql
# Wed, 15 Sep 2021 18:58:19 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Dec 2021 19:25:24 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         curl -Lf -o /tmp/nss.rpm http://mirror.centos.org/centos/7/updates/x86_64/Packages/nss-3.67.0-4.el7_9.x86_64.rpm;     rpmkeys --checksig /tmp/nss.rpm;     yum install -y /tmp/nss.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Thu, 30 Dec 2021 19:25:25 GMT
ENV PERCONA_VERSION=5.6.51-rel91.0.1.el7
# Thu, 30 Dec 2021 19:36:53 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Thu, 30 Dec 2021 19:36:55 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Dec 2021 19:36:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Dec 2021 19:36:55 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Thu, 30 Dec 2021 19:36:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Dec 2021 19:36:56 GMT
USER mysql
# Thu, 30 Dec 2021 19:36:56 GMT
EXPOSE 3306
# Thu, 30 Dec 2021 19:36:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd68507e31292f16aa2d29907b401abd6ab53be7b485f2bdea2a7182e63d1af`  
		Last Modified: Wed, 15 Sep 2021 19:05:51 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ee280aea028899106d471852f72f47591667f5edf38214be74a6121932ea56`  
		Last Modified: Wed, 15 Sep 2021 19:05:49 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729721338aa7f33aa759726ffa7b1c50288e2dcae602d0323eecab0ff98c9c26`  
		Last Modified: Thu, 30 Dec 2021 19:38:06 GMT  
		Size: 59.7 MB (59728568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d8b9873953ce124f23ca0f1406a9518ca744b77cfbebdd6d9f79a785fa7a09`  
		Last Modified: Thu, 30 Dec 2021 19:38:08 GMT  
		Size: 59.5 MB (59476470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927c076538b02993035990718d78a0b06fe3a6fc95b571ce334ae270c2cd4cc8`  
		Last Modified: Thu, 30 Dec 2021 19:37:58 GMT  
		Size: 5.0 KB (4956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1806011b64a9860267de7f898bd25bd33c0a6a69901dc7f8319e855bea3c1303`  
		Last Modified: Thu, 30 Dec 2021 19:37:58 GMT  
		Size: 2.9 KB (2942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7`

```console
$ docker pull percona@sha256:152551a63255c5e252858b5ca632082b275c048a086b1355c70925af64250f63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5.7` - linux; amd64

```console
$ docker pull percona@sha256:37dd6744679dc7ed62bd1f4929469530a06eaf7f15de88e8de10a01782eb784f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.8 MB (416792246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a7406e542f53a3e7a9855b461e71ebe566606461b004e7e4720502acdb26ac`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:54:56 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Wed, 19 Jul 2023 20:55:38 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Wed, 19 Jul 2023 20:55:39 GMT
ENV PS_VERSION=5.7.39-42.1
# Wed, 19 Jul 2023 20:55:39 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:55:39 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Wed, 19 Jul 2023 20:56:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Wed, 19 Jul 2023 20:56:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 19 Jul 2023 20:56:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 19 Jul 2023 20:56:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 19 Jul 2023 20:56:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:56:26 GMT
USER mysql
# Wed, 19 Jul 2023 20:56:26 GMT
EXPOSE 3306
# Wed, 19 Jul 2023 20:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461daf9f83a293e04611358beed29d44d873ea2c8e8ec5d7ff861c5880530150`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e369e7c761b19ce864cbdb8eee412673d760ff8011cea3da197a062340b1a1`  
		Last Modified: Wed, 19 Jul 2023 21:02:05 GMT  
		Size: 190.4 MB (190392071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b521a644912a1d8f52b9c4b16a66da3f8b381b9c5ebb2a6ed6dc01de15fe00`  
		Last Modified: Wed, 19 Jul 2023 21:02:12 GMT  
		Size: 137.5 MB (137526118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b84cf62dae1737678206fcf51e9eb2b62c3f15fe6a7b5807b8d64c62dc9224`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649ef554e0e53bb5da6b9b155236875e9e0670f1be9c6904f4d79fdbd82a6f98`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7-centos`

```console
$ docker pull percona@sha256:152551a63255c5e252858b5ca632082b275c048a086b1355c70925af64250f63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5.7-centos` - linux; amd64

```console
$ docker pull percona@sha256:37dd6744679dc7ed62bd1f4929469530a06eaf7f15de88e8de10a01782eb784f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.8 MB (416792246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a7406e542f53a3e7a9855b461e71ebe566606461b004e7e4720502acdb26ac`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:54:56 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Wed, 19 Jul 2023 20:55:38 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Wed, 19 Jul 2023 20:55:39 GMT
ENV PS_VERSION=5.7.39-42.1
# Wed, 19 Jul 2023 20:55:39 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:55:39 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Wed, 19 Jul 2023 20:56:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Wed, 19 Jul 2023 20:56:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 19 Jul 2023 20:56:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 19 Jul 2023 20:56:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 19 Jul 2023 20:56:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:56:26 GMT
USER mysql
# Wed, 19 Jul 2023 20:56:26 GMT
EXPOSE 3306
# Wed, 19 Jul 2023 20:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461daf9f83a293e04611358beed29d44d873ea2c8e8ec5d7ff861c5880530150`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e369e7c761b19ce864cbdb8eee412673d760ff8011cea3da197a062340b1a1`  
		Last Modified: Wed, 19 Jul 2023 21:02:05 GMT  
		Size: 190.4 MB (190392071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b521a644912a1d8f52b9c4b16a66da3f8b381b9c5ebb2a6ed6dc01de15fe00`  
		Last Modified: Wed, 19 Jul 2023 21:02:12 GMT  
		Size: 137.5 MB (137526118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b84cf62dae1737678206fcf51e9eb2b62c3f15fe6a7b5807b8d64c62dc9224`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649ef554e0e53bb5da6b9b155236875e9e0670f1be9c6904f4d79fdbd82a6f98`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.39`

```console
$ docker pull percona@sha256:152551a63255c5e252858b5ca632082b275c048a086b1355c70925af64250f63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5.7.39` - linux; amd64

```console
$ docker pull percona@sha256:37dd6744679dc7ed62bd1f4929469530a06eaf7f15de88e8de10a01782eb784f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.8 MB (416792246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a7406e542f53a3e7a9855b461e71ebe566606461b004e7e4720502acdb26ac`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:54:56 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Wed, 19 Jul 2023 20:55:38 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Wed, 19 Jul 2023 20:55:39 GMT
ENV PS_VERSION=5.7.39-42.1
# Wed, 19 Jul 2023 20:55:39 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:55:39 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Wed, 19 Jul 2023 20:56:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Wed, 19 Jul 2023 20:56:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 19 Jul 2023 20:56:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 19 Jul 2023 20:56:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 19 Jul 2023 20:56:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:56:26 GMT
USER mysql
# Wed, 19 Jul 2023 20:56:26 GMT
EXPOSE 3306
# Wed, 19 Jul 2023 20:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461daf9f83a293e04611358beed29d44d873ea2c8e8ec5d7ff861c5880530150`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e369e7c761b19ce864cbdb8eee412673d760ff8011cea3da197a062340b1a1`  
		Last Modified: Wed, 19 Jul 2023 21:02:05 GMT  
		Size: 190.4 MB (190392071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b521a644912a1d8f52b9c4b16a66da3f8b381b9c5ebb2a6ed6dc01de15fe00`  
		Last Modified: Wed, 19 Jul 2023 21:02:12 GMT  
		Size: 137.5 MB (137526118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b84cf62dae1737678206fcf51e9eb2b62c3f15fe6a7b5807b8d64c62dc9224`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649ef554e0e53bb5da6b9b155236875e9e0670f1be9c6904f4d79fdbd82a6f98`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.39-centos`

```console
$ docker pull percona@sha256:152551a63255c5e252858b5ca632082b275c048a086b1355c70925af64250f63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5.7.39-centos` - linux; amd64

```console
$ docker pull percona@sha256:37dd6744679dc7ed62bd1f4929469530a06eaf7f15de88e8de10a01782eb784f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.8 MB (416792246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a7406e542f53a3e7a9855b461e71ebe566606461b004e7e4720502acdb26ac`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:54:56 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Wed, 19 Jul 2023 20:55:38 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Wed, 19 Jul 2023 20:55:39 GMT
ENV PS_VERSION=5.7.39-42.1
# Wed, 19 Jul 2023 20:55:39 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:55:39 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Wed, 19 Jul 2023 20:56:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Wed, 19 Jul 2023 20:56:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 19 Jul 2023 20:56:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 19 Jul 2023 20:56:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 19 Jul 2023 20:56:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:56:26 GMT
USER mysql
# Wed, 19 Jul 2023 20:56:26 GMT
EXPOSE 3306
# Wed, 19 Jul 2023 20:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461daf9f83a293e04611358beed29d44d873ea2c8e8ec5d7ff861c5880530150`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e369e7c761b19ce864cbdb8eee412673d760ff8011cea3da197a062340b1a1`  
		Last Modified: Wed, 19 Jul 2023 21:02:05 GMT  
		Size: 190.4 MB (190392071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b521a644912a1d8f52b9c4b16a66da3f8b381b9c5ebb2a6ed6dc01de15fe00`  
		Last Modified: Wed, 19 Jul 2023 21:02:12 GMT  
		Size: 137.5 MB (137526118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b84cf62dae1737678206fcf51e9eb2b62c3f15fe6a7b5807b8d64c62dc9224`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649ef554e0e53bb5da6b9b155236875e9e0670f1be9c6904f4d79fdbd82a6f98`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8`

```console
$ docker pull percona@sha256:6f60b35e5f518e0dd46237895a4dba83b8e3e76328197299ea972600caf7d7ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8` - linux; amd64

```console
$ docker pull percona@sha256:8babb7b44f39864e7fc11374d93d3f852d2d1ec9a15a6a0f1cda14b020958419
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.3 MB (383335198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ce2b3c131386b54b83e7022b5128dece4a3f50b6fe41733f00a72a98aa69f1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Jun 2023 00:23:56 GMT
ADD file:a5dc577a850ef41488490ddc01c977760aaa7fc688e77923c15be6c9f12674af in / 
# Fri, 23 Jun 2023 00:23:56 GMT
CMD ["/bin/bash"]
# Fri, 23 Jun 2023 00:41:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 23 Jun 2023 00:41:13 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_VERSION=8.0.33-25.1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV OS_VER=el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_REPO=testing
# Fri, 23 Jun 2023 00:41:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Fri, 23 Jun 2023 00:42:07 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Fri, 23 Jun 2023 00:42:11 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Fri, 23 Jun 2023 00:42:12 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Fri, 23 Jun 2023 00:42:12 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Fri, 23 Jun 2023 00:42:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jun 2023 00:42:12 GMT
USER mysql
# Fri, 23 Jun 2023 00:42:12 GMT
EXPOSE 3306 33060
# Fri, 23 Jun 2023 00:42:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:fd5367e01a11dce2026f7954fed19fca5829ed8a5816767ce069cda19e8b880e`  
		Last Modified: Fri, 23 Jun 2023 00:25:15 GMT  
		Size: 88.0 MB (87962811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bce2f5c31c83f94f136286aa47a15096ef1fe91e17aa8a4565af115549f15f`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.6 KB (1636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57914938b6feea2ca15088c32824fe36d315d524ba6143be76f4d1a1338b74a2`  
		Last Modified: Fri, 23 Jun 2023 00:42:58 GMT  
		Size: 7.3 MB (7326811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d313ab89a3ab23608351b5f778095610efdbc000dc174d4881221ce2ba4309`  
		Last Modified: Fri, 23 Jun 2023 00:43:37 GMT  
		Size: 288.0 MB (288039685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59e5e66ea115bc515f1cbadaf38bc07a1bfac33017e96ad729ea3443492fb2c`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0115118d13b5c42a3029767175c1727983b42050a09862aa94a51298d945e62`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8-centos`

```console
$ docker pull percona@sha256:6f60b35e5f518e0dd46237895a4dba83b8e3e76328197299ea972600caf7d7ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8-centos` - linux; amd64

```console
$ docker pull percona@sha256:8babb7b44f39864e7fc11374d93d3f852d2d1ec9a15a6a0f1cda14b020958419
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.3 MB (383335198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ce2b3c131386b54b83e7022b5128dece4a3f50b6fe41733f00a72a98aa69f1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Jun 2023 00:23:56 GMT
ADD file:a5dc577a850ef41488490ddc01c977760aaa7fc688e77923c15be6c9f12674af in / 
# Fri, 23 Jun 2023 00:23:56 GMT
CMD ["/bin/bash"]
# Fri, 23 Jun 2023 00:41:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 23 Jun 2023 00:41:13 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_VERSION=8.0.33-25.1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV OS_VER=el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_REPO=testing
# Fri, 23 Jun 2023 00:41:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Fri, 23 Jun 2023 00:42:07 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Fri, 23 Jun 2023 00:42:11 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Fri, 23 Jun 2023 00:42:12 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Fri, 23 Jun 2023 00:42:12 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Fri, 23 Jun 2023 00:42:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jun 2023 00:42:12 GMT
USER mysql
# Fri, 23 Jun 2023 00:42:12 GMT
EXPOSE 3306 33060
# Fri, 23 Jun 2023 00:42:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:fd5367e01a11dce2026f7954fed19fca5829ed8a5816767ce069cda19e8b880e`  
		Last Modified: Fri, 23 Jun 2023 00:25:15 GMT  
		Size: 88.0 MB (87962811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bce2f5c31c83f94f136286aa47a15096ef1fe91e17aa8a4565af115549f15f`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.6 KB (1636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57914938b6feea2ca15088c32824fe36d315d524ba6143be76f4d1a1338b74a2`  
		Last Modified: Fri, 23 Jun 2023 00:42:58 GMT  
		Size: 7.3 MB (7326811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d313ab89a3ab23608351b5f778095610efdbc000dc174d4881221ce2ba4309`  
		Last Modified: Fri, 23 Jun 2023 00:43:37 GMT  
		Size: 288.0 MB (288039685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59e5e66ea115bc515f1cbadaf38bc07a1bfac33017e96ad729ea3443492fb2c`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0115118d13b5c42a3029767175c1727983b42050a09862aa94a51298d945e62`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0`

```console
$ docker pull percona@sha256:6f60b35e5f518e0dd46237895a4dba83b8e3e76328197299ea972600caf7d7ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8.0` - linux; amd64

```console
$ docker pull percona@sha256:8babb7b44f39864e7fc11374d93d3f852d2d1ec9a15a6a0f1cda14b020958419
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.3 MB (383335198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ce2b3c131386b54b83e7022b5128dece4a3f50b6fe41733f00a72a98aa69f1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Jun 2023 00:23:56 GMT
ADD file:a5dc577a850ef41488490ddc01c977760aaa7fc688e77923c15be6c9f12674af in / 
# Fri, 23 Jun 2023 00:23:56 GMT
CMD ["/bin/bash"]
# Fri, 23 Jun 2023 00:41:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 23 Jun 2023 00:41:13 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_VERSION=8.0.33-25.1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV OS_VER=el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_REPO=testing
# Fri, 23 Jun 2023 00:41:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Fri, 23 Jun 2023 00:42:07 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Fri, 23 Jun 2023 00:42:11 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Fri, 23 Jun 2023 00:42:12 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Fri, 23 Jun 2023 00:42:12 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Fri, 23 Jun 2023 00:42:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jun 2023 00:42:12 GMT
USER mysql
# Fri, 23 Jun 2023 00:42:12 GMT
EXPOSE 3306 33060
# Fri, 23 Jun 2023 00:42:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:fd5367e01a11dce2026f7954fed19fca5829ed8a5816767ce069cda19e8b880e`  
		Last Modified: Fri, 23 Jun 2023 00:25:15 GMT  
		Size: 88.0 MB (87962811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bce2f5c31c83f94f136286aa47a15096ef1fe91e17aa8a4565af115549f15f`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.6 KB (1636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57914938b6feea2ca15088c32824fe36d315d524ba6143be76f4d1a1338b74a2`  
		Last Modified: Fri, 23 Jun 2023 00:42:58 GMT  
		Size: 7.3 MB (7326811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d313ab89a3ab23608351b5f778095610efdbc000dc174d4881221ce2ba4309`  
		Last Modified: Fri, 23 Jun 2023 00:43:37 GMT  
		Size: 288.0 MB (288039685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59e5e66ea115bc515f1cbadaf38bc07a1bfac33017e96ad729ea3443492fb2c`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0115118d13b5c42a3029767175c1727983b42050a09862aa94a51298d945e62`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0-centos`

```console
$ docker pull percona@sha256:6f60b35e5f518e0dd46237895a4dba83b8e3e76328197299ea972600caf7d7ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8.0-centos` - linux; amd64

```console
$ docker pull percona@sha256:8babb7b44f39864e7fc11374d93d3f852d2d1ec9a15a6a0f1cda14b020958419
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.3 MB (383335198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ce2b3c131386b54b83e7022b5128dece4a3f50b6fe41733f00a72a98aa69f1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Jun 2023 00:23:56 GMT
ADD file:a5dc577a850ef41488490ddc01c977760aaa7fc688e77923c15be6c9f12674af in / 
# Fri, 23 Jun 2023 00:23:56 GMT
CMD ["/bin/bash"]
# Fri, 23 Jun 2023 00:41:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 23 Jun 2023 00:41:13 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_VERSION=8.0.33-25.1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV OS_VER=el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_REPO=testing
# Fri, 23 Jun 2023 00:41:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Fri, 23 Jun 2023 00:42:07 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Fri, 23 Jun 2023 00:42:11 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Fri, 23 Jun 2023 00:42:12 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Fri, 23 Jun 2023 00:42:12 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Fri, 23 Jun 2023 00:42:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jun 2023 00:42:12 GMT
USER mysql
# Fri, 23 Jun 2023 00:42:12 GMT
EXPOSE 3306 33060
# Fri, 23 Jun 2023 00:42:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:fd5367e01a11dce2026f7954fed19fca5829ed8a5816767ce069cda19e8b880e`  
		Last Modified: Fri, 23 Jun 2023 00:25:15 GMT  
		Size: 88.0 MB (87962811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bce2f5c31c83f94f136286aa47a15096ef1fe91e17aa8a4565af115549f15f`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.6 KB (1636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57914938b6feea2ca15088c32824fe36d315d524ba6143be76f4d1a1338b74a2`  
		Last Modified: Fri, 23 Jun 2023 00:42:58 GMT  
		Size: 7.3 MB (7326811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d313ab89a3ab23608351b5f778095610efdbc000dc174d4881221ce2ba4309`  
		Last Modified: Fri, 23 Jun 2023 00:43:37 GMT  
		Size: 288.0 MB (288039685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59e5e66ea115bc515f1cbadaf38bc07a1bfac33017e96ad729ea3443492fb2c`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0115118d13b5c42a3029767175c1727983b42050a09862aa94a51298d945e62`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.33-25`

```console
$ docker pull percona@sha256:6f60b35e5f518e0dd46237895a4dba83b8e3e76328197299ea972600caf7d7ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8.0.33-25` - linux; amd64

```console
$ docker pull percona@sha256:8babb7b44f39864e7fc11374d93d3f852d2d1ec9a15a6a0f1cda14b020958419
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.3 MB (383335198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ce2b3c131386b54b83e7022b5128dece4a3f50b6fe41733f00a72a98aa69f1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Jun 2023 00:23:56 GMT
ADD file:a5dc577a850ef41488490ddc01c977760aaa7fc688e77923c15be6c9f12674af in / 
# Fri, 23 Jun 2023 00:23:56 GMT
CMD ["/bin/bash"]
# Fri, 23 Jun 2023 00:41:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 23 Jun 2023 00:41:13 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_VERSION=8.0.33-25.1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV OS_VER=el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_REPO=testing
# Fri, 23 Jun 2023 00:41:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Fri, 23 Jun 2023 00:42:07 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Fri, 23 Jun 2023 00:42:11 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Fri, 23 Jun 2023 00:42:12 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Fri, 23 Jun 2023 00:42:12 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Fri, 23 Jun 2023 00:42:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jun 2023 00:42:12 GMT
USER mysql
# Fri, 23 Jun 2023 00:42:12 GMT
EXPOSE 3306 33060
# Fri, 23 Jun 2023 00:42:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:fd5367e01a11dce2026f7954fed19fca5829ed8a5816767ce069cda19e8b880e`  
		Last Modified: Fri, 23 Jun 2023 00:25:15 GMT  
		Size: 88.0 MB (87962811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bce2f5c31c83f94f136286aa47a15096ef1fe91e17aa8a4565af115549f15f`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.6 KB (1636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57914938b6feea2ca15088c32824fe36d315d524ba6143be76f4d1a1338b74a2`  
		Last Modified: Fri, 23 Jun 2023 00:42:58 GMT  
		Size: 7.3 MB (7326811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d313ab89a3ab23608351b5f778095610efdbc000dc174d4881221ce2ba4309`  
		Last Modified: Fri, 23 Jun 2023 00:43:37 GMT  
		Size: 288.0 MB (288039685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59e5e66ea115bc515f1cbadaf38bc07a1bfac33017e96ad729ea3443492fb2c`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0115118d13b5c42a3029767175c1727983b42050a09862aa94a51298d945e62`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.33-25-centos`

```console
$ docker pull percona@sha256:6f60b35e5f518e0dd46237895a4dba83b8e3e76328197299ea972600caf7d7ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8.0.33-25-centos` - linux; amd64

```console
$ docker pull percona@sha256:8babb7b44f39864e7fc11374d93d3f852d2d1ec9a15a6a0f1cda14b020958419
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.3 MB (383335198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ce2b3c131386b54b83e7022b5128dece4a3f50b6fe41733f00a72a98aa69f1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Jun 2023 00:23:56 GMT
ADD file:a5dc577a850ef41488490ddc01c977760aaa7fc688e77923c15be6c9f12674af in / 
# Fri, 23 Jun 2023 00:23:56 GMT
CMD ["/bin/bash"]
# Fri, 23 Jun 2023 00:41:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 23 Jun 2023 00:41:13 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_VERSION=8.0.33-25.1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV OS_VER=el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_REPO=testing
# Fri, 23 Jun 2023 00:41:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Fri, 23 Jun 2023 00:42:07 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Fri, 23 Jun 2023 00:42:11 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Fri, 23 Jun 2023 00:42:12 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Fri, 23 Jun 2023 00:42:12 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Fri, 23 Jun 2023 00:42:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jun 2023 00:42:12 GMT
USER mysql
# Fri, 23 Jun 2023 00:42:12 GMT
EXPOSE 3306 33060
# Fri, 23 Jun 2023 00:42:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:fd5367e01a11dce2026f7954fed19fca5829ed8a5816767ce069cda19e8b880e`  
		Last Modified: Fri, 23 Jun 2023 00:25:15 GMT  
		Size: 88.0 MB (87962811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bce2f5c31c83f94f136286aa47a15096ef1fe91e17aa8a4565af115549f15f`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.6 KB (1636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57914938b6feea2ca15088c32824fe36d315d524ba6143be76f4d1a1338b74a2`  
		Last Modified: Fri, 23 Jun 2023 00:42:58 GMT  
		Size: 7.3 MB (7326811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d313ab89a3ab23608351b5f778095610efdbc000dc174d4881221ce2ba4309`  
		Last Modified: Fri, 23 Jun 2023 00:43:37 GMT  
		Size: 288.0 MB (288039685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59e5e66ea115bc515f1cbadaf38bc07a1bfac33017e96ad729ea3443492fb2c`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0115118d13b5c42a3029767175c1727983b42050a09862aa94a51298d945e62`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:centos`

```console
$ docker pull percona@sha256:152551a63255c5e252858b5ca632082b275c048a086b1355c70925af64250f63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:centos` - linux; amd64

```console
$ docker pull percona@sha256:37dd6744679dc7ed62bd1f4929469530a06eaf7f15de88e8de10a01782eb784f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.8 MB (416792246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a7406e542f53a3e7a9855b461e71ebe566606461b004e7e4720502acdb26ac`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:54:56 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Wed, 19 Jul 2023 20:55:38 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Wed, 19 Jul 2023 20:55:39 GMT
ENV PS_VERSION=5.7.39-42.1
# Wed, 19 Jul 2023 20:55:39 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:55:39 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Wed, 19 Jul 2023 20:56:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Wed, 19 Jul 2023 20:56:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 19 Jul 2023 20:56:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 19 Jul 2023 20:56:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 19 Jul 2023 20:56:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:56:26 GMT
USER mysql
# Wed, 19 Jul 2023 20:56:26 GMT
EXPOSE 3306
# Wed, 19 Jul 2023 20:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461daf9f83a293e04611358beed29d44d873ea2c8e8ec5d7ff861c5880530150`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e369e7c761b19ce864cbdb8eee412673d760ff8011cea3da197a062340b1a1`  
		Last Modified: Wed, 19 Jul 2023 21:02:05 GMT  
		Size: 190.4 MB (190392071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b521a644912a1d8f52b9c4b16a66da3f8b381b9c5ebb2a6ed6dc01de15fe00`  
		Last Modified: Wed, 19 Jul 2023 21:02:12 GMT  
		Size: 137.5 MB (137526118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b84cf62dae1737678206fcf51e9eb2b62c3f15fe6a7b5807b8d64c62dc9224`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649ef554e0e53bb5da6b9b155236875e9e0670f1be9c6904f4d79fdbd82a6f98`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5`

```console
$ docker pull percona@sha256:152551a63255c5e252858b5ca632082b275c048a086b1355c70925af64250f63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-5` - linux; amd64

```console
$ docker pull percona@sha256:37dd6744679dc7ed62bd1f4929469530a06eaf7f15de88e8de10a01782eb784f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.8 MB (416792246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a7406e542f53a3e7a9855b461e71ebe566606461b004e7e4720502acdb26ac`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:54:56 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Wed, 19 Jul 2023 20:55:38 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Wed, 19 Jul 2023 20:55:39 GMT
ENV PS_VERSION=5.7.39-42.1
# Wed, 19 Jul 2023 20:55:39 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:55:39 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Wed, 19 Jul 2023 20:56:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Wed, 19 Jul 2023 20:56:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 19 Jul 2023 20:56:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 19 Jul 2023 20:56:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 19 Jul 2023 20:56:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:56:26 GMT
USER mysql
# Wed, 19 Jul 2023 20:56:26 GMT
EXPOSE 3306
# Wed, 19 Jul 2023 20:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461daf9f83a293e04611358beed29d44d873ea2c8e8ec5d7ff861c5880530150`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e369e7c761b19ce864cbdb8eee412673d760ff8011cea3da197a062340b1a1`  
		Last Modified: Wed, 19 Jul 2023 21:02:05 GMT  
		Size: 190.4 MB (190392071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b521a644912a1d8f52b9c4b16a66da3f8b381b9c5ebb2a6ed6dc01de15fe00`  
		Last Modified: Wed, 19 Jul 2023 21:02:12 GMT  
		Size: 137.5 MB (137526118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b84cf62dae1737678206fcf51e9eb2b62c3f15fe6a7b5807b8d64c62dc9224`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649ef554e0e53bb5da6b9b155236875e9e0670f1be9c6904f4d79fdbd82a6f98`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.6`

```console
$ docker pull percona@sha256:8c915f6fff3a43383938b4015ee3740dc1886fd5016a1404ff45b55de71e49cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-5.6` - linux; amd64

```console
$ docker pull percona@sha256:a865615cf007e34fc520a72786a807909f8c75fd233388a0a0445fa82b5319cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.3 MB (195312192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56b1d76c933806bd31b1a5833d091c41c5bc6c9d0953c4a2c764668d37c6f79e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 18:58:17 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 15 Sep 2021 18:58:18 GMT
RUN groupdel input && groupadd -g 999 mysql
# Wed, 15 Sep 2021 18:58:19 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Dec 2021 19:25:24 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         curl -Lf -o /tmp/nss.rpm http://mirror.centos.org/centos/7/updates/x86_64/Packages/nss-3.67.0-4.el7_9.x86_64.rpm;     rpmkeys --checksig /tmp/nss.rpm;     yum install -y /tmp/nss.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Thu, 30 Dec 2021 19:25:25 GMT
ENV PERCONA_VERSION=5.6.51-rel91.0.1.el7
# Thu, 30 Dec 2021 19:36:53 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Thu, 30 Dec 2021 19:36:55 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Dec 2021 19:36:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Dec 2021 19:36:55 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Thu, 30 Dec 2021 19:36:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Dec 2021 19:36:56 GMT
USER mysql
# Thu, 30 Dec 2021 19:36:56 GMT
EXPOSE 3306
# Thu, 30 Dec 2021 19:36:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd68507e31292f16aa2d29907b401abd6ab53be7b485f2bdea2a7182e63d1af`  
		Last Modified: Wed, 15 Sep 2021 19:05:51 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ee280aea028899106d471852f72f47591667f5edf38214be74a6121932ea56`  
		Last Modified: Wed, 15 Sep 2021 19:05:49 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729721338aa7f33aa759726ffa7b1c50288e2dcae602d0323eecab0ff98c9c26`  
		Last Modified: Thu, 30 Dec 2021 19:38:06 GMT  
		Size: 59.7 MB (59728568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d8b9873953ce124f23ca0f1406a9518ca744b77cfbebdd6d9f79a785fa7a09`  
		Last Modified: Thu, 30 Dec 2021 19:38:08 GMT  
		Size: 59.5 MB (59476470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927c076538b02993035990718d78a0b06fe3a6fc95b571ce334ae270c2cd4cc8`  
		Last Modified: Thu, 30 Dec 2021 19:37:58 GMT  
		Size: 5.0 KB (4956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1806011b64a9860267de7f898bd25bd33c0a6a69901dc7f8319e855bea3c1303`  
		Last Modified: Thu, 30 Dec 2021 19:37:58 GMT  
		Size: 2.9 KB (2942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.6.51-2`

```console
$ docker pull percona@sha256:8c915f6fff3a43383938b4015ee3740dc1886fd5016a1404ff45b55de71e49cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-5.6.51-2` - linux; amd64

```console
$ docker pull percona@sha256:a865615cf007e34fc520a72786a807909f8c75fd233388a0a0445fa82b5319cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.3 MB (195312192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56b1d76c933806bd31b1a5833d091c41c5bc6c9d0953c4a2c764668d37c6f79e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 18:58:17 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 15 Sep 2021 18:58:18 GMT
RUN groupdel input && groupadd -g 999 mysql
# Wed, 15 Sep 2021 18:58:19 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Dec 2021 19:25:24 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         curl -Lf -o /tmp/nss.rpm http://mirror.centos.org/centos/7/updates/x86_64/Packages/nss-3.67.0-4.el7_9.x86_64.rpm;     rpmkeys --checksig /tmp/nss.rpm;     yum install -y /tmp/nss.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Thu, 30 Dec 2021 19:25:25 GMT
ENV PERCONA_VERSION=5.6.51-rel91.0.1.el7
# Thu, 30 Dec 2021 19:36:53 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Thu, 30 Dec 2021 19:36:55 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Dec 2021 19:36:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Dec 2021 19:36:55 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Thu, 30 Dec 2021 19:36:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Dec 2021 19:36:56 GMT
USER mysql
# Thu, 30 Dec 2021 19:36:56 GMT
EXPOSE 3306
# Thu, 30 Dec 2021 19:36:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd68507e31292f16aa2d29907b401abd6ab53be7b485f2bdea2a7182e63d1af`  
		Last Modified: Wed, 15 Sep 2021 19:05:51 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ee280aea028899106d471852f72f47591667f5edf38214be74a6121932ea56`  
		Last Modified: Wed, 15 Sep 2021 19:05:49 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729721338aa7f33aa759726ffa7b1c50288e2dcae602d0323eecab0ff98c9c26`  
		Last Modified: Thu, 30 Dec 2021 19:38:06 GMT  
		Size: 59.7 MB (59728568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d8b9873953ce124f23ca0f1406a9518ca744b77cfbebdd6d9f79a785fa7a09`  
		Last Modified: Thu, 30 Dec 2021 19:38:08 GMT  
		Size: 59.5 MB (59476470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927c076538b02993035990718d78a0b06fe3a6fc95b571ce334ae270c2cd4cc8`  
		Last Modified: Thu, 30 Dec 2021 19:37:58 GMT  
		Size: 5.0 KB (4956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1806011b64a9860267de7f898bd25bd33c0a6a69901dc7f8319e855bea3c1303`  
		Last Modified: Thu, 30 Dec 2021 19:37:58 GMT  
		Size: 2.9 KB (2942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.7`

```console
$ docker pull percona@sha256:152551a63255c5e252858b5ca632082b275c048a086b1355c70925af64250f63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-5.7` - linux; amd64

```console
$ docker pull percona@sha256:37dd6744679dc7ed62bd1f4929469530a06eaf7f15de88e8de10a01782eb784f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.8 MB (416792246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a7406e542f53a3e7a9855b461e71ebe566606461b004e7e4720502acdb26ac`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:54:56 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Wed, 19 Jul 2023 20:55:38 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Wed, 19 Jul 2023 20:55:39 GMT
ENV PS_VERSION=5.7.39-42.1
# Wed, 19 Jul 2023 20:55:39 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:55:39 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Wed, 19 Jul 2023 20:56:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Wed, 19 Jul 2023 20:56:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 19 Jul 2023 20:56:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 19 Jul 2023 20:56:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 19 Jul 2023 20:56:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:56:26 GMT
USER mysql
# Wed, 19 Jul 2023 20:56:26 GMT
EXPOSE 3306
# Wed, 19 Jul 2023 20:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461daf9f83a293e04611358beed29d44d873ea2c8e8ec5d7ff861c5880530150`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e369e7c761b19ce864cbdb8eee412673d760ff8011cea3da197a062340b1a1`  
		Last Modified: Wed, 19 Jul 2023 21:02:05 GMT  
		Size: 190.4 MB (190392071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b521a644912a1d8f52b9c4b16a66da3f8b381b9c5ebb2a6ed6dc01de15fe00`  
		Last Modified: Wed, 19 Jul 2023 21:02:12 GMT  
		Size: 137.5 MB (137526118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b84cf62dae1737678206fcf51e9eb2b62c3f15fe6a7b5807b8d64c62dc9224`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649ef554e0e53bb5da6b9b155236875e9e0670f1be9c6904f4d79fdbd82a6f98`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.7.39`

```console
$ docker pull percona@sha256:152551a63255c5e252858b5ca632082b275c048a086b1355c70925af64250f63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-5.7.39` - linux; amd64

```console
$ docker pull percona@sha256:37dd6744679dc7ed62bd1f4929469530a06eaf7f15de88e8de10a01782eb784f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.8 MB (416792246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a7406e542f53a3e7a9855b461e71ebe566606461b004e7e4720502acdb26ac`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:54:56 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Wed, 19 Jul 2023 20:55:38 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Wed, 19 Jul 2023 20:55:39 GMT
ENV PS_VERSION=5.7.39-42.1
# Wed, 19 Jul 2023 20:55:39 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:55:39 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Wed, 19 Jul 2023 20:56:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Wed, 19 Jul 2023 20:56:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 19 Jul 2023 20:56:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 19 Jul 2023 20:56:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 19 Jul 2023 20:56:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 19 Jul 2023 20:56:26 GMT
USER mysql
# Wed, 19 Jul 2023 20:56:26 GMT
EXPOSE 3306
# Wed, 19 Jul 2023 20:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461daf9f83a293e04611358beed29d44d873ea2c8e8ec5d7ff861c5880530150`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e369e7c761b19ce864cbdb8eee412673d760ff8011cea3da197a062340b1a1`  
		Last Modified: Wed, 19 Jul 2023 21:02:05 GMT  
		Size: 190.4 MB (190392071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b521a644912a1d8f52b9c4b16a66da3f8b381b9c5ebb2a6ed6dc01de15fe00`  
		Last Modified: Wed, 19 Jul 2023 21:02:12 GMT  
		Size: 137.5 MB (137526118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b84cf62dae1737678206fcf51e9eb2b62c3f15fe6a7b5807b8d64c62dc9224`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649ef554e0e53bb5da6b9b155236875e9e0670f1be9c6904f4d79fdbd82a6f98`  
		Last Modified: Wed, 19 Jul 2023 21:01:54 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8`

```console
$ docker pull percona@sha256:6f60b35e5f518e0dd46237895a4dba83b8e3e76328197299ea972600caf7d7ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-8` - linux; amd64

```console
$ docker pull percona@sha256:8babb7b44f39864e7fc11374d93d3f852d2d1ec9a15a6a0f1cda14b020958419
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.3 MB (383335198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ce2b3c131386b54b83e7022b5128dece4a3f50b6fe41733f00a72a98aa69f1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Jun 2023 00:23:56 GMT
ADD file:a5dc577a850ef41488490ddc01c977760aaa7fc688e77923c15be6c9f12674af in / 
# Fri, 23 Jun 2023 00:23:56 GMT
CMD ["/bin/bash"]
# Fri, 23 Jun 2023 00:41:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 23 Jun 2023 00:41:13 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_VERSION=8.0.33-25.1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV OS_VER=el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_REPO=testing
# Fri, 23 Jun 2023 00:41:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Fri, 23 Jun 2023 00:42:07 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Fri, 23 Jun 2023 00:42:11 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Fri, 23 Jun 2023 00:42:12 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Fri, 23 Jun 2023 00:42:12 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Fri, 23 Jun 2023 00:42:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jun 2023 00:42:12 GMT
USER mysql
# Fri, 23 Jun 2023 00:42:12 GMT
EXPOSE 3306 33060
# Fri, 23 Jun 2023 00:42:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:fd5367e01a11dce2026f7954fed19fca5829ed8a5816767ce069cda19e8b880e`  
		Last Modified: Fri, 23 Jun 2023 00:25:15 GMT  
		Size: 88.0 MB (87962811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bce2f5c31c83f94f136286aa47a15096ef1fe91e17aa8a4565af115549f15f`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.6 KB (1636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57914938b6feea2ca15088c32824fe36d315d524ba6143be76f4d1a1338b74a2`  
		Last Modified: Fri, 23 Jun 2023 00:42:58 GMT  
		Size: 7.3 MB (7326811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d313ab89a3ab23608351b5f778095610efdbc000dc174d4881221ce2ba4309`  
		Last Modified: Fri, 23 Jun 2023 00:43:37 GMT  
		Size: 288.0 MB (288039685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59e5e66ea115bc515f1cbadaf38bc07a1bfac33017e96ad729ea3443492fb2c`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0115118d13b5c42a3029767175c1727983b42050a09862aa94a51298d945e62`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0`

```console
$ docker pull percona@sha256:6f60b35e5f518e0dd46237895a4dba83b8e3e76328197299ea972600caf7d7ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-8.0` - linux; amd64

```console
$ docker pull percona@sha256:8babb7b44f39864e7fc11374d93d3f852d2d1ec9a15a6a0f1cda14b020958419
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.3 MB (383335198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ce2b3c131386b54b83e7022b5128dece4a3f50b6fe41733f00a72a98aa69f1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Jun 2023 00:23:56 GMT
ADD file:a5dc577a850ef41488490ddc01c977760aaa7fc688e77923c15be6c9f12674af in / 
# Fri, 23 Jun 2023 00:23:56 GMT
CMD ["/bin/bash"]
# Fri, 23 Jun 2023 00:41:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 23 Jun 2023 00:41:13 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_VERSION=8.0.33-25.1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV OS_VER=el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_REPO=testing
# Fri, 23 Jun 2023 00:41:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Fri, 23 Jun 2023 00:42:07 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Fri, 23 Jun 2023 00:42:11 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Fri, 23 Jun 2023 00:42:12 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Fri, 23 Jun 2023 00:42:12 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Fri, 23 Jun 2023 00:42:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jun 2023 00:42:12 GMT
USER mysql
# Fri, 23 Jun 2023 00:42:12 GMT
EXPOSE 3306 33060
# Fri, 23 Jun 2023 00:42:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:fd5367e01a11dce2026f7954fed19fca5829ed8a5816767ce069cda19e8b880e`  
		Last Modified: Fri, 23 Jun 2023 00:25:15 GMT  
		Size: 88.0 MB (87962811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bce2f5c31c83f94f136286aa47a15096ef1fe91e17aa8a4565af115549f15f`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.6 KB (1636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57914938b6feea2ca15088c32824fe36d315d524ba6143be76f4d1a1338b74a2`  
		Last Modified: Fri, 23 Jun 2023 00:42:58 GMT  
		Size: 7.3 MB (7326811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d313ab89a3ab23608351b5f778095610efdbc000dc174d4881221ce2ba4309`  
		Last Modified: Fri, 23 Jun 2023 00:43:37 GMT  
		Size: 288.0 MB (288039685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59e5e66ea115bc515f1cbadaf38bc07a1bfac33017e96ad729ea3443492fb2c`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0115118d13b5c42a3029767175c1727983b42050a09862aa94a51298d945e62`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0.33-25`

```console
$ docker pull percona@sha256:6f60b35e5f518e0dd46237895a4dba83b8e3e76328197299ea972600caf7d7ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-8.0.33-25` - linux; amd64

```console
$ docker pull percona@sha256:8babb7b44f39864e7fc11374d93d3f852d2d1ec9a15a6a0f1cda14b020958419
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.3 MB (383335198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ce2b3c131386b54b83e7022b5128dece4a3f50b6fe41733f00a72a98aa69f1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Jun 2023 00:23:56 GMT
ADD file:a5dc577a850ef41488490ddc01c977760aaa7fc688e77923c15be6c9f12674af in / 
# Fri, 23 Jun 2023 00:23:56 GMT
CMD ["/bin/bash"]
# Fri, 23 Jun 2023 00:41:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 23 Jun 2023 00:41:13 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_VERSION=8.0.33-25.1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV OS_VER=el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_REPO=testing
# Fri, 23 Jun 2023 00:41:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Fri, 23 Jun 2023 00:42:07 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Fri, 23 Jun 2023 00:42:11 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Fri, 23 Jun 2023 00:42:12 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Fri, 23 Jun 2023 00:42:12 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Fri, 23 Jun 2023 00:42:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jun 2023 00:42:12 GMT
USER mysql
# Fri, 23 Jun 2023 00:42:12 GMT
EXPOSE 3306 33060
# Fri, 23 Jun 2023 00:42:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:fd5367e01a11dce2026f7954fed19fca5829ed8a5816767ce069cda19e8b880e`  
		Last Modified: Fri, 23 Jun 2023 00:25:15 GMT  
		Size: 88.0 MB (87962811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bce2f5c31c83f94f136286aa47a15096ef1fe91e17aa8a4565af115549f15f`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.6 KB (1636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57914938b6feea2ca15088c32824fe36d315d524ba6143be76f4d1a1338b74a2`  
		Last Modified: Fri, 23 Jun 2023 00:42:58 GMT  
		Size: 7.3 MB (7326811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d313ab89a3ab23608351b5f778095610efdbc000dc174d4881221ce2ba4309`  
		Last Modified: Fri, 23 Jun 2023 00:43:37 GMT  
		Size: 288.0 MB (288039685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59e5e66ea115bc515f1cbadaf38bc07a1bfac33017e96ad729ea3443492fb2c`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0115118d13b5c42a3029767175c1727983b42050a09862aa94a51298d945e62`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:417a33e5efa24d070b09fb98686b87855a4407996e444bd0969e41d9d648e14e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:9bf13f930154fb98ac8eb383ff4cb474b0c5e55e9f06d5bd61bd351e614e3ad9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.0 MB (218982875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96d6b644c893ebc4931a60b83039bd095a5e08478a77483afd5defe634249ae7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 21:00:21 GMT
ENV PSMDB_VERSION=4.2.24-24
# Wed, 19 Jul 2023 21:00:21 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 21:00:21 GMT
ENV FULL_PERCONA_VERSION=4.2.24-24.el8
# Wed, 19 Jul 2023 21:00:21 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 19 Jul 2023 21:00:21 GMT
ENV PSMDB_REPO=release
# Wed, 19 Jul 2023 21:00:24 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 19 Jul 2023 21:01:18 GMT
RUN set -ex;     percona-release enable psmdb-42 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 19 Jul 2023 21:01:19 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Wed, 19 Jul 2023 21:01:19 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 19 Jul 2023 21:01:19 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 19 Jul 2023 21:01:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 19 Jul 2023 21:01:22 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 19 Jul 2023 21:01:24 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -;     rm -f /tmp/SHA256SUMS;     chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 19 Jul 2023 21:01:24 GMT
VOLUME [/data/db]
# Wed, 19 Jul 2023 21:01:24 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Wed, 19 Jul 2023 21:01:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Jul 2023 21:01:25 GMT
EXPOSE 27017
# Wed, 19 Jul 2023 21:01:25 GMT
USER 1001
# Wed, 19 Jul 2023 21:01:25 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e9678bb5b7740544ef9b6e0adaf854ae190ff342cd33800e36552209b9afaf`  
		Last Modified: Wed, 19 Jul 2023 21:04:19 GMT  
		Size: 3.8 MB (3780726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e79f0731191b7de3b22ba64651251cbe013e731edaedacfbb1ffa162bca5164`  
		Last Modified: Wed, 19 Jul 2023 21:04:34 GMT  
		Size: 117.2 MB (117246830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cecf075293fa1b5edd9fa3857a3608f971d8dfeeaf99d24e6dd8bb43d1f1bbe`  
		Last Modified: Wed, 19 Jul 2023 21:04:19 GMT  
		Size: 1.7 KB (1674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dece26f0a5a06f593068ae57a27dac26d29cddfdbb432de7c7a4594979ede15`  
		Last Modified: Wed, 19 Jul 2023 21:04:17 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797db8c8348c835d01a7290c086fb7b29d5a0fddc16b7447b49456bf42e6c1a3`  
		Last Modified: Wed, 19 Jul 2023 21:04:17 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56511a35297055062106a03d16897e06ca36ce82e68384a91eebce60dc9445f9`  
		Last Modified: Wed, 19 Jul 2023 21:04:17 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1458c80147cf317e35fd4232c27d6ac19dfe40a39fa9037bcba5e014c8f21d`  
		Last Modified: Wed, 19 Jul 2023 21:04:18 GMT  
		Size: 8.2 MB (8151466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26833b6f777712a761f1b53a7a16fd211827b0d7330335b0fe583409906cf4e7`  
		Last Modified: Wed, 19 Jul 2023 21:04:17 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2.24`

```console
$ docker pull percona@sha256:417a33e5efa24d070b09fb98686b87855a4407996e444bd0969e41d9d648e14e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2.24` - linux; amd64

```console
$ docker pull percona@sha256:9bf13f930154fb98ac8eb383ff4cb474b0c5e55e9f06d5bd61bd351e614e3ad9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.0 MB (218982875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96d6b644c893ebc4931a60b83039bd095a5e08478a77483afd5defe634249ae7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 21:00:21 GMT
ENV PSMDB_VERSION=4.2.24-24
# Wed, 19 Jul 2023 21:00:21 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 21:00:21 GMT
ENV FULL_PERCONA_VERSION=4.2.24-24.el8
# Wed, 19 Jul 2023 21:00:21 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 19 Jul 2023 21:00:21 GMT
ENV PSMDB_REPO=release
# Wed, 19 Jul 2023 21:00:24 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 19 Jul 2023 21:01:18 GMT
RUN set -ex;     percona-release enable psmdb-42 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 19 Jul 2023 21:01:19 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Wed, 19 Jul 2023 21:01:19 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 19 Jul 2023 21:01:19 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 19 Jul 2023 21:01:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 19 Jul 2023 21:01:22 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 19 Jul 2023 21:01:24 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -;     rm -f /tmp/SHA256SUMS;     chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 19 Jul 2023 21:01:24 GMT
VOLUME [/data/db]
# Wed, 19 Jul 2023 21:01:24 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Wed, 19 Jul 2023 21:01:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Jul 2023 21:01:25 GMT
EXPOSE 27017
# Wed, 19 Jul 2023 21:01:25 GMT
USER 1001
# Wed, 19 Jul 2023 21:01:25 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e9678bb5b7740544ef9b6e0adaf854ae190ff342cd33800e36552209b9afaf`  
		Last Modified: Wed, 19 Jul 2023 21:04:19 GMT  
		Size: 3.8 MB (3780726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e79f0731191b7de3b22ba64651251cbe013e731edaedacfbb1ffa162bca5164`  
		Last Modified: Wed, 19 Jul 2023 21:04:34 GMT  
		Size: 117.2 MB (117246830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cecf075293fa1b5edd9fa3857a3608f971d8dfeeaf99d24e6dd8bb43d1f1bbe`  
		Last Modified: Wed, 19 Jul 2023 21:04:19 GMT  
		Size: 1.7 KB (1674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dece26f0a5a06f593068ae57a27dac26d29cddfdbb432de7c7a4594979ede15`  
		Last Modified: Wed, 19 Jul 2023 21:04:17 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797db8c8348c835d01a7290c086fb7b29d5a0fddc16b7447b49456bf42e6c1a3`  
		Last Modified: Wed, 19 Jul 2023 21:04:17 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56511a35297055062106a03d16897e06ca36ce82e68384a91eebce60dc9445f9`  
		Last Modified: Wed, 19 Jul 2023 21:04:17 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1458c80147cf317e35fd4232c27d6ac19dfe40a39fa9037bcba5e014c8f21d`  
		Last Modified: Wed, 19 Jul 2023 21:04:18 GMT  
		Size: 8.2 MB (8151466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26833b6f777712a761f1b53a7a16fd211827b0d7330335b0fe583409906cf4e7`  
		Last Modified: Wed, 19 Jul 2023 21:04:17 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.4`

```console
$ docker pull percona@sha256:f09d8b27b4f0692f79a8ee09e3e1cb0e369838f4dc36db9e8a58b9ef7f7eedd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4` - linux; amd64

```console
$ docker pull percona@sha256:ebcdbe61cab0d70e5da771d522a29f50d2dcc4b3290a52ca29d9df044ef127f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.5 MB (237524598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f05044b9788877ed284ee63ffb72151acccd2493a1dc4a3e22dd1f0ee1703c8b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:56:40 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 19 Jul 2023 20:59:11 GMT
ENV PSMDB_VERSION=4.4.22-21
# Wed, 19 Jul 2023 20:59:11 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:59:11 GMT
ENV FULL_PERCONA_VERSION=4.4.22-21.el8
# Wed, 19 Jul 2023 20:59:11 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 19 Jul 2023 20:59:11 GMT
ENV PSMDB_REPO=release
# Wed, 19 Jul 2023 21:00:06 GMT
RUN set -ex;     percona-release enable psmdb-44 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 19 Jul 2023 21:00:07 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Wed, 19 Jul 2023 21:00:07 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 19 Jul 2023 21:00:08 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 19 Jul 2023 21:00:08 GMT
ENV GOSU_VERSION=1.11
# Wed, 19 Jul 2023 21:00:11 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 19 Jul 2023 21:00:13 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 19 Jul 2023 21:00:13 GMT
VOLUME [/data/db]
# Wed, 19 Jul 2023 21:00:14 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 19 Jul 2023 21:00:14 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Wed, 19 Jul 2023 21:00:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Jul 2023 21:00:14 GMT
EXPOSE 27017
# Wed, 19 Jul 2023 21:00:14 GMT
USER 1001
# Wed, 19 Jul 2023 21:00:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfeeb16bf8999edb45d62d837e2ffada6ed220395b6a998d1464045211c00cb`  
		Last Modified: Wed, 19 Jul 2023 21:02:46 GMT  
		Size: 3.8 MB (3780725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc48270b12b6e8573229e85e54544765d38c5f1a5961123410a222fc68bf7246`  
		Last Modified: Wed, 19 Jul 2023 21:04:07 GMT  
		Size: 135.8 MB (135788927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522371c78b2da0c8d2d9da9e905d8a8e52a8f3dc35f8b743216d496062277025`  
		Last Modified: Wed, 19 Jul 2023 21:03:47 GMT  
		Size: 1.7 KB (1674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd5d48230675b0a33ac2c53354e00b5b6e441080cd6d6bfd7f90ffde89c391e`  
		Last Modified: Wed, 19 Jul 2023 21:03:47 GMT  
		Size: 4.1 KB (4102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0993c9297f19c4f1d108dc25cc516edf0bf734e0a2c82f89175b6d5239c2546a`  
		Last Modified: Wed, 19 Jul 2023 21:03:45 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558c1170e1df3360a090b3368c37cf155fbb0453a8cda4462ddefb273b7b46c8`  
		Last Modified: Wed, 19 Jul 2023 21:03:45 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730cf5236bbe8cab26bea91c358ec7d20b63ab39ffa77743875b2808d46b1284`  
		Last Modified: Wed, 19 Jul 2023 21:03:46 GMT  
		Size: 8.1 MB (8137888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688e3eec3c26f684042cce2cb26673808cee58dd28170b2aed5b513a4132764b`  
		Last Modified: Wed, 19 Jul 2023 21:03:45 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86519eb4bcbe8b48013addf85cee05112506ad5f03c6b17eb3bb61ab5e74b31a`  
		Last Modified: Wed, 19 Jul 2023 21:03:45 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.4.22`

```console
$ docker pull percona@sha256:f09d8b27b4f0692f79a8ee09e3e1cb0e369838f4dc36db9e8a58b9ef7f7eedd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4.22` - linux; amd64

```console
$ docker pull percona@sha256:ebcdbe61cab0d70e5da771d522a29f50d2dcc4b3290a52ca29d9df044ef127f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.5 MB (237524598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f05044b9788877ed284ee63ffb72151acccd2493a1dc4a3e22dd1f0ee1703c8b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:56:40 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 19 Jul 2023 20:59:11 GMT
ENV PSMDB_VERSION=4.4.22-21
# Wed, 19 Jul 2023 20:59:11 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:59:11 GMT
ENV FULL_PERCONA_VERSION=4.4.22-21.el8
# Wed, 19 Jul 2023 20:59:11 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 19 Jul 2023 20:59:11 GMT
ENV PSMDB_REPO=release
# Wed, 19 Jul 2023 21:00:06 GMT
RUN set -ex;     percona-release enable psmdb-44 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 19 Jul 2023 21:00:07 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Wed, 19 Jul 2023 21:00:07 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 19 Jul 2023 21:00:08 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 19 Jul 2023 21:00:08 GMT
ENV GOSU_VERSION=1.11
# Wed, 19 Jul 2023 21:00:11 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 19 Jul 2023 21:00:13 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 19 Jul 2023 21:00:13 GMT
VOLUME [/data/db]
# Wed, 19 Jul 2023 21:00:14 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 19 Jul 2023 21:00:14 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Wed, 19 Jul 2023 21:00:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Jul 2023 21:00:14 GMT
EXPOSE 27017
# Wed, 19 Jul 2023 21:00:14 GMT
USER 1001
# Wed, 19 Jul 2023 21:00:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfeeb16bf8999edb45d62d837e2ffada6ed220395b6a998d1464045211c00cb`  
		Last Modified: Wed, 19 Jul 2023 21:02:46 GMT  
		Size: 3.8 MB (3780725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc48270b12b6e8573229e85e54544765d38c5f1a5961123410a222fc68bf7246`  
		Last Modified: Wed, 19 Jul 2023 21:04:07 GMT  
		Size: 135.8 MB (135788927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522371c78b2da0c8d2d9da9e905d8a8e52a8f3dc35f8b743216d496062277025`  
		Last Modified: Wed, 19 Jul 2023 21:03:47 GMT  
		Size: 1.7 KB (1674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd5d48230675b0a33ac2c53354e00b5b6e441080cd6d6bfd7f90ffde89c391e`  
		Last Modified: Wed, 19 Jul 2023 21:03:47 GMT  
		Size: 4.1 KB (4102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0993c9297f19c4f1d108dc25cc516edf0bf734e0a2c82f89175b6d5239c2546a`  
		Last Modified: Wed, 19 Jul 2023 21:03:45 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558c1170e1df3360a090b3368c37cf155fbb0453a8cda4462ddefb273b7b46c8`  
		Last Modified: Wed, 19 Jul 2023 21:03:45 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730cf5236bbe8cab26bea91c358ec7d20b63ab39ffa77743875b2808d46b1284`  
		Last Modified: Wed, 19 Jul 2023 21:03:46 GMT  
		Size: 8.1 MB (8137888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688e3eec3c26f684042cce2cb26673808cee58dd28170b2aed5b513a4132764b`  
		Last Modified: Wed, 19 Jul 2023 21:03:45 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86519eb4bcbe8b48013addf85cee05112506ad5f03c6b17eb3bb61ab5e74b31a`  
		Last Modified: Wed, 19 Jul 2023 21:03:45 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-5.0`

```console
$ docker pull percona@sha256:fa0e444748db3ff83028a6078d2f54818d85f361a5aef109617e8c08a50b6ff9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0` - linux; amd64

```console
$ docker pull percona@sha256:ee7cfc8c66e10b8e254495fb9e40b77dc40fb4c19eb1ad3d757d45d3252bdd75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.1 MB (250128615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a009326b6d7a3604106da13a7acdcad6ad9f3868ab114f69f0ec14a4912b51d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:56:40 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 19 Jul 2023 20:58:00 GMT
ENV PSMDB_VERSION=5.0.18-15
# Wed, 19 Jul 2023 20:58:01 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:58:01 GMT
ENV FULL_PERCONA_VERSION=5.0.18-15.el8
# Wed, 19 Jul 2023 20:58:01 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 19 Jul 2023 20:58:01 GMT
ENV PSMDB_REPO=release
# Wed, 19 Jul 2023 20:58:58 GMT
RUN set -ex;     percona-release enable psmdb-50 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 19 Jul 2023 20:58:59 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Wed, 19 Jul 2023 20:58:59 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 19 Jul 2023 20:59:00 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 19 Jul 2023 20:59:00 GMT
ENV GOSU_VERSION=1.11
# Wed, 19 Jul 2023 20:59:02 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 19 Jul 2023 20:59:04 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 19 Jul 2023 20:59:04 GMT
VOLUME [/data/db]
# Wed, 19 Jul 2023 20:59:05 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 19 Jul 2023 20:59:05 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Wed, 19 Jul 2023 20:59:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Jul 2023 20:59:05 GMT
EXPOSE 27017
# Wed, 19 Jul 2023 20:59:05 GMT
USER 1001
# Wed, 19 Jul 2023 20:59:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfeeb16bf8999edb45d62d837e2ffada6ed220395b6a998d1464045211c00cb`  
		Last Modified: Wed, 19 Jul 2023 21:02:46 GMT  
		Size: 3.8 MB (3780725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd845c49278956bd8137f2926049705289fc0ba2b25639dfc112c3fdd304231`  
		Last Modified: Wed, 19 Jul 2023 21:03:35 GMT  
		Size: 148.4 MB (148392930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eb2cb98ee02615351d2ede77bb7cffc1cfe2779a381f21cef187970ff01a71`  
		Last Modified: Wed, 19 Jul 2023 21:03:17 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4e4b962090116d45303fb6a3edf79030232d8375eedb8a77d357ceada8aa76`  
		Last Modified: Wed, 19 Jul 2023 21:03:17 GMT  
		Size: 4.1 KB (4101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0517123faf5fd64ff4e8bc47010f80fa09d990e118118b55b52a548cba70b5`  
		Last Modified: Wed, 19 Jul 2023 21:03:15 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bd601960d99ba75cef20bdf8809a0097e9de16d750d9522cbe7e648fb87293`  
		Last Modified: Wed, 19 Jul 2023 21:03:15 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef31239a775565f1864e2fa49b7ec537ff0879551d553400d81afa083e845550`  
		Last Modified: Wed, 19 Jul 2023 21:03:16 GMT  
		Size: 8.1 MB (8137901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3261247ac06e0c8c922f3ec3b9c79418a4c89cdfcbcdd1d19adeb8f88261ae48`  
		Last Modified: Wed, 19 Jul 2023 21:03:15 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b291da9a8c39bec59391364ce1f29d7566f87d7d2ac6e683dd45b1d9337ce8c`  
		Last Modified: Wed, 19 Jul 2023 21:03:15 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-5.0.18`

```console
$ docker pull percona@sha256:fa0e444748db3ff83028a6078d2f54818d85f361a5aef109617e8c08a50b6ff9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0.18` - linux; amd64

```console
$ docker pull percona@sha256:ee7cfc8c66e10b8e254495fb9e40b77dc40fb4c19eb1ad3d757d45d3252bdd75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.1 MB (250128615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a009326b6d7a3604106da13a7acdcad6ad9f3868ab114f69f0ec14a4912b51d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:56:40 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 19 Jul 2023 20:58:00 GMT
ENV PSMDB_VERSION=5.0.18-15
# Wed, 19 Jul 2023 20:58:01 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:58:01 GMT
ENV FULL_PERCONA_VERSION=5.0.18-15.el8
# Wed, 19 Jul 2023 20:58:01 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 19 Jul 2023 20:58:01 GMT
ENV PSMDB_REPO=release
# Wed, 19 Jul 2023 20:58:58 GMT
RUN set -ex;     percona-release enable psmdb-50 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 19 Jul 2023 20:58:59 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Wed, 19 Jul 2023 20:58:59 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 19 Jul 2023 20:59:00 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 19 Jul 2023 20:59:00 GMT
ENV GOSU_VERSION=1.11
# Wed, 19 Jul 2023 20:59:02 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 19 Jul 2023 20:59:04 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 19 Jul 2023 20:59:04 GMT
VOLUME [/data/db]
# Wed, 19 Jul 2023 20:59:05 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 19 Jul 2023 20:59:05 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Wed, 19 Jul 2023 20:59:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Jul 2023 20:59:05 GMT
EXPOSE 27017
# Wed, 19 Jul 2023 20:59:05 GMT
USER 1001
# Wed, 19 Jul 2023 20:59:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfeeb16bf8999edb45d62d837e2ffada6ed220395b6a998d1464045211c00cb`  
		Last Modified: Wed, 19 Jul 2023 21:02:46 GMT  
		Size: 3.8 MB (3780725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd845c49278956bd8137f2926049705289fc0ba2b25639dfc112c3fdd304231`  
		Last Modified: Wed, 19 Jul 2023 21:03:35 GMT  
		Size: 148.4 MB (148392930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eb2cb98ee02615351d2ede77bb7cffc1cfe2779a381f21cef187970ff01a71`  
		Last Modified: Wed, 19 Jul 2023 21:03:17 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4e4b962090116d45303fb6a3edf79030232d8375eedb8a77d357ceada8aa76`  
		Last Modified: Wed, 19 Jul 2023 21:03:17 GMT  
		Size: 4.1 KB (4101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0517123faf5fd64ff4e8bc47010f80fa09d990e118118b55b52a548cba70b5`  
		Last Modified: Wed, 19 Jul 2023 21:03:15 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bd601960d99ba75cef20bdf8809a0097e9de16d750d9522cbe7e648fb87293`  
		Last Modified: Wed, 19 Jul 2023 21:03:15 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef31239a775565f1864e2fa49b7ec537ff0879551d553400d81afa083e845550`  
		Last Modified: Wed, 19 Jul 2023 21:03:16 GMT  
		Size: 8.1 MB (8137901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3261247ac06e0c8c922f3ec3b9c79418a4c89cdfcbcdd1d19adeb8f88261ae48`  
		Last Modified: Wed, 19 Jul 2023 21:03:15 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b291da9a8c39bec59391364ce1f29d7566f87d7d2ac6e683dd45b1d9337ce8c`  
		Last Modified: Wed, 19 Jul 2023 21:03:15 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-6.0`

```console
$ docker pull percona@sha256:5bb1c8564947411895126da1fcfadadc30364bc2b214afe88e8c41305f49821a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-6.0` - linux; amd64

```console
$ docker pull percona@sha256:7f91269828cc2ed58d8fe8210b5aa6a1645d4a240d9384aeb6a76fef21a2c439
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.2 MB (273186119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e37c582bb7788d9ecc2d37753578bd9af9aeebad57479b20892f7cf4b1b5834c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:56:40 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 19 Jul 2023 20:56:40 GMT
ENV PSMDB_VERSION=6.0.6-5
# Wed, 19 Jul 2023 20:56:40 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:56:40 GMT
ENV FULL_PERCONA_VERSION=6.0.6-5.el8
# Wed, 19 Jul 2023 20:56:40 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 19 Jul 2023 20:56:40 GMT
ENV PSMDB_REPO=release
# Wed, 19 Jul 2023 20:57:39 GMT
RUN set -ex;     percona-release enable psmdb-60 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         percona-mongodb-mongosh         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-60/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 19 Jul 2023 20:57:41 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Wed, 19 Jul 2023 20:57:41 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 19 Jul 2023 20:57:41 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 19 Jul 2023 20:57:41 GMT
ENV GOSU_VERSION=1.11
# Wed, 19 Jul 2023 20:57:45 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 19 Jul 2023 20:57:47 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 19 Jul 2023 20:57:48 GMT
VOLUME [/data/db]
# Wed, 19 Jul 2023 20:57:48 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 19 Jul 2023 20:57:49 GMT
COPY file:7ab35f422fd362616b84e1dc71329cc9be05b7f834182c48bf98ceb92ee28956 in /entrypoint.sh 
# Wed, 19 Jul 2023 20:57:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Jul 2023 20:57:49 GMT
EXPOSE 27017
# Wed, 19 Jul 2023 20:57:49 GMT
USER 1001
# Wed, 19 Jul 2023 20:57:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfeeb16bf8999edb45d62d837e2ffada6ed220395b6a998d1464045211c00cb`  
		Last Modified: Wed, 19 Jul 2023 21:02:46 GMT  
		Size: 3.8 MB (3780725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316344c17489e6f24318a372aeabb2d69181e56930416ad2cada081290cadd50`  
		Last Modified: Wed, 19 Jul 2023 21:03:06 GMT  
		Size: 171.5 MB (171450441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92094b053c0f1f80800052550f0e6f3f6988f148b2c80b4c51f2a8878f465623`  
		Last Modified: Wed, 19 Jul 2023 21:02:44 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41275153d1746fbbe646d3bf79dc294d80b55de662b194e0d43e999719748e22`  
		Last Modified: Wed, 19 Jul 2023 21:02:44 GMT  
		Size: 4.1 KB (4100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3795d4cc5379a200b3afdca151e3ddabb483e87f95b83c918f5d2a9f19897a60`  
		Last Modified: Wed, 19 Jul 2023 21:02:43 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3312a928ce66eda2f07167075f8088f2a8f3c02f18e57b250794f13765a557d6`  
		Last Modified: Wed, 19 Jul 2023 21:02:43 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a1b596804d4930da784910045c7117c486912da3f5e9d1887d7219c7393227`  
		Last Modified: Wed, 19 Jul 2023 21:02:44 GMT  
		Size: 8.1 MB (8137887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f651bbf31dce44f34e25d7fffe16390f36c2838563751c1c4607b38a56bb33ba`  
		Last Modified: Wed, 19 Jul 2023 21:02:42 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad0fd0917bc890a07ed660e7ae80ad226dae255264663ed603ef832d22a8776`  
		Last Modified: Wed, 19 Jul 2023 21:02:43 GMT  
		Size: 4.6 KB (4566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-6.0.6`

```console
$ docker pull percona@sha256:5bb1c8564947411895126da1fcfadadc30364bc2b214afe88e8c41305f49821a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-6.0.6` - linux; amd64

```console
$ docker pull percona@sha256:7f91269828cc2ed58d8fe8210b5aa6a1645d4a240d9384aeb6a76fef21a2c439
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.2 MB (273186119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e37c582bb7788d9ecc2d37753578bd9af9aeebad57479b20892f7cf4b1b5834c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:56:40 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 19 Jul 2023 20:56:40 GMT
ENV PSMDB_VERSION=6.0.6-5
# Wed, 19 Jul 2023 20:56:40 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:56:40 GMT
ENV FULL_PERCONA_VERSION=6.0.6-5.el8
# Wed, 19 Jul 2023 20:56:40 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 19 Jul 2023 20:56:40 GMT
ENV PSMDB_REPO=release
# Wed, 19 Jul 2023 20:57:39 GMT
RUN set -ex;     percona-release enable psmdb-60 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         percona-mongodb-mongosh         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-60/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 19 Jul 2023 20:57:41 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Wed, 19 Jul 2023 20:57:41 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 19 Jul 2023 20:57:41 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 19 Jul 2023 20:57:41 GMT
ENV GOSU_VERSION=1.11
# Wed, 19 Jul 2023 20:57:45 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 19 Jul 2023 20:57:47 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 19 Jul 2023 20:57:48 GMT
VOLUME [/data/db]
# Wed, 19 Jul 2023 20:57:48 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 19 Jul 2023 20:57:49 GMT
COPY file:7ab35f422fd362616b84e1dc71329cc9be05b7f834182c48bf98ceb92ee28956 in /entrypoint.sh 
# Wed, 19 Jul 2023 20:57:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Jul 2023 20:57:49 GMT
EXPOSE 27017
# Wed, 19 Jul 2023 20:57:49 GMT
USER 1001
# Wed, 19 Jul 2023 20:57:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfeeb16bf8999edb45d62d837e2ffada6ed220395b6a998d1464045211c00cb`  
		Last Modified: Wed, 19 Jul 2023 21:02:46 GMT  
		Size: 3.8 MB (3780725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316344c17489e6f24318a372aeabb2d69181e56930416ad2cada081290cadd50`  
		Last Modified: Wed, 19 Jul 2023 21:03:06 GMT  
		Size: 171.5 MB (171450441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92094b053c0f1f80800052550f0e6f3f6988f148b2c80b4c51f2a8878f465623`  
		Last Modified: Wed, 19 Jul 2023 21:02:44 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41275153d1746fbbe646d3bf79dc294d80b55de662b194e0d43e999719748e22`  
		Last Modified: Wed, 19 Jul 2023 21:02:44 GMT  
		Size: 4.1 KB (4100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3795d4cc5379a200b3afdca151e3ddabb483e87f95b83c918f5d2a9f19897a60`  
		Last Modified: Wed, 19 Jul 2023 21:02:43 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3312a928ce66eda2f07167075f8088f2a8f3c02f18e57b250794f13765a557d6`  
		Last Modified: Wed, 19 Jul 2023 21:02:43 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a1b596804d4930da784910045c7117c486912da3f5e9d1887d7219c7393227`  
		Last Modified: Wed, 19 Jul 2023 21:02:44 GMT  
		Size: 8.1 MB (8137887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f651bbf31dce44f34e25d7fffe16390f36c2838563751c1c4607b38a56bb33ba`  
		Last Modified: Wed, 19 Jul 2023 21:02:42 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad0fd0917bc890a07ed660e7ae80ad226dae255264663ed603ef832d22a8776`  
		Last Modified: Wed, 19 Jul 2023 21:02:43 GMT  
		Size: 4.6 KB (4566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
