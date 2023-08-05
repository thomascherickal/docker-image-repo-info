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
$ docker pull percona@sha256:917e909741490967eb1dcddaf4ae532591553af1d9d899f838a13a2451e13104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5` - linux; amd64

```console
$ docker pull percona@sha256:7a227334ec43908ce406b2008cd5bd0ac404a89943e79b5f18857fb19e22c0e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.0 MB (419019729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600b9ba8d1577af9fa44e0765ca47fc45ffb6b41b52198fbeaa782fd841d9ea2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:37:14 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:37:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 05 Aug 2023 02:37:48 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 05 Aug 2023 02:37:48 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:37:48 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 05 Aug 2023 02:38:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:38:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 05 Aug 2023 02:38:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:38:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:38:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:38:26 GMT
USER mysql
# Sat, 05 Aug 2023 02:38:26 GMT
EXPOSE 3306
# Sat, 05 Aug 2023 02:38:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c336c62cff80b45ee85a0fa59f487562fb97a60b6a378466408a5339184788`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246478ec69e60b803e615bd1822bbc541da434fc39e827e4b729e66087d6d4f2`  
		Last Modified: Sat, 05 Aug 2023 02:44:27 GMT  
		Size: 192.6 MB (192560961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128fd83d981eaadfa0f79125eda4a3644b513d6b30fb18221054437407088974`  
		Last Modified: Sat, 05 Aug 2023 02:44:33 GMT  
		Size: 137.5 MB (137531359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e43ed1f0be0a87de5bf18ece0d8c06c0102e487c244cd8a5a2a0fd21e7274a8`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b658c06491156c996cd6d918fb83f6d134df292838612393a3333d154d653d5`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5-centos`

```console
$ docker pull percona@sha256:917e909741490967eb1dcddaf4ae532591553af1d9d899f838a13a2451e13104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5-centos` - linux; amd64

```console
$ docker pull percona@sha256:7a227334ec43908ce406b2008cd5bd0ac404a89943e79b5f18857fb19e22c0e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.0 MB (419019729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600b9ba8d1577af9fa44e0765ca47fc45ffb6b41b52198fbeaa782fd841d9ea2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:37:14 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:37:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 05 Aug 2023 02:37:48 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 05 Aug 2023 02:37:48 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:37:48 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 05 Aug 2023 02:38:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:38:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 05 Aug 2023 02:38:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:38:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:38:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:38:26 GMT
USER mysql
# Sat, 05 Aug 2023 02:38:26 GMT
EXPOSE 3306
# Sat, 05 Aug 2023 02:38:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c336c62cff80b45ee85a0fa59f487562fb97a60b6a378466408a5339184788`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246478ec69e60b803e615bd1822bbc541da434fc39e827e4b729e66087d6d4f2`  
		Last Modified: Sat, 05 Aug 2023 02:44:27 GMT  
		Size: 192.6 MB (192560961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128fd83d981eaadfa0f79125eda4a3644b513d6b30fb18221054437407088974`  
		Last Modified: Sat, 05 Aug 2023 02:44:33 GMT  
		Size: 137.5 MB (137531359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e43ed1f0be0a87de5bf18ece0d8c06c0102e487c244cd8a5a2a0fd21e7274a8`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b658c06491156c996cd6d918fb83f6d134df292838612393a3333d154d653d5`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
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
$ docker pull percona@sha256:917e909741490967eb1dcddaf4ae532591553af1d9d899f838a13a2451e13104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5.7` - linux; amd64

```console
$ docker pull percona@sha256:7a227334ec43908ce406b2008cd5bd0ac404a89943e79b5f18857fb19e22c0e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.0 MB (419019729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600b9ba8d1577af9fa44e0765ca47fc45ffb6b41b52198fbeaa782fd841d9ea2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:37:14 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:37:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 05 Aug 2023 02:37:48 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 05 Aug 2023 02:37:48 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:37:48 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 05 Aug 2023 02:38:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:38:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 05 Aug 2023 02:38:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:38:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:38:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:38:26 GMT
USER mysql
# Sat, 05 Aug 2023 02:38:26 GMT
EXPOSE 3306
# Sat, 05 Aug 2023 02:38:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c336c62cff80b45ee85a0fa59f487562fb97a60b6a378466408a5339184788`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246478ec69e60b803e615bd1822bbc541da434fc39e827e4b729e66087d6d4f2`  
		Last Modified: Sat, 05 Aug 2023 02:44:27 GMT  
		Size: 192.6 MB (192560961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128fd83d981eaadfa0f79125eda4a3644b513d6b30fb18221054437407088974`  
		Last Modified: Sat, 05 Aug 2023 02:44:33 GMT  
		Size: 137.5 MB (137531359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e43ed1f0be0a87de5bf18ece0d8c06c0102e487c244cd8a5a2a0fd21e7274a8`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b658c06491156c996cd6d918fb83f6d134df292838612393a3333d154d653d5`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7-centos`

```console
$ docker pull percona@sha256:917e909741490967eb1dcddaf4ae532591553af1d9d899f838a13a2451e13104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5.7-centos` - linux; amd64

```console
$ docker pull percona@sha256:7a227334ec43908ce406b2008cd5bd0ac404a89943e79b5f18857fb19e22c0e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.0 MB (419019729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600b9ba8d1577af9fa44e0765ca47fc45ffb6b41b52198fbeaa782fd841d9ea2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:37:14 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:37:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 05 Aug 2023 02:37:48 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 05 Aug 2023 02:37:48 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:37:48 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 05 Aug 2023 02:38:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:38:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 05 Aug 2023 02:38:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:38:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:38:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:38:26 GMT
USER mysql
# Sat, 05 Aug 2023 02:38:26 GMT
EXPOSE 3306
# Sat, 05 Aug 2023 02:38:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c336c62cff80b45ee85a0fa59f487562fb97a60b6a378466408a5339184788`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246478ec69e60b803e615bd1822bbc541da434fc39e827e4b729e66087d6d4f2`  
		Last Modified: Sat, 05 Aug 2023 02:44:27 GMT  
		Size: 192.6 MB (192560961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128fd83d981eaadfa0f79125eda4a3644b513d6b30fb18221054437407088974`  
		Last Modified: Sat, 05 Aug 2023 02:44:33 GMT  
		Size: 137.5 MB (137531359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e43ed1f0be0a87de5bf18ece0d8c06c0102e487c244cd8a5a2a0fd21e7274a8`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b658c06491156c996cd6d918fb83f6d134df292838612393a3333d154d653d5`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.39`

```console
$ docker pull percona@sha256:917e909741490967eb1dcddaf4ae532591553af1d9d899f838a13a2451e13104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5.7.39` - linux; amd64

```console
$ docker pull percona@sha256:7a227334ec43908ce406b2008cd5bd0ac404a89943e79b5f18857fb19e22c0e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.0 MB (419019729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600b9ba8d1577af9fa44e0765ca47fc45ffb6b41b52198fbeaa782fd841d9ea2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:37:14 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:37:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 05 Aug 2023 02:37:48 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 05 Aug 2023 02:37:48 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:37:48 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 05 Aug 2023 02:38:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:38:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 05 Aug 2023 02:38:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:38:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:38:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:38:26 GMT
USER mysql
# Sat, 05 Aug 2023 02:38:26 GMT
EXPOSE 3306
# Sat, 05 Aug 2023 02:38:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c336c62cff80b45ee85a0fa59f487562fb97a60b6a378466408a5339184788`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246478ec69e60b803e615bd1822bbc541da434fc39e827e4b729e66087d6d4f2`  
		Last Modified: Sat, 05 Aug 2023 02:44:27 GMT  
		Size: 192.6 MB (192560961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128fd83d981eaadfa0f79125eda4a3644b513d6b30fb18221054437407088974`  
		Last Modified: Sat, 05 Aug 2023 02:44:33 GMT  
		Size: 137.5 MB (137531359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e43ed1f0be0a87de5bf18ece0d8c06c0102e487c244cd8a5a2a0fd21e7274a8`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b658c06491156c996cd6d918fb83f6d134df292838612393a3333d154d653d5`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.39-centos`

```console
$ docker pull percona@sha256:917e909741490967eb1dcddaf4ae532591553af1d9d899f838a13a2451e13104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:5.7.39-centos` - linux; amd64

```console
$ docker pull percona@sha256:7a227334ec43908ce406b2008cd5bd0ac404a89943e79b5f18857fb19e22c0e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.0 MB (419019729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600b9ba8d1577af9fa44e0765ca47fc45ffb6b41b52198fbeaa782fd841d9ea2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:37:14 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:37:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 05 Aug 2023 02:37:48 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 05 Aug 2023 02:37:48 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:37:48 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 05 Aug 2023 02:38:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:38:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 05 Aug 2023 02:38:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:38:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:38:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:38:26 GMT
USER mysql
# Sat, 05 Aug 2023 02:38:26 GMT
EXPOSE 3306
# Sat, 05 Aug 2023 02:38:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c336c62cff80b45ee85a0fa59f487562fb97a60b6a378466408a5339184788`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246478ec69e60b803e615bd1822bbc541da434fc39e827e4b729e66087d6d4f2`  
		Last Modified: Sat, 05 Aug 2023 02:44:27 GMT  
		Size: 192.6 MB (192560961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128fd83d981eaadfa0f79125eda4a3644b513d6b30fb18221054437407088974`  
		Last Modified: Sat, 05 Aug 2023 02:44:33 GMT  
		Size: 137.5 MB (137531359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e43ed1f0be0a87de5bf18ece0d8c06c0102e487c244cd8a5a2a0fd21e7274a8`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b658c06491156c996cd6d918fb83f6d134df292838612393a3333d154d653d5`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8`

```console
$ docker pull percona@sha256:96ef2a88078bf7466e69fe4a9627f71a25a7ed9b159a43267b4c8683e10d25ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8` - linux; amd64

```console
$ docker pull percona@sha256:8ee63a2dec0103c268ceb62ec570aabacd09f08018b9b6d27b0223748a182df8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.0 MB (383039058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5045329e3827d761c44560f86bed5bf1fdbdd6b542d9adf75016eeac8d09451d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:21 GMT
ADD file:103ed4e03109149f7699d9416e637526bc20a44d619dab1e50978e1876e22e88 in / 
# Sat, 05 Aug 2023 02:18:22 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:36:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:36:04 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV OS_VER=el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_REPO=testing
# Sat, 05 Aug 2023 02:36:07 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 05 Aug 2023 02:36:59 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:37:03 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 05 Aug 2023 02:37:03 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:37:03 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:37:03 GMT
USER mysql
# Sat, 05 Aug 2023 02:37:03 GMT
EXPOSE 3306 33060
# Sat, 05 Aug 2023 02:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f491dee0cae0e9048add4bd00a02d967b05be1bdea41cad6d85bc71a93f7379f`  
		Last Modified: Sat, 05 Aug 2023 02:19:49 GMT  
		Size: 88.0 MB (87961495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670e47ce96c1e6866a26866282b9af430aa11907c8899a0e32338456f2dc6c4`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.6 KB (1632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d615ab55531f934d4f8a7978717660b1ade4a01615d9a2fa0bec13abdb9e70b4`  
		Last Modified: Sat, 05 Aug 2023 02:43:15 GMT  
		Size: 7.3 MB (7328834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f23e970da7a2719ffbf306e0e4d99e9551684caa890df67980481309f78f92`  
		Last Modified: Sat, 05 Aug 2023 02:43:53 GMT  
		Size: 287.7 MB (287742843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d0648cdecce8ea0c3d8fcab8c6dfdb75ea6961ab9406086e2b15aa6f42a41e`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b096004652db826b7ec7391ba631b771ce45df3b85ddf22cd0dfbb743d2a03`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8-centos`

```console
$ docker pull percona@sha256:96ef2a88078bf7466e69fe4a9627f71a25a7ed9b159a43267b4c8683e10d25ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8-centos` - linux; amd64

```console
$ docker pull percona@sha256:8ee63a2dec0103c268ceb62ec570aabacd09f08018b9b6d27b0223748a182df8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.0 MB (383039058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5045329e3827d761c44560f86bed5bf1fdbdd6b542d9adf75016eeac8d09451d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:21 GMT
ADD file:103ed4e03109149f7699d9416e637526bc20a44d619dab1e50978e1876e22e88 in / 
# Sat, 05 Aug 2023 02:18:22 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:36:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:36:04 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV OS_VER=el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_REPO=testing
# Sat, 05 Aug 2023 02:36:07 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 05 Aug 2023 02:36:59 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:37:03 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 05 Aug 2023 02:37:03 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:37:03 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:37:03 GMT
USER mysql
# Sat, 05 Aug 2023 02:37:03 GMT
EXPOSE 3306 33060
# Sat, 05 Aug 2023 02:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f491dee0cae0e9048add4bd00a02d967b05be1bdea41cad6d85bc71a93f7379f`  
		Last Modified: Sat, 05 Aug 2023 02:19:49 GMT  
		Size: 88.0 MB (87961495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670e47ce96c1e6866a26866282b9af430aa11907c8899a0e32338456f2dc6c4`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.6 KB (1632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d615ab55531f934d4f8a7978717660b1ade4a01615d9a2fa0bec13abdb9e70b4`  
		Last Modified: Sat, 05 Aug 2023 02:43:15 GMT  
		Size: 7.3 MB (7328834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f23e970da7a2719ffbf306e0e4d99e9551684caa890df67980481309f78f92`  
		Last Modified: Sat, 05 Aug 2023 02:43:53 GMT  
		Size: 287.7 MB (287742843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d0648cdecce8ea0c3d8fcab8c6dfdb75ea6961ab9406086e2b15aa6f42a41e`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b096004652db826b7ec7391ba631b771ce45df3b85ddf22cd0dfbb743d2a03`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0`

```console
$ docker pull percona@sha256:96ef2a88078bf7466e69fe4a9627f71a25a7ed9b159a43267b4c8683e10d25ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8.0` - linux; amd64

```console
$ docker pull percona@sha256:8ee63a2dec0103c268ceb62ec570aabacd09f08018b9b6d27b0223748a182df8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.0 MB (383039058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5045329e3827d761c44560f86bed5bf1fdbdd6b542d9adf75016eeac8d09451d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:21 GMT
ADD file:103ed4e03109149f7699d9416e637526bc20a44d619dab1e50978e1876e22e88 in / 
# Sat, 05 Aug 2023 02:18:22 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:36:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:36:04 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV OS_VER=el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_REPO=testing
# Sat, 05 Aug 2023 02:36:07 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 05 Aug 2023 02:36:59 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:37:03 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 05 Aug 2023 02:37:03 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:37:03 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:37:03 GMT
USER mysql
# Sat, 05 Aug 2023 02:37:03 GMT
EXPOSE 3306 33060
# Sat, 05 Aug 2023 02:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f491dee0cae0e9048add4bd00a02d967b05be1bdea41cad6d85bc71a93f7379f`  
		Last Modified: Sat, 05 Aug 2023 02:19:49 GMT  
		Size: 88.0 MB (87961495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670e47ce96c1e6866a26866282b9af430aa11907c8899a0e32338456f2dc6c4`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.6 KB (1632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d615ab55531f934d4f8a7978717660b1ade4a01615d9a2fa0bec13abdb9e70b4`  
		Last Modified: Sat, 05 Aug 2023 02:43:15 GMT  
		Size: 7.3 MB (7328834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f23e970da7a2719ffbf306e0e4d99e9551684caa890df67980481309f78f92`  
		Last Modified: Sat, 05 Aug 2023 02:43:53 GMT  
		Size: 287.7 MB (287742843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d0648cdecce8ea0c3d8fcab8c6dfdb75ea6961ab9406086e2b15aa6f42a41e`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b096004652db826b7ec7391ba631b771ce45df3b85ddf22cd0dfbb743d2a03`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0-centos`

```console
$ docker pull percona@sha256:96ef2a88078bf7466e69fe4a9627f71a25a7ed9b159a43267b4c8683e10d25ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8.0-centos` - linux; amd64

```console
$ docker pull percona@sha256:8ee63a2dec0103c268ceb62ec570aabacd09f08018b9b6d27b0223748a182df8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.0 MB (383039058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5045329e3827d761c44560f86bed5bf1fdbdd6b542d9adf75016eeac8d09451d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:21 GMT
ADD file:103ed4e03109149f7699d9416e637526bc20a44d619dab1e50978e1876e22e88 in / 
# Sat, 05 Aug 2023 02:18:22 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:36:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:36:04 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV OS_VER=el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_REPO=testing
# Sat, 05 Aug 2023 02:36:07 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 05 Aug 2023 02:36:59 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:37:03 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 05 Aug 2023 02:37:03 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:37:03 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:37:03 GMT
USER mysql
# Sat, 05 Aug 2023 02:37:03 GMT
EXPOSE 3306 33060
# Sat, 05 Aug 2023 02:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f491dee0cae0e9048add4bd00a02d967b05be1bdea41cad6d85bc71a93f7379f`  
		Last Modified: Sat, 05 Aug 2023 02:19:49 GMT  
		Size: 88.0 MB (87961495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670e47ce96c1e6866a26866282b9af430aa11907c8899a0e32338456f2dc6c4`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.6 KB (1632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d615ab55531f934d4f8a7978717660b1ade4a01615d9a2fa0bec13abdb9e70b4`  
		Last Modified: Sat, 05 Aug 2023 02:43:15 GMT  
		Size: 7.3 MB (7328834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f23e970da7a2719ffbf306e0e4d99e9551684caa890df67980481309f78f92`  
		Last Modified: Sat, 05 Aug 2023 02:43:53 GMT  
		Size: 287.7 MB (287742843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d0648cdecce8ea0c3d8fcab8c6dfdb75ea6961ab9406086e2b15aa6f42a41e`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b096004652db826b7ec7391ba631b771ce45df3b85ddf22cd0dfbb743d2a03`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.33-25`

```console
$ docker pull percona@sha256:96ef2a88078bf7466e69fe4a9627f71a25a7ed9b159a43267b4c8683e10d25ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8.0.33-25` - linux; amd64

```console
$ docker pull percona@sha256:8ee63a2dec0103c268ceb62ec570aabacd09f08018b9b6d27b0223748a182df8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.0 MB (383039058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5045329e3827d761c44560f86bed5bf1fdbdd6b542d9adf75016eeac8d09451d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:21 GMT
ADD file:103ed4e03109149f7699d9416e637526bc20a44d619dab1e50978e1876e22e88 in / 
# Sat, 05 Aug 2023 02:18:22 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:36:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:36:04 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV OS_VER=el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_REPO=testing
# Sat, 05 Aug 2023 02:36:07 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 05 Aug 2023 02:36:59 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:37:03 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 05 Aug 2023 02:37:03 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:37:03 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:37:03 GMT
USER mysql
# Sat, 05 Aug 2023 02:37:03 GMT
EXPOSE 3306 33060
# Sat, 05 Aug 2023 02:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f491dee0cae0e9048add4bd00a02d967b05be1bdea41cad6d85bc71a93f7379f`  
		Last Modified: Sat, 05 Aug 2023 02:19:49 GMT  
		Size: 88.0 MB (87961495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670e47ce96c1e6866a26866282b9af430aa11907c8899a0e32338456f2dc6c4`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.6 KB (1632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d615ab55531f934d4f8a7978717660b1ade4a01615d9a2fa0bec13abdb9e70b4`  
		Last Modified: Sat, 05 Aug 2023 02:43:15 GMT  
		Size: 7.3 MB (7328834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f23e970da7a2719ffbf306e0e4d99e9551684caa890df67980481309f78f92`  
		Last Modified: Sat, 05 Aug 2023 02:43:53 GMT  
		Size: 287.7 MB (287742843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d0648cdecce8ea0c3d8fcab8c6dfdb75ea6961ab9406086e2b15aa6f42a41e`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b096004652db826b7ec7391ba631b771ce45df3b85ddf22cd0dfbb743d2a03`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.33-25-centos`

```console
$ docker pull percona@sha256:96ef2a88078bf7466e69fe4a9627f71a25a7ed9b159a43267b4c8683e10d25ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8.0.33-25-centos` - linux; amd64

```console
$ docker pull percona@sha256:8ee63a2dec0103c268ceb62ec570aabacd09f08018b9b6d27b0223748a182df8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.0 MB (383039058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5045329e3827d761c44560f86bed5bf1fdbdd6b542d9adf75016eeac8d09451d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:21 GMT
ADD file:103ed4e03109149f7699d9416e637526bc20a44d619dab1e50978e1876e22e88 in / 
# Sat, 05 Aug 2023 02:18:22 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:36:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:36:04 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV OS_VER=el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_REPO=testing
# Sat, 05 Aug 2023 02:36:07 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 05 Aug 2023 02:36:59 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:37:03 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 05 Aug 2023 02:37:03 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:37:03 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:37:03 GMT
USER mysql
# Sat, 05 Aug 2023 02:37:03 GMT
EXPOSE 3306 33060
# Sat, 05 Aug 2023 02:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f491dee0cae0e9048add4bd00a02d967b05be1bdea41cad6d85bc71a93f7379f`  
		Last Modified: Sat, 05 Aug 2023 02:19:49 GMT  
		Size: 88.0 MB (87961495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670e47ce96c1e6866a26866282b9af430aa11907c8899a0e32338456f2dc6c4`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.6 KB (1632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d615ab55531f934d4f8a7978717660b1ade4a01615d9a2fa0bec13abdb9e70b4`  
		Last Modified: Sat, 05 Aug 2023 02:43:15 GMT  
		Size: 7.3 MB (7328834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f23e970da7a2719ffbf306e0e4d99e9551684caa890df67980481309f78f92`  
		Last Modified: Sat, 05 Aug 2023 02:43:53 GMT  
		Size: 287.7 MB (287742843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d0648cdecce8ea0c3d8fcab8c6dfdb75ea6961ab9406086e2b15aa6f42a41e`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b096004652db826b7ec7391ba631b771ce45df3b85ddf22cd0dfbb743d2a03`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:centos`

```console
$ docker pull percona@sha256:917e909741490967eb1dcddaf4ae532591553af1d9d899f838a13a2451e13104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:centos` - linux; amd64

```console
$ docker pull percona@sha256:7a227334ec43908ce406b2008cd5bd0ac404a89943e79b5f18857fb19e22c0e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.0 MB (419019729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600b9ba8d1577af9fa44e0765ca47fc45ffb6b41b52198fbeaa782fd841d9ea2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:37:14 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:37:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 05 Aug 2023 02:37:48 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 05 Aug 2023 02:37:48 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:37:48 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 05 Aug 2023 02:38:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:38:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 05 Aug 2023 02:38:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:38:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:38:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:38:26 GMT
USER mysql
# Sat, 05 Aug 2023 02:38:26 GMT
EXPOSE 3306
# Sat, 05 Aug 2023 02:38:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c336c62cff80b45ee85a0fa59f487562fb97a60b6a378466408a5339184788`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246478ec69e60b803e615bd1822bbc541da434fc39e827e4b729e66087d6d4f2`  
		Last Modified: Sat, 05 Aug 2023 02:44:27 GMT  
		Size: 192.6 MB (192560961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128fd83d981eaadfa0f79125eda4a3644b513d6b30fb18221054437407088974`  
		Last Modified: Sat, 05 Aug 2023 02:44:33 GMT  
		Size: 137.5 MB (137531359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e43ed1f0be0a87de5bf18ece0d8c06c0102e487c244cd8a5a2a0fd21e7274a8`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b658c06491156c996cd6d918fb83f6d134df292838612393a3333d154d653d5`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5`

```console
$ docker pull percona@sha256:917e909741490967eb1dcddaf4ae532591553af1d9d899f838a13a2451e13104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-5` - linux; amd64

```console
$ docker pull percona@sha256:7a227334ec43908ce406b2008cd5bd0ac404a89943e79b5f18857fb19e22c0e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.0 MB (419019729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600b9ba8d1577af9fa44e0765ca47fc45ffb6b41b52198fbeaa782fd841d9ea2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:37:14 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:37:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 05 Aug 2023 02:37:48 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 05 Aug 2023 02:37:48 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:37:48 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 05 Aug 2023 02:38:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:38:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 05 Aug 2023 02:38:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:38:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:38:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:38:26 GMT
USER mysql
# Sat, 05 Aug 2023 02:38:26 GMT
EXPOSE 3306
# Sat, 05 Aug 2023 02:38:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c336c62cff80b45ee85a0fa59f487562fb97a60b6a378466408a5339184788`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246478ec69e60b803e615bd1822bbc541da434fc39e827e4b729e66087d6d4f2`  
		Last Modified: Sat, 05 Aug 2023 02:44:27 GMT  
		Size: 192.6 MB (192560961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128fd83d981eaadfa0f79125eda4a3644b513d6b30fb18221054437407088974`  
		Last Modified: Sat, 05 Aug 2023 02:44:33 GMT  
		Size: 137.5 MB (137531359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e43ed1f0be0a87de5bf18ece0d8c06c0102e487c244cd8a5a2a0fd21e7274a8`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b658c06491156c996cd6d918fb83f6d134df292838612393a3333d154d653d5`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
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
$ docker pull percona@sha256:917e909741490967eb1dcddaf4ae532591553af1d9d899f838a13a2451e13104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-5.7` - linux; amd64

```console
$ docker pull percona@sha256:7a227334ec43908ce406b2008cd5bd0ac404a89943e79b5f18857fb19e22c0e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.0 MB (419019729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600b9ba8d1577af9fa44e0765ca47fc45ffb6b41b52198fbeaa782fd841d9ea2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:37:14 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:37:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 05 Aug 2023 02:37:48 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 05 Aug 2023 02:37:48 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:37:48 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 05 Aug 2023 02:38:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:38:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 05 Aug 2023 02:38:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:38:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:38:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:38:26 GMT
USER mysql
# Sat, 05 Aug 2023 02:38:26 GMT
EXPOSE 3306
# Sat, 05 Aug 2023 02:38:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c336c62cff80b45ee85a0fa59f487562fb97a60b6a378466408a5339184788`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246478ec69e60b803e615bd1822bbc541da434fc39e827e4b729e66087d6d4f2`  
		Last Modified: Sat, 05 Aug 2023 02:44:27 GMT  
		Size: 192.6 MB (192560961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128fd83d981eaadfa0f79125eda4a3644b513d6b30fb18221054437407088974`  
		Last Modified: Sat, 05 Aug 2023 02:44:33 GMT  
		Size: 137.5 MB (137531359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e43ed1f0be0a87de5bf18ece0d8c06c0102e487c244cd8a5a2a0fd21e7274a8`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b658c06491156c996cd6d918fb83f6d134df292838612393a3333d154d653d5`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.7.39`

```console
$ docker pull percona@sha256:917e909741490967eb1dcddaf4ae532591553af1d9d899f838a13a2451e13104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-5.7.39` - linux; amd64

```console
$ docker pull percona@sha256:7a227334ec43908ce406b2008cd5bd0ac404a89943e79b5f18857fb19e22c0e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.0 MB (419019729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600b9ba8d1577af9fa44e0765ca47fc45ffb6b41b52198fbeaa782fd841d9ea2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:37:14 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:37:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 05 Aug 2023 02:37:48 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 05 Aug 2023 02:37:48 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:37:48 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 05 Aug 2023 02:38:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:38:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 05 Aug 2023 02:38:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:38:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:38:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:38:26 GMT
USER mysql
# Sat, 05 Aug 2023 02:38:26 GMT
EXPOSE 3306
# Sat, 05 Aug 2023 02:38:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c336c62cff80b45ee85a0fa59f487562fb97a60b6a378466408a5339184788`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246478ec69e60b803e615bd1822bbc541da434fc39e827e4b729e66087d6d4f2`  
		Last Modified: Sat, 05 Aug 2023 02:44:27 GMT  
		Size: 192.6 MB (192560961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128fd83d981eaadfa0f79125eda4a3644b513d6b30fb18221054437407088974`  
		Last Modified: Sat, 05 Aug 2023 02:44:33 GMT  
		Size: 137.5 MB (137531359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e43ed1f0be0a87de5bf18ece0d8c06c0102e487c244cd8a5a2a0fd21e7274a8`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b658c06491156c996cd6d918fb83f6d134df292838612393a3333d154d653d5`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8`

```console
$ docker pull percona@sha256:96ef2a88078bf7466e69fe4a9627f71a25a7ed9b159a43267b4c8683e10d25ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-8` - linux; amd64

```console
$ docker pull percona@sha256:8ee63a2dec0103c268ceb62ec570aabacd09f08018b9b6d27b0223748a182df8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.0 MB (383039058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5045329e3827d761c44560f86bed5bf1fdbdd6b542d9adf75016eeac8d09451d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:21 GMT
ADD file:103ed4e03109149f7699d9416e637526bc20a44d619dab1e50978e1876e22e88 in / 
# Sat, 05 Aug 2023 02:18:22 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:36:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:36:04 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV OS_VER=el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_REPO=testing
# Sat, 05 Aug 2023 02:36:07 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 05 Aug 2023 02:36:59 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:37:03 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 05 Aug 2023 02:37:03 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:37:03 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:37:03 GMT
USER mysql
# Sat, 05 Aug 2023 02:37:03 GMT
EXPOSE 3306 33060
# Sat, 05 Aug 2023 02:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f491dee0cae0e9048add4bd00a02d967b05be1bdea41cad6d85bc71a93f7379f`  
		Last Modified: Sat, 05 Aug 2023 02:19:49 GMT  
		Size: 88.0 MB (87961495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670e47ce96c1e6866a26866282b9af430aa11907c8899a0e32338456f2dc6c4`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.6 KB (1632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d615ab55531f934d4f8a7978717660b1ade4a01615d9a2fa0bec13abdb9e70b4`  
		Last Modified: Sat, 05 Aug 2023 02:43:15 GMT  
		Size: 7.3 MB (7328834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f23e970da7a2719ffbf306e0e4d99e9551684caa890df67980481309f78f92`  
		Last Modified: Sat, 05 Aug 2023 02:43:53 GMT  
		Size: 287.7 MB (287742843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d0648cdecce8ea0c3d8fcab8c6dfdb75ea6961ab9406086e2b15aa6f42a41e`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b096004652db826b7ec7391ba631b771ce45df3b85ddf22cd0dfbb743d2a03`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0`

```console
$ docker pull percona@sha256:96ef2a88078bf7466e69fe4a9627f71a25a7ed9b159a43267b4c8683e10d25ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-8.0` - linux; amd64

```console
$ docker pull percona@sha256:8ee63a2dec0103c268ceb62ec570aabacd09f08018b9b6d27b0223748a182df8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.0 MB (383039058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5045329e3827d761c44560f86bed5bf1fdbdd6b542d9adf75016eeac8d09451d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:21 GMT
ADD file:103ed4e03109149f7699d9416e637526bc20a44d619dab1e50978e1876e22e88 in / 
# Sat, 05 Aug 2023 02:18:22 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:36:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:36:04 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV OS_VER=el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_REPO=testing
# Sat, 05 Aug 2023 02:36:07 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 05 Aug 2023 02:36:59 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:37:03 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 05 Aug 2023 02:37:03 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:37:03 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:37:03 GMT
USER mysql
# Sat, 05 Aug 2023 02:37:03 GMT
EXPOSE 3306 33060
# Sat, 05 Aug 2023 02:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f491dee0cae0e9048add4bd00a02d967b05be1bdea41cad6d85bc71a93f7379f`  
		Last Modified: Sat, 05 Aug 2023 02:19:49 GMT  
		Size: 88.0 MB (87961495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670e47ce96c1e6866a26866282b9af430aa11907c8899a0e32338456f2dc6c4`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.6 KB (1632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d615ab55531f934d4f8a7978717660b1ade4a01615d9a2fa0bec13abdb9e70b4`  
		Last Modified: Sat, 05 Aug 2023 02:43:15 GMT  
		Size: 7.3 MB (7328834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f23e970da7a2719ffbf306e0e4d99e9551684caa890df67980481309f78f92`  
		Last Modified: Sat, 05 Aug 2023 02:43:53 GMT  
		Size: 287.7 MB (287742843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d0648cdecce8ea0c3d8fcab8c6dfdb75ea6961ab9406086e2b15aa6f42a41e`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b096004652db826b7ec7391ba631b771ce45df3b85ddf22cd0dfbb743d2a03`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0.33-25`

```console
$ docker pull percona@sha256:96ef2a88078bf7466e69fe4a9627f71a25a7ed9b159a43267b4c8683e10d25ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-8.0.33-25` - linux; amd64

```console
$ docker pull percona@sha256:8ee63a2dec0103c268ceb62ec570aabacd09f08018b9b6d27b0223748a182df8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.0 MB (383039058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5045329e3827d761c44560f86bed5bf1fdbdd6b542d9adf75016eeac8d09451d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:21 GMT
ADD file:103ed4e03109149f7699d9416e637526bc20a44d619dab1e50978e1876e22e88 in / 
# Sat, 05 Aug 2023 02:18:22 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:36:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:36:04 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_VERSION=8.0.33-25.1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Sat, 05 Aug 2023 02:36:04 GMT
ENV OS_VER=el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Sat, 05 Aug 2023 02:36:04 GMT
ENV PS_REPO=testing
# Sat, 05 Aug 2023 02:36:07 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Sat, 05 Aug 2023 02:36:59 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:37:03 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Sat, 05 Aug 2023 02:37:03 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:37:03 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:37:03 GMT
USER mysql
# Sat, 05 Aug 2023 02:37:03 GMT
EXPOSE 3306 33060
# Sat, 05 Aug 2023 02:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f491dee0cae0e9048add4bd00a02d967b05be1bdea41cad6d85bc71a93f7379f`  
		Last Modified: Sat, 05 Aug 2023 02:19:49 GMT  
		Size: 88.0 MB (87961495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670e47ce96c1e6866a26866282b9af430aa11907c8899a0e32338456f2dc6c4`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.6 KB (1632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d615ab55531f934d4f8a7978717660b1ade4a01615d9a2fa0bec13abdb9e70b4`  
		Last Modified: Sat, 05 Aug 2023 02:43:15 GMT  
		Size: 7.3 MB (7328834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f23e970da7a2719ffbf306e0e4d99e9551684caa890df67980481309f78f92`  
		Last Modified: Sat, 05 Aug 2023 02:43:53 GMT  
		Size: 287.7 MB (287742843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d0648cdecce8ea0c3d8fcab8c6dfdb75ea6961ab9406086e2b15aa6f42a41e`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b096004652db826b7ec7391ba631b771ce45df3b85ddf22cd0dfbb743d2a03`  
		Last Modified: Sat, 05 Aug 2023 02:43:14 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:834ef5c7b8e6fef0ea9cd0b0ccb2dda695918297b42c0d5e81f8ccaad7b3e10f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:496b74852365c466f12578e70370988dea33801c613ab6c75cde93b41a9a75d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.1 MB (219057763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfbe111938d4a1343f641676a7e50c2f8b4867184f87f8b10b54dc3d28f8c47b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:41:58 GMT
ENV PSMDB_VERSION=4.2.24-24
# Sat, 05 Aug 2023 02:41:58 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:41:58 GMT
ENV FULL_PERCONA_VERSION=4.2.24-24.el8
# Sat, 05 Aug 2023 02:41:58 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 05 Aug 2023 02:41:58 GMT
ENV PSMDB_REPO=release
# Sat, 05 Aug 2023 02:42:01 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 05 Aug 2023 02:42:47 GMT
RUN set -ex;     percona-release enable psmdb-42 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 05 Aug 2023 02:42:48 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 05 Aug 2023 02:42:48 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 05 Aug 2023 02:42:49 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 05 Aug 2023 02:42:49 GMT
ENV GOSU_VERSION=1.11
# Sat, 05 Aug 2023 02:42:51 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 05 Aug 2023 02:42:53 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -;     rm -f /tmp/SHA256SUMS;     chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 05 Aug 2023 02:42:53 GMT
VOLUME [/data/db]
# Sat, 05 Aug 2023 02:42:53 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Sat, 05 Aug 2023 02:42:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Aug 2023 02:42:54 GMT
EXPOSE 27017
# Sat, 05 Aug 2023 02:42:54 GMT
USER 1001
# Sat, 05 Aug 2023 02:42:54 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fe55b577f35b2e3214ee0c80e3f125b04361c7d422e7b11f2f6dc89d054698`  
		Last Modified: Sat, 05 Aug 2023 02:46:32 GMT  
		Size: 3.8 MB (3790421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d9c907441dd2fb44ee227e9753545c0e3a866f19d1671ff795788b5ddae9f9`  
		Last Modified: Sat, 05 Aug 2023 02:46:45 GMT  
		Size: 117.3 MB (117258681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10196e7d599fb38dfdb161d198de299fef4d4cec325ac2a90d5e46b82ece49f`  
		Last Modified: Sat, 05 Aug 2023 02:46:31 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f6d3f27ad1fbda0840cb7ca477037b6c08f275a8b36c8eebfa7892e9df773a`  
		Last Modified: Sat, 05 Aug 2023 02:46:29 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81ed758e7227d1f3d895ddef89608f240c22b11b01b15211eab0ca019bb46ef`  
		Last Modified: Sat, 05 Aug 2023 02:46:29 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6255dcc1a76890d649287ed30da091761e6c26d84ffc1752a418b4f2c62d4d2a`  
		Last Modified: Sat, 05 Aug 2023 02:46:29 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f15f8563fd5840d1a3eee6822ef042c41a093295cf0b2ca7cf0fb4f69012078`  
		Last Modified: Sat, 05 Aug 2023 02:46:30 GMT  
		Size: 8.2 MB (8151460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6162883bee527ee5da4cf6176e0fad4baf25fb2eeafe32028814241ac258e0e6`  
		Last Modified: Sat, 05 Aug 2023 02:46:29 GMT  
		Size: 4.6 KB (4555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2.24`

```console
$ docker pull percona@sha256:834ef5c7b8e6fef0ea9cd0b0ccb2dda695918297b42c0d5e81f8ccaad7b3e10f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2.24` - linux; amd64

```console
$ docker pull percona@sha256:496b74852365c466f12578e70370988dea33801c613ab6c75cde93b41a9a75d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.1 MB (219057763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfbe111938d4a1343f641676a7e50c2f8b4867184f87f8b10b54dc3d28f8c47b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:41:58 GMT
ENV PSMDB_VERSION=4.2.24-24
# Sat, 05 Aug 2023 02:41:58 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:41:58 GMT
ENV FULL_PERCONA_VERSION=4.2.24-24.el8
# Sat, 05 Aug 2023 02:41:58 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 05 Aug 2023 02:41:58 GMT
ENV PSMDB_REPO=release
# Sat, 05 Aug 2023 02:42:01 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 05 Aug 2023 02:42:47 GMT
RUN set -ex;     percona-release enable psmdb-42 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 05 Aug 2023 02:42:48 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 05 Aug 2023 02:42:48 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 05 Aug 2023 02:42:49 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 05 Aug 2023 02:42:49 GMT
ENV GOSU_VERSION=1.11
# Sat, 05 Aug 2023 02:42:51 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 05 Aug 2023 02:42:53 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -;     rm -f /tmp/SHA256SUMS;     chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 05 Aug 2023 02:42:53 GMT
VOLUME [/data/db]
# Sat, 05 Aug 2023 02:42:53 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Sat, 05 Aug 2023 02:42:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Aug 2023 02:42:54 GMT
EXPOSE 27017
# Sat, 05 Aug 2023 02:42:54 GMT
USER 1001
# Sat, 05 Aug 2023 02:42:54 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fe55b577f35b2e3214ee0c80e3f125b04361c7d422e7b11f2f6dc89d054698`  
		Last Modified: Sat, 05 Aug 2023 02:46:32 GMT  
		Size: 3.8 MB (3790421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d9c907441dd2fb44ee227e9753545c0e3a866f19d1671ff795788b5ddae9f9`  
		Last Modified: Sat, 05 Aug 2023 02:46:45 GMT  
		Size: 117.3 MB (117258681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10196e7d599fb38dfdb161d198de299fef4d4cec325ac2a90d5e46b82ece49f`  
		Last Modified: Sat, 05 Aug 2023 02:46:31 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f6d3f27ad1fbda0840cb7ca477037b6c08f275a8b36c8eebfa7892e9df773a`  
		Last Modified: Sat, 05 Aug 2023 02:46:29 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81ed758e7227d1f3d895ddef89608f240c22b11b01b15211eab0ca019bb46ef`  
		Last Modified: Sat, 05 Aug 2023 02:46:29 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6255dcc1a76890d649287ed30da091761e6c26d84ffc1752a418b4f2c62d4d2a`  
		Last Modified: Sat, 05 Aug 2023 02:46:29 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f15f8563fd5840d1a3eee6822ef042c41a093295cf0b2ca7cf0fb4f69012078`  
		Last Modified: Sat, 05 Aug 2023 02:46:30 GMT  
		Size: 8.2 MB (8151460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6162883bee527ee5da4cf6176e0fad4baf25fb2eeafe32028814241ac258e0e6`  
		Last Modified: Sat, 05 Aug 2023 02:46:29 GMT  
		Size: 4.6 KB (4555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.4`

```console
$ docker pull percona@sha256:c239705bfb45d3d82192f25b0fc26a8852328d0582abe475e5a3448e30174aae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4` - linux; amd64

```console
$ docker pull percona@sha256:7a31f81f96296323ff033ba015cbdd8ab5654d604712a7c02939582861fb0d22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.6 MB (237595900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1977141cc927400819649d21421f58fa3c0b84847ac1d1118d5a905a128e33f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:38:43 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 05 Aug 2023 02:40:59 GMT
ENV PSMDB_VERSION=4.4.22-21
# Sat, 05 Aug 2023 02:40:59 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:40:59 GMT
ENV FULL_PERCONA_VERSION=4.4.22-21.el8
# Sat, 05 Aug 2023 02:40:59 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 05 Aug 2023 02:41:00 GMT
ENV PSMDB_REPO=release
# Sat, 05 Aug 2023 02:41:48 GMT
RUN set -ex;     percona-release enable psmdb-44 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 05 Aug 2023 02:41:49 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 05 Aug 2023 02:41:49 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 05 Aug 2023 02:41:49 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 05 Aug 2023 02:41:49 GMT
ENV GOSU_VERSION=1.11
# Sat, 05 Aug 2023 02:41:52 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 05 Aug 2023 02:41:54 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 05 Aug 2023 02:41:54 GMT
VOLUME [/data/db]
# Sat, 05 Aug 2023 02:41:54 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 05 Aug 2023 02:41:54 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Sat, 05 Aug 2023 02:41:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Aug 2023 02:41:54 GMT
EXPOSE 27017
# Sat, 05 Aug 2023 02:41:55 GMT
USER 1001
# Sat, 05 Aug 2023 02:41:55 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57009482fd55816f25227289cfc8b0a086fd3aecb1118cd78296a2812242a3ca`  
		Last Modified: Sat, 05 Aug 2023 02:45:04 GMT  
		Size: 3.8 MB (3790449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95079a3fccb2584b90e99d03c94ff892f7fa90ce47f053bf752dec80125a6fd0`  
		Last Modified: Sat, 05 Aug 2023 02:46:20 GMT  
		Size: 135.8 MB (135797189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c94088d172c64026a14b18b1be0de57bfe497ddebb4788b8d39c3e729e14085`  
		Last Modified: Sat, 05 Aug 2023 02:46:02 GMT  
		Size: 1.7 KB (1670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e0c1586df59510cd3716c2a61fed1258eccba381e591b58942cbddb577af77`  
		Last Modified: Sat, 05 Aug 2023 02:46:02 GMT  
		Size: 4.1 KB (4098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec741bb4f4c876f1d8340ce35a258a1d92fc80b7e4517be721f6f12d54d1484`  
		Last Modified: Sat, 05 Aug 2023 02:46:00 GMT  
		Size: 10.6 KB (10572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a59c6d7e5d11dc766bd0bb9e9e7e45cbf5ab33c25d1e5e679a301ad98fd6315`  
		Last Modified: Sat, 05 Aug 2023 02:46:00 GMT  
		Size: 914.5 KB (914541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e81ec4631c520e4e2de7bc046ac14a05fa9020321bea3dc2e73712df76a93cb`  
		Last Modified: Sat, 05 Aug 2023 02:46:01 GMT  
		Size: 8.1 MB (8137881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4442fac3f7f7776ebd35c06e49abd3e92c873983b0f1beedbc294b8076a69436`  
		Last Modified: Sat, 05 Aug 2023 02:46:00 GMT  
		Size: 13.2 KB (13203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe57b4cc3ec75b7e93ee684396b84fae979b66f5d974eef48a3808f41fed50ab`  
		Last Modified: Sat, 05 Aug 2023 02:46:00 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.4.22`

```console
$ docker pull percona@sha256:c239705bfb45d3d82192f25b0fc26a8852328d0582abe475e5a3448e30174aae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4.22` - linux; amd64

```console
$ docker pull percona@sha256:7a31f81f96296323ff033ba015cbdd8ab5654d604712a7c02939582861fb0d22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.6 MB (237595900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1977141cc927400819649d21421f58fa3c0b84847ac1d1118d5a905a128e33f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:38:43 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 05 Aug 2023 02:40:59 GMT
ENV PSMDB_VERSION=4.4.22-21
# Sat, 05 Aug 2023 02:40:59 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:40:59 GMT
ENV FULL_PERCONA_VERSION=4.4.22-21.el8
# Sat, 05 Aug 2023 02:40:59 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 05 Aug 2023 02:41:00 GMT
ENV PSMDB_REPO=release
# Sat, 05 Aug 2023 02:41:48 GMT
RUN set -ex;     percona-release enable psmdb-44 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 05 Aug 2023 02:41:49 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 05 Aug 2023 02:41:49 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 05 Aug 2023 02:41:49 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 05 Aug 2023 02:41:49 GMT
ENV GOSU_VERSION=1.11
# Sat, 05 Aug 2023 02:41:52 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 05 Aug 2023 02:41:54 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 05 Aug 2023 02:41:54 GMT
VOLUME [/data/db]
# Sat, 05 Aug 2023 02:41:54 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 05 Aug 2023 02:41:54 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Sat, 05 Aug 2023 02:41:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Aug 2023 02:41:54 GMT
EXPOSE 27017
# Sat, 05 Aug 2023 02:41:55 GMT
USER 1001
# Sat, 05 Aug 2023 02:41:55 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57009482fd55816f25227289cfc8b0a086fd3aecb1118cd78296a2812242a3ca`  
		Last Modified: Sat, 05 Aug 2023 02:45:04 GMT  
		Size: 3.8 MB (3790449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95079a3fccb2584b90e99d03c94ff892f7fa90ce47f053bf752dec80125a6fd0`  
		Last Modified: Sat, 05 Aug 2023 02:46:20 GMT  
		Size: 135.8 MB (135797189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c94088d172c64026a14b18b1be0de57bfe497ddebb4788b8d39c3e729e14085`  
		Last Modified: Sat, 05 Aug 2023 02:46:02 GMT  
		Size: 1.7 KB (1670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e0c1586df59510cd3716c2a61fed1258eccba381e591b58942cbddb577af77`  
		Last Modified: Sat, 05 Aug 2023 02:46:02 GMT  
		Size: 4.1 KB (4098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec741bb4f4c876f1d8340ce35a258a1d92fc80b7e4517be721f6f12d54d1484`  
		Last Modified: Sat, 05 Aug 2023 02:46:00 GMT  
		Size: 10.6 KB (10572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a59c6d7e5d11dc766bd0bb9e9e7e45cbf5ab33c25d1e5e679a301ad98fd6315`  
		Last Modified: Sat, 05 Aug 2023 02:46:00 GMT  
		Size: 914.5 KB (914541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e81ec4631c520e4e2de7bc046ac14a05fa9020321bea3dc2e73712df76a93cb`  
		Last Modified: Sat, 05 Aug 2023 02:46:01 GMT  
		Size: 8.1 MB (8137881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4442fac3f7f7776ebd35c06e49abd3e92c873983b0f1beedbc294b8076a69436`  
		Last Modified: Sat, 05 Aug 2023 02:46:00 GMT  
		Size: 13.2 KB (13203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe57b4cc3ec75b7e93ee684396b84fae979b66f5d974eef48a3808f41fed50ab`  
		Last Modified: Sat, 05 Aug 2023 02:46:00 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-5.0`

```console
$ docker pull percona@sha256:eb5079ffe9e7a01187687e1a2ec18a07b814d583693885ac41bcb5353cb6584e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0` - linux; amd64

```console
$ docker pull percona@sha256:a157dce551d689ecaab2c3126142ef4e1dbca79e08624646cc08dd8d8edd8498
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.2 MB (250204467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61397b95e994a12ab05f0bb6e007a48cb82dbafe4fca0ab2589258bc5f809d1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:38:43 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 05 Aug 2023 02:39:49 GMT
ENV PSMDB_VERSION=5.0.18-15
# Sat, 05 Aug 2023 02:39:49 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:39:49 GMT
ENV FULL_PERCONA_VERSION=5.0.18-15.el8
# Sat, 05 Aug 2023 02:39:49 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 05 Aug 2023 02:39:49 GMT
ENV PSMDB_REPO=release
# Sat, 05 Aug 2023 02:40:38 GMT
RUN set -ex;     percona-release enable psmdb-50 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 05 Aug 2023 02:40:39 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 05 Aug 2023 02:40:39 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 05 Aug 2023 02:40:39 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 05 Aug 2023 02:40:40 GMT
ENV GOSU_VERSION=1.11
# Sat, 05 Aug 2023 02:40:43 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 05 Aug 2023 02:40:45 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 05 Aug 2023 02:40:45 GMT
VOLUME [/data/db]
# Sat, 05 Aug 2023 02:40:46 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 05 Aug 2023 02:40:46 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Sat, 05 Aug 2023 02:40:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Aug 2023 02:40:46 GMT
EXPOSE 27017
# Sat, 05 Aug 2023 02:40:46 GMT
USER 1001
# Sat, 05 Aug 2023 02:40:46 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57009482fd55816f25227289cfc8b0a086fd3aecb1118cd78296a2812242a3ca`  
		Last Modified: Sat, 05 Aug 2023 02:45:04 GMT  
		Size: 3.8 MB (3790449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd92c276efa8e5b68b5b7fcecf6b58f4b7a20a6776d915b86975073cecb2822`  
		Last Modified: Sat, 05 Aug 2023 02:45:50 GMT  
		Size: 148.4 MB (148405720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f461e81d9f3700256e8b65d37bee411185b2ca5a1b3feff8a1d9b779c1e75b`  
		Last Modified: Sat, 05 Aug 2023 02:45:33 GMT  
		Size: 1.7 KB (1673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070f0d0b1c680ccf52cd9079aa3802ea0f39a5c34463143461c913bae028c3f2`  
		Last Modified: Sat, 05 Aug 2023 02:45:33 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e69f8b607deab0b234a92af126c63835c3b61f0d41f395e19623238991dd84`  
		Last Modified: Sat, 05 Aug 2023 02:45:31 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1cb4bea1eae352c8e86f6630ce34409b909aa021fe6cfd4b7c92e15297e7813`  
		Last Modified: Sat, 05 Aug 2023 02:45:31 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b92eb86ae980fb67b38d8230bdeeee45effe10199bab48b8d6fa73c8b788b`  
		Last Modified: Sat, 05 Aug 2023 02:45:33 GMT  
		Size: 8.1 MB (8137890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93c8d9477c278503c5bb8709cde113949dd5934e286b7bdc5a2d8f80f85ea09`  
		Last Modified: Sat, 05 Aug 2023 02:45:31 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18bd184a5acad57f4c6fba34f6871f9eeb6778de66a16d70cbd08c6e84da28b`  
		Last Modified: Sat, 05 Aug 2023 02:45:31 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-5.0.18`

```console
$ docker pull percona@sha256:eb5079ffe9e7a01187687e1a2ec18a07b814d583693885ac41bcb5353cb6584e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0.18` - linux; amd64

```console
$ docker pull percona@sha256:a157dce551d689ecaab2c3126142ef4e1dbca79e08624646cc08dd8d8edd8498
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.2 MB (250204467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61397b95e994a12ab05f0bb6e007a48cb82dbafe4fca0ab2589258bc5f809d1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:38:43 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 05 Aug 2023 02:39:49 GMT
ENV PSMDB_VERSION=5.0.18-15
# Sat, 05 Aug 2023 02:39:49 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:39:49 GMT
ENV FULL_PERCONA_VERSION=5.0.18-15.el8
# Sat, 05 Aug 2023 02:39:49 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 05 Aug 2023 02:39:49 GMT
ENV PSMDB_REPO=release
# Sat, 05 Aug 2023 02:40:38 GMT
RUN set -ex;     percona-release enable psmdb-50 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 05 Aug 2023 02:40:39 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 05 Aug 2023 02:40:39 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 05 Aug 2023 02:40:39 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 05 Aug 2023 02:40:40 GMT
ENV GOSU_VERSION=1.11
# Sat, 05 Aug 2023 02:40:43 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 05 Aug 2023 02:40:45 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 05 Aug 2023 02:40:45 GMT
VOLUME [/data/db]
# Sat, 05 Aug 2023 02:40:46 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 05 Aug 2023 02:40:46 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Sat, 05 Aug 2023 02:40:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Aug 2023 02:40:46 GMT
EXPOSE 27017
# Sat, 05 Aug 2023 02:40:46 GMT
USER 1001
# Sat, 05 Aug 2023 02:40:46 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57009482fd55816f25227289cfc8b0a086fd3aecb1118cd78296a2812242a3ca`  
		Last Modified: Sat, 05 Aug 2023 02:45:04 GMT  
		Size: 3.8 MB (3790449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd92c276efa8e5b68b5b7fcecf6b58f4b7a20a6776d915b86975073cecb2822`  
		Last Modified: Sat, 05 Aug 2023 02:45:50 GMT  
		Size: 148.4 MB (148405720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f461e81d9f3700256e8b65d37bee411185b2ca5a1b3feff8a1d9b779c1e75b`  
		Last Modified: Sat, 05 Aug 2023 02:45:33 GMT  
		Size: 1.7 KB (1673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070f0d0b1c680ccf52cd9079aa3802ea0f39a5c34463143461c913bae028c3f2`  
		Last Modified: Sat, 05 Aug 2023 02:45:33 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e69f8b607deab0b234a92af126c63835c3b61f0d41f395e19623238991dd84`  
		Last Modified: Sat, 05 Aug 2023 02:45:31 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1cb4bea1eae352c8e86f6630ce34409b909aa021fe6cfd4b7c92e15297e7813`  
		Last Modified: Sat, 05 Aug 2023 02:45:31 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b92eb86ae980fb67b38d8230bdeeee45effe10199bab48b8d6fa73c8b788b`  
		Last Modified: Sat, 05 Aug 2023 02:45:33 GMT  
		Size: 8.1 MB (8137890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93c8d9477c278503c5bb8709cde113949dd5934e286b7bdc5a2d8f80f85ea09`  
		Last Modified: Sat, 05 Aug 2023 02:45:31 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18bd184a5acad57f4c6fba34f6871f9eeb6778de66a16d70cbd08c6e84da28b`  
		Last Modified: Sat, 05 Aug 2023 02:45:31 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-6.0`

```console
$ docker pull percona@sha256:e441d67543960d0bc89653ed0f6b862308e5630f4afa448e57208e2aba0dd571
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-6.0` - linux; amd64

```console
$ docker pull percona@sha256:9171645f625909cb21cdfe4f9a82c764db0c56a5e867d35124b71b4bd4030c79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.3 MB (273255826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c80a33a0620016638ccbbf4d6502980a515ebad6e92c28160fbc24b7e58f331`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:38:43 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 05 Aug 2023 02:38:43 GMT
ENV PSMDB_VERSION=6.0.6-5
# Sat, 05 Aug 2023 02:38:43 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:38:43 GMT
ENV FULL_PERCONA_VERSION=6.0.6-5.el8
# Sat, 05 Aug 2023 02:38:43 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 05 Aug 2023 02:38:44 GMT
ENV PSMDB_REPO=release
# Sat, 05 Aug 2023 02:39:35 GMT
RUN set -ex;     percona-release enable psmdb-60 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         percona-mongodb-mongosh         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-60/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 05 Aug 2023 02:39:36 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 05 Aug 2023 02:39:36 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 05 Aug 2023 02:39:37 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 05 Aug 2023 02:39:37 GMT
ENV GOSU_VERSION=1.11
# Sat, 05 Aug 2023 02:39:40 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 05 Aug 2023 02:39:43 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 05 Aug 2023 02:39:43 GMT
VOLUME [/data/db]
# Sat, 05 Aug 2023 02:39:44 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 05 Aug 2023 02:39:44 GMT
COPY file:7ab35f422fd362616b84e1dc71329cc9be05b7f834182c48bf98ceb92ee28956 in /entrypoint.sh 
# Sat, 05 Aug 2023 02:39:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Aug 2023 02:39:44 GMT
EXPOSE 27017
# Sat, 05 Aug 2023 02:39:44 GMT
USER 1001
# Sat, 05 Aug 2023 02:39:44 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57009482fd55816f25227289cfc8b0a086fd3aecb1118cd78296a2812242a3ca`  
		Last Modified: Sat, 05 Aug 2023 02:45:04 GMT  
		Size: 3.8 MB (3790449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aada92cc74feabd7f036fa62e92d7486494fd7eeb32169853eac63d89d6cc335`  
		Last Modified: Sat, 05 Aug 2023 02:45:22 GMT  
		Size: 171.5 MB (171457076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04091c0a0ca708cb0ba5127fd18ab25fbad57b6735a713e8888add8aff01b73`  
		Last Modified: Sat, 05 Aug 2023 02:45:03 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f53c502f4e69265cde9d852c4c107370c73890d5f6c4e04e68775e54764320`  
		Last Modified: Sat, 05 Aug 2023 02:45:02 GMT  
		Size: 4.1 KB (4101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d680fb10eb2b8edb9087f6b54e0cbda82b44c99d7e5b8c96af70ca5ac109af65`  
		Last Modified: Sat, 05 Aug 2023 02:45:00 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1d81e265209e98a17d5a2bd518098eafed7b24a37e0db6200be56cdcec6eef`  
		Last Modified: Sat, 05 Aug 2023 02:45:01 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b298a09d7027f47a37aae68afd38aab9540bc2730aff175879fcb54455099146`  
		Last Modified: Sat, 05 Aug 2023 02:45:02 GMT  
		Size: 8.1 MB (8137886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5d18c9bb10f213c9777681b384dc42ef80aaa2001307b3ec9fff2a7362b675`  
		Last Modified: Sat, 05 Aug 2023 02:45:00 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fde879b52bc4bb68759c5dfe55bc96ed550e74f89b87a50e51c12effa26c787`  
		Last Modified: Sat, 05 Aug 2023 02:45:00 GMT  
		Size: 4.6 KB (4567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-6.0.6`

```console
$ docker pull percona@sha256:e441d67543960d0bc89653ed0f6b862308e5630f4afa448e57208e2aba0dd571
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-6.0.6` - linux; amd64

```console
$ docker pull percona@sha256:9171645f625909cb21cdfe4f9a82c764db0c56a5e867d35124b71b4bd4030c79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.3 MB (273255826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c80a33a0620016638ccbbf4d6502980a515ebad6e92c28160fbc24b7e58f331`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:38:43 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 05 Aug 2023 02:38:43 GMT
ENV PSMDB_VERSION=6.0.6-5
# Sat, 05 Aug 2023 02:38:43 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:38:43 GMT
ENV FULL_PERCONA_VERSION=6.0.6-5.el8
# Sat, 05 Aug 2023 02:38:43 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 05 Aug 2023 02:38:44 GMT
ENV PSMDB_REPO=release
# Sat, 05 Aug 2023 02:39:35 GMT
RUN set -ex;     percona-release enable psmdb-60 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         percona-mongodb-mongosh         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-60/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 05 Aug 2023 02:39:36 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 05 Aug 2023 02:39:36 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 05 Aug 2023 02:39:37 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 05 Aug 2023 02:39:37 GMT
ENV GOSU_VERSION=1.11
# Sat, 05 Aug 2023 02:39:40 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 05 Aug 2023 02:39:43 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 05 Aug 2023 02:39:43 GMT
VOLUME [/data/db]
# Sat, 05 Aug 2023 02:39:44 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 05 Aug 2023 02:39:44 GMT
COPY file:7ab35f422fd362616b84e1dc71329cc9be05b7f834182c48bf98ceb92ee28956 in /entrypoint.sh 
# Sat, 05 Aug 2023 02:39:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Aug 2023 02:39:44 GMT
EXPOSE 27017
# Sat, 05 Aug 2023 02:39:44 GMT
USER 1001
# Sat, 05 Aug 2023 02:39:44 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57009482fd55816f25227289cfc8b0a086fd3aecb1118cd78296a2812242a3ca`  
		Last Modified: Sat, 05 Aug 2023 02:45:04 GMT  
		Size: 3.8 MB (3790449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aada92cc74feabd7f036fa62e92d7486494fd7eeb32169853eac63d89d6cc335`  
		Last Modified: Sat, 05 Aug 2023 02:45:22 GMT  
		Size: 171.5 MB (171457076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04091c0a0ca708cb0ba5127fd18ab25fbad57b6735a713e8888add8aff01b73`  
		Last Modified: Sat, 05 Aug 2023 02:45:03 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f53c502f4e69265cde9d852c4c107370c73890d5f6c4e04e68775e54764320`  
		Last Modified: Sat, 05 Aug 2023 02:45:02 GMT  
		Size: 4.1 KB (4101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d680fb10eb2b8edb9087f6b54e0cbda82b44c99d7e5b8c96af70ca5ac109af65`  
		Last Modified: Sat, 05 Aug 2023 02:45:00 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1d81e265209e98a17d5a2bd518098eafed7b24a37e0db6200be56cdcec6eef`  
		Last Modified: Sat, 05 Aug 2023 02:45:01 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b298a09d7027f47a37aae68afd38aab9540bc2730aff175879fcb54455099146`  
		Last Modified: Sat, 05 Aug 2023 02:45:02 GMT  
		Size: 8.1 MB (8137886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5d18c9bb10f213c9777681b384dc42ef80aaa2001307b3ec9fff2a7362b675`  
		Last Modified: Sat, 05 Aug 2023 02:45:00 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fde879b52bc4bb68759c5dfe55bc96ed550e74f89b87a50e51c12effa26c787`  
		Last Modified: Sat, 05 Aug 2023 02:45:00 GMT  
		Size: 4.6 KB (4567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
