<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `percona`

-	[`percona:5`](#percona5)
-	[`percona:5.6`](#percona56)
-	[`percona:5.6.48`](#percona5648)
-	[`percona:5.6.48-centos`](#percona5648-centos)
-	[`percona:5.6-centos`](#percona56-centos)
-	[`percona:5.7`](#percona57)
-	[`percona:5.7.29`](#percona5729)
-	[`percona:5.7.29-centos`](#percona5729-centos)
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
-	[`percona:ps-5.7.29`](#perconaps-5729)
-	[`percona:ps-8`](#perconaps-8)
-	[`percona:ps-8.0`](#perconaps-80)
-	[`percona:ps-8.0.19-10`](#perconaps-8019-10)
-	[`percona:psmdb-3.6`](#perconapsmdb-36)
-	[`percona:psmdb-3.6.17`](#perconapsmdb-3617)
-	[`percona:psmdb-4.0`](#perconapsmdb-40)
-	[`percona:psmdb-4.0.18`](#perconapsmdb-4018)
-	[`percona:psmdb-4.2`](#perconapsmdb-42)
-	[`percona:psmdb-4.2.6`](#perconapsmdb-426)

## `percona:5`

```console
$ docker pull percona@sha256:ad09adc6c7179c60ef79a831a22172676fe19f0ad01111e99247a989a49484bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5` - linux; amd64

```console
$ docker pull percona@sha256:9e0c1812c84554d9c06485f7f0050f0b3c8ba9630864f696350a87a0be47253b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196705657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9f9dd11707cb77cd23cce00a3f1182d3b117316f5da73c67d382897ba60df0`
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
# Tue, 05 May 2020 21:40:17 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Tue, 05 May 2020 21:41:09 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:41:10 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 05 May 2020 21:41:10 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:41:10 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:41:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:41:11 GMT
USER mysql
# Tue, 05 May 2020 21:41:11 GMT
EXPOSE 3306
# Tue, 05 May 2020 21:41:11 GMT
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
	-	`sha256:39b3f573e662710378c7bb060bd6cff06c2351252b3d8d6ec0a330e7c9a138e1`  
		Last Modified: Tue, 05 May 2020 21:45:31 GMT  
		Size: 114.3 MB (114302691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd56ff0ce5034969f0eedf05ab222c5ac4f23de06a09e8f41a7e02a8c5a99638`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94441704ff25f1414e9417d23d9de95c22f9a3e7f37bb49652ceda306e4df5be`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
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
$ docker pull percona@sha256:ad09adc6c7179c60ef79a831a22172676fe19f0ad01111e99247a989a49484bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7` - linux; amd64

```console
$ docker pull percona@sha256:9e0c1812c84554d9c06485f7f0050f0b3c8ba9630864f696350a87a0be47253b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196705657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9f9dd11707cb77cd23cce00a3f1182d3b117316f5da73c67d382897ba60df0`
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
# Tue, 05 May 2020 21:40:17 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Tue, 05 May 2020 21:41:09 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:41:10 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 05 May 2020 21:41:10 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:41:10 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:41:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:41:11 GMT
USER mysql
# Tue, 05 May 2020 21:41:11 GMT
EXPOSE 3306
# Tue, 05 May 2020 21:41:11 GMT
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
	-	`sha256:39b3f573e662710378c7bb060bd6cff06c2351252b3d8d6ec0a330e7c9a138e1`  
		Last Modified: Tue, 05 May 2020 21:45:31 GMT  
		Size: 114.3 MB (114302691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd56ff0ce5034969f0eedf05ab222c5ac4f23de06a09e8f41a7e02a8c5a99638`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94441704ff25f1414e9417d23d9de95c22f9a3e7f37bb49652ceda306e4df5be`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.29`

```console
$ docker pull percona@sha256:ad09adc6c7179c60ef79a831a22172676fe19f0ad01111e99247a989a49484bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7.29` - linux; amd64

```console
$ docker pull percona@sha256:9e0c1812c84554d9c06485f7f0050f0b3c8ba9630864f696350a87a0be47253b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196705657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9f9dd11707cb77cd23cce00a3f1182d3b117316f5da73c67d382897ba60df0`
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
# Tue, 05 May 2020 21:40:17 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Tue, 05 May 2020 21:41:09 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:41:10 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 05 May 2020 21:41:10 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:41:10 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:41:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:41:11 GMT
USER mysql
# Tue, 05 May 2020 21:41:11 GMT
EXPOSE 3306
# Tue, 05 May 2020 21:41:11 GMT
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
	-	`sha256:39b3f573e662710378c7bb060bd6cff06c2351252b3d8d6ec0a330e7c9a138e1`  
		Last Modified: Tue, 05 May 2020 21:45:31 GMT  
		Size: 114.3 MB (114302691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd56ff0ce5034969f0eedf05ab222c5ac4f23de06a09e8f41a7e02a8c5a99638`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94441704ff25f1414e9417d23d9de95c22f9a3e7f37bb49652ceda306e4df5be`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.29-centos`

```console
$ docker pull percona@sha256:ad09adc6c7179c60ef79a831a22172676fe19f0ad01111e99247a989a49484bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7.29-centos` - linux; amd64

```console
$ docker pull percona@sha256:9e0c1812c84554d9c06485f7f0050f0b3c8ba9630864f696350a87a0be47253b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196705657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9f9dd11707cb77cd23cce00a3f1182d3b117316f5da73c67d382897ba60df0`
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
# Tue, 05 May 2020 21:40:17 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Tue, 05 May 2020 21:41:09 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:41:10 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 05 May 2020 21:41:10 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:41:10 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:41:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:41:11 GMT
USER mysql
# Tue, 05 May 2020 21:41:11 GMT
EXPOSE 3306
# Tue, 05 May 2020 21:41:11 GMT
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
	-	`sha256:39b3f573e662710378c7bb060bd6cff06c2351252b3d8d6ec0a330e7c9a138e1`  
		Last Modified: Tue, 05 May 2020 21:45:31 GMT  
		Size: 114.3 MB (114302691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd56ff0ce5034969f0eedf05ab222c5ac4f23de06a09e8f41a7e02a8c5a99638`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94441704ff25f1414e9417d23d9de95c22f9a3e7f37bb49652ceda306e4df5be`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7-centos`

```console
$ docker pull percona@sha256:ad09adc6c7179c60ef79a831a22172676fe19f0ad01111e99247a989a49484bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7-centos` - linux; amd64

```console
$ docker pull percona@sha256:9e0c1812c84554d9c06485f7f0050f0b3c8ba9630864f696350a87a0be47253b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196705657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9f9dd11707cb77cd23cce00a3f1182d3b117316f5da73c67d382897ba60df0`
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
# Tue, 05 May 2020 21:40:17 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Tue, 05 May 2020 21:41:09 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:41:10 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 05 May 2020 21:41:10 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:41:10 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:41:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:41:11 GMT
USER mysql
# Tue, 05 May 2020 21:41:11 GMT
EXPOSE 3306
# Tue, 05 May 2020 21:41:11 GMT
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
	-	`sha256:39b3f573e662710378c7bb060bd6cff06c2351252b3d8d6ec0a330e7c9a138e1`  
		Last Modified: Tue, 05 May 2020 21:45:31 GMT  
		Size: 114.3 MB (114302691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd56ff0ce5034969f0eedf05ab222c5ac4f23de06a09e8f41a7e02a8c5a99638`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94441704ff25f1414e9417d23d9de95c22f9a3e7f37bb49652ceda306e4df5be`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5-centos`

```console
$ docker pull percona@sha256:ad09adc6c7179c60ef79a831a22172676fe19f0ad01111e99247a989a49484bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5-centos` - linux; amd64

```console
$ docker pull percona@sha256:9e0c1812c84554d9c06485f7f0050f0b3c8ba9630864f696350a87a0be47253b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196705657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9f9dd11707cb77cd23cce00a3f1182d3b117316f5da73c67d382897ba60df0`
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
# Tue, 05 May 2020 21:40:17 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Tue, 05 May 2020 21:41:09 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:41:10 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 05 May 2020 21:41:10 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:41:10 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:41:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:41:11 GMT
USER mysql
# Tue, 05 May 2020 21:41:11 GMT
EXPOSE 3306
# Tue, 05 May 2020 21:41:11 GMT
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
	-	`sha256:39b3f573e662710378c7bb060bd6cff06c2351252b3d8d6ec0a330e7c9a138e1`  
		Last Modified: Tue, 05 May 2020 21:45:31 GMT  
		Size: 114.3 MB (114302691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd56ff0ce5034969f0eedf05ab222c5ac4f23de06a09e8f41a7e02a8c5a99638`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94441704ff25f1414e9417d23d9de95c22f9a3e7f37bb49652ceda306e4df5be`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
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
$ docker pull percona@sha256:ad09adc6c7179c60ef79a831a22172676fe19f0ad01111e99247a989a49484bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:centos` - linux; amd64

```console
$ docker pull percona@sha256:9e0c1812c84554d9c06485f7f0050f0b3c8ba9630864f696350a87a0be47253b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196705657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9f9dd11707cb77cd23cce00a3f1182d3b117316f5da73c67d382897ba60df0`
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
# Tue, 05 May 2020 21:40:17 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Tue, 05 May 2020 21:41:09 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:41:10 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 05 May 2020 21:41:10 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:41:10 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:41:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:41:11 GMT
USER mysql
# Tue, 05 May 2020 21:41:11 GMT
EXPOSE 3306
# Tue, 05 May 2020 21:41:11 GMT
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
	-	`sha256:39b3f573e662710378c7bb060bd6cff06c2351252b3d8d6ec0a330e7c9a138e1`  
		Last Modified: Tue, 05 May 2020 21:45:31 GMT  
		Size: 114.3 MB (114302691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd56ff0ce5034969f0eedf05ab222c5ac4f23de06a09e8f41a7e02a8c5a99638`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94441704ff25f1414e9417d23d9de95c22f9a3e7f37bb49652ceda306e4df5be`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:latest`

```console
$ docker pull percona@sha256:ad09adc6c7179c60ef79a831a22172676fe19f0ad01111e99247a989a49484bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:latest` - linux; amd64

```console
$ docker pull percona@sha256:9e0c1812c84554d9c06485f7f0050f0b3c8ba9630864f696350a87a0be47253b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196705657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9f9dd11707cb77cd23cce00a3f1182d3b117316f5da73c67d382897ba60df0`
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
# Tue, 05 May 2020 21:40:17 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Tue, 05 May 2020 21:41:09 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:41:10 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 05 May 2020 21:41:10 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:41:10 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:41:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:41:11 GMT
USER mysql
# Tue, 05 May 2020 21:41:11 GMT
EXPOSE 3306
# Tue, 05 May 2020 21:41:11 GMT
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
	-	`sha256:39b3f573e662710378c7bb060bd6cff06c2351252b3d8d6ec0a330e7c9a138e1`  
		Last Modified: Tue, 05 May 2020 21:45:31 GMT  
		Size: 114.3 MB (114302691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd56ff0ce5034969f0eedf05ab222c5ac4f23de06a09e8f41a7e02a8c5a99638`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94441704ff25f1414e9417d23d9de95c22f9a3e7f37bb49652ceda306e4df5be`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5`

```console
$ docker pull percona@sha256:ad09adc6c7179c60ef79a831a22172676fe19f0ad01111e99247a989a49484bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5` - linux; amd64

```console
$ docker pull percona@sha256:9e0c1812c84554d9c06485f7f0050f0b3c8ba9630864f696350a87a0be47253b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196705657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9f9dd11707cb77cd23cce00a3f1182d3b117316f5da73c67d382897ba60df0`
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
# Tue, 05 May 2020 21:40:17 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Tue, 05 May 2020 21:41:09 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:41:10 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 05 May 2020 21:41:10 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:41:10 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:41:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:41:11 GMT
USER mysql
# Tue, 05 May 2020 21:41:11 GMT
EXPOSE 3306
# Tue, 05 May 2020 21:41:11 GMT
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
	-	`sha256:39b3f573e662710378c7bb060bd6cff06c2351252b3d8d6ec0a330e7c9a138e1`  
		Last Modified: Tue, 05 May 2020 21:45:31 GMT  
		Size: 114.3 MB (114302691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd56ff0ce5034969f0eedf05ab222c5ac4f23de06a09e8f41a7e02a8c5a99638`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94441704ff25f1414e9417d23d9de95c22f9a3e7f37bb49652ceda306e4df5be`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
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
$ docker pull percona@sha256:ad09adc6c7179c60ef79a831a22172676fe19f0ad01111e99247a989a49484bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.7` - linux; amd64

```console
$ docker pull percona@sha256:9e0c1812c84554d9c06485f7f0050f0b3c8ba9630864f696350a87a0be47253b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196705657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9f9dd11707cb77cd23cce00a3f1182d3b117316f5da73c67d382897ba60df0`
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
# Tue, 05 May 2020 21:40:17 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Tue, 05 May 2020 21:41:09 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:41:10 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 05 May 2020 21:41:10 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:41:10 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:41:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:41:11 GMT
USER mysql
# Tue, 05 May 2020 21:41:11 GMT
EXPOSE 3306
# Tue, 05 May 2020 21:41:11 GMT
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
	-	`sha256:39b3f573e662710378c7bb060bd6cff06c2351252b3d8d6ec0a330e7c9a138e1`  
		Last Modified: Tue, 05 May 2020 21:45:31 GMT  
		Size: 114.3 MB (114302691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd56ff0ce5034969f0eedf05ab222c5ac4f23de06a09e8f41a7e02a8c5a99638`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94441704ff25f1414e9417d23d9de95c22f9a3e7f37bb49652ceda306e4df5be`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.7.29`

```console
$ docker pull percona@sha256:ad09adc6c7179c60ef79a831a22172676fe19f0ad01111e99247a989a49484bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.7.29` - linux; amd64

```console
$ docker pull percona@sha256:9e0c1812c84554d9c06485f7f0050f0b3c8ba9630864f696350a87a0be47253b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196705657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9f9dd11707cb77cd23cce00a3f1182d3b117316f5da73c67d382897ba60df0`
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
# Tue, 05 May 2020 21:40:17 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Tue, 05 May 2020 21:41:09 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:41:10 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 05 May 2020 21:41:10 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:41:10 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:41:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:41:11 GMT
USER mysql
# Tue, 05 May 2020 21:41:11 GMT
EXPOSE 3306
# Tue, 05 May 2020 21:41:11 GMT
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
	-	`sha256:39b3f573e662710378c7bb060bd6cff06c2351252b3d8d6ec0a330e7c9a138e1`  
		Last Modified: Tue, 05 May 2020 21:45:31 GMT  
		Size: 114.3 MB (114302691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd56ff0ce5034969f0eedf05ab222c5ac4f23de06a09e8f41a7e02a8c5a99638`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94441704ff25f1414e9417d23d9de95c22f9a3e7f37bb49652ceda306e4df5be`  
		Last Modified: Tue, 05 May 2020 21:45:08 GMT  
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
$ docker pull percona@sha256:2809665b23882260d404ed5029174578ddb41074c81960ea0a81c068cca546e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6` - linux; amd64

```console
$ docker pull percona@sha256:30881f6296629af25e09caafcf322ace88adc81798be7feeb7b92c50088cad75
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.8 MB (155843783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28fb287b76168d4d12c8a0058ecc18a1389a4b11c116aaed47cbadc177969259`
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
# Tue, 05 May 2020 21:44:02 GMT
ENV PSMDB_VERSION=3.6.17-4.0
# Tue, 05 May 2020 21:44:02 GMT
LABEL org.label-schema.schema-version=3.6.17-4.0
# Tue, 05 May 2020 21:44:03 GMT
LABEL org.opencontainers.image.version=3.6.17-4.0
# Thu, 07 May 2020 15:24:42 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Thu, 07 May 2020 15:24:42 GMT
ENV OS_VER=el7
# Thu, 07 May 2020 15:24:42 GMT
ENV FULL_PERCONA_VERSION=3.6.17-4.0.el7
# Thu, 07 May 2020 15:24:42 GMT
ENV K8S_TOOLS_VERSION=0.4.2
# Thu, 07 May 2020 15:24:47 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Thu, 07 May 2020 15:25:02 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         yum-utils         shadow-utils         curl         procps-ng         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         yum clean all;         rm -rf /var/cache/yum /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Thu, 07 May 2020 15:25:03 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 07 May 2020 15:25:03 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 07 May 2020 15:25:04 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 07 May 2020 15:25:07 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 07 May 2020 15:25:07 GMT
VOLUME [/data/db]
# Thu, 07 May 2020 15:25:07 GMT
COPY file:85995e73e1e4d284ba65fabe65ed1e96fcb9c00ac0d328edb8b0b48749d784e1 in /entrypoint.sh 
# Thu, 07 May 2020 15:25:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 May 2020 15:25:07 GMT
EXPOSE 27017
# Thu, 07 May 2020 15:25:07 GMT
USER 1001
# Thu, 07 May 2020 15:25:08 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e85f6335b4e175d44877c04effca1678100667be75f6bab34c7c1020f4c4c8e`  
		Last Modified: Thu, 07 May 2020 15:26:12 GMT  
		Size: 6.5 MB (6473599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f344f549d4c54e18420478303e3e8b316108fffb013b1433d48cda03dfc2e1`  
		Last Modified: Thu, 07 May 2020 15:26:12 GMT  
		Size: 6.8 MB (6793353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4490737f1854e4f6d597f253fa676c32a4a64850512a3946774e6e88c23a13cf`  
		Last Modified: Thu, 07 May 2020 15:26:21 GMT  
		Size: 59.1 MB (59111061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5be1cf33c18826c987905d9f6ba37265978192115b82092e929dc36fc54964`  
		Last Modified: Thu, 07 May 2020 15:26:10 GMT  
		Size: 1.6 KB (1590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e695c63b00402297daa0c92b0da1e349e0f3fc19f3cabc3ddb8f71e515efd07d`  
		Last Modified: Thu, 07 May 2020 15:26:09 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739f4339123e72bd213aad08c2d989fce57f3e5255700aaebb8687085a49f0bd`  
		Last Modified: Thu, 07 May 2020 15:26:10 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77dcb5be1c090f7f0db605d465b64b06ba6259033026eb9f6b4aaffeacecd3ed`  
		Last Modified: Thu, 07 May 2020 15:26:11 GMT  
		Size: 7.6 MB (7565367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720cae703f9183a8b0b3a8b391b07a88b0bda9065a825b8fc10a245a93fccc1c`  
		Last Modified: Thu, 07 May 2020 15:26:09 GMT  
		Size: 4.0 KB (4018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-3.6.17`

```console
$ docker pull percona@sha256:2809665b23882260d404ed5029174578ddb41074c81960ea0a81c068cca546e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6.17` - linux; amd64

```console
$ docker pull percona@sha256:30881f6296629af25e09caafcf322ace88adc81798be7feeb7b92c50088cad75
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.8 MB (155843783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28fb287b76168d4d12c8a0058ecc18a1389a4b11c116aaed47cbadc177969259`
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
# Tue, 05 May 2020 21:44:02 GMT
ENV PSMDB_VERSION=3.6.17-4.0
# Tue, 05 May 2020 21:44:02 GMT
LABEL org.label-schema.schema-version=3.6.17-4.0
# Tue, 05 May 2020 21:44:03 GMT
LABEL org.opencontainers.image.version=3.6.17-4.0
# Thu, 07 May 2020 15:24:42 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Thu, 07 May 2020 15:24:42 GMT
ENV OS_VER=el7
# Thu, 07 May 2020 15:24:42 GMT
ENV FULL_PERCONA_VERSION=3.6.17-4.0.el7
# Thu, 07 May 2020 15:24:42 GMT
ENV K8S_TOOLS_VERSION=0.4.2
# Thu, 07 May 2020 15:24:47 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Thu, 07 May 2020 15:25:02 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         yum-utils         shadow-utils         curl         procps-ng         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         yum clean all;         rm -rf /var/cache/yum /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Thu, 07 May 2020 15:25:03 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 07 May 2020 15:25:03 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 07 May 2020 15:25:04 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 07 May 2020 15:25:07 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 07 May 2020 15:25:07 GMT
VOLUME [/data/db]
# Thu, 07 May 2020 15:25:07 GMT
COPY file:85995e73e1e4d284ba65fabe65ed1e96fcb9c00ac0d328edb8b0b48749d784e1 in /entrypoint.sh 
# Thu, 07 May 2020 15:25:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 May 2020 15:25:07 GMT
EXPOSE 27017
# Thu, 07 May 2020 15:25:07 GMT
USER 1001
# Thu, 07 May 2020 15:25:08 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e85f6335b4e175d44877c04effca1678100667be75f6bab34c7c1020f4c4c8e`  
		Last Modified: Thu, 07 May 2020 15:26:12 GMT  
		Size: 6.5 MB (6473599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f344f549d4c54e18420478303e3e8b316108fffb013b1433d48cda03dfc2e1`  
		Last Modified: Thu, 07 May 2020 15:26:12 GMT  
		Size: 6.8 MB (6793353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4490737f1854e4f6d597f253fa676c32a4a64850512a3946774e6e88c23a13cf`  
		Last Modified: Thu, 07 May 2020 15:26:21 GMT  
		Size: 59.1 MB (59111061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5be1cf33c18826c987905d9f6ba37265978192115b82092e929dc36fc54964`  
		Last Modified: Thu, 07 May 2020 15:26:10 GMT  
		Size: 1.6 KB (1590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e695c63b00402297daa0c92b0da1e349e0f3fc19f3cabc3ddb8f71e515efd07d`  
		Last Modified: Thu, 07 May 2020 15:26:09 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739f4339123e72bd213aad08c2d989fce57f3e5255700aaebb8687085a49f0bd`  
		Last Modified: Thu, 07 May 2020 15:26:10 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77dcb5be1c090f7f0db605d465b64b06ba6259033026eb9f6b4aaffeacecd3ed`  
		Last Modified: Thu, 07 May 2020 15:26:11 GMT  
		Size: 7.6 MB (7565367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720cae703f9183a8b0b3a8b391b07a88b0bda9065a825b8fc10a245a93fccc1c`  
		Last Modified: Thu, 07 May 2020 15:26:09 GMT  
		Size: 4.0 KB (4018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.0`

```console
$ docker pull percona@sha256:858cece41a236cf1d2f3e47725986ce0d97042a176f7bd079dc556372bf3bd85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0` - linux; amd64

```console
$ docker pull percona@sha256:80e07baf5281aee9c7dbef10ab3ba16c255b1cfd59da4f3eb56043af4202d371
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159591752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc4e728b52c8c22db189eb0089bbc352285899f5679aa611c5720b33b761aa63`
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
# Tue, 05 May 2020 21:42:45 GMT
ENV PSMDB_VERSION=4.0.18-11
# Tue, 05 May 2020 21:42:45 GMT
LABEL org.label-schema.schema-version=4.0.18-11
# Tue, 05 May 2020 21:42:45 GMT
LABEL org.opencontainers.image.version=4.0.18-11
# Thu, 07 May 2020 15:23:55 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-40 release
# Thu, 07 May 2020 15:23:55 GMT
ENV OS_VER=el7
# Thu, 07 May 2020 15:23:55 GMT
ENV FULL_PERCONA_VERSION=4.0.18-11.el7
# Thu, 07 May 2020 15:23:55 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 07 May 2020 15:24:00 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Thu, 07 May 2020 15:24:21 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 07 May 2020 15:24:22 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 07 May 2020 15:24:22 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 07 May 2020 15:24:23 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 07 May 2020 15:24:23 GMT
ENV GOSU_VERSION=1.11
# Thu, 07 May 2020 15:24:25 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 07 May 2020 15:24:28 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 07 May 2020 15:24:28 GMT
VOLUME [/data/db]
# Thu, 07 May 2020 15:24:28 GMT
COPY file:85995e73e1e4d284ba65fabe65ed1e96fcb9c00ac0d328edb8b0b48749d784e1 in /entrypoint.sh 
# Thu, 07 May 2020 15:24:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 May 2020 15:24:28 GMT
EXPOSE 27017
# Thu, 07 May 2020 15:24:29 GMT
USER 1001
# Thu, 07 May 2020 15:24:29 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ef9694f9631625a207bc725faca3127a8ff35730902838e9a6abe87760976b`  
		Last Modified: Thu, 07 May 2020 15:25:57 GMT  
		Size: 6.5 MB (6473844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c090ee9f40168b3f1e02cab71dbdb98f5282323a3fb0e7e1e022f3a0fe206b3`  
		Last Modified: Thu, 07 May 2020 15:26:03 GMT  
		Size: 6.8 MB (6793460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28accaa4c1bd9b3980f653c28e9a37a3394cce169baf819e49ea4acabfb04df8`  
		Last Modified: Thu, 07 May 2020 15:26:04 GMT  
		Size: 61.4 MB (61369701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4843ab4a75920f4caee8e545c0f0e664fcdbd9ef7372f559b958597fd04b2c6d`  
		Last Modified: Thu, 07 May 2020 15:25:54 GMT  
		Size: 1.6 KB (1593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d257afe58b55969ab10706dc55a93ac54010da57deb9c4af306a251d6236925`  
		Last Modified: Thu, 07 May 2020 15:25:54 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c9c127156ef0d6de2adb4cd687e3b56f19d1c341968753c0950f88ef6afb7f`  
		Last Modified: Thu, 07 May 2020 15:25:53 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5a5230fc4604c86229dbffbfb83f76fb80d9fc1a4b41495dd562ef11da03da`  
		Last Modified: Thu, 07 May 2020 15:25:53 GMT  
		Size: 915.5 KB (915466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28aee8f4cb87a72bc035b25f229b41479c85aa80b527acafad67ae0bafc3d77`  
		Last Modified: Thu, 07 May 2020 15:25:55 GMT  
		Size: 8.1 MB (8138878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f63a22e3ee4b85af09baafe7bdc08652750ce0ee09df042b88832446b8f321`  
		Last Modified: Thu, 07 May 2020 15:25:53 GMT  
		Size: 4.0 KB (4017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.0.18`

```console
$ docker pull percona@sha256:858cece41a236cf1d2f3e47725986ce0d97042a176f7bd079dc556372bf3bd85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0.18` - linux; amd64

```console
$ docker pull percona@sha256:80e07baf5281aee9c7dbef10ab3ba16c255b1cfd59da4f3eb56043af4202d371
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159591752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc4e728b52c8c22db189eb0089bbc352285899f5679aa611c5720b33b761aa63`
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
# Tue, 05 May 2020 21:42:45 GMT
ENV PSMDB_VERSION=4.0.18-11
# Tue, 05 May 2020 21:42:45 GMT
LABEL org.label-schema.schema-version=4.0.18-11
# Tue, 05 May 2020 21:42:45 GMT
LABEL org.opencontainers.image.version=4.0.18-11
# Thu, 07 May 2020 15:23:55 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-40 release
# Thu, 07 May 2020 15:23:55 GMT
ENV OS_VER=el7
# Thu, 07 May 2020 15:23:55 GMT
ENV FULL_PERCONA_VERSION=4.0.18-11.el7
# Thu, 07 May 2020 15:23:55 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 07 May 2020 15:24:00 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Thu, 07 May 2020 15:24:21 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 07 May 2020 15:24:22 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 07 May 2020 15:24:22 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 07 May 2020 15:24:23 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 07 May 2020 15:24:23 GMT
ENV GOSU_VERSION=1.11
# Thu, 07 May 2020 15:24:25 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 07 May 2020 15:24:28 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 07 May 2020 15:24:28 GMT
VOLUME [/data/db]
# Thu, 07 May 2020 15:24:28 GMT
COPY file:85995e73e1e4d284ba65fabe65ed1e96fcb9c00ac0d328edb8b0b48749d784e1 in /entrypoint.sh 
# Thu, 07 May 2020 15:24:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 May 2020 15:24:28 GMT
EXPOSE 27017
# Thu, 07 May 2020 15:24:29 GMT
USER 1001
# Thu, 07 May 2020 15:24:29 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ef9694f9631625a207bc725faca3127a8ff35730902838e9a6abe87760976b`  
		Last Modified: Thu, 07 May 2020 15:25:57 GMT  
		Size: 6.5 MB (6473844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c090ee9f40168b3f1e02cab71dbdb98f5282323a3fb0e7e1e022f3a0fe206b3`  
		Last Modified: Thu, 07 May 2020 15:26:03 GMT  
		Size: 6.8 MB (6793460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28accaa4c1bd9b3980f653c28e9a37a3394cce169baf819e49ea4acabfb04df8`  
		Last Modified: Thu, 07 May 2020 15:26:04 GMT  
		Size: 61.4 MB (61369701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4843ab4a75920f4caee8e545c0f0e664fcdbd9ef7372f559b958597fd04b2c6d`  
		Last Modified: Thu, 07 May 2020 15:25:54 GMT  
		Size: 1.6 KB (1593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d257afe58b55969ab10706dc55a93ac54010da57deb9c4af306a251d6236925`  
		Last Modified: Thu, 07 May 2020 15:25:54 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c9c127156ef0d6de2adb4cd687e3b56f19d1c341968753c0950f88ef6afb7f`  
		Last Modified: Thu, 07 May 2020 15:25:53 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5a5230fc4604c86229dbffbfb83f76fb80d9fc1a4b41495dd562ef11da03da`  
		Last Modified: Thu, 07 May 2020 15:25:53 GMT  
		Size: 915.5 KB (915466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28aee8f4cb87a72bc035b25f229b41479c85aa80b527acafad67ae0bafc3d77`  
		Last Modified: Thu, 07 May 2020 15:25:55 GMT  
		Size: 8.1 MB (8138878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f63a22e3ee4b85af09baafe7bdc08652750ce0ee09df042b88832446b8f321`  
		Last Modified: Thu, 07 May 2020 15:25:53 GMT  
		Size: 4.0 KB (4017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:a18c92df75e21088f1d7197a9333b12cfaf8a7f8ddd6e639e11e981f36dc4d9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:6f18b089e66b9e31cb0bd0d1cd9d591ff75cf7cc8ac160549bba5dabbcb36c90
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.1 MB (169108775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30b4812490c35628349beabfdb7d2ac9606c62fc5c2a369ac7cd20eecf5ed5f9`
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
# Thu, 07 May 2020 15:23:04 GMT
ENV PSMDB_VERSION=4.2.6-6
# Thu, 07 May 2020 15:23:04 GMT
LABEL org.label-schema.schema-version=4.2.6-6
# Thu, 07 May 2020 15:23:04 GMT
LABEL org.opencontainers.image.version=4.2.6-6
# Thu, 07 May 2020 15:23:09 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Thu, 07 May 2020 15:23:09 GMT
ENV OS_VER=el7
# Thu, 07 May 2020 15:23:09 GMT
ENV FULL_PERCONA_VERSION=4.2.6-6.el7
# Thu, 07 May 2020 15:23:09 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 07 May 2020 15:23:14 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Thu, 07 May 2020 15:23:33 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 07 May 2020 15:23:34 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 07 May 2020 15:23:34 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 07 May 2020 15:23:35 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 07 May 2020 15:23:35 GMT
ENV GOSU_VERSION=1.11
# Thu, 07 May 2020 15:23:37 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 07 May 2020 15:23:40 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 07 May 2020 15:23:40 GMT
VOLUME [/data/db]
# Thu, 07 May 2020 15:23:40 GMT
COPY file:d143ecb7a542d31ae4c95807064d8fad35f488059238d10fcd8b10f214d58331 in /entrypoint.sh 
# Thu, 07 May 2020 15:23:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 May 2020 15:23:41 GMT
EXPOSE 27017
# Thu, 07 May 2020 15:23:41 GMT
USER 1001
# Thu, 07 May 2020 15:23:41 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52475835fa8dfd1625deba437eb238de6abee9a585a4a858c6e7e827f6defa1`  
		Last Modified: Thu, 07 May 2020 15:25:39 GMT  
		Size: 6.5 MB (6473821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9708c4a499009c73b0db463884bfa47834e6ddd07a4626c6f4ff9b01a3410552`  
		Last Modified: Thu, 07 May 2020 15:25:39 GMT  
		Size: 6.8 MB (6793269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604eb98ff43e5cc193e59a2ff61f0d593f98eec0ec29c07ca58e4c82a0cc84b5`  
		Last Modified: Thu, 07 May 2020 15:25:48 GMT  
		Size: 70.9 MB (70886506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a40c152f04722fd006b7559feecba5580ab19b14886fca6a6cb9001be8a4cf2`  
		Last Modified: Thu, 07 May 2020 15:25:37 GMT  
		Size: 1.6 KB (1593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695c17cf0001e07e3a59438ee7b661e13026ecbfff97f1c025e3a70266044ae7`  
		Last Modified: Thu, 07 May 2020 15:25:36 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc8d8bd96327497821c94886ed30aeeb5b0545aef53558256aa8ee6b7753e19`  
		Last Modified: Thu, 07 May 2020 15:25:36 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645a2fc5095d48e22984bba3040481de621a575c50b3a2cdc2969338d0420ddf`  
		Last Modified: Thu, 07 May 2020 15:25:36 GMT  
		Size: 915.5 KB (915475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427f06d80a5d6467924823ecc5cd817877dfcca534264cfb3ab6b42a1c9cbc0c`  
		Last Modified: Thu, 07 May 2020 15:25:38 GMT  
		Size: 8.1 MB (8138880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e313ce0ca3b19719ba918549ba4bc4d4d88adad1ae76ecf0b93fecb82406529`  
		Last Modified: Thu, 07 May 2020 15:25:36 GMT  
		Size: 4.4 KB (4438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2.6`

```console
$ docker pull percona@sha256:a18c92df75e21088f1d7197a9333b12cfaf8a7f8ddd6e639e11e981f36dc4d9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.2.6` - linux; amd64

```console
$ docker pull percona@sha256:6f18b089e66b9e31cb0bd0d1cd9d591ff75cf7cc8ac160549bba5dabbcb36c90
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.1 MB (169108775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30b4812490c35628349beabfdb7d2ac9606c62fc5c2a369ac7cd20eecf5ed5f9`
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
# Thu, 07 May 2020 15:23:04 GMT
ENV PSMDB_VERSION=4.2.6-6
# Thu, 07 May 2020 15:23:04 GMT
LABEL org.label-schema.schema-version=4.2.6-6
# Thu, 07 May 2020 15:23:04 GMT
LABEL org.opencontainers.image.version=4.2.6-6
# Thu, 07 May 2020 15:23:09 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Thu, 07 May 2020 15:23:09 GMT
ENV OS_VER=el7
# Thu, 07 May 2020 15:23:09 GMT
ENV FULL_PERCONA_VERSION=4.2.6-6.el7
# Thu, 07 May 2020 15:23:09 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 07 May 2020 15:23:14 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Thu, 07 May 2020 15:23:33 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 07 May 2020 15:23:34 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 07 May 2020 15:23:34 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 07 May 2020 15:23:35 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 07 May 2020 15:23:35 GMT
ENV GOSU_VERSION=1.11
# Thu, 07 May 2020 15:23:37 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 07 May 2020 15:23:40 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 07 May 2020 15:23:40 GMT
VOLUME [/data/db]
# Thu, 07 May 2020 15:23:40 GMT
COPY file:d143ecb7a542d31ae4c95807064d8fad35f488059238d10fcd8b10f214d58331 in /entrypoint.sh 
# Thu, 07 May 2020 15:23:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 May 2020 15:23:41 GMT
EXPOSE 27017
# Thu, 07 May 2020 15:23:41 GMT
USER 1001
# Thu, 07 May 2020 15:23:41 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52475835fa8dfd1625deba437eb238de6abee9a585a4a858c6e7e827f6defa1`  
		Last Modified: Thu, 07 May 2020 15:25:39 GMT  
		Size: 6.5 MB (6473821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9708c4a499009c73b0db463884bfa47834e6ddd07a4626c6f4ff9b01a3410552`  
		Last Modified: Thu, 07 May 2020 15:25:39 GMT  
		Size: 6.8 MB (6793269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604eb98ff43e5cc193e59a2ff61f0d593f98eec0ec29c07ca58e4c82a0cc84b5`  
		Last Modified: Thu, 07 May 2020 15:25:48 GMT  
		Size: 70.9 MB (70886506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a40c152f04722fd006b7559feecba5580ab19b14886fca6a6cb9001be8a4cf2`  
		Last Modified: Thu, 07 May 2020 15:25:37 GMT  
		Size: 1.6 KB (1593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695c17cf0001e07e3a59438ee7b661e13026ecbfff97f1c025e3a70266044ae7`  
		Last Modified: Thu, 07 May 2020 15:25:36 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc8d8bd96327497821c94886ed30aeeb5b0545aef53558256aa8ee6b7753e19`  
		Last Modified: Thu, 07 May 2020 15:25:36 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645a2fc5095d48e22984bba3040481de621a575c50b3a2cdc2969338d0420ddf`  
		Last Modified: Thu, 07 May 2020 15:25:36 GMT  
		Size: 915.5 KB (915475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427f06d80a5d6467924823ecc5cd817877dfcca534264cfb3ab6b42a1c9cbc0c`  
		Last Modified: Thu, 07 May 2020 15:25:38 GMT  
		Size: 8.1 MB (8138880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e313ce0ca3b19719ba918549ba4bc4d4d88adad1ae76ecf0b93fecb82406529`  
		Last Modified: Thu, 07 May 2020 15:25:36 GMT  
		Size: 4.4 KB (4438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
