<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `percona`

-	[`percona:5`](#percona5)
-	[`percona:5.6`](#percona56)
-	[`percona:5.6.48`](#percona5648)
-	[`percona:5.6.48-centos`](#percona5648-centos)
-	[`percona:5.6-centos`](#percona56-centos)
-	[`percona:5.7`](#percona57)
-	[`percona:5.7.30`](#percona5730)
-	[`percona:5.7.30-centos`](#percona5730-centos)
-	[`percona:5.7-centos`](#percona57-centos)
-	[`percona:5-centos`](#percona5-centos)
-	[`percona:8`](#percona8)
-	[`percona:8.0`](#percona80)
-	[`percona:8.0.19-10`](#percona8019-10)
-	[`percona:8.0.19-10-centos`](#percona8019-10-centos)
-	[`percona:8.0-centos`](#percona80-centos)
-	[`percona:8-centos`](#percona8-centos)
-	[`percona:centos`](#perconacentos)
-	[`percona:latest`](#perconalatest)
-	[`percona:ps-5`](#perconaps-5)
-	[`percona:ps-5.6`](#perconaps-56)
-	[`percona:ps-5.6.47`](#perconaps-5647)
-	[`percona:ps-5.7`](#perconaps-57)
-	[`percona:ps-5.7.30`](#perconaps-5730)
-	[`percona:ps-8`](#perconaps-8)
-	[`percona:ps-8.0`](#perconaps-80)
-	[`percona:ps-8.0.19-10`](#perconaps-8019-10)
-	[`percona:psmdb-3.6`](#perconapsmdb-36)
-	[`percona:psmdb-3.6.18`](#perconapsmdb-3618)
-	[`percona:psmdb-4.0`](#perconapsmdb-40)
-	[`percona:psmdb-4.0.19`](#perconapsmdb-4019)
-	[`percona:psmdb-4.2`](#perconapsmdb-42)
-	[`percona:psmdb-4.2.8`](#perconapsmdb-428)

## `percona:5`

```console
$ docker pull percona@sha256:2e105f177eba86761b754c198a20d949e3c523fc84f39e1d4da1fe8d03a1e0fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5` - linux; amd64

```console
$ docker pull percona@sha256:a9893b317d1b044fc633751c524a83d4beb8be8b71b0c7953efdbe19c6573ed3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (197041749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46b5bbcdce85d204b0686315a0ee36e8b6d3cac132de8b11834c3e574dfc1fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:40:12 GMT
RUN groupdel input && groupadd -g 999 mysql
# Tue, 05 May 2020 21:40:13 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:40:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Thu, 21 May 2020 04:35:10 GMT
ENV PERCONA_VERSION=5.7.30-33.1.el7
# Thu, 21 May 2020 04:36:03 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 21 May 2020 04:36:04 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 21 May 2020 04:36:05 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 21 May 2020 04:36:05 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 21 May 2020 04:36:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 May 2020 04:36:05 GMT
USER mysql
# Thu, 21 May 2020 04:36:05 GMT
EXPOSE 3306
# Thu, 21 May 2020 04:36:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37487d9cd8bc83a07051a75ee8263a8d1f0db1fcb3b659c010a5b79b8c523375`  
		Last Modified: Tue, 05 May 2020 21:45:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac8e4e1ff8746e7beb42291d98b9dd79c30af37eb9574f5f48d4bd7805c03e`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea79009bc580ccf1fa76f5ef8574193affe3a98e12b985af44428b224b98430`  
		Last Modified: Tue, 05 May 2020 21:45:10 GMT  
		Size: 6.5 MB (6516282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ecc2b8fa3fb5405a9a6a989784c7bee30aef4b280d8fc6402e8429aa5b274d`  
		Last Modified: Thu, 21 May 2020 04:36:59 GMT  
		Size: 114.6 MB (114638778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ebb4f075ce740c790630b746887e6b2f2e88cf73e2e1dd8750306bfd7b8c4`  
		Last Modified: Thu, 21 May 2020 04:36:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997f9812b9c69636a391ae9ed5b4fb2761ced7894c413c8de23708aac358227`  
		Last Modified: Thu, 21 May 2020 04:36:39 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6`

```console
$ docker pull percona@sha256:daba4ebd0e6d66eac8007ad4b924df00f904bbbcad4562b352c2331439501953
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.6` - linux; amd64

```console
$ docker pull percona@sha256:93dcc0d96bf39da4fcc2ed1519cebfbf50c61c75a37971387c9c31dfa2b86cf3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140085308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d028c31a5e5d22d9b0abdf802091a0bbb39a6d3bbca5522c2b7e02111011c207`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:40:12 GMT
RUN groupdel input && groupadd -g 999 mysql
# Tue, 05 May 2020 21:40:13 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:41:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Wed, 13 May 2020 14:20:07 GMT
ENV PERCONA_VERSION=5.6.48-rel88.0.1.el7
# Wed, 13 May 2020 14:20:48 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 13 May 2020 14:20:49 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Wed, 13 May 2020 14:20:49 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 13 May 2020 14:20:49 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Wed, 13 May 2020 14:20:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 May 2020 14:20:49 GMT
USER mysql
# Wed, 13 May 2020 14:20:49 GMT
EXPOSE 3306
# Wed, 13 May 2020 14:20:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37487d9cd8bc83a07051a75ee8263a8d1f0db1fcb3b659c010a5b79b8c523375`  
		Last Modified: Tue, 05 May 2020 21:45:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac8e4e1ff8746e7beb42291d98b9dd79c30af37eb9574f5f48d4bd7805c03e`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22a722a0c1803de3bdf959794ffa8fcf8fe8a9cb2a9f873ecb9c4ac30134803`  
		Last Modified: Tue, 05 May 2020 21:45:43 GMT  
		Size: 6.5 MB (6516278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5010d335491e35be80ec886e88307e5eaeaa6b52999c14f2172a4a653acc299`  
		Last Modified: Wed, 13 May 2020 14:21:35 GMT  
		Size: 57.7 MB (57678972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afa58ed8bc4e290bc1ec5e6a642f4592f842f5cd9a513885955defd8af442b`  
		Last Modified: Wed, 13 May 2020 14:21:23 GMT  
		Size: 4.9 KB (4880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2b6385ff7071f3d87d10f18ecdf408296b990891cf528c84c2d5a5b271cc2d`  
		Last Modified: Wed, 13 May 2020 14:21:23 GMT  
		Size: 2.9 KB (2942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6.48`

```console
$ docker pull percona@sha256:daba4ebd0e6d66eac8007ad4b924df00f904bbbcad4562b352c2331439501953
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.6.48` - linux; amd64

```console
$ docker pull percona@sha256:93dcc0d96bf39da4fcc2ed1519cebfbf50c61c75a37971387c9c31dfa2b86cf3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140085308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d028c31a5e5d22d9b0abdf802091a0bbb39a6d3bbca5522c2b7e02111011c207`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:40:12 GMT
RUN groupdel input && groupadd -g 999 mysql
# Tue, 05 May 2020 21:40:13 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:41:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Wed, 13 May 2020 14:20:07 GMT
ENV PERCONA_VERSION=5.6.48-rel88.0.1.el7
# Wed, 13 May 2020 14:20:48 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 13 May 2020 14:20:49 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Wed, 13 May 2020 14:20:49 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 13 May 2020 14:20:49 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Wed, 13 May 2020 14:20:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 May 2020 14:20:49 GMT
USER mysql
# Wed, 13 May 2020 14:20:49 GMT
EXPOSE 3306
# Wed, 13 May 2020 14:20:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37487d9cd8bc83a07051a75ee8263a8d1f0db1fcb3b659c010a5b79b8c523375`  
		Last Modified: Tue, 05 May 2020 21:45:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac8e4e1ff8746e7beb42291d98b9dd79c30af37eb9574f5f48d4bd7805c03e`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22a722a0c1803de3bdf959794ffa8fcf8fe8a9cb2a9f873ecb9c4ac30134803`  
		Last Modified: Tue, 05 May 2020 21:45:43 GMT  
		Size: 6.5 MB (6516278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5010d335491e35be80ec886e88307e5eaeaa6b52999c14f2172a4a653acc299`  
		Last Modified: Wed, 13 May 2020 14:21:35 GMT  
		Size: 57.7 MB (57678972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afa58ed8bc4e290bc1ec5e6a642f4592f842f5cd9a513885955defd8af442b`  
		Last Modified: Wed, 13 May 2020 14:21:23 GMT  
		Size: 4.9 KB (4880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2b6385ff7071f3d87d10f18ecdf408296b990891cf528c84c2d5a5b271cc2d`  
		Last Modified: Wed, 13 May 2020 14:21:23 GMT  
		Size: 2.9 KB (2942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6.48-centos`

```console
$ docker pull percona@sha256:daba4ebd0e6d66eac8007ad4b924df00f904bbbcad4562b352c2331439501953
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.6.48-centos` - linux; amd64

```console
$ docker pull percona@sha256:93dcc0d96bf39da4fcc2ed1519cebfbf50c61c75a37971387c9c31dfa2b86cf3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140085308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d028c31a5e5d22d9b0abdf802091a0bbb39a6d3bbca5522c2b7e02111011c207`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:40:12 GMT
RUN groupdel input && groupadd -g 999 mysql
# Tue, 05 May 2020 21:40:13 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:41:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Wed, 13 May 2020 14:20:07 GMT
ENV PERCONA_VERSION=5.6.48-rel88.0.1.el7
# Wed, 13 May 2020 14:20:48 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 13 May 2020 14:20:49 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Wed, 13 May 2020 14:20:49 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 13 May 2020 14:20:49 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Wed, 13 May 2020 14:20:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 May 2020 14:20:49 GMT
USER mysql
# Wed, 13 May 2020 14:20:49 GMT
EXPOSE 3306
# Wed, 13 May 2020 14:20:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37487d9cd8bc83a07051a75ee8263a8d1f0db1fcb3b659c010a5b79b8c523375`  
		Last Modified: Tue, 05 May 2020 21:45:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac8e4e1ff8746e7beb42291d98b9dd79c30af37eb9574f5f48d4bd7805c03e`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22a722a0c1803de3bdf959794ffa8fcf8fe8a9cb2a9f873ecb9c4ac30134803`  
		Last Modified: Tue, 05 May 2020 21:45:43 GMT  
		Size: 6.5 MB (6516278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5010d335491e35be80ec886e88307e5eaeaa6b52999c14f2172a4a653acc299`  
		Last Modified: Wed, 13 May 2020 14:21:35 GMT  
		Size: 57.7 MB (57678972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afa58ed8bc4e290bc1ec5e6a642f4592f842f5cd9a513885955defd8af442b`  
		Last Modified: Wed, 13 May 2020 14:21:23 GMT  
		Size: 4.9 KB (4880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2b6385ff7071f3d87d10f18ecdf408296b990891cf528c84c2d5a5b271cc2d`  
		Last Modified: Wed, 13 May 2020 14:21:23 GMT  
		Size: 2.9 KB (2942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6-centos`

```console
$ docker pull percona@sha256:daba4ebd0e6d66eac8007ad4b924df00f904bbbcad4562b352c2331439501953
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.6-centos` - linux; amd64

```console
$ docker pull percona@sha256:93dcc0d96bf39da4fcc2ed1519cebfbf50c61c75a37971387c9c31dfa2b86cf3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140085308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d028c31a5e5d22d9b0abdf802091a0bbb39a6d3bbca5522c2b7e02111011c207`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:40:12 GMT
RUN groupdel input && groupadd -g 999 mysql
# Tue, 05 May 2020 21:40:13 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:41:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Wed, 13 May 2020 14:20:07 GMT
ENV PERCONA_VERSION=5.6.48-rel88.0.1.el7
# Wed, 13 May 2020 14:20:48 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 13 May 2020 14:20:49 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Wed, 13 May 2020 14:20:49 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 13 May 2020 14:20:49 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Wed, 13 May 2020 14:20:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 May 2020 14:20:49 GMT
USER mysql
# Wed, 13 May 2020 14:20:49 GMT
EXPOSE 3306
# Wed, 13 May 2020 14:20:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37487d9cd8bc83a07051a75ee8263a8d1f0db1fcb3b659c010a5b79b8c523375`  
		Last Modified: Tue, 05 May 2020 21:45:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac8e4e1ff8746e7beb42291d98b9dd79c30af37eb9574f5f48d4bd7805c03e`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22a722a0c1803de3bdf959794ffa8fcf8fe8a9cb2a9f873ecb9c4ac30134803`  
		Last Modified: Tue, 05 May 2020 21:45:43 GMT  
		Size: 6.5 MB (6516278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5010d335491e35be80ec886e88307e5eaeaa6b52999c14f2172a4a653acc299`  
		Last Modified: Wed, 13 May 2020 14:21:35 GMT  
		Size: 57.7 MB (57678972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afa58ed8bc4e290bc1ec5e6a642f4592f842f5cd9a513885955defd8af442b`  
		Last Modified: Wed, 13 May 2020 14:21:23 GMT  
		Size: 4.9 KB (4880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2b6385ff7071f3d87d10f18ecdf408296b990891cf528c84c2d5a5b271cc2d`  
		Last Modified: Wed, 13 May 2020 14:21:23 GMT  
		Size: 2.9 KB (2942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7`

```console
$ docker pull percona@sha256:2e105f177eba86761b754c198a20d949e3c523fc84f39e1d4da1fe8d03a1e0fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7` - linux; amd64

```console
$ docker pull percona@sha256:a9893b317d1b044fc633751c524a83d4beb8be8b71b0c7953efdbe19c6573ed3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (197041749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46b5bbcdce85d204b0686315a0ee36e8b6d3cac132de8b11834c3e574dfc1fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:40:12 GMT
RUN groupdel input && groupadd -g 999 mysql
# Tue, 05 May 2020 21:40:13 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:40:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Thu, 21 May 2020 04:35:10 GMT
ENV PERCONA_VERSION=5.7.30-33.1.el7
# Thu, 21 May 2020 04:36:03 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 21 May 2020 04:36:04 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 21 May 2020 04:36:05 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 21 May 2020 04:36:05 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 21 May 2020 04:36:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 May 2020 04:36:05 GMT
USER mysql
# Thu, 21 May 2020 04:36:05 GMT
EXPOSE 3306
# Thu, 21 May 2020 04:36:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37487d9cd8bc83a07051a75ee8263a8d1f0db1fcb3b659c010a5b79b8c523375`  
		Last Modified: Tue, 05 May 2020 21:45:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac8e4e1ff8746e7beb42291d98b9dd79c30af37eb9574f5f48d4bd7805c03e`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea79009bc580ccf1fa76f5ef8574193affe3a98e12b985af44428b224b98430`  
		Last Modified: Tue, 05 May 2020 21:45:10 GMT  
		Size: 6.5 MB (6516282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ecc2b8fa3fb5405a9a6a989784c7bee30aef4b280d8fc6402e8429aa5b274d`  
		Last Modified: Thu, 21 May 2020 04:36:59 GMT  
		Size: 114.6 MB (114638778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ebb4f075ce740c790630b746887e6b2f2e88cf73e2e1dd8750306bfd7b8c4`  
		Last Modified: Thu, 21 May 2020 04:36:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997f9812b9c69636a391ae9ed5b4fb2761ced7894c413c8de23708aac358227`  
		Last Modified: Thu, 21 May 2020 04:36:39 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.30`

```console
$ docker pull percona@sha256:2e105f177eba86761b754c198a20d949e3c523fc84f39e1d4da1fe8d03a1e0fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7.30` - linux; amd64

```console
$ docker pull percona@sha256:a9893b317d1b044fc633751c524a83d4beb8be8b71b0c7953efdbe19c6573ed3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (197041749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46b5bbcdce85d204b0686315a0ee36e8b6d3cac132de8b11834c3e574dfc1fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:40:12 GMT
RUN groupdel input && groupadd -g 999 mysql
# Tue, 05 May 2020 21:40:13 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:40:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Thu, 21 May 2020 04:35:10 GMT
ENV PERCONA_VERSION=5.7.30-33.1.el7
# Thu, 21 May 2020 04:36:03 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 21 May 2020 04:36:04 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 21 May 2020 04:36:05 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 21 May 2020 04:36:05 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 21 May 2020 04:36:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 May 2020 04:36:05 GMT
USER mysql
# Thu, 21 May 2020 04:36:05 GMT
EXPOSE 3306
# Thu, 21 May 2020 04:36:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37487d9cd8bc83a07051a75ee8263a8d1f0db1fcb3b659c010a5b79b8c523375`  
		Last Modified: Tue, 05 May 2020 21:45:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac8e4e1ff8746e7beb42291d98b9dd79c30af37eb9574f5f48d4bd7805c03e`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea79009bc580ccf1fa76f5ef8574193affe3a98e12b985af44428b224b98430`  
		Last Modified: Tue, 05 May 2020 21:45:10 GMT  
		Size: 6.5 MB (6516282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ecc2b8fa3fb5405a9a6a989784c7bee30aef4b280d8fc6402e8429aa5b274d`  
		Last Modified: Thu, 21 May 2020 04:36:59 GMT  
		Size: 114.6 MB (114638778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ebb4f075ce740c790630b746887e6b2f2e88cf73e2e1dd8750306bfd7b8c4`  
		Last Modified: Thu, 21 May 2020 04:36:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997f9812b9c69636a391ae9ed5b4fb2761ced7894c413c8de23708aac358227`  
		Last Modified: Thu, 21 May 2020 04:36:39 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.30-centos`

```console
$ docker pull percona@sha256:2e105f177eba86761b754c198a20d949e3c523fc84f39e1d4da1fe8d03a1e0fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7.30-centos` - linux; amd64

```console
$ docker pull percona@sha256:a9893b317d1b044fc633751c524a83d4beb8be8b71b0c7953efdbe19c6573ed3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (197041749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46b5bbcdce85d204b0686315a0ee36e8b6d3cac132de8b11834c3e574dfc1fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:40:12 GMT
RUN groupdel input && groupadd -g 999 mysql
# Tue, 05 May 2020 21:40:13 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:40:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Thu, 21 May 2020 04:35:10 GMT
ENV PERCONA_VERSION=5.7.30-33.1.el7
# Thu, 21 May 2020 04:36:03 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 21 May 2020 04:36:04 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 21 May 2020 04:36:05 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 21 May 2020 04:36:05 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 21 May 2020 04:36:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 May 2020 04:36:05 GMT
USER mysql
# Thu, 21 May 2020 04:36:05 GMT
EXPOSE 3306
# Thu, 21 May 2020 04:36:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37487d9cd8bc83a07051a75ee8263a8d1f0db1fcb3b659c010a5b79b8c523375`  
		Last Modified: Tue, 05 May 2020 21:45:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac8e4e1ff8746e7beb42291d98b9dd79c30af37eb9574f5f48d4bd7805c03e`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea79009bc580ccf1fa76f5ef8574193affe3a98e12b985af44428b224b98430`  
		Last Modified: Tue, 05 May 2020 21:45:10 GMT  
		Size: 6.5 MB (6516282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ecc2b8fa3fb5405a9a6a989784c7bee30aef4b280d8fc6402e8429aa5b274d`  
		Last Modified: Thu, 21 May 2020 04:36:59 GMT  
		Size: 114.6 MB (114638778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ebb4f075ce740c790630b746887e6b2f2e88cf73e2e1dd8750306bfd7b8c4`  
		Last Modified: Thu, 21 May 2020 04:36:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997f9812b9c69636a391ae9ed5b4fb2761ced7894c413c8de23708aac358227`  
		Last Modified: Thu, 21 May 2020 04:36:39 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7-centos`

```console
$ docker pull percona@sha256:2e105f177eba86761b754c198a20d949e3c523fc84f39e1d4da1fe8d03a1e0fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7-centos` - linux; amd64

```console
$ docker pull percona@sha256:a9893b317d1b044fc633751c524a83d4beb8be8b71b0c7953efdbe19c6573ed3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (197041749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46b5bbcdce85d204b0686315a0ee36e8b6d3cac132de8b11834c3e574dfc1fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:40:12 GMT
RUN groupdel input && groupadd -g 999 mysql
# Tue, 05 May 2020 21:40:13 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:40:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Thu, 21 May 2020 04:35:10 GMT
ENV PERCONA_VERSION=5.7.30-33.1.el7
# Thu, 21 May 2020 04:36:03 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 21 May 2020 04:36:04 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 21 May 2020 04:36:05 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 21 May 2020 04:36:05 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 21 May 2020 04:36:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 May 2020 04:36:05 GMT
USER mysql
# Thu, 21 May 2020 04:36:05 GMT
EXPOSE 3306
# Thu, 21 May 2020 04:36:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37487d9cd8bc83a07051a75ee8263a8d1f0db1fcb3b659c010a5b79b8c523375`  
		Last Modified: Tue, 05 May 2020 21:45:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac8e4e1ff8746e7beb42291d98b9dd79c30af37eb9574f5f48d4bd7805c03e`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea79009bc580ccf1fa76f5ef8574193affe3a98e12b985af44428b224b98430`  
		Last Modified: Tue, 05 May 2020 21:45:10 GMT  
		Size: 6.5 MB (6516282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ecc2b8fa3fb5405a9a6a989784c7bee30aef4b280d8fc6402e8429aa5b274d`  
		Last Modified: Thu, 21 May 2020 04:36:59 GMT  
		Size: 114.6 MB (114638778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ebb4f075ce740c790630b746887e6b2f2e88cf73e2e1dd8750306bfd7b8c4`  
		Last Modified: Thu, 21 May 2020 04:36:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997f9812b9c69636a391ae9ed5b4fb2761ced7894c413c8de23708aac358227`  
		Last Modified: Thu, 21 May 2020 04:36:39 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5-centos`

```console
$ docker pull percona@sha256:2e105f177eba86761b754c198a20d949e3c523fc84f39e1d4da1fe8d03a1e0fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5-centos` - linux; amd64

```console
$ docker pull percona@sha256:a9893b317d1b044fc633751c524a83d4beb8be8b71b0c7953efdbe19c6573ed3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (197041749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46b5bbcdce85d204b0686315a0ee36e8b6d3cac132de8b11834c3e574dfc1fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:40:12 GMT
RUN groupdel input && groupadd -g 999 mysql
# Tue, 05 May 2020 21:40:13 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:40:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Thu, 21 May 2020 04:35:10 GMT
ENV PERCONA_VERSION=5.7.30-33.1.el7
# Thu, 21 May 2020 04:36:03 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 21 May 2020 04:36:04 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 21 May 2020 04:36:05 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 21 May 2020 04:36:05 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 21 May 2020 04:36:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 May 2020 04:36:05 GMT
USER mysql
# Thu, 21 May 2020 04:36:05 GMT
EXPOSE 3306
# Thu, 21 May 2020 04:36:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37487d9cd8bc83a07051a75ee8263a8d1f0db1fcb3b659c010a5b79b8c523375`  
		Last Modified: Tue, 05 May 2020 21:45:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac8e4e1ff8746e7beb42291d98b9dd79c30af37eb9574f5f48d4bd7805c03e`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea79009bc580ccf1fa76f5ef8574193affe3a98e12b985af44428b224b98430`  
		Last Modified: Tue, 05 May 2020 21:45:10 GMT  
		Size: 6.5 MB (6516282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ecc2b8fa3fb5405a9a6a989784c7bee30aef4b280d8fc6402e8429aa5b274d`  
		Last Modified: Thu, 21 May 2020 04:36:59 GMT  
		Size: 114.6 MB (114638778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ebb4f075ce740c790630b746887e6b2f2e88cf73e2e1dd8750306bfd7b8c4`  
		Last Modified: Thu, 21 May 2020 04:36:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997f9812b9c69636a391ae9ed5b4fb2761ced7894c413c8de23708aac358227`  
		Last Modified: Thu, 21 May 2020 04:36:39 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8`

```console
$ docker pull percona@sha256:b3db261ed6edbf136c51a8ca1c7859da8edad61ed3a3715a7c1f0aa965875e56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8` - linux; amd64

```console
$ docker pull percona@sha256:c07d08fb7357ff52e655550525a1d021dc679bf59589a1b50144cae6cd31e936
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.8 MB (224750500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e16910846759f931f0a0445c6266082091b036b21b0364ac1cc275b6c3fd2f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:39:07 GMT
RUN groupadd -g 1001 mysql
# Tue, 05 May 2020 21:39:08 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:39:13 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Tue, 05 May 2020 21:39:13 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Tue, 05 May 2020 21:40:05 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:40:06 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Tue, 05 May 2020 21:40:06 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:40:06 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:40:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:40:06 GMT
USER mysql
# Tue, 05 May 2020 21:40:07 GMT
EXPOSE 3306 33060
# Tue, 05 May 2020 21:40:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e386a719ceae0f0238e80a8fbcd5e5144f3c4675860fc1677674d224a4f043`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b0b666a45f4b0619d873f8a797c2e1c0451a196871908efd2d3442c506e6ef`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b1a9d6f75e0d0123edeb268d2aa760548242a912592232d7b1d93ae8f9f1d6`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 6.5 MB (6516428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c189211552cdd321ae7bdf84cb5d708260161c01e43a0fb44dd068344bd7178e`  
		Last Modified: Tue, 05 May 2020 21:44:59 GMT  
		Size: 142.3 MB (142347625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bece8a5f214edeb3d4cb18eb23f42c557b8a6dc78be2e519ece4071aba7976`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fd35f5cfa69a7c2447e98e1679dab078ccb489807f4a139ee9630bf5210469`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 3.1 KB (3068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0`

```console
$ docker pull percona@sha256:b3db261ed6edbf136c51a8ca1c7859da8edad61ed3a3715a7c1f0aa965875e56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0` - linux; amd64

```console
$ docker pull percona@sha256:c07d08fb7357ff52e655550525a1d021dc679bf59589a1b50144cae6cd31e936
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.8 MB (224750500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e16910846759f931f0a0445c6266082091b036b21b0364ac1cc275b6c3fd2f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:39:07 GMT
RUN groupadd -g 1001 mysql
# Tue, 05 May 2020 21:39:08 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:39:13 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Tue, 05 May 2020 21:39:13 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Tue, 05 May 2020 21:40:05 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:40:06 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Tue, 05 May 2020 21:40:06 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:40:06 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:40:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:40:06 GMT
USER mysql
# Tue, 05 May 2020 21:40:07 GMT
EXPOSE 3306 33060
# Tue, 05 May 2020 21:40:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e386a719ceae0f0238e80a8fbcd5e5144f3c4675860fc1677674d224a4f043`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b0b666a45f4b0619d873f8a797c2e1c0451a196871908efd2d3442c506e6ef`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b1a9d6f75e0d0123edeb268d2aa760548242a912592232d7b1d93ae8f9f1d6`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 6.5 MB (6516428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c189211552cdd321ae7bdf84cb5d708260161c01e43a0fb44dd068344bd7178e`  
		Last Modified: Tue, 05 May 2020 21:44:59 GMT  
		Size: 142.3 MB (142347625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bece8a5f214edeb3d4cb18eb23f42c557b8a6dc78be2e519ece4071aba7976`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fd35f5cfa69a7c2447e98e1679dab078ccb489807f4a139ee9630bf5210469`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 3.1 KB (3068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.19-10`

```console
$ docker pull percona@sha256:b3db261ed6edbf136c51a8ca1c7859da8edad61ed3a3715a7c1f0aa965875e56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0.19-10` - linux; amd64

```console
$ docker pull percona@sha256:c07d08fb7357ff52e655550525a1d021dc679bf59589a1b50144cae6cd31e936
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.8 MB (224750500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e16910846759f931f0a0445c6266082091b036b21b0364ac1cc275b6c3fd2f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:39:07 GMT
RUN groupadd -g 1001 mysql
# Tue, 05 May 2020 21:39:08 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:39:13 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Tue, 05 May 2020 21:39:13 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Tue, 05 May 2020 21:40:05 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:40:06 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Tue, 05 May 2020 21:40:06 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:40:06 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:40:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:40:06 GMT
USER mysql
# Tue, 05 May 2020 21:40:07 GMT
EXPOSE 3306 33060
# Tue, 05 May 2020 21:40:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e386a719ceae0f0238e80a8fbcd5e5144f3c4675860fc1677674d224a4f043`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b0b666a45f4b0619d873f8a797c2e1c0451a196871908efd2d3442c506e6ef`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b1a9d6f75e0d0123edeb268d2aa760548242a912592232d7b1d93ae8f9f1d6`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 6.5 MB (6516428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c189211552cdd321ae7bdf84cb5d708260161c01e43a0fb44dd068344bd7178e`  
		Last Modified: Tue, 05 May 2020 21:44:59 GMT  
		Size: 142.3 MB (142347625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bece8a5f214edeb3d4cb18eb23f42c557b8a6dc78be2e519ece4071aba7976`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fd35f5cfa69a7c2447e98e1679dab078ccb489807f4a139ee9630bf5210469`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 3.1 KB (3068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.19-10-centos`

```console
$ docker pull percona@sha256:b3db261ed6edbf136c51a8ca1c7859da8edad61ed3a3715a7c1f0aa965875e56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0.19-10-centos` - linux; amd64

```console
$ docker pull percona@sha256:c07d08fb7357ff52e655550525a1d021dc679bf59589a1b50144cae6cd31e936
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.8 MB (224750500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e16910846759f931f0a0445c6266082091b036b21b0364ac1cc275b6c3fd2f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:39:07 GMT
RUN groupadd -g 1001 mysql
# Tue, 05 May 2020 21:39:08 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:39:13 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Tue, 05 May 2020 21:39:13 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Tue, 05 May 2020 21:40:05 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:40:06 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Tue, 05 May 2020 21:40:06 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:40:06 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:40:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:40:06 GMT
USER mysql
# Tue, 05 May 2020 21:40:07 GMT
EXPOSE 3306 33060
# Tue, 05 May 2020 21:40:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e386a719ceae0f0238e80a8fbcd5e5144f3c4675860fc1677674d224a4f043`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b0b666a45f4b0619d873f8a797c2e1c0451a196871908efd2d3442c506e6ef`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b1a9d6f75e0d0123edeb268d2aa760548242a912592232d7b1d93ae8f9f1d6`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 6.5 MB (6516428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c189211552cdd321ae7bdf84cb5d708260161c01e43a0fb44dd068344bd7178e`  
		Last Modified: Tue, 05 May 2020 21:44:59 GMT  
		Size: 142.3 MB (142347625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bece8a5f214edeb3d4cb18eb23f42c557b8a6dc78be2e519ece4071aba7976`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fd35f5cfa69a7c2447e98e1679dab078ccb489807f4a139ee9630bf5210469`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 3.1 KB (3068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0-centos`

```console
$ docker pull percona@sha256:b3db261ed6edbf136c51a8ca1c7859da8edad61ed3a3715a7c1f0aa965875e56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0-centos` - linux; amd64

```console
$ docker pull percona@sha256:c07d08fb7357ff52e655550525a1d021dc679bf59589a1b50144cae6cd31e936
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.8 MB (224750500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e16910846759f931f0a0445c6266082091b036b21b0364ac1cc275b6c3fd2f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:39:07 GMT
RUN groupadd -g 1001 mysql
# Tue, 05 May 2020 21:39:08 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:39:13 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Tue, 05 May 2020 21:39:13 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Tue, 05 May 2020 21:40:05 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:40:06 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Tue, 05 May 2020 21:40:06 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:40:06 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:40:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:40:06 GMT
USER mysql
# Tue, 05 May 2020 21:40:07 GMT
EXPOSE 3306 33060
# Tue, 05 May 2020 21:40:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e386a719ceae0f0238e80a8fbcd5e5144f3c4675860fc1677674d224a4f043`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b0b666a45f4b0619d873f8a797c2e1c0451a196871908efd2d3442c506e6ef`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b1a9d6f75e0d0123edeb268d2aa760548242a912592232d7b1d93ae8f9f1d6`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 6.5 MB (6516428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c189211552cdd321ae7bdf84cb5d708260161c01e43a0fb44dd068344bd7178e`  
		Last Modified: Tue, 05 May 2020 21:44:59 GMT  
		Size: 142.3 MB (142347625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bece8a5f214edeb3d4cb18eb23f42c557b8a6dc78be2e519ece4071aba7976`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fd35f5cfa69a7c2447e98e1679dab078ccb489807f4a139ee9630bf5210469`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 3.1 KB (3068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8-centos`

```console
$ docker pull percona@sha256:b3db261ed6edbf136c51a8ca1c7859da8edad61ed3a3715a7c1f0aa965875e56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8-centos` - linux; amd64

```console
$ docker pull percona@sha256:c07d08fb7357ff52e655550525a1d021dc679bf59589a1b50144cae6cd31e936
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.8 MB (224750500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e16910846759f931f0a0445c6266082091b036b21b0364ac1cc275b6c3fd2f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:39:07 GMT
RUN groupadd -g 1001 mysql
# Tue, 05 May 2020 21:39:08 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:39:13 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Tue, 05 May 2020 21:39:13 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Tue, 05 May 2020 21:40:05 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:40:06 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Tue, 05 May 2020 21:40:06 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:40:06 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:40:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:40:06 GMT
USER mysql
# Tue, 05 May 2020 21:40:07 GMT
EXPOSE 3306 33060
# Tue, 05 May 2020 21:40:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e386a719ceae0f0238e80a8fbcd5e5144f3c4675860fc1677674d224a4f043`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b0b666a45f4b0619d873f8a797c2e1c0451a196871908efd2d3442c506e6ef`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b1a9d6f75e0d0123edeb268d2aa760548242a912592232d7b1d93ae8f9f1d6`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 6.5 MB (6516428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c189211552cdd321ae7bdf84cb5d708260161c01e43a0fb44dd068344bd7178e`  
		Last Modified: Tue, 05 May 2020 21:44:59 GMT  
		Size: 142.3 MB (142347625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bece8a5f214edeb3d4cb18eb23f42c557b8a6dc78be2e519ece4071aba7976`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fd35f5cfa69a7c2447e98e1679dab078ccb489807f4a139ee9630bf5210469`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 3.1 KB (3068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:centos`

```console
$ docker pull percona@sha256:2e105f177eba86761b754c198a20d949e3c523fc84f39e1d4da1fe8d03a1e0fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:centos` - linux; amd64

```console
$ docker pull percona@sha256:a9893b317d1b044fc633751c524a83d4beb8be8b71b0c7953efdbe19c6573ed3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (197041749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46b5bbcdce85d204b0686315a0ee36e8b6d3cac132de8b11834c3e574dfc1fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:40:12 GMT
RUN groupdel input && groupadd -g 999 mysql
# Tue, 05 May 2020 21:40:13 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:40:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Thu, 21 May 2020 04:35:10 GMT
ENV PERCONA_VERSION=5.7.30-33.1.el7
# Thu, 21 May 2020 04:36:03 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 21 May 2020 04:36:04 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 21 May 2020 04:36:05 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 21 May 2020 04:36:05 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 21 May 2020 04:36:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 May 2020 04:36:05 GMT
USER mysql
# Thu, 21 May 2020 04:36:05 GMT
EXPOSE 3306
# Thu, 21 May 2020 04:36:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37487d9cd8bc83a07051a75ee8263a8d1f0db1fcb3b659c010a5b79b8c523375`  
		Last Modified: Tue, 05 May 2020 21:45:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac8e4e1ff8746e7beb42291d98b9dd79c30af37eb9574f5f48d4bd7805c03e`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea79009bc580ccf1fa76f5ef8574193affe3a98e12b985af44428b224b98430`  
		Last Modified: Tue, 05 May 2020 21:45:10 GMT  
		Size: 6.5 MB (6516282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ecc2b8fa3fb5405a9a6a989784c7bee30aef4b280d8fc6402e8429aa5b274d`  
		Last Modified: Thu, 21 May 2020 04:36:59 GMT  
		Size: 114.6 MB (114638778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ebb4f075ce740c790630b746887e6b2f2e88cf73e2e1dd8750306bfd7b8c4`  
		Last Modified: Thu, 21 May 2020 04:36:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997f9812b9c69636a391ae9ed5b4fb2761ced7894c413c8de23708aac358227`  
		Last Modified: Thu, 21 May 2020 04:36:39 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:latest`

```console
$ docker pull percona@sha256:2e105f177eba86761b754c198a20d949e3c523fc84f39e1d4da1fe8d03a1e0fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:latest` - linux; amd64

```console
$ docker pull percona@sha256:a9893b317d1b044fc633751c524a83d4beb8be8b71b0c7953efdbe19c6573ed3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (197041749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46b5bbcdce85d204b0686315a0ee36e8b6d3cac132de8b11834c3e574dfc1fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:40:12 GMT
RUN groupdel input && groupadd -g 999 mysql
# Tue, 05 May 2020 21:40:13 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:40:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Thu, 21 May 2020 04:35:10 GMT
ENV PERCONA_VERSION=5.7.30-33.1.el7
# Thu, 21 May 2020 04:36:03 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 21 May 2020 04:36:04 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 21 May 2020 04:36:05 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 21 May 2020 04:36:05 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 21 May 2020 04:36:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 May 2020 04:36:05 GMT
USER mysql
# Thu, 21 May 2020 04:36:05 GMT
EXPOSE 3306
# Thu, 21 May 2020 04:36:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37487d9cd8bc83a07051a75ee8263a8d1f0db1fcb3b659c010a5b79b8c523375`  
		Last Modified: Tue, 05 May 2020 21:45:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac8e4e1ff8746e7beb42291d98b9dd79c30af37eb9574f5f48d4bd7805c03e`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea79009bc580ccf1fa76f5ef8574193affe3a98e12b985af44428b224b98430`  
		Last Modified: Tue, 05 May 2020 21:45:10 GMT  
		Size: 6.5 MB (6516282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ecc2b8fa3fb5405a9a6a989784c7bee30aef4b280d8fc6402e8429aa5b274d`  
		Last Modified: Thu, 21 May 2020 04:36:59 GMT  
		Size: 114.6 MB (114638778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ebb4f075ce740c790630b746887e6b2f2e88cf73e2e1dd8750306bfd7b8c4`  
		Last Modified: Thu, 21 May 2020 04:36:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997f9812b9c69636a391ae9ed5b4fb2761ced7894c413c8de23708aac358227`  
		Last Modified: Thu, 21 May 2020 04:36:39 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5`

```console
$ docker pull percona@sha256:2e105f177eba86761b754c198a20d949e3c523fc84f39e1d4da1fe8d03a1e0fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5` - linux; amd64

```console
$ docker pull percona@sha256:a9893b317d1b044fc633751c524a83d4beb8be8b71b0c7953efdbe19c6573ed3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (197041749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46b5bbcdce85d204b0686315a0ee36e8b6d3cac132de8b11834c3e574dfc1fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:40:12 GMT
RUN groupdel input && groupadd -g 999 mysql
# Tue, 05 May 2020 21:40:13 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:40:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Thu, 21 May 2020 04:35:10 GMT
ENV PERCONA_VERSION=5.7.30-33.1.el7
# Thu, 21 May 2020 04:36:03 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 21 May 2020 04:36:04 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 21 May 2020 04:36:05 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 21 May 2020 04:36:05 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 21 May 2020 04:36:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 May 2020 04:36:05 GMT
USER mysql
# Thu, 21 May 2020 04:36:05 GMT
EXPOSE 3306
# Thu, 21 May 2020 04:36:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37487d9cd8bc83a07051a75ee8263a8d1f0db1fcb3b659c010a5b79b8c523375`  
		Last Modified: Tue, 05 May 2020 21:45:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac8e4e1ff8746e7beb42291d98b9dd79c30af37eb9574f5f48d4bd7805c03e`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea79009bc580ccf1fa76f5ef8574193affe3a98e12b985af44428b224b98430`  
		Last Modified: Tue, 05 May 2020 21:45:10 GMT  
		Size: 6.5 MB (6516282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ecc2b8fa3fb5405a9a6a989784c7bee30aef4b280d8fc6402e8429aa5b274d`  
		Last Modified: Thu, 21 May 2020 04:36:59 GMT  
		Size: 114.6 MB (114638778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ebb4f075ce740c790630b746887e6b2f2e88cf73e2e1dd8750306bfd7b8c4`  
		Last Modified: Thu, 21 May 2020 04:36:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997f9812b9c69636a391ae9ed5b4fb2761ced7894c413c8de23708aac358227`  
		Last Modified: Thu, 21 May 2020 04:36:39 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.6`

```console
$ docker pull percona@sha256:daba4ebd0e6d66eac8007ad4b924df00f904bbbcad4562b352c2331439501953
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.6` - linux; amd64

```console
$ docker pull percona@sha256:93dcc0d96bf39da4fcc2ed1519cebfbf50c61c75a37971387c9c31dfa2b86cf3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140085308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d028c31a5e5d22d9b0abdf802091a0bbb39a6d3bbca5522c2b7e02111011c207`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:40:12 GMT
RUN groupdel input && groupadd -g 999 mysql
# Tue, 05 May 2020 21:40:13 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:41:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Wed, 13 May 2020 14:20:07 GMT
ENV PERCONA_VERSION=5.6.48-rel88.0.1.el7
# Wed, 13 May 2020 14:20:48 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 13 May 2020 14:20:49 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Wed, 13 May 2020 14:20:49 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 13 May 2020 14:20:49 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Wed, 13 May 2020 14:20:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 May 2020 14:20:49 GMT
USER mysql
# Wed, 13 May 2020 14:20:49 GMT
EXPOSE 3306
# Wed, 13 May 2020 14:20:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37487d9cd8bc83a07051a75ee8263a8d1f0db1fcb3b659c010a5b79b8c523375`  
		Last Modified: Tue, 05 May 2020 21:45:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac8e4e1ff8746e7beb42291d98b9dd79c30af37eb9574f5f48d4bd7805c03e`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22a722a0c1803de3bdf959794ffa8fcf8fe8a9cb2a9f873ecb9c4ac30134803`  
		Last Modified: Tue, 05 May 2020 21:45:43 GMT  
		Size: 6.5 MB (6516278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5010d335491e35be80ec886e88307e5eaeaa6b52999c14f2172a4a653acc299`  
		Last Modified: Wed, 13 May 2020 14:21:35 GMT  
		Size: 57.7 MB (57678972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afa58ed8bc4e290bc1ec5e6a642f4592f842f5cd9a513885955defd8af442b`  
		Last Modified: Wed, 13 May 2020 14:21:23 GMT  
		Size: 4.9 KB (4880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2b6385ff7071f3d87d10f18ecdf408296b990891cf528c84c2d5a5b271cc2d`  
		Last Modified: Wed, 13 May 2020 14:21:23 GMT  
		Size: 2.9 KB (2942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.6.47`

```console
$ docker pull percona@sha256:daba4ebd0e6d66eac8007ad4b924df00f904bbbcad4562b352c2331439501953
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.6.47` - linux; amd64

```console
$ docker pull percona@sha256:93dcc0d96bf39da4fcc2ed1519cebfbf50c61c75a37971387c9c31dfa2b86cf3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140085308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d028c31a5e5d22d9b0abdf802091a0bbb39a6d3bbca5522c2b7e02111011c207`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:40:12 GMT
RUN groupdel input && groupadd -g 999 mysql
# Tue, 05 May 2020 21:40:13 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:41:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Wed, 13 May 2020 14:20:07 GMT
ENV PERCONA_VERSION=5.6.48-rel88.0.1.el7
# Wed, 13 May 2020 14:20:48 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 13 May 2020 14:20:49 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Wed, 13 May 2020 14:20:49 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 13 May 2020 14:20:49 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Wed, 13 May 2020 14:20:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 May 2020 14:20:49 GMT
USER mysql
# Wed, 13 May 2020 14:20:49 GMT
EXPOSE 3306
# Wed, 13 May 2020 14:20:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37487d9cd8bc83a07051a75ee8263a8d1f0db1fcb3b659c010a5b79b8c523375`  
		Last Modified: Tue, 05 May 2020 21:45:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac8e4e1ff8746e7beb42291d98b9dd79c30af37eb9574f5f48d4bd7805c03e`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22a722a0c1803de3bdf959794ffa8fcf8fe8a9cb2a9f873ecb9c4ac30134803`  
		Last Modified: Tue, 05 May 2020 21:45:43 GMT  
		Size: 6.5 MB (6516278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5010d335491e35be80ec886e88307e5eaeaa6b52999c14f2172a4a653acc299`  
		Last Modified: Wed, 13 May 2020 14:21:35 GMT  
		Size: 57.7 MB (57678972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afa58ed8bc4e290bc1ec5e6a642f4592f842f5cd9a513885955defd8af442b`  
		Last Modified: Wed, 13 May 2020 14:21:23 GMT  
		Size: 4.9 KB (4880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2b6385ff7071f3d87d10f18ecdf408296b990891cf528c84c2d5a5b271cc2d`  
		Last Modified: Wed, 13 May 2020 14:21:23 GMT  
		Size: 2.9 KB (2942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.7`

```console
$ docker pull percona@sha256:2e105f177eba86761b754c198a20d949e3c523fc84f39e1d4da1fe8d03a1e0fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.7` - linux; amd64

```console
$ docker pull percona@sha256:a9893b317d1b044fc633751c524a83d4beb8be8b71b0c7953efdbe19c6573ed3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (197041749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46b5bbcdce85d204b0686315a0ee36e8b6d3cac132de8b11834c3e574dfc1fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:40:12 GMT
RUN groupdel input && groupadd -g 999 mysql
# Tue, 05 May 2020 21:40:13 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:40:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Thu, 21 May 2020 04:35:10 GMT
ENV PERCONA_VERSION=5.7.30-33.1.el7
# Thu, 21 May 2020 04:36:03 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 21 May 2020 04:36:04 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 21 May 2020 04:36:05 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 21 May 2020 04:36:05 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 21 May 2020 04:36:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 May 2020 04:36:05 GMT
USER mysql
# Thu, 21 May 2020 04:36:05 GMT
EXPOSE 3306
# Thu, 21 May 2020 04:36:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37487d9cd8bc83a07051a75ee8263a8d1f0db1fcb3b659c010a5b79b8c523375`  
		Last Modified: Tue, 05 May 2020 21:45:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac8e4e1ff8746e7beb42291d98b9dd79c30af37eb9574f5f48d4bd7805c03e`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea79009bc580ccf1fa76f5ef8574193affe3a98e12b985af44428b224b98430`  
		Last Modified: Tue, 05 May 2020 21:45:10 GMT  
		Size: 6.5 MB (6516282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ecc2b8fa3fb5405a9a6a989784c7bee30aef4b280d8fc6402e8429aa5b274d`  
		Last Modified: Thu, 21 May 2020 04:36:59 GMT  
		Size: 114.6 MB (114638778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ebb4f075ce740c790630b746887e6b2f2e88cf73e2e1dd8750306bfd7b8c4`  
		Last Modified: Thu, 21 May 2020 04:36:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997f9812b9c69636a391ae9ed5b4fb2761ced7894c413c8de23708aac358227`  
		Last Modified: Thu, 21 May 2020 04:36:39 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.7.30`

```console
$ docker pull percona@sha256:2e105f177eba86761b754c198a20d949e3c523fc84f39e1d4da1fe8d03a1e0fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.7.30` - linux; amd64

```console
$ docker pull percona@sha256:a9893b317d1b044fc633751c524a83d4beb8be8b71b0c7953efdbe19c6573ed3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (197041749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46b5bbcdce85d204b0686315a0ee36e8b6d3cac132de8b11834c3e574dfc1fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:40:12 GMT
RUN groupdel input && groupadd -g 999 mysql
# Tue, 05 May 2020 21:40:13 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:40:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Thu, 21 May 2020 04:35:10 GMT
ENV PERCONA_VERSION=5.7.30-33.1.el7
# Thu, 21 May 2020 04:36:03 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 21 May 2020 04:36:04 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 21 May 2020 04:36:05 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 21 May 2020 04:36:05 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 21 May 2020 04:36:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 May 2020 04:36:05 GMT
USER mysql
# Thu, 21 May 2020 04:36:05 GMT
EXPOSE 3306
# Thu, 21 May 2020 04:36:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37487d9cd8bc83a07051a75ee8263a8d1f0db1fcb3b659c010a5b79b8c523375`  
		Last Modified: Tue, 05 May 2020 21:45:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac8e4e1ff8746e7beb42291d98b9dd79c30af37eb9574f5f48d4bd7805c03e`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea79009bc580ccf1fa76f5ef8574193affe3a98e12b985af44428b224b98430`  
		Last Modified: Tue, 05 May 2020 21:45:10 GMT  
		Size: 6.5 MB (6516282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ecc2b8fa3fb5405a9a6a989784c7bee30aef4b280d8fc6402e8429aa5b274d`  
		Last Modified: Thu, 21 May 2020 04:36:59 GMT  
		Size: 114.6 MB (114638778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ebb4f075ce740c790630b746887e6b2f2e88cf73e2e1dd8750306bfd7b8c4`  
		Last Modified: Thu, 21 May 2020 04:36:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997f9812b9c69636a391ae9ed5b4fb2761ced7894c413c8de23708aac358227`  
		Last Modified: Thu, 21 May 2020 04:36:39 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8`

```console
$ docker pull percona@sha256:b3db261ed6edbf136c51a8ca1c7859da8edad61ed3a3715a7c1f0aa965875e56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8` - linux; amd64

```console
$ docker pull percona@sha256:c07d08fb7357ff52e655550525a1d021dc679bf59589a1b50144cae6cd31e936
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.8 MB (224750500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e16910846759f931f0a0445c6266082091b036b21b0364ac1cc275b6c3fd2f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:39:07 GMT
RUN groupadd -g 1001 mysql
# Tue, 05 May 2020 21:39:08 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:39:13 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Tue, 05 May 2020 21:39:13 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Tue, 05 May 2020 21:40:05 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:40:06 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Tue, 05 May 2020 21:40:06 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:40:06 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:40:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:40:06 GMT
USER mysql
# Tue, 05 May 2020 21:40:07 GMT
EXPOSE 3306 33060
# Tue, 05 May 2020 21:40:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e386a719ceae0f0238e80a8fbcd5e5144f3c4675860fc1677674d224a4f043`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b0b666a45f4b0619d873f8a797c2e1c0451a196871908efd2d3442c506e6ef`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b1a9d6f75e0d0123edeb268d2aa760548242a912592232d7b1d93ae8f9f1d6`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 6.5 MB (6516428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c189211552cdd321ae7bdf84cb5d708260161c01e43a0fb44dd068344bd7178e`  
		Last Modified: Tue, 05 May 2020 21:44:59 GMT  
		Size: 142.3 MB (142347625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bece8a5f214edeb3d4cb18eb23f42c557b8a6dc78be2e519ece4071aba7976`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fd35f5cfa69a7c2447e98e1679dab078ccb489807f4a139ee9630bf5210469`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 3.1 KB (3068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0`

```console
$ docker pull percona@sha256:b3db261ed6edbf136c51a8ca1c7859da8edad61ed3a3715a7c1f0aa965875e56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8.0` - linux; amd64

```console
$ docker pull percona@sha256:c07d08fb7357ff52e655550525a1d021dc679bf59589a1b50144cae6cd31e936
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.8 MB (224750500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e16910846759f931f0a0445c6266082091b036b21b0364ac1cc275b6c3fd2f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:39:07 GMT
RUN groupadd -g 1001 mysql
# Tue, 05 May 2020 21:39:08 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:39:13 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Tue, 05 May 2020 21:39:13 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Tue, 05 May 2020 21:40:05 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:40:06 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Tue, 05 May 2020 21:40:06 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:40:06 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:40:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:40:06 GMT
USER mysql
# Tue, 05 May 2020 21:40:07 GMT
EXPOSE 3306 33060
# Tue, 05 May 2020 21:40:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e386a719ceae0f0238e80a8fbcd5e5144f3c4675860fc1677674d224a4f043`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b0b666a45f4b0619d873f8a797c2e1c0451a196871908efd2d3442c506e6ef`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b1a9d6f75e0d0123edeb268d2aa760548242a912592232d7b1d93ae8f9f1d6`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 6.5 MB (6516428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c189211552cdd321ae7bdf84cb5d708260161c01e43a0fb44dd068344bd7178e`  
		Last Modified: Tue, 05 May 2020 21:44:59 GMT  
		Size: 142.3 MB (142347625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bece8a5f214edeb3d4cb18eb23f42c557b8a6dc78be2e519ece4071aba7976`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fd35f5cfa69a7c2447e98e1679dab078ccb489807f4a139ee9630bf5210469`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 3.1 KB (3068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0.19-10`

```console
$ docker pull percona@sha256:b3db261ed6edbf136c51a8ca1c7859da8edad61ed3a3715a7c1f0aa965875e56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8.0.19-10` - linux; amd64

```console
$ docker pull percona@sha256:c07d08fb7357ff52e655550525a1d021dc679bf59589a1b50144cae6cd31e936
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.8 MB (224750500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e16910846759f931f0a0445c6266082091b036b21b0364ac1cc275b6c3fd2f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:39:07 GMT
RUN groupadd -g 1001 mysql
# Tue, 05 May 2020 21:39:08 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:39:13 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Tue, 05 May 2020 21:39:13 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Tue, 05 May 2020 21:40:05 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:40:06 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Tue, 05 May 2020 21:40:06 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:40:06 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:40:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:40:06 GMT
USER mysql
# Tue, 05 May 2020 21:40:07 GMT
EXPOSE 3306 33060
# Tue, 05 May 2020 21:40:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e386a719ceae0f0238e80a8fbcd5e5144f3c4675860fc1677674d224a4f043`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b0b666a45f4b0619d873f8a797c2e1c0451a196871908efd2d3442c506e6ef`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b1a9d6f75e0d0123edeb268d2aa760548242a912592232d7b1d93ae8f9f1d6`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 6.5 MB (6516428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c189211552cdd321ae7bdf84cb5d708260161c01e43a0fb44dd068344bd7178e`  
		Last Modified: Tue, 05 May 2020 21:44:59 GMT  
		Size: 142.3 MB (142347625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bece8a5f214edeb3d4cb18eb23f42c557b8a6dc78be2e519ece4071aba7976`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fd35f5cfa69a7c2447e98e1679dab078ccb489807f4a139ee9630bf5210469`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 3.1 KB (3068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-3.6`

```console
$ docker pull percona@sha256:295d360a85dc46ee443cd340dfcadcbc406d119c29700784eb1c5afe8de37b26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6` - linux; amd64

```console
$ docker pull percona@sha256:5bb2e2fa02ba7570561ad727c5ad45b61986dcc88efbde3447cb4a904a1c08c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.0 MB (157035853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bb0898e4443c69e665418e86e273338005e2d89b1666a8ac7c9ffab515a3729`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:42:02 GMT
LABEL org.label-schema.schema-version=1.0
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.vendor=Percona
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.license=SSPLv1
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.vendor=Percona
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 26 May 2020 21:45:33 GMT
ENV PSMDB_VERSION=3.6.18-6.0
# Tue, 26 May 2020 21:45:34 GMT
LABEL org.label-schema.schema-version=3.6.18-6.0
# Tue, 26 May 2020 21:45:34 GMT
LABEL org.opencontainers.image.version=3.6.18-6.0
# Tue, 26 May 2020 21:45:40 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Tue, 26 May 2020 21:45:40 GMT
ENV OS_VER=el7
# Tue, 26 May 2020 21:45:41 GMT
ENV FULL_PERCONA_VERSION=3.6.18-6.0.el7
# Tue, 26 May 2020 21:45:41 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 02 Jul 2020 17:21:14 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-2.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-6.8.2-1.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Thu, 02 Jul 2020 17:21:32 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         yum-utils         shadow-utils         curl         procps-ng         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         yum clean all;         rm -rf /var/cache/yum /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Thu, 02 Jul 2020 17:21:32 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 02 Jul 2020 17:21:33 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 02 Jul 2020 17:21:33 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 02 Jul 2020 17:21:35 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 02 Jul 2020 17:21:36 GMT
VOLUME [/data/db]
# Thu, 02 Jul 2020 17:21:36 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Thu, 02 Jul 2020 17:21:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Jul 2020 17:21:36 GMT
EXPOSE 27017
# Thu, 02 Jul 2020 17:21:36 GMT
USER 1001
# Thu, 02 Jul 2020 17:21:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b9cf95a40ddab7409d772516d80954ddbf1ea23d0b61ad382f8cfc15eb086b`  
		Last Modified: Tue, 26 May 2020 21:47:12 GMT  
		Size: 6.5 MB (6470308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224b3b313dda5e5a1d45077b7a7380fe3616b6b1f9993a464b0f0742503a5ef6`  
		Last Modified: Thu, 02 Jul 2020 17:22:19 GMT  
		Size: 6.9 MB (6866852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e9f32fd306993d08b51cfbc4c17d20a137743d3d3633b37d9ccf7ef8ca5f28`  
		Last Modified: Thu, 02 Jul 2020 17:22:27 GMT  
		Size: 59.7 MB (59658881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e683bdb8b3e4e93c793d57b71c3a1ec06e4a2f0a41ab3d33917c1a6741f800ce`  
		Last Modified: Thu, 02 Jul 2020 17:22:16 GMT  
		Size: 1.6 KB (1593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e012d00cdfac70ed89214d6c727457048aa09261a226f16a77f672cd68d5ff0`  
		Last Modified: Thu, 02 Jul 2020 17:22:16 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f8729ed74d84ee001ebfad26a5c65e83ddfe7960e50404e021433067391c3a`  
		Last Modified: Thu, 02 Jul 2020 17:22:16 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6657db9ed2cf25bbd739123194bf42a6ea0a3e16e488add8ebb78fe01dcd61`  
		Last Modified: Thu, 02 Jul 2020 17:22:19 GMT  
		Size: 8.1 MB (8138884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91023628d75393aa573a82271a79e3d39e66c5ccd1dc62c683a51540e74a1407`  
		Last Modified: Thu, 02 Jul 2020 17:22:16 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-3.6.18`

```console
$ docker pull percona@sha256:295d360a85dc46ee443cd340dfcadcbc406d119c29700784eb1c5afe8de37b26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6.18` - linux; amd64

```console
$ docker pull percona@sha256:5bb2e2fa02ba7570561ad727c5ad45b61986dcc88efbde3447cb4a904a1c08c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.0 MB (157035853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bb0898e4443c69e665418e86e273338005e2d89b1666a8ac7c9ffab515a3729`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:42:02 GMT
LABEL org.label-schema.schema-version=1.0
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.vendor=Percona
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.license=SSPLv1
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.vendor=Percona
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 26 May 2020 21:45:33 GMT
ENV PSMDB_VERSION=3.6.18-6.0
# Tue, 26 May 2020 21:45:34 GMT
LABEL org.label-schema.schema-version=3.6.18-6.0
# Tue, 26 May 2020 21:45:34 GMT
LABEL org.opencontainers.image.version=3.6.18-6.0
# Tue, 26 May 2020 21:45:40 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Tue, 26 May 2020 21:45:40 GMT
ENV OS_VER=el7
# Tue, 26 May 2020 21:45:41 GMT
ENV FULL_PERCONA_VERSION=3.6.18-6.0.el7
# Tue, 26 May 2020 21:45:41 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 02 Jul 2020 17:21:14 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-2.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-6.8.2-1.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Thu, 02 Jul 2020 17:21:32 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         yum-utils         shadow-utils         curl         procps-ng         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         yum clean all;         rm -rf /var/cache/yum /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Thu, 02 Jul 2020 17:21:32 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 02 Jul 2020 17:21:33 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 02 Jul 2020 17:21:33 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 02 Jul 2020 17:21:35 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 02 Jul 2020 17:21:36 GMT
VOLUME [/data/db]
# Thu, 02 Jul 2020 17:21:36 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Thu, 02 Jul 2020 17:21:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Jul 2020 17:21:36 GMT
EXPOSE 27017
# Thu, 02 Jul 2020 17:21:36 GMT
USER 1001
# Thu, 02 Jul 2020 17:21:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b9cf95a40ddab7409d772516d80954ddbf1ea23d0b61ad382f8cfc15eb086b`  
		Last Modified: Tue, 26 May 2020 21:47:12 GMT  
		Size: 6.5 MB (6470308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224b3b313dda5e5a1d45077b7a7380fe3616b6b1f9993a464b0f0742503a5ef6`  
		Last Modified: Thu, 02 Jul 2020 17:22:19 GMT  
		Size: 6.9 MB (6866852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e9f32fd306993d08b51cfbc4c17d20a137743d3d3633b37d9ccf7ef8ca5f28`  
		Last Modified: Thu, 02 Jul 2020 17:22:27 GMT  
		Size: 59.7 MB (59658881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e683bdb8b3e4e93c793d57b71c3a1ec06e4a2f0a41ab3d33917c1a6741f800ce`  
		Last Modified: Thu, 02 Jul 2020 17:22:16 GMT  
		Size: 1.6 KB (1593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e012d00cdfac70ed89214d6c727457048aa09261a226f16a77f672cd68d5ff0`  
		Last Modified: Thu, 02 Jul 2020 17:22:16 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f8729ed74d84ee001ebfad26a5c65e83ddfe7960e50404e021433067391c3a`  
		Last Modified: Thu, 02 Jul 2020 17:22:16 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6657db9ed2cf25bbd739123194bf42a6ea0a3e16e488add8ebb78fe01dcd61`  
		Last Modified: Thu, 02 Jul 2020 17:22:19 GMT  
		Size: 8.1 MB (8138884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91023628d75393aa573a82271a79e3d39e66c5ccd1dc62c683a51540e74a1407`  
		Last Modified: Thu, 02 Jul 2020 17:22:16 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.0`

```console
$ docker pull percona@sha256:50b2f422b1f59d3281f53346503046ce76cb2091f3101f2d6ad564a783d87bd5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0` - linux; amd64

```console
$ docker pull percona@sha256:4c8f0f472d747dbe9abec92bd7755b0ca9dbdcff855422e0f1932d2c3629421d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.8 MB (159807459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:283525e93531b3c2ee68229bd61450f57f03847c11c5bfff8cd9c7d81c74f93d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:42:02 GMT
LABEL org.label-schema.schema-version=1.0
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.vendor=Percona
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.license=SSPLv1
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.vendor=Percona
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 02 Jul 2020 17:20:15 GMT
ENV PSMDB_VERSION=4.0.19-12
# Thu, 02 Jul 2020 17:20:15 GMT
LABEL org.label-schema.schema-version=4.0.19-12
# Thu, 02 Jul 2020 17:20:15 GMT
LABEL org.opencontainers.image.version=4.0.19-12
# Thu, 02 Jul 2020 17:20:20 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-40 release
# Thu, 02 Jul 2020 17:20:20 GMT
ENV OS_VER=el7
# Thu, 02 Jul 2020 17:20:20 GMT
ENV FULL_PERCONA_VERSION=4.0.19-12.el7
# Thu, 02 Jul 2020 17:20:20 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 02 Jul 2020 17:20:25 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-2.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-6.8.2-1.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Thu, 02 Jul 2020 17:20:57 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 02 Jul 2020 17:20:57 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 02 Jul 2020 17:20:58 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 02 Jul 2020 17:20:58 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 02 Jul 2020 17:20:59 GMT
ENV GOSU_VERSION=1.11
# Thu, 02 Jul 2020 17:21:02 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 02 Jul 2020 17:21:04 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 02 Jul 2020 17:21:04 GMT
VOLUME [/data/db]
# Thu, 02 Jul 2020 17:21:04 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Thu, 02 Jul 2020 17:21:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Jul 2020 17:21:05 GMT
EXPOSE 27017
# Thu, 02 Jul 2020 17:21:05 GMT
USER 1001
# Thu, 02 Jul 2020 17:21:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5109611112125f79258a9f8d59c3ef11256cc2d34cdd8e1ebb9633d218bbdf08`  
		Last Modified: Thu, 02 Jul 2020 17:22:02 GMT  
		Size: 6.5 MB (6471413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018ff6fd1bd6bd93645c4e94b8a1ba0375eb0c9d95e74d7b77a38efe80fcd229`  
		Last Modified: Thu, 02 Jul 2020 17:22:02 GMT  
		Size: 6.9 MB (6867143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071041a0d2c46a1358a0c5c369b0f3796aca1a81cbdad7796ec7548d91435e17`  
		Last Modified: Thu, 02 Jul 2020 17:22:11 GMT  
		Size: 61.5 MB (61513630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ad5af3fc92236f0711c1051eaec699bcaaabba482bc0282b9fede2af93e209`  
		Last Modified: Thu, 02 Jul 2020 17:22:00 GMT  
		Size: 1.6 KB (1594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35750ebe5d0f1e9bc83635cd6642c1ff83bb20fb0bb9a27e16d1b024fa276609`  
		Last Modified: Thu, 02 Jul 2020 17:21:59 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d0904fab10023a2e21d916489eed4462bf884ed282ccc48e955adbf17ec208`  
		Last Modified: Thu, 02 Jul 2020 17:21:59 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c132430f30e0ce4bc221e0fcf7602010dad8fc66a0aae599a53f608b5daf39`  
		Last Modified: Thu, 02 Jul 2020 17:22:00 GMT  
		Size: 915.5 KB (915466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c37bfbfe55ca6cf935126e6c298df8654b7bece6811e1f673c9e09f27253e2`  
		Last Modified: Thu, 02 Jul 2020 17:22:01 GMT  
		Size: 8.1 MB (8138879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2485e5ab8ac8154cb077075aa9c2b59a46d2c76fe2898dbf5d8bce634fe3f926`  
		Last Modified: Thu, 02 Jul 2020 17:22:00 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.0.19`

```console
$ docker pull percona@sha256:50b2f422b1f59d3281f53346503046ce76cb2091f3101f2d6ad564a783d87bd5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0.19` - linux; amd64

```console
$ docker pull percona@sha256:4c8f0f472d747dbe9abec92bd7755b0ca9dbdcff855422e0f1932d2c3629421d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.8 MB (159807459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:283525e93531b3c2ee68229bd61450f57f03847c11c5bfff8cd9c7d81c74f93d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:42:02 GMT
LABEL org.label-schema.schema-version=1.0
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.vendor=Percona
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.license=SSPLv1
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.vendor=Percona
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 02 Jul 2020 17:20:15 GMT
ENV PSMDB_VERSION=4.0.19-12
# Thu, 02 Jul 2020 17:20:15 GMT
LABEL org.label-schema.schema-version=4.0.19-12
# Thu, 02 Jul 2020 17:20:15 GMT
LABEL org.opencontainers.image.version=4.0.19-12
# Thu, 02 Jul 2020 17:20:20 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-40 release
# Thu, 02 Jul 2020 17:20:20 GMT
ENV OS_VER=el7
# Thu, 02 Jul 2020 17:20:20 GMT
ENV FULL_PERCONA_VERSION=4.0.19-12.el7
# Thu, 02 Jul 2020 17:20:20 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 02 Jul 2020 17:20:25 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-2.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-6.8.2-1.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Thu, 02 Jul 2020 17:20:57 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 02 Jul 2020 17:20:57 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 02 Jul 2020 17:20:58 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 02 Jul 2020 17:20:58 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 02 Jul 2020 17:20:59 GMT
ENV GOSU_VERSION=1.11
# Thu, 02 Jul 2020 17:21:02 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 02 Jul 2020 17:21:04 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 02 Jul 2020 17:21:04 GMT
VOLUME [/data/db]
# Thu, 02 Jul 2020 17:21:04 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Thu, 02 Jul 2020 17:21:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Jul 2020 17:21:05 GMT
EXPOSE 27017
# Thu, 02 Jul 2020 17:21:05 GMT
USER 1001
# Thu, 02 Jul 2020 17:21:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5109611112125f79258a9f8d59c3ef11256cc2d34cdd8e1ebb9633d218bbdf08`  
		Last Modified: Thu, 02 Jul 2020 17:22:02 GMT  
		Size: 6.5 MB (6471413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018ff6fd1bd6bd93645c4e94b8a1ba0375eb0c9d95e74d7b77a38efe80fcd229`  
		Last Modified: Thu, 02 Jul 2020 17:22:02 GMT  
		Size: 6.9 MB (6867143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071041a0d2c46a1358a0c5c369b0f3796aca1a81cbdad7796ec7548d91435e17`  
		Last Modified: Thu, 02 Jul 2020 17:22:11 GMT  
		Size: 61.5 MB (61513630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ad5af3fc92236f0711c1051eaec699bcaaabba482bc0282b9fede2af93e209`  
		Last Modified: Thu, 02 Jul 2020 17:22:00 GMT  
		Size: 1.6 KB (1594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35750ebe5d0f1e9bc83635cd6642c1ff83bb20fb0bb9a27e16d1b024fa276609`  
		Last Modified: Thu, 02 Jul 2020 17:21:59 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d0904fab10023a2e21d916489eed4462bf884ed282ccc48e955adbf17ec208`  
		Last Modified: Thu, 02 Jul 2020 17:21:59 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c132430f30e0ce4bc221e0fcf7602010dad8fc66a0aae599a53f608b5daf39`  
		Last Modified: Thu, 02 Jul 2020 17:22:00 GMT  
		Size: 915.5 KB (915466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c37bfbfe55ca6cf935126e6c298df8654b7bece6811e1f673c9e09f27253e2`  
		Last Modified: Thu, 02 Jul 2020 17:22:01 GMT  
		Size: 8.1 MB (8138879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2485e5ab8ac8154cb077075aa9c2b59a46d2c76fe2898dbf5d8bce634fe3f926`  
		Last Modified: Thu, 02 Jul 2020 17:22:00 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:02293d5f6a43a9d7cde3200e73854acd9a08cc77ff57d88718fbf4fec1db3afa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:fdb21fdecc16eafdc382732b0b96837308fb17dbd96fe941fbcdce205ecf82a8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.3 MB (169297374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:126f7492bd259800f80428214feccc04c175599bcec0f4f65fa224bbb4f9b3a8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:42:02 GMT
LABEL org.label-schema.schema-version=1.0
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.vendor=Percona
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.license=SSPLv1
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.vendor=Percona
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 01 Jul 2020 20:27:04 GMT
ENV PSMDB_VERSION=4.2.7-7
# Wed, 01 Jul 2020 20:27:04 GMT
LABEL org.label-schema.schema-version=4.2.7-7
# Wed, 01 Jul 2020 20:27:05 GMT
LABEL org.opencontainers.image.version=4.2.7-7
# Wed, 01 Jul 2020 20:27:08 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Wed, 01 Jul 2020 20:27:09 GMT
ENV OS_VER=el7
# Wed, 01 Jul 2020 20:27:09 GMT
ENV FULL_PERCONA_VERSION=4.2.7-7.el7
# Wed, 01 Jul 2020 20:27:09 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 01 Jul 2020 20:27:14 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-2.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-6.8.2-1.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Wed, 01 Jul 2020 20:27:32 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 01 Jul 2020 20:27:33 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 01 Jul 2020 20:27:33 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 01 Jul 2020 20:27:34 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 01 Jul 2020 20:27:34 GMT
ENV GOSU_VERSION=1.11
# Wed, 01 Jul 2020 20:27:37 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 01 Jul 2020 20:27:39 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 01 Jul 2020 20:27:40 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Wed, 01 Jul 2020 20:27:40 GMT
VOLUME [/data/db]
# Wed, 01 Jul 2020 20:27:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Jul 2020 20:27:40 GMT
EXPOSE 27017
# Wed, 01 Jul 2020 20:27:40 GMT
USER 1001
# Wed, 01 Jul 2020 20:27:40 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d1ce653b81ece6d11af560aaea7a08f5e552ab43800a79fcedae22b0a79bf8`  
		Last Modified: Wed, 01 Jul 2020 20:28:13 GMT  
		Size: 6.5 MB (6471394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a644eb356b623127e483caff86aa558ba1ede3b3ba3a88c00d52790cc7d11bf`  
		Last Modified: Wed, 01 Jul 2020 20:28:13 GMT  
		Size: 6.9 MB (6867115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc51a77ad81b3e577ecef08e7c8424dd8e3ac16bacb8a8b787d80bd8bc70f8b`  
		Last Modified: Wed, 01 Jul 2020 20:28:22 GMT  
		Size: 71.0 MB (71003594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e1b53b03836d26a6c5d70eb317ba29c49663b342afe928c99ef7bad920da36`  
		Last Modified: Wed, 01 Jul 2020 20:28:11 GMT  
		Size: 1.6 KB (1594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a766cc4af2ba963516f749a604017cdece299421290c4bddd8b2a5214b0eb10`  
		Last Modified: Wed, 01 Jul 2020 20:28:10 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898761a0ffa617e0546fc54e170b66ecadaa01b7f5547f705bcda115466fe4d0`  
		Last Modified: Wed, 01 Jul 2020 20:28:10 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3101fd52a1462b4f6a72faebb1fb17b694a55f7866414be5f5b3b2ce8b8bcf4f`  
		Last Modified: Wed, 01 Jul 2020 20:28:10 GMT  
		Size: 915.5 KB (915475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289454960c62601b11ed927825f26c416dbf55565a9a56b1b9f1721cd3b424c3`  
		Last Modified: Wed, 01 Jul 2020 20:28:11 GMT  
		Size: 8.1 MB (8138868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7345a9fd40f5a4ba408527d14f0db6694d25526ad9478e4649664730347aa3d5`  
		Last Modified: Wed, 01 Jul 2020 20:28:10 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2.8`

```console
$ docker pull percona@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
