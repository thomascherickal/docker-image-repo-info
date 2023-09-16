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
$ docker pull percona@sha256:c6cec5f9c14edc620a6b12fbba50a3a8dffa21fc7724c37503044432c904b482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5` - linux; amd64

```console
$ docker pull percona@sha256:a73b5048c98576f126077b4ac202a16caf66abebe08b330615e46eac6f3990e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422738287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef9ed4d199cd1798ea6627a94cc29fc7580824bf0cf5e39f9132dcee8b5dc50`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:19:29 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:20:04 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 16 Sep 2023 03:20:05 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 16 Sep 2023 03:20:05 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:20:05 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 16 Sep 2023 03:20:44 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:20:45 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 16 Sep 2023 03:20:45 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:20:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:20:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:20:46 GMT
USER mysql
# Sat, 16 Sep 2023 03:20:46 GMT
EXPOSE 3306
# Sat, 16 Sep 2023 03:20:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f444e97db0bf5d50f5015a158a00bd5e453060943342f50cd305119e04ecc3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f512ea8d3aec4fe796c01a42c138a1865db0af5bbb181535f7b815db30908aa8`  
		Last Modified: Sat, 16 Sep 2023 03:27:23 GMT  
		Size: 196.3 MB (196271669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5017199f5cf25acfe2e4bf52f8ad3b297c2299ab04b85ddd2f2390bb12d13bb3`  
		Last Modified: Sat, 16 Sep 2023 03:27:21 GMT  
		Size: 137.5 MB (137541712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b594fad71442b6e1ab26f111cacaec4f79a1b00589d5a9e795a0b797e8b36a82`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b7a9503470801e82fdbfdd3b7346e4301ac0e879acd895b1281b7e039ffa3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 3.1 KB (3062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5-centos`

```console
$ docker pull percona@sha256:c6cec5f9c14edc620a6b12fbba50a3a8dffa21fc7724c37503044432c904b482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5-centos` - linux; amd64

```console
$ docker pull percona@sha256:a73b5048c98576f126077b4ac202a16caf66abebe08b330615e46eac6f3990e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422738287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef9ed4d199cd1798ea6627a94cc29fc7580824bf0cf5e39f9132dcee8b5dc50`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:19:29 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:20:04 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 16 Sep 2023 03:20:05 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 16 Sep 2023 03:20:05 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:20:05 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 16 Sep 2023 03:20:44 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:20:45 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 16 Sep 2023 03:20:45 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:20:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:20:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:20:46 GMT
USER mysql
# Sat, 16 Sep 2023 03:20:46 GMT
EXPOSE 3306
# Sat, 16 Sep 2023 03:20:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f444e97db0bf5d50f5015a158a00bd5e453060943342f50cd305119e04ecc3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f512ea8d3aec4fe796c01a42c138a1865db0af5bbb181535f7b815db30908aa8`  
		Last Modified: Sat, 16 Sep 2023 03:27:23 GMT  
		Size: 196.3 MB (196271669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5017199f5cf25acfe2e4bf52f8ad3b297c2299ab04b85ddd2f2390bb12d13bb3`  
		Last Modified: Sat, 16 Sep 2023 03:27:21 GMT  
		Size: 137.5 MB (137541712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b594fad71442b6e1ab26f111cacaec4f79a1b00589d5a9e795a0b797e8b36a82`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b7a9503470801e82fdbfdd3b7346e4301ac0e879acd895b1281b7e039ffa3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 3.1 KB (3062 bytes)  
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
$ docker pull percona@sha256:c6cec5f9c14edc620a6b12fbba50a3a8dffa21fc7724c37503044432c904b482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5.7` - linux; amd64

```console
$ docker pull percona@sha256:a73b5048c98576f126077b4ac202a16caf66abebe08b330615e46eac6f3990e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422738287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef9ed4d199cd1798ea6627a94cc29fc7580824bf0cf5e39f9132dcee8b5dc50`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:19:29 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:20:04 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 16 Sep 2023 03:20:05 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 16 Sep 2023 03:20:05 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:20:05 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 16 Sep 2023 03:20:44 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:20:45 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 16 Sep 2023 03:20:45 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:20:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:20:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:20:46 GMT
USER mysql
# Sat, 16 Sep 2023 03:20:46 GMT
EXPOSE 3306
# Sat, 16 Sep 2023 03:20:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f444e97db0bf5d50f5015a158a00bd5e453060943342f50cd305119e04ecc3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f512ea8d3aec4fe796c01a42c138a1865db0af5bbb181535f7b815db30908aa8`  
		Last Modified: Sat, 16 Sep 2023 03:27:23 GMT  
		Size: 196.3 MB (196271669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5017199f5cf25acfe2e4bf52f8ad3b297c2299ab04b85ddd2f2390bb12d13bb3`  
		Last Modified: Sat, 16 Sep 2023 03:27:21 GMT  
		Size: 137.5 MB (137541712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b594fad71442b6e1ab26f111cacaec4f79a1b00589d5a9e795a0b797e8b36a82`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b7a9503470801e82fdbfdd3b7346e4301ac0e879acd895b1281b7e039ffa3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 3.1 KB (3062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7-centos`

```console
$ docker pull percona@sha256:c6cec5f9c14edc620a6b12fbba50a3a8dffa21fc7724c37503044432c904b482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5.7-centos` - linux; amd64

```console
$ docker pull percona@sha256:a73b5048c98576f126077b4ac202a16caf66abebe08b330615e46eac6f3990e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422738287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef9ed4d199cd1798ea6627a94cc29fc7580824bf0cf5e39f9132dcee8b5dc50`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:19:29 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:20:04 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 16 Sep 2023 03:20:05 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 16 Sep 2023 03:20:05 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:20:05 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 16 Sep 2023 03:20:44 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:20:45 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 16 Sep 2023 03:20:45 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:20:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:20:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:20:46 GMT
USER mysql
# Sat, 16 Sep 2023 03:20:46 GMT
EXPOSE 3306
# Sat, 16 Sep 2023 03:20:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f444e97db0bf5d50f5015a158a00bd5e453060943342f50cd305119e04ecc3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f512ea8d3aec4fe796c01a42c138a1865db0af5bbb181535f7b815db30908aa8`  
		Last Modified: Sat, 16 Sep 2023 03:27:23 GMT  
		Size: 196.3 MB (196271669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5017199f5cf25acfe2e4bf52f8ad3b297c2299ab04b85ddd2f2390bb12d13bb3`  
		Last Modified: Sat, 16 Sep 2023 03:27:21 GMT  
		Size: 137.5 MB (137541712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b594fad71442b6e1ab26f111cacaec4f79a1b00589d5a9e795a0b797e8b36a82`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b7a9503470801e82fdbfdd3b7346e4301ac0e879acd895b1281b7e039ffa3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 3.1 KB (3062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.39`

```console
$ docker pull percona@sha256:c6cec5f9c14edc620a6b12fbba50a3a8dffa21fc7724c37503044432c904b482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5.7.39` - linux; amd64

```console
$ docker pull percona@sha256:a73b5048c98576f126077b4ac202a16caf66abebe08b330615e46eac6f3990e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422738287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef9ed4d199cd1798ea6627a94cc29fc7580824bf0cf5e39f9132dcee8b5dc50`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:19:29 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:20:04 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 16 Sep 2023 03:20:05 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 16 Sep 2023 03:20:05 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:20:05 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 16 Sep 2023 03:20:44 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:20:45 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 16 Sep 2023 03:20:45 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:20:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:20:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:20:46 GMT
USER mysql
# Sat, 16 Sep 2023 03:20:46 GMT
EXPOSE 3306
# Sat, 16 Sep 2023 03:20:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f444e97db0bf5d50f5015a158a00bd5e453060943342f50cd305119e04ecc3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f512ea8d3aec4fe796c01a42c138a1865db0af5bbb181535f7b815db30908aa8`  
		Last Modified: Sat, 16 Sep 2023 03:27:23 GMT  
		Size: 196.3 MB (196271669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5017199f5cf25acfe2e4bf52f8ad3b297c2299ab04b85ddd2f2390bb12d13bb3`  
		Last Modified: Sat, 16 Sep 2023 03:27:21 GMT  
		Size: 137.5 MB (137541712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b594fad71442b6e1ab26f111cacaec4f79a1b00589d5a9e795a0b797e8b36a82`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b7a9503470801e82fdbfdd3b7346e4301ac0e879acd895b1281b7e039ffa3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 3.1 KB (3062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.39-centos`

```console
$ docker pull percona@sha256:c6cec5f9c14edc620a6b12fbba50a3a8dffa21fc7724c37503044432c904b482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5.7.39-centos` - linux; amd64

```console
$ docker pull percona@sha256:a73b5048c98576f126077b4ac202a16caf66abebe08b330615e46eac6f3990e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422738287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef9ed4d199cd1798ea6627a94cc29fc7580824bf0cf5e39f9132dcee8b5dc50`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:19:29 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:20:04 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 16 Sep 2023 03:20:05 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 16 Sep 2023 03:20:05 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:20:05 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 16 Sep 2023 03:20:44 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:20:45 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 16 Sep 2023 03:20:45 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:20:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:20:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:20:46 GMT
USER mysql
# Sat, 16 Sep 2023 03:20:46 GMT
EXPOSE 3306
# Sat, 16 Sep 2023 03:20:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f444e97db0bf5d50f5015a158a00bd5e453060943342f50cd305119e04ecc3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f512ea8d3aec4fe796c01a42c138a1865db0af5bbb181535f7b815db30908aa8`  
		Last Modified: Sat, 16 Sep 2023 03:27:23 GMT  
		Size: 196.3 MB (196271669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5017199f5cf25acfe2e4bf52f8ad3b297c2299ab04b85ddd2f2390bb12d13bb3`  
		Last Modified: Sat, 16 Sep 2023 03:27:21 GMT  
		Size: 137.5 MB (137541712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b594fad71442b6e1ab26f111cacaec4f79a1b00589d5a9e795a0b797e8b36a82`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b7a9503470801e82fdbfdd3b7346e4301ac0e879acd895b1281b7e039ffa3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 3.1 KB (3062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8`

```console
$ docker pull percona@sha256:2e01ea8231b2e6e7f2de456733657146256f10ccfae35c28aea66d913d1ca248
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8` - linux; amd64

```console
$ docker pull percona@sha256:ae8292248648fdc91e23a763165c0ecb1023021258026a2b17fb07e6f50ba1ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.3 MB (386307418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d149e90e32fe93d48e2a5e000737efab116a1daf5b6accf690855df59c960f1d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:18 GMT
ADD file:ca759c2861c7b47f87efcda8b2d88a6e2a3e34fa5a4e6bcebab50b985aaf2868 in / 
# Sat, 16 Sep 2023 02:40:19 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:18:18 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:18:19 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV OS_VER=el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_REPO=testing
# Sat, 16 Sep 2023 03:18:22 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 16 Sep 2023 03:19:19 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:19:23 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 16 Sep 2023 03:19:23 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:19:23 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:19:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:19:24 GMT
USER mysql
# Sat, 16 Sep 2023 03:19:24 GMT
EXPOSE 3306 33060
# Sat, 16 Sep 2023 03:19:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3eb6a50586d1e36befa4b41c2f504fdca518e4dbab482447202e95f02d9a6d78`  
		Last Modified: Sat, 16 Sep 2023 02:41:45 GMT  
		Size: 88.0 MB (87981331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b862f5c29fc2f5d3ec755acbd06e50014dd1b43f1f19e7d4308bf3dc6400213`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e79402c6d72a78cdee928786910d1d7733f70b63e909191e90340bfff252b4`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 7.3 MB (7318755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c329149170975f92c22d07c1e4729f89b6e995b852f8f9b922c80fd35cea11e1`  
		Last Modified: Sat, 16 Sep 2023 03:26:36 GMT  
		Size: 291.0 MB (291001444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d7cb6108d9d66e59db734407518df57d9df29ff29b5a52140aed2a9d0189d2`  
		Last Modified: Sat, 16 Sep 2023 03:25:55 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1ebb922232888f9a3c70f046afb603ae93ca8de117240f198813f43c671af`  
		Last Modified: Sat, 16 Sep 2023 03:25:54 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8-centos`

```console
$ docker pull percona@sha256:2e01ea8231b2e6e7f2de456733657146256f10ccfae35c28aea66d913d1ca248
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8-centos` - linux; amd64

```console
$ docker pull percona@sha256:ae8292248648fdc91e23a763165c0ecb1023021258026a2b17fb07e6f50ba1ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.3 MB (386307418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d149e90e32fe93d48e2a5e000737efab116a1daf5b6accf690855df59c960f1d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:18 GMT
ADD file:ca759c2861c7b47f87efcda8b2d88a6e2a3e34fa5a4e6bcebab50b985aaf2868 in / 
# Sat, 16 Sep 2023 02:40:19 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:18:18 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:18:19 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV OS_VER=el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_REPO=testing
# Sat, 16 Sep 2023 03:18:22 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 16 Sep 2023 03:19:19 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:19:23 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 16 Sep 2023 03:19:23 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:19:23 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:19:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:19:24 GMT
USER mysql
# Sat, 16 Sep 2023 03:19:24 GMT
EXPOSE 3306 33060
# Sat, 16 Sep 2023 03:19:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3eb6a50586d1e36befa4b41c2f504fdca518e4dbab482447202e95f02d9a6d78`  
		Last Modified: Sat, 16 Sep 2023 02:41:45 GMT  
		Size: 88.0 MB (87981331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b862f5c29fc2f5d3ec755acbd06e50014dd1b43f1f19e7d4308bf3dc6400213`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e79402c6d72a78cdee928786910d1d7733f70b63e909191e90340bfff252b4`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 7.3 MB (7318755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c329149170975f92c22d07c1e4729f89b6e995b852f8f9b922c80fd35cea11e1`  
		Last Modified: Sat, 16 Sep 2023 03:26:36 GMT  
		Size: 291.0 MB (291001444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d7cb6108d9d66e59db734407518df57d9df29ff29b5a52140aed2a9d0189d2`  
		Last Modified: Sat, 16 Sep 2023 03:25:55 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1ebb922232888f9a3c70f046afb603ae93ca8de117240f198813f43c671af`  
		Last Modified: Sat, 16 Sep 2023 03:25:54 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0`

```console
$ docker pull percona@sha256:2e01ea8231b2e6e7f2de456733657146256f10ccfae35c28aea66d913d1ca248
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8.0` - linux; amd64

```console
$ docker pull percona@sha256:ae8292248648fdc91e23a763165c0ecb1023021258026a2b17fb07e6f50ba1ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.3 MB (386307418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d149e90e32fe93d48e2a5e000737efab116a1daf5b6accf690855df59c960f1d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:18 GMT
ADD file:ca759c2861c7b47f87efcda8b2d88a6e2a3e34fa5a4e6bcebab50b985aaf2868 in / 
# Sat, 16 Sep 2023 02:40:19 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:18:18 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:18:19 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV OS_VER=el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_REPO=testing
# Sat, 16 Sep 2023 03:18:22 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 16 Sep 2023 03:19:19 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:19:23 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 16 Sep 2023 03:19:23 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:19:23 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:19:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:19:24 GMT
USER mysql
# Sat, 16 Sep 2023 03:19:24 GMT
EXPOSE 3306 33060
# Sat, 16 Sep 2023 03:19:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3eb6a50586d1e36befa4b41c2f504fdca518e4dbab482447202e95f02d9a6d78`  
		Last Modified: Sat, 16 Sep 2023 02:41:45 GMT  
		Size: 88.0 MB (87981331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b862f5c29fc2f5d3ec755acbd06e50014dd1b43f1f19e7d4308bf3dc6400213`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e79402c6d72a78cdee928786910d1d7733f70b63e909191e90340bfff252b4`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 7.3 MB (7318755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c329149170975f92c22d07c1e4729f89b6e995b852f8f9b922c80fd35cea11e1`  
		Last Modified: Sat, 16 Sep 2023 03:26:36 GMT  
		Size: 291.0 MB (291001444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d7cb6108d9d66e59db734407518df57d9df29ff29b5a52140aed2a9d0189d2`  
		Last Modified: Sat, 16 Sep 2023 03:25:55 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1ebb922232888f9a3c70f046afb603ae93ca8de117240f198813f43c671af`  
		Last Modified: Sat, 16 Sep 2023 03:25:54 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0-centos`

```console
$ docker pull percona@sha256:2e01ea8231b2e6e7f2de456733657146256f10ccfae35c28aea66d913d1ca248
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8.0-centos` - linux; amd64

```console
$ docker pull percona@sha256:ae8292248648fdc91e23a763165c0ecb1023021258026a2b17fb07e6f50ba1ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.3 MB (386307418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d149e90e32fe93d48e2a5e000737efab116a1daf5b6accf690855df59c960f1d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:18 GMT
ADD file:ca759c2861c7b47f87efcda8b2d88a6e2a3e34fa5a4e6bcebab50b985aaf2868 in / 
# Sat, 16 Sep 2023 02:40:19 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:18:18 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:18:19 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV OS_VER=el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_REPO=testing
# Sat, 16 Sep 2023 03:18:22 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 16 Sep 2023 03:19:19 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:19:23 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 16 Sep 2023 03:19:23 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:19:23 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:19:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:19:24 GMT
USER mysql
# Sat, 16 Sep 2023 03:19:24 GMT
EXPOSE 3306 33060
# Sat, 16 Sep 2023 03:19:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3eb6a50586d1e36befa4b41c2f504fdca518e4dbab482447202e95f02d9a6d78`  
		Last Modified: Sat, 16 Sep 2023 02:41:45 GMT  
		Size: 88.0 MB (87981331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b862f5c29fc2f5d3ec755acbd06e50014dd1b43f1f19e7d4308bf3dc6400213`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e79402c6d72a78cdee928786910d1d7733f70b63e909191e90340bfff252b4`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 7.3 MB (7318755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c329149170975f92c22d07c1e4729f89b6e995b852f8f9b922c80fd35cea11e1`  
		Last Modified: Sat, 16 Sep 2023 03:26:36 GMT  
		Size: 291.0 MB (291001444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d7cb6108d9d66e59db734407518df57d9df29ff29b5a52140aed2a9d0189d2`  
		Last Modified: Sat, 16 Sep 2023 03:25:55 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1ebb922232888f9a3c70f046afb603ae93ca8de117240f198813f43c671af`  
		Last Modified: Sat, 16 Sep 2023 03:25:54 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.33-25`

```console
$ docker pull percona@sha256:2e01ea8231b2e6e7f2de456733657146256f10ccfae35c28aea66d913d1ca248
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8.0.33-25` - linux; amd64

```console
$ docker pull percona@sha256:ae8292248648fdc91e23a763165c0ecb1023021258026a2b17fb07e6f50ba1ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.3 MB (386307418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d149e90e32fe93d48e2a5e000737efab116a1daf5b6accf690855df59c960f1d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:18 GMT
ADD file:ca759c2861c7b47f87efcda8b2d88a6e2a3e34fa5a4e6bcebab50b985aaf2868 in / 
# Sat, 16 Sep 2023 02:40:19 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:18:18 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:18:19 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV OS_VER=el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_REPO=testing
# Sat, 16 Sep 2023 03:18:22 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 16 Sep 2023 03:19:19 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:19:23 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 16 Sep 2023 03:19:23 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:19:23 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:19:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:19:24 GMT
USER mysql
# Sat, 16 Sep 2023 03:19:24 GMT
EXPOSE 3306 33060
# Sat, 16 Sep 2023 03:19:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3eb6a50586d1e36befa4b41c2f504fdca518e4dbab482447202e95f02d9a6d78`  
		Last Modified: Sat, 16 Sep 2023 02:41:45 GMT  
		Size: 88.0 MB (87981331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b862f5c29fc2f5d3ec755acbd06e50014dd1b43f1f19e7d4308bf3dc6400213`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e79402c6d72a78cdee928786910d1d7733f70b63e909191e90340bfff252b4`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 7.3 MB (7318755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c329149170975f92c22d07c1e4729f89b6e995b852f8f9b922c80fd35cea11e1`  
		Last Modified: Sat, 16 Sep 2023 03:26:36 GMT  
		Size: 291.0 MB (291001444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d7cb6108d9d66e59db734407518df57d9df29ff29b5a52140aed2a9d0189d2`  
		Last Modified: Sat, 16 Sep 2023 03:25:55 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1ebb922232888f9a3c70f046afb603ae93ca8de117240f198813f43c671af`  
		Last Modified: Sat, 16 Sep 2023 03:25:54 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.33-25-centos`

```console
$ docker pull percona@sha256:2e01ea8231b2e6e7f2de456733657146256f10ccfae35c28aea66d913d1ca248
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8.0.33-25-centos` - linux; amd64

```console
$ docker pull percona@sha256:ae8292248648fdc91e23a763165c0ecb1023021258026a2b17fb07e6f50ba1ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.3 MB (386307418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d149e90e32fe93d48e2a5e000737efab116a1daf5b6accf690855df59c960f1d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:18 GMT
ADD file:ca759c2861c7b47f87efcda8b2d88a6e2a3e34fa5a4e6bcebab50b985aaf2868 in / 
# Sat, 16 Sep 2023 02:40:19 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:18:18 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:18:19 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV OS_VER=el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_REPO=testing
# Sat, 16 Sep 2023 03:18:22 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 16 Sep 2023 03:19:19 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:19:23 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 16 Sep 2023 03:19:23 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:19:23 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:19:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:19:24 GMT
USER mysql
# Sat, 16 Sep 2023 03:19:24 GMT
EXPOSE 3306 33060
# Sat, 16 Sep 2023 03:19:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3eb6a50586d1e36befa4b41c2f504fdca518e4dbab482447202e95f02d9a6d78`  
		Last Modified: Sat, 16 Sep 2023 02:41:45 GMT  
		Size: 88.0 MB (87981331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b862f5c29fc2f5d3ec755acbd06e50014dd1b43f1f19e7d4308bf3dc6400213`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e79402c6d72a78cdee928786910d1d7733f70b63e909191e90340bfff252b4`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 7.3 MB (7318755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c329149170975f92c22d07c1e4729f89b6e995b852f8f9b922c80fd35cea11e1`  
		Last Modified: Sat, 16 Sep 2023 03:26:36 GMT  
		Size: 291.0 MB (291001444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d7cb6108d9d66e59db734407518df57d9df29ff29b5a52140aed2a9d0189d2`  
		Last Modified: Sat, 16 Sep 2023 03:25:55 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1ebb922232888f9a3c70f046afb603ae93ca8de117240f198813f43c671af`  
		Last Modified: Sat, 16 Sep 2023 03:25:54 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:centos`

```console
$ docker pull percona@sha256:c6cec5f9c14edc620a6b12fbba50a3a8dffa21fc7724c37503044432c904b482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:centos` - linux; amd64

```console
$ docker pull percona@sha256:a73b5048c98576f126077b4ac202a16caf66abebe08b330615e46eac6f3990e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422738287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef9ed4d199cd1798ea6627a94cc29fc7580824bf0cf5e39f9132dcee8b5dc50`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:19:29 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:20:04 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 16 Sep 2023 03:20:05 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 16 Sep 2023 03:20:05 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:20:05 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 16 Sep 2023 03:20:44 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:20:45 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 16 Sep 2023 03:20:45 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:20:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:20:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:20:46 GMT
USER mysql
# Sat, 16 Sep 2023 03:20:46 GMT
EXPOSE 3306
# Sat, 16 Sep 2023 03:20:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f444e97db0bf5d50f5015a158a00bd5e453060943342f50cd305119e04ecc3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f512ea8d3aec4fe796c01a42c138a1865db0af5bbb181535f7b815db30908aa8`  
		Last Modified: Sat, 16 Sep 2023 03:27:23 GMT  
		Size: 196.3 MB (196271669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5017199f5cf25acfe2e4bf52f8ad3b297c2299ab04b85ddd2f2390bb12d13bb3`  
		Last Modified: Sat, 16 Sep 2023 03:27:21 GMT  
		Size: 137.5 MB (137541712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b594fad71442b6e1ab26f111cacaec4f79a1b00589d5a9e795a0b797e8b36a82`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b7a9503470801e82fdbfdd3b7346e4301ac0e879acd895b1281b7e039ffa3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 3.1 KB (3062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5`

```console
$ docker pull percona@sha256:c6cec5f9c14edc620a6b12fbba50a3a8dffa21fc7724c37503044432c904b482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-5` - linux; amd64

```console
$ docker pull percona@sha256:a73b5048c98576f126077b4ac202a16caf66abebe08b330615e46eac6f3990e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422738287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef9ed4d199cd1798ea6627a94cc29fc7580824bf0cf5e39f9132dcee8b5dc50`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:19:29 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:20:04 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 16 Sep 2023 03:20:05 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 16 Sep 2023 03:20:05 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:20:05 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 16 Sep 2023 03:20:44 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:20:45 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 16 Sep 2023 03:20:45 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:20:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:20:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:20:46 GMT
USER mysql
# Sat, 16 Sep 2023 03:20:46 GMT
EXPOSE 3306
# Sat, 16 Sep 2023 03:20:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f444e97db0bf5d50f5015a158a00bd5e453060943342f50cd305119e04ecc3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f512ea8d3aec4fe796c01a42c138a1865db0af5bbb181535f7b815db30908aa8`  
		Last Modified: Sat, 16 Sep 2023 03:27:23 GMT  
		Size: 196.3 MB (196271669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5017199f5cf25acfe2e4bf52f8ad3b297c2299ab04b85ddd2f2390bb12d13bb3`  
		Last Modified: Sat, 16 Sep 2023 03:27:21 GMT  
		Size: 137.5 MB (137541712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b594fad71442b6e1ab26f111cacaec4f79a1b00589d5a9e795a0b797e8b36a82`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b7a9503470801e82fdbfdd3b7346e4301ac0e879acd895b1281b7e039ffa3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 3.1 KB (3062 bytes)  
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
$ docker pull percona@sha256:c6cec5f9c14edc620a6b12fbba50a3a8dffa21fc7724c37503044432c904b482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-5.7` - linux; amd64

```console
$ docker pull percona@sha256:a73b5048c98576f126077b4ac202a16caf66abebe08b330615e46eac6f3990e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422738287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef9ed4d199cd1798ea6627a94cc29fc7580824bf0cf5e39f9132dcee8b5dc50`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:19:29 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:20:04 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 16 Sep 2023 03:20:05 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 16 Sep 2023 03:20:05 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:20:05 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 16 Sep 2023 03:20:44 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:20:45 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 16 Sep 2023 03:20:45 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:20:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:20:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:20:46 GMT
USER mysql
# Sat, 16 Sep 2023 03:20:46 GMT
EXPOSE 3306
# Sat, 16 Sep 2023 03:20:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f444e97db0bf5d50f5015a158a00bd5e453060943342f50cd305119e04ecc3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f512ea8d3aec4fe796c01a42c138a1865db0af5bbb181535f7b815db30908aa8`  
		Last Modified: Sat, 16 Sep 2023 03:27:23 GMT  
		Size: 196.3 MB (196271669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5017199f5cf25acfe2e4bf52f8ad3b297c2299ab04b85ddd2f2390bb12d13bb3`  
		Last Modified: Sat, 16 Sep 2023 03:27:21 GMT  
		Size: 137.5 MB (137541712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b594fad71442b6e1ab26f111cacaec4f79a1b00589d5a9e795a0b797e8b36a82`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b7a9503470801e82fdbfdd3b7346e4301ac0e879acd895b1281b7e039ffa3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 3.1 KB (3062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.7.39`

```console
$ docker pull percona@sha256:c6cec5f9c14edc620a6b12fbba50a3a8dffa21fc7724c37503044432c904b482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-5.7.39` - linux; amd64

```console
$ docker pull percona@sha256:a73b5048c98576f126077b4ac202a16caf66abebe08b330615e46eac6f3990e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422738287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef9ed4d199cd1798ea6627a94cc29fc7580824bf0cf5e39f9132dcee8b5dc50`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:19:29 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:20:04 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 16 Sep 2023 03:20:05 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 16 Sep 2023 03:20:05 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:20:05 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 16 Sep 2023 03:20:44 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:20:45 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 16 Sep 2023 03:20:45 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:20:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:20:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:20:46 GMT
USER mysql
# Sat, 16 Sep 2023 03:20:46 GMT
EXPOSE 3306
# Sat, 16 Sep 2023 03:20:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f444e97db0bf5d50f5015a158a00bd5e453060943342f50cd305119e04ecc3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f512ea8d3aec4fe796c01a42c138a1865db0af5bbb181535f7b815db30908aa8`  
		Last Modified: Sat, 16 Sep 2023 03:27:23 GMT  
		Size: 196.3 MB (196271669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5017199f5cf25acfe2e4bf52f8ad3b297c2299ab04b85ddd2f2390bb12d13bb3`  
		Last Modified: Sat, 16 Sep 2023 03:27:21 GMT  
		Size: 137.5 MB (137541712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b594fad71442b6e1ab26f111cacaec4f79a1b00589d5a9e795a0b797e8b36a82`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b7a9503470801e82fdbfdd3b7346e4301ac0e879acd895b1281b7e039ffa3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 3.1 KB (3062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8`

```console
$ docker pull percona@sha256:2e01ea8231b2e6e7f2de456733657146256f10ccfae35c28aea66d913d1ca248
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-8` - linux; amd64

```console
$ docker pull percona@sha256:ae8292248648fdc91e23a763165c0ecb1023021258026a2b17fb07e6f50ba1ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.3 MB (386307418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d149e90e32fe93d48e2a5e000737efab116a1daf5b6accf690855df59c960f1d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:18 GMT
ADD file:ca759c2861c7b47f87efcda8b2d88a6e2a3e34fa5a4e6bcebab50b985aaf2868 in / 
# Sat, 16 Sep 2023 02:40:19 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:18:18 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:18:19 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV OS_VER=el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_REPO=testing
# Sat, 16 Sep 2023 03:18:22 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 16 Sep 2023 03:19:19 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:19:23 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 16 Sep 2023 03:19:23 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:19:23 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:19:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:19:24 GMT
USER mysql
# Sat, 16 Sep 2023 03:19:24 GMT
EXPOSE 3306 33060
# Sat, 16 Sep 2023 03:19:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3eb6a50586d1e36befa4b41c2f504fdca518e4dbab482447202e95f02d9a6d78`  
		Last Modified: Sat, 16 Sep 2023 02:41:45 GMT  
		Size: 88.0 MB (87981331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b862f5c29fc2f5d3ec755acbd06e50014dd1b43f1f19e7d4308bf3dc6400213`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e79402c6d72a78cdee928786910d1d7733f70b63e909191e90340bfff252b4`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 7.3 MB (7318755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c329149170975f92c22d07c1e4729f89b6e995b852f8f9b922c80fd35cea11e1`  
		Last Modified: Sat, 16 Sep 2023 03:26:36 GMT  
		Size: 291.0 MB (291001444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d7cb6108d9d66e59db734407518df57d9df29ff29b5a52140aed2a9d0189d2`  
		Last Modified: Sat, 16 Sep 2023 03:25:55 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1ebb922232888f9a3c70f046afb603ae93ca8de117240f198813f43c671af`  
		Last Modified: Sat, 16 Sep 2023 03:25:54 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0`

```console
$ docker pull percona@sha256:2e01ea8231b2e6e7f2de456733657146256f10ccfae35c28aea66d913d1ca248
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-8.0` - linux; amd64

```console
$ docker pull percona@sha256:ae8292248648fdc91e23a763165c0ecb1023021258026a2b17fb07e6f50ba1ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.3 MB (386307418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d149e90e32fe93d48e2a5e000737efab116a1daf5b6accf690855df59c960f1d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:18 GMT
ADD file:ca759c2861c7b47f87efcda8b2d88a6e2a3e34fa5a4e6bcebab50b985aaf2868 in / 
# Sat, 16 Sep 2023 02:40:19 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:18:18 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:18:19 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV OS_VER=el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_REPO=testing
# Sat, 16 Sep 2023 03:18:22 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 16 Sep 2023 03:19:19 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:19:23 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 16 Sep 2023 03:19:23 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:19:23 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:19:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:19:24 GMT
USER mysql
# Sat, 16 Sep 2023 03:19:24 GMT
EXPOSE 3306 33060
# Sat, 16 Sep 2023 03:19:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3eb6a50586d1e36befa4b41c2f504fdca518e4dbab482447202e95f02d9a6d78`  
		Last Modified: Sat, 16 Sep 2023 02:41:45 GMT  
		Size: 88.0 MB (87981331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b862f5c29fc2f5d3ec755acbd06e50014dd1b43f1f19e7d4308bf3dc6400213`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e79402c6d72a78cdee928786910d1d7733f70b63e909191e90340bfff252b4`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 7.3 MB (7318755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c329149170975f92c22d07c1e4729f89b6e995b852f8f9b922c80fd35cea11e1`  
		Last Modified: Sat, 16 Sep 2023 03:26:36 GMT  
		Size: 291.0 MB (291001444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d7cb6108d9d66e59db734407518df57d9df29ff29b5a52140aed2a9d0189d2`  
		Last Modified: Sat, 16 Sep 2023 03:25:55 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1ebb922232888f9a3c70f046afb603ae93ca8de117240f198813f43c671af`  
		Last Modified: Sat, 16 Sep 2023 03:25:54 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0.33-25`

```console
$ docker pull percona@sha256:2e01ea8231b2e6e7f2de456733657146256f10ccfae35c28aea66d913d1ca248
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-8.0.33-25` - linux; amd64

```console
$ docker pull percona@sha256:ae8292248648fdc91e23a763165c0ecb1023021258026a2b17fb07e6f50ba1ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.3 MB (386307418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d149e90e32fe93d48e2a5e000737efab116a1daf5b6accf690855df59c960f1d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:18 GMT
ADD file:ca759c2861c7b47f87efcda8b2d88a6e2a3e34fa5a4e6bcebab50b985aaf2868 in / 
# Sat, 16 Sep 2023 02:40:19 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:18:18 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:18:19 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 16 Sep 2023 03:18:19 GMT
ENV OS_VER=el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 16 Sep 2023 03:18:19 GMT
ENV PS_REPO=testing
# Sat, 16 Sep 2023 03:18:22 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 16 Sep 2023 03:19:19 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:19:23 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 16 Sep 2023 03:19:23 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:19:23 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:19:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:19:24 GMT
USER mysql
# Sat, 16 Sep 2023 03:19:24 GMT
EXPOSE 3306 33060
# Sat, 16 Sep 2023 03:19:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3eb6a50586d1e36befa4b41c2f504fdca518e4dbab482447202e95f02d9a6d78`  
		Last Modified: Sat, 16 Sep 2023 02:41:45 GMT  
		Size: 88.0 MB (87981331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b862f5c29fc2f5d3ec755acbd06e50014dd1b43f1f19e7d4308bf3dc6400213`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e79402c6d72a78cdee928786910d1d7733f70b63e909191e90340bfff252b4`  
		Last Modified: Sat, 16 Sep 2023 03:25:56 GMT  
		Size: 7.3 MB (7318755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c329149170975f92c22d07c1e4729f89b6e995b852f8f9b922c80fd35cea11e1`  
		Last Modified: Sat, 16 Sep 2023 03:26:36 GMT  
		Size: 291.0 MB (291001444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d7cb6108d9d66e59db734407518df57d9df29ff29b5a52140aed2a9d0189d2`  
		Last Modified: Sat, 16 Sep 2023 03:25:55 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1ebb922232888f9a3c70f046afb603ae93ca8de117240f198813f43c671af`  
		Last Modified: Sat, 16 Sep 2023 03:25:54 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:23abd672819951926cc88313b72ffb55e38216b9a33a8f28d4535acab28dee82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:7945b80af0a2c7469457dad587627d88457dc09605580a3660c8b9f636424500
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.0 MB (219041553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0a7612184008c7ab6b31a6a43b6fe944ad67fc1e0bc16e15f9c376232ea60fb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:24:25 GMT
ENV PSMDB_VERSION=4.2.24-24
# Sat, 16 Sep 2023 03:24:25 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:24:25 GMT
ENV FULL_PERCONA_VERSION=4.2.24-24.el8
# Sat, 16 Sep 2023 03:24:25 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 16 Sep 2023 03:24:25 GMT
ENV PSMDB_REPO=release
# Sat, 16 Sep 2023 03:24:28 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 16 Sep 2023 03:25:16 GMT
RUN set -ex;     percona-release enable psmdb-42 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 16 Sep 2023 03:25:17 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 16 Sep 2023 03:25:17 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 16 Sep 2023 03:25:18 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 16 Sep 2023 03:25:18 GMT
ENV GOSU_VERSION=1.11
# Sat, 16 Sep 2023 03:25:21 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 16 Sep 2023 03:25:23 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -;     rm -f /tmp/SHA256SUMS;     chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 16 Sep 2023 03:25:23 GMT
VOLUME [/data/db]
# Sat, 16 Sep 2023 03:25:23 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Sat, 16 Sep 2023 03:25:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Sep 2023 03:25:23 GMT
EXPOSE 27017
# Sat, 16 Sep 2023 03:25:23 GMT
USER 1001
# Sat, 16 Sep 2023 03:25:24 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164f7a68b7030bc124d9cf34d07c76d54ec1e79572e31be3295e182a2e21c6d8`  
		Last Modified: Sat, 16 Sep 2023 03:29:36 GMT  
		Size: 3.8 MB (3787089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa491dd6268e0b275a5a4fcf806e2dc7223b0e14fd3acc0934b505750da44f01`  
		Last Modified: Sat, 16 Sep 2023 03:29:49 GMT  
		Size: 117.2 MB (117248300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e22a62adb6db81041318c87098dbeacedd0f94a5e386156a837ee8b447869d2`  
		Last Modified: Sat, 16 Sep 2023 03:29:34 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee62e609fee604f1c59eacedc4931822640150fe98cc28cb3fac909d072b0c5`  
		Last Modified: Sat, 16 Sep 2023 03:29:32 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14fdbc03b279777b2c0b114065624c47425321bc690f66299718abd1411c62fb`  
		Last Modified: Sat, 16 Sep 2023 03:29:32 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc65965ba646c52e9491c7f1596407af88f353a61f5f24c817915c18fcde045`  
		Last Modified: Sat, 16 Sep 2023 03:29:34 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f40cca8a55dad9ae9da7a03390bf5f4237ab2e2c6865f3c960f626819021c7f`  
		Last Modified: Sat, 16 Sep 2023 03:29:34 GMT  
		Size: 8.2 MB (8151461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5966d0fa83dea102b0f55fd20f6b988f830c5ea4837ca6697106dcb76144cef`  
		Last Modified: Sat, 16 Sep 2023 03:29:33 GMT  
		Size: 4.6 KB (4556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2.24`

```console
$ docker pull percona@sha256:23abd672819951926cc88313b72ffb55e38216b9a33a8f28d4535acab28dee82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2.24` - linux; amd64

```console
$ docker pull percona@sha256:7945b80af0a2c7469457dad587627d88457dc09605580a3660c8b9f636424500
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.0 MB (219041553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0a7612184008c7ab6b31a6a43b6fe944ad67fc1e0bc16e15f9c376232ea60fb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:24:25 GMT
ENV PSMDB_VERSION=4.2.24-24
# Sat, 16 Sep 2023 03:24:25 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:24:25 GMT
ENV FULL_PERCONA_VERSION=4.2.24-24.el8
# Sat, 16 Sep 2023 03:24:25 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 16 Sep 2023 03:24:25 GMT
ENV PSMDB_REPO=release
# Sat, 16 Sep 2023 03:24:28 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 16 Sep 2023 03:25:16 GMT
RUN set -ex;     percona-release enable psmdb-42 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 16 Sep 2023 03:25:17 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 16 Sep 2023 03:25:17 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 16 Sep 2023 03:25:18 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 16 Sep 2023 03:25:18 GMT
ENV GOSU_VERSION=1.11
# Sat, 16 Sep 2023 03:25:21 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 16 Sep 2023 03:25:23 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -;     rm -f /tmp/SHA256SUMS;     chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 16 Sep 2023 03:25:23 GMT
VOLUME [/data/db]
# Sat, 16 Sep 2023 03:25:23 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Sat, 16 Sep 2023 03:25:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Sep 2023 03:25:23 GMT
EXPOSE 27017
# Sat, 16 Sep 2023 03:25:23 GMT
USER 1001
# Sat, 16 Sep 2023 03:25:24 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164f7a68b7030bc124d9cf34d07c76d54ec1e79572e31be3295e182a2e21c6d8`  
		Last Modified: Sat, 16 Sep 2023 03:29:36 GMT  
		Size: 3.8 MB (3787089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa491dd6268e0b275a5a4fcf806e2dc7223b0e14fd3acc0934b505750da44f01`  
		Last Modified: Sat, 16 Sep 2023 03:29:49 GMT  
		Size: 117.2 MB (117248300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e22a62adb6db81041318c87098dbeacedd0f94a5e386156a837ee8b447869d2`  
		Last Modified: Sat, 16 Sep 2023 03:29:34 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee62e609fee604f1c59eacedc4931822640150fe98cc28cb3fac909d072b0c5`  
		Last Modified: Sat, 16 Sep 2023 03:29:32 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14fdbc03b279777b2c0b114065624c47425321bc690f66299718abd1411c62fb`  
		Last Modified: Sat, 16 Sep 2023 03:29:32 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc65965ba646c52e9491c7f1596407af88f353a61f5f24c817915c18fcde045`  
		Last Modified: Sat, 16 Sep 2023 03:29:34 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f40cca8a55dad9ae9da7a03390bf5f4237ab2e2c6865f3c960f626819021c7f`  
		Last Modified: Sat, 16 Sep 2023 03:29:34 GMT  
		Size: 8.2 MB (8151461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5966d0fa83dea102b0f55fd20f6b988f830c5ea4837ca6697106dcb76144cef`  
		Last Modified: Sat, 16 Sep 2023 03:29:33 GMT  
		Size: 4.6 KB (4556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.4`

```console
$ docker pull percona@sha256:c1d21c2f4497ec62f77a284d5fee49e7c03bc0ecd598a1306a04ba45342889e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4` - linux; amd64

```console
$ docker pull percona@sha256:1bcf9ad1246413083ef89c2982e1c9dd4dd25bb88dfc3862b339032ce6fef012
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.6 MB (237567526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffd830a53b347b0eb40ecc8828a564514d3e27b9fa150eb185ceb72293a8ed4d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:20:57 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 16 Sep 2023 03:23:14 GMT
ENV PSMDB_VERSION=4.4.22-21
# Sat, 16 Sep 2023 03:23:15 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:23:15 GMT
ENV FULL_PERCONA_VERSION=4.4.22-21.el8
# Sat, 16 Sep 2023 03:23:15 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 16 Sep 2023 03:23:15 GMT
ENV PSMDB_REPO=release
# Sat, 16 Sep 2023 03:24:06 GMT
RUN set -ex;     percona-release enable psmdb-44 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 16 Sep 2023 03:24:07 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 16 Sep 2023 03:24:07 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 16 Sep 2023 03:24:08 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 16 Sep 2023 03:24:08 GMT
ENV GOSU_VERSION=1.11
# Sat, 16 Sep 2023 03:24:10 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 16 Sep 2023 03:24:12 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 16 Sep 2023 03:24:12 GMT
VOLUME [/data/db]
# Sat, 16 Sep 2023 03:24:13 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 16 Sep 2023 03:24:13 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Sat, 16 Sep 2023 03:24:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Sep 2023 03:24:13 GMT
EXPOSE 27017
# Sat, 16 Sep 2023 03:24:13 GMT
USER 1001
# Sat, 16 Sep 2023 03:24:13 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05e3d36be41c8199349fc1fbf86a3bbc59e02a85af0a54a344e3be2526541d3`  
		Last Modified: Sat, 16 Sep 2023 03:28:02 GMT  
		Size: 3.8 MB (3787089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e54ff162db57c7d144feb0389c3530d109205efec0388e9e9603987a4114e5`  
		Last Modified: Sat, 16 Sep 2023 03:29:21 GMT  
		Size: 135.8 MB (135774644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786e05d09e9a80aa0579350a6bcdce8f577cdf3346f2ef91300445da278c14ab`  
		Last Modified: Sat, 16 Sep 2023 03:29:02 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b344a316644c660de39209499f7b9b81630b9cdc57adf3e12e30191ca84d1614`  
		Last Modified: Sat, 16 Sep 2023 03:29:02 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646ac6209edb2c87239c2a843c162afe141cd5f92e79117dd9257b7141701b66`  
		Last Modified: Sat, 16 Sep 2023 03:29:01 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4959b31cd07fffcd1df50e0f737c260fd31a486286ac1309d19eb451cd378c1c`  
		Last Modified: Sat, 16 Sep 2023 03:29:02 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dc0fb6c1ded9be533e4ecc8efff05c51a811b1cc845068bc350fd47505f3e3`  
		Last Modified: Sat, 16 Sep 2023 03:29:02 GMT  
		Size: 8.1 MB (8137885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d95bedb436b5533dbcf9477eec10a8baccb941e82c4eba3e6dbadf8c7a580a`  
		Last Modified: Sat, 16 Sep 2023 03:29:00 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0cf6fa3ad13b2d92feb6417ab0e0beb7c49e436b46f6c1067b78731705ae12`  
		Last Modified: Sat, 16 Sep 2023 03:29:01 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.4.22`

```console
$ docker pull percona@sha256:c1d21c2f4497ec62f77a284d5fee49e7c03bc0ecd598a1306a04ba45342889e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4.22` - linux; amd64

```console
$ docker pull percona@sha256:1bcf9ad1246413083ef89c2982e1c9dd4dd25bb88dfc3862b339032ce6fef012
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.6 MB (237567526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffd830a53b347b0eb40ecc8828a564514d3e27b9fa150eb185ceb72293a8ed4d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:20:57 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 16 Sep 2023 03:23:14 GMT
ENV PSMDB_VERSION=4.4.22-21
# Sat, 16 Sep 2023 03:23:15 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:23:15 GMT
ENV FULL_PERCONA_VERSION=4.4.22-21.el8
# Sat, 16 Sep 2023 03:23:15 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 16 Sep 2023 03:23:15 GMT
ENV PSMDB_REPO=release
# Sat, 16 Sep 2023 03:24:06 GMT
RUN set -ex;     percona-release enable psmdb-44 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 16 Sep 2023 03:24:07 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 16 Sep 2023 03:24:07 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 16 Sep 2023 03:24:08 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 16 Sep 2023 03:24:08 GMT
ENV GOSU_VERSION=1.11
# Sat, 16 Sep 2023 03:24:10 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 16 Sep 2023 03:24:12 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 16 Sep 2023 03:24:12 GMT
VOLUME [/data/db]
# Sat, 16 Sep 2023 03:24:13 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 16 Sep 2023 03:24:13 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Sat, 16 Sep 2023 03:24:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Sep 2023 03:24:13 GMT
EXPOSE 27017
# Sat, 16 Sep 2023 03:24:13 GMT
USER 1001
# Sat, 16 Sep 2023 03:24:13 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05e3d36be41c8199349fc1fbf86a3bbc59e02a85af0a54a344e3be2526541d3`  
		Last Modified: Sat, 16 Sep 2023 03:28:02 GMT  
		Size: 3.8 MB (3787089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e54ff162db57c7d144feb0389c3530d109205efec0388e9e9603987a4114e5`  
		Last Modified: Sat, 16 Sep 2023 03:29:21 GMT  
		Size: 135.8 MB (135774644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786e05d09e9a80aa0579350a6bcdce8f577cdf3346f2ef91300445da278c14ab`  
		Last Modified: Sat, 16 Sep 2023 03:29:02 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b344a316644c660de39209499f7b9b81630b9cdc57adf3e12e30191ca84d1614`  
		Last Modified: Sat, 16 Sep 2023 03:29:02 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646ac6209edb2c87239c2a843c162afe141cd5f92e79117dd9257b7141701b66`  
		Last Modified: Sat, 16 Sep 2023 03:29:01 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4959b31cd07fffcd1df50e0f737c260fd31a486286ac1309d19eb451cd378c1c`  
		Last Modified: Sat, 16 Sep 2023 03:29:02 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dc0fb6c1ded9be533e4ecc8efff05c51a811b1cc845068bc350fd47505f3e3`  
		Last Modified: Sat, 16 Sep 2023 03:29:02 GMT  
		Size: 8.1 MB (8137885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d95bedb436b5533dbcf9477eec10a8baccb941e82c4eba3e6dbadf8c7a580a`  
		Last Modified: Sat, 16 Sep 2023 03:29:00 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0cf6fa3ad13b2d92feb6417ab0e0beb7c49e436b46f6c1067b78731705ae12`  
		Last Modified: Sat, 16 Sep 2023 03:29:01 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-5.0`

```console
$ docker pull percona@sha256:c4b4be632649a35476b3e34e510424fcfcedca19a094fc3ad679ae91425d519c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0` - linux; amd64

```console
$ docker pull percona@sha256:dfabd9b9e0153636145e8f264b6e813c2983b3a7da13e30fda0b290498eede46
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.2 MB (250190246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0db2202d3cd2e31e87fc46e378d2e70ba77f2767bd55407c46211ee146865762`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:20:57 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 16 Sep 2023 03:22:04 GMT
ENV PSMDB_VERSION=5.0.18-15
# Sat, 16 Sep 2023 03:22:05 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:22:05 GMT
ENV FULL_PERCONA_VERSION=5.0.18-15.el8
# Sat, 16 Sep 2023 03:22:05 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 16 Sep 2023 03:22:05 GMT
ENV PSMDB_REPO=release
# Sat, 16 Sep 2023 03:22:56 GMT
RUN set -ex;     percona-release enable psmdb-50 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 16 Sep 2023 03:22:58 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 16 Sep 2023 03:22:58 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 16 Sep 2023 03:22:58 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 16 Sep 2023 03:22:58 GMT
ENV GOSU_VERSION=1.11
# Sat, 16 Sep 2023 03:23:01 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 16 Sep 2023 03:23:03 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 16 Sep 2023 03:23:03 GMT
VOLUME [/data/db]
# Sat, 16 Sep 2023 03:23:04 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 16 Sep 2023 03:23:04 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Sat, 16 Sep 2023 03:23:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Sep 2023 03:23:04 GMT
EXPOSE 27017
# Sat, 16 Sep 2023 03:23:04 GMT
USER 1001
# Sat, 16 Sep 2023 03:23:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05e3d36be41c8199349fc1fbf86a3bbc59e02a85af0a54a344e3be2526541d3`  
		Last Modified: Sat, 16 Sep 2023 03:28:02 GMT  
		Size: 3.8 MB (3787089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff70f2e66b57cd0fda23607ce78aac917d21d9ccf02db59bbc3083ac13dc8ded`  
		Last Modified: Sat, 16 Sep 2023 03:28:51 GMT  
		Size: 148.4 MB (148397360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e221e65c1b87a74ec925de090de38d953e057f2228e68c677696b390ff79d6`  
		Last Modified: Sat, 16 Sep 2023 03:28:32 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c35f372f2a40219aa75920000dba5c283f7a8ea7851717d2472cc334a13391`  
		Last Modified: Sat, 16 Sep 2023 03:28:32 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a493c1a2444558b040b64a0d4e47c30b3175ad5410408a6e2695f3ff8f26eaf`  
		Last Modified: Sat, 16 Sep 2023 03:28:30 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990611eec7b00eff3536f2a6e6d4f312d6dac59dcc5777bd59882e723dce9540`  
		Last Modified: Sat, 16 Sep 2023 03:28:31 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10f0cbe2260d255154812730941b13cebc1e2ff07c61195d2e33ca76edf67dc`  
		Last Modified: Sat, 16 Sep 2023 03:28:33 GMT  
		Size: 8.1 MB (8137888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b63594111c753e86af94d423428ba1a87e420ff2a9e10428d5d9a717f07fd1`  
		Last Modified: Sat, 16 Sep 2023 03:28:30 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46e9cfe9b3455df82eb3154b89667832270d12d681ca705a5fb07528aa5c3b4`  
		Last Modified: Sat, 16 Sep 2023 03:28:30 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-5.0.18`

```console
$ docker pull percona@sha256:c4b4be632649a35476b3e34e510424fcfcedca19a094fc3ad679ae91425d519c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0.18` - linux; amd64

```console
$ docker pull percona@sha256:dfabd9b9e0153636145e8f264b6e813c2983b3a7da13e30fda0b290498eede46
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.2 MB (250190246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0db2202d3cd2e31e87fc46e378d2e70ba77f2767bd55407c46211ee146865762`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:20:57 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 16 Sep 2023 03:22:04 GMT
ENV PSMDB_VERSION=5.0.18-15
# Sat, 16 Sep 2023 03:22:05 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:22:05 GMT
ENV FULL_PERCONA_VERSION=5.0.18-15.el8
# Sat, 16 Sep 2023 03:22:05 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 16 Sep 2023 03:22:05 GMT
ENV PSMDB_REPO=release
# Sat, 16 Sep 2023 03:22:56 GMT
RUN set -ex;     percona-release enable psmdb-50 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 16 Sep 2023 03:22:58 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 16 Sep 2023 03:22:58 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 16 Sep 2023 03:22:58 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 16 Sep 2023 03:22:58 GMT
ENV GOSU_VERSION=1.11
# Sat, 16 Sep 2023 03:23:01 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 16 Sep 2023 03:23:03 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 16 Sep 2023 03:23:03 GMT
VOLUME [/data/db]
# Sat, 16 Sep 2023 03:23:04 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 16 Sep 2023 03:23:04 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Sat, 16 Sep 2023 03:23:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Sep 2023 03:23:04 GMT
EXPOSE 27017
# Sat, 16 Sep 2023 03:23:04 GMT
USER 1001
# Sat, 16 Sep 2023 03:23:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05e3d36be41c8199349fc1fbf86a3bbc59e02a85af0a54a344e3be2526541d3`  
		Last Modified: Sat, 16 Sep 2023 03:28:02 GMT  
		Size: 3.8 MB (3787089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff70f2e66b57cd0fda23607ce78aac917d21d9ccf02db59bbc3083ac13dc8ded`  
		Last Modified: Sat, 16 Sep 2023 03:28:51 GMT  
		Size: 148.4 MB (148397360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e221e65c1b87a74ec925de090de38d953e057f2228e68c677696b390ff79d6`  
		Last Modified: Sat, 16 Sep 2023 03:28:32 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c35f372f2a40219aa75920000dba5c283f7a8ea7851717d2472cc334a13391`  
		Last Modified: Sat, 16 Sep 2023 03:28:32 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a493c1a2444558b040b64a0d4e47c30b3175ad5410408a6e2695f3ff8f26eaf`  
		Last Modified: Sat, 16 Sep 2023 03:28:30 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990611eec7b00eff3536f2a6e6d4f312d6dac59dcc5777bd59882e723dce9540`  
		Last Modified: Sat, 16 Sep 2023 03:28:31 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10f0cbe2260d255154812730941b13cebc1e2ff07c61195d2e33ca76edf67dc`  
		Last Modified: Sat, 16 Sep 2023 03:28:33 GMT  
		Size: 8.1 MB (8137888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b63594111c753e86af94d423428ba1a87e420ff2a9e10428d5d9a717f07fd1`  
		Last Modified: Sat, 16 Sep 2023 03:28:30 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46e9cfe9b3455df82eb3154b89667832270d12d681ca705a5fb07528aa5c3b4`  
		Last Modified: Sat, 16 Sep 2023 03:28:30 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-6.0`

```console
$ docker pull percona@sha256:ded7b39fba731d32a7ab789b698ebbaac684344ad492c186ca079eba6581621d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-6.0` - linux; amd64

```console
$ docker pull percona@sha256:41d8d8b0d3181637b5dd493b660980570f32df6d254e202eb16d3793823a4cbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.6 MB (273606863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1beee0ffb717a17048ce1f17eedc2ec80d713f43b3ee9c39dbe9c6d5d5e94f31`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:20:57 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 16 Sep 2023 03:20:57 GMT
ENV PSMDB_VERSION=6.0.6-5
# Sat, 16 Sep 2023 03:20:57 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:20:57 GMT
ENV FULL_PERCONA_VERSION=6.0.6-5.el8
# Sat, 16 Sep 2023 03:20:57 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 16 Sep 2023 03:20:57 GMT
ENV PSMDB_REPO=release
# Sat, 16 Sep 2023 03:21:53 GMT
RUN set -ex;     percona-release enable psmdb-60 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         percona-mongodb-mongosh         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-60/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 16 Sep 2023 03:21:54 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 16 Sep 2023 03:21:54 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 16 Sep 2023 03:21:55 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 16 Sep 2023 03:21:55 GMT
ENV GOSU_VERSION=1.11
# Sat, 16 Sep 2023 03:21:58 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 16 Sep 2023 03:22:00 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 16 Sep 2023 03:22:00 GMT
VOLUME [/data/db]
# Sat, 16 Sep 2023 03:22:01 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 16 Sep 2023 03:22:01 GMT
COPY file:7ab35f422fd362616b84e1dc71329cc9be05b7f834182c48bf98ceb92ee28956 in /entrypoint.sh 
# Sat, 16 Sep 2023 03:22:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Sep 2023 03:22:01 GMT
EXPOSE 27017
# Sat, 16 Sep 2023 03:22:01 GMT
USER 1001
# Sat, 16 Sep 2023 03:22:01 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05e3d36be41c8199349fc1fbf86a3bbc59e02a85af0a54a344e3be2526541d3`  
		Last Modified: Sat, 16 Sep 2023 03:28:02 GMT  
		Size: 3.8 MB (3787089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6797beff72ae7d4fb4042b0fbfa43229b899e9e2d03fe23f2c33c158ef4e3009`  
		Last Modified: Sat, 16 Sep 2023 03:28:20 GMT  
		Size: 171.8 MB (171813971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8207b8bc10dbfe3dac16324aeaba242a3cf036c263bac1407a56cce0fd3cea7`  
		Last Modified: Sat, 16 Sep 2023 03:27:58 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd461e079adf112c435382b24f3769a4e88bd43d411a092d5a5ff0b17d711426`  
		Last Modified: Sat, 16 Sep 2023 03:27:59 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606fca07bd5ba781da4820182065ffbe912bb07ec46f198af2d05b54142b6322`  
		Last Modified: Sat, 16 Sep 2023 03:27:56 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ed15729968bb75f0f6c602164192d3cfa61d331a1fb772c6dddec8e9dd7e0d`  
		Last Modified: Sat, 16 Sep 2023 03:27:58 GMT  
		Size: 914.5 KB (914546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d8477fb148d790ed4faad835bad6bdfc63f96f71abdcda7233fec85a4dc8ec`  
		Last Modified: Sat, 16 Sep 2023 03:27:58 GMT  
		Size: 8.1 MB (8137889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42a2ba3f90f7b01d71c4346365d6fc4ab229d0d1e131ffc45f47290d79d14d8`  
		Last Modified: Sat, 16 Sep 2023 03:27:56 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4c139e1d69ec80bed495fe387d648484d98948fbb6117458956fa55df3c2e9`  
		Last Modified: Sat, 16 Sep 2023 03:27:56 GMT  
		Size: 4.6 KB (4566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-6.0.6`

```console
$ docker pull percona@sha256:ded7b39fba731d32a7ab789b698ebbaac684344ad492c186ca079eba6581621d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-6.0.6` - linux; amd64

```console
$ docker pull percona@sha256:41d8d8b0d3181637b5dd493b660980570f32df6d254e202eb16d3793823a4cbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.6 MB (273606863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1beee0ffb717a17048ce1f17eedc2ec80d713f43b3ee9c39dbe9c6d5d5e94f31`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:20:57 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 16 Sep 2023 03:20:57 GMT
ENV PSMDB_VERSION=6.0.6-5
# Sat, 16 Sep 2023 03:20:57 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:20:57 GMT
ENV FULL_PERCONA_VERSION=6.0.6-5.el8
# Sat, 16 Sep 2023 03:20:57 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 16 Sep 2023 03:20:57 GMT
ENV PSMDB_REPO=release
# Sat, 16 Sep 2023 03:21:53 GMT
RUN set -ex;     percona-release enable psmdb-60 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         percona-mongodb-mongosh         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-60/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 16 Sep 2023 03:21:54 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 16 Sep 2023 03:21:54 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 16 Sep 2023 03:21:55 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 16 Sep 2023 03:21:55 GMT
ENV GOSU_VERSION=1.11
# Sat, 16 Sep 2023 03:21:58 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 16 Sep 2023 03:22:00 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 16 Sep 2023 03:22:00 GMT
VOLUME [/data/db]
# Sat, 16 Sep 2023 03:22:01 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 16 Sep 2023 03:22:01 GMT
COPY file:7ab35f422fd362616b84e1dc71329cc9be05b7f834182c48bf98ceb92ee28956 in /entrypoint.sh 
# Sat, 16 Sep 2023 03:22:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Sep 2023 03:22:01 GMT
EXPOSE 27017
# Sat, 16 Sep 2023 03:22:01 GMT
USER 1001
# Sat, 16 Sep 2023 03:22:01 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05e3d36be41c8199349fc1fbf86a3bbc59e02a85af0a54a344e3be2526541d3`  
		Last Modified: Sat, 16 Sep 2023 03:28:02 GMT  
		Size: 3.8 MB (3787089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6797beff72ae7d4fb4042b0fbfa43229b899e9e2d03fe23f2c33c158ef4e3009`  
		Last Modified: Sat, 16 Sep 2023 03:28:20 GMT  
		Size: 171.8 MB (171813971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8207b8bc10dbfe3dac16324aeaba242a3cf036c263bac1407a56cce0fd3cea7`  
		Last Modified: Sat, 16 Sep 2023 03:27:58 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd461e079adf112c435382b24f3769a4e88bd43d411a092d5a5ff0b17d711426`  
		Last Modified: Sat, 16 Sep 2023 03:27:59 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606fca07bd5ba781da4820182065ffbe912bb07ec46f198af2d05b54142b6322`  
		Last Modified: Sat, 16 Sep 2023 03:27:56 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ed15729968bb75f0f6c602164192d3cfa61d331a1fb772c6dddec8e9dd7e0d`  
		Last Modified: Sat, 16 Sep 2023 03:27:58 GMT  
		Size: 914.5 KB (914546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d8477fb148d790ed4faad835bad6bdfc63f96f71abdcda7233fec85a4dc8ec`  
		Last Modified: Sat, 16 Sep 2023 03:27:58 GMT  
		Size: 8.1 MB (8137889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42a2ba3f90f7b01d71c4346365d6fc4ab229d0d1e131ffc45f47290d79d14d8`  
		Last Modified: Sat, 16 Sep 2023 03:27:56 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4c139e1d69ec80bed495fe387d648484d98948fbb6117458956fa55df3c2e9`  
		Last Modified: Sat, 16 Sep 2023 03:27:56 GMT  
		Size: 4.6 KB (4566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
