<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `percona`

-	[`percona:5`](#percona5)
-	[`percona:5.6`](#percona56)
-	[`percona:5.6.47`](#percona5647)
-	[`percona:5.6.47-centos`](#percona5647-centos)
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
-	[`percona:psmdb-4.2.5`](#perconapsmdb-425)

## `percona:5`

```console
$ docker pull percona@sha256:b9d2bf785a43b122a109bf233b0ae18aa98e8bd9b86a3d2eecd7c1d70b3e4739
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5` - linux; amd64

```console
$ docker pull percona@sha256:d801123bbfaf750924f993f5c59189d144a93feb928b8aef95e541dd61c62881
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196408390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0128954d5b0faaf39b6ff058fbcbb9a2f07f6b60c663312fada05c826cc93b3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:34:15 GMT
RUN groupdel input && groupadd -g 999 mysql
# Thu, 30 Jan 2020 23:34:15 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:34:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Wed, 05 Feb 2020 23:35:34 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Wed, 05 Feb 2020 23:37:01 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 05 Feb 2020 23:37:02 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 05 Feb 2020 23:37:02 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 05 Feb 2020 23:37:03 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 05 Feb 2020 23:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Feb 2020 23:37:03 GMT
USER mysql
# Wed, 05 Feb 2020 23:37:03 GMT
EXPOSE 3306
# Wed, 05 Feb 2020 23:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41876e5543b58e7c452f162a531b7fed8fd228ab59ecd9f10bec3de5510092`  
		Last Modified: Thu, 30 Jan 2020 23:37:24 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ef0baa29ddb873dbc81a8f0a044e9bbd01dedde4adf9df51e79e2ede50d832`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ffcf5dd2e603082b9bd847b058b227c15955c7cd1fb07ab954a9c2413275b2`  
		Last Modified: Thu, 30 Jan 2020 23:37:25 GMT  
		Size: 6.4 MB (6438113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957e94b3b4fdf505a520f31b2923d37a6a00e2ff2a9a5f8a0a982391eed0f6e2`  
		Last Modified: Wed, 05 Feb 2020 23:38:07 GMT  
		Size: 114.2 MB (114183023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b87447119d4ac1b9281878658de608e732a0ece81b6eac05bb78dd69536268`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020903636e3080388f087f7db0cd4898b625066e37d7fde08aa9f329c1a33f85`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6`

```console
$ docker pull percona@sha256:6e7663c302a2bae40ac5ed1cc66e1ebfaa6562fea488d7410d81ee4f5d3fc062
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.6` - linux; amd64

```console
$ docker pull percona@sha256:e77a18d8abe8c6a8b741b7ba58b6e020c283027807faf4d3b6c5c403b3631e4a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.8 MB (139805570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a00a0872b8df291f587ac74ba255a2a042fabd3a7bf530e5bfd86f80c6055ff`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:34:15 GMT
RUN groupdel input && groupadd -g 999 mysql
# Thu, 30 Jan 2020 23:34:15 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:35:32 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Thu, 30 Jan 2020 23:35:33 GMT
ENV PERCONA_VERSION=5.6.47-rel87.0.1.el7
# Thu, 30 Jan 2020 23:36:14 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:36:15 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Jan 2020 23:36:15 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:36:15 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:36:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:36:16 GMT
USER mysql
# Thu, 30 Jan 2020 23:36:16 GMT
EXPOSE 3306
# Thu, 30 Jan 2020 23:36:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41876e5543b58e7c452f162a531b7fed8fd228ab59ecd9f10bec3de5510092`  
		Last Modified: Thu, 30 Jan 2020 23:37:24 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ef0baa29ddb873dbc81a8f0a044e9bbd01dedde4adf9df51e79e2ede50d832`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5892fb24bbc2b3b3ac50cd99711500635a814cefd5185f7544c92cf9a5763c2`  
		Last Modified: Thu, 30 Jan 2020 23:38:00 GMT  
		Size: 6.4 MB (6438137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f269d97ff7c87de17f939b8d5b146b65dca30d6cfccf2b303b87fd32ce72971`  
		Last Modified: Thu, 30 Jan 2020 23:38:08 GMT  
		Size: 57.6 MB (57576805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977017066ad7b9b02060f04115cead186246564e814059f3c0063bdc9f5d7f3a`  
		Last Modified: Thu, 30 Jan 2020 23:37:58 GMT  
		Size: 4.9 KB (4880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef40a45729664f63076da68020d602f8388b6e56552e95eeada12628854176a7`  
		Last Modified: Thu, 30 Jan 2020 23:37:58 GMT  
		Size: 2.9 KB (2941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6.47`

```console
$ docker pull percona@sha256:6e7663c302a2bae40ac5ed1cc66e1ebfaa6562fea488d7410d81ee4f5d3fc062
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.6.47` - linux; amd64

```console
$ docker pull percona@sha256:e77a18d8abe8c6a8b741b7ba58b6e020c283027807faf4d3b6c5c403b3631e4a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.8 MB (139805570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a00a0872b8df291f587ac74ba255a2a042fabd3a7bf530e5bfd86f80c6055ff`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:34:15 GMT
RUN groupdel input && groupadd -g 999 mysql
# Thu, 30 Jan 2020 23:34:15 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:35:32 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Thu, 30 Jan 2020 23:35:33 GMT
ENV PERCONA_VERSION=5.6.47-rel87.0.1.el7
# Thu, 30 Jan 2020 23:36:14 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:36:15 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Jan 2020 23:36:15 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:36:15 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:36:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:36:16 GMT
USER mysql
# Thu, 30 Jan 2020 23:36:16 GMT
EXPOSE 3306
# Thu, 30 Jan 2020 23:36:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41876e5543b58e7c452f162a531b7fed8fd228ab59ecd9f10bec3de5510092`  
		Last Modified: Thu, 30 Jan 2020 23:37:24 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ef0baa29ddb873dbc81a8f0a044e9bbd01dedde4adf9df51e79e2ede50d832`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5892fb24bbc2b3b3ac50cd99711500635a814cefd5185f7544c92cf9a5763c2`  
		Last Modified: Thu, 30 Jan 2020 23:38:00 GMT  
		Size: 6.4 MB (6438137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f269d97ff7c87de17f939b8d5b146b65dca30d6cfccf2b303b87fd32ce72971`  
		Last Modified: Thu, 30 Jan 2020 23:38:08 GMT  
		Size: 57.6 MB (57576805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977017066ad7b9b02060f04115cead186246564e814059f3c0063bdc9f5d7f3a`  
		Last Modified: Thu, 30 Jan 2020 23:37:58 GMT  
		Size: 4.9 KB (4880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef40a45729664f63076da68020d602f8388b6e56552e95eeada12628854176a7`  
		Last Modified: Thu, 30 Jan 2020 23:37:58 GMT  
		Size: 2.9 KB (2941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6.47-centos`

```console
$ docker pull percona@sha256:6e7663c302a2bae40ac5ed1cc66e1ebfaa6562fea488d7410d81ee4f5d3fc062
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.6.47-centos` - linux; amd64

```console
$ docker pull percona@sha256:e77a18d8abe8c6a8b741b7ba58b6e020c283027807faf4d3b6c5c403b3631e4a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.8 MB (139805570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a00a0872b8df291f587ac74ba255a2a042fabd3a7bf530e5bfd86f80c6055ff`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:34:15 GMT
RUN groupdel input && groupadd -g 999 mysql
# Thu, 30 Jan 2020 23:34:15 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:35:32 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Thu, 30 Jan 2020 23:35:33 GMT
ENV PERCONA_VERSION=5.6.47-rel87.0.1.el7
# Thu, 30 Jan 2020 23:36:14 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:36:15 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Jan 2020 23:36:15 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:36:15 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:36:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:36:16 GMT
USER mysql
# Thu, 30 Jan 2020 23:36:16 GMT
EXPOSE 3306
# Thu, 30 Jan 2020 23:36:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41876e5543b58e7c452f162a531b7fed8fd228ab59ecd9f10bec3de5510092`  
		Last Modified: Thu, 30 Jan 2020 23:37:24 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ef0baa29ddb873dbc81a8f0a044e9bbd01dedde4adf9df51e79e2ede50d832`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5892fb24bbc2b3b3ac50cd99711500635a814cefd5185f7544c92cf9a5763c2`  
		Last Modified: Thu, 30 Jan 2020 23:38:00 GMT  
		Size: 6.4 MB (6438137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f269d97ff7c87de17f939b8d5b146b65dca30d6cfccf2b303b87fd32ce72971`  
		Last Modified: Thu, 30 Jan 2020 23:38:08 GMT  
		Size: 57.6 MB (57576805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977017066ad7b9b02060f04115cead186246564e814059f3c0063bdc9f5d7f3a`  
		Last Modified: Thu, 30 Jan 2020 23:37:58 GMT  
		Size: 4.9 KB (4880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef40a45729664f63076da68020d602f8388b6e56552e95eeada12628854176a7`  
		Last Modified: Thu, 30 Jan 2020 23:37:58 GMT  
		Size: 2.9 KB (2941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6-centos`

```console
$ docker pull percona@sha256:6e7663c302a2bae40ac5ed1cc66e1ebfaa6562fea488d7410d81ee4f5d3fc062
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.6-centos` - linux; amd64

```console
$ docker pull percona@sha256:e77a18d8abe8c6a8b741b7ba58b6e020c283027807faf4d3b6c5c403b3631e4a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.8 MB (139805570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a00a0872b8df291f587ac74ba255a2a042fabd3a7bf530e5bfd86f80c6055ff`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:34:15 GMT
RUN groupdel input && groupadd -g 999 mysql
# Thu, 30 Jan 2020 23:34:15 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:35:32 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Thu, 30 Jan 2020 23:35:33 GMT
ENV PERCONA_VERSION=5.6.47-rel87.0.1.el7
# Thu, 30 Jan 2020 23:36:14 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:36:15 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Jan 2020 23:36:15 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:36:15 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:36:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:36:16 GMT
USER mysql
# Thu, 30 Jan 2020 23:36:16 GMT
EXPOSE 3306
# Thu, 30 Jan 2020 23:36:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41876e5543b58e7c452f162a531b7fed8fd228ab59ecd9f10bec3de5510092`  
		Last Modified: Thu, 30 Jan 2020 23:37:24 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ef0baa29ddb873dbc81a8f0a044e9bbd01dedde4adf9df51e79e2ede50d832`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5892fb24bbc2b3b3ac50cd99711500635a814cefd5185f7544c92cf9a5763c2`  
		Last Modified: Thu, 30 Jan 2020 23:38:00 GMT  
		Size: 6.4 MB (6438137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f269d97ff7c87de17f939b8d5b146b65dca30d6cfccf2b303b87fd32ce72971`  
		Last Modified: Thu, 30 Jan 2020 23:38:08 GMT  
		Size: 57.6 MB (57576805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977017066ad7b9b02060f04115cead186246564e814059f3c0063bdc9f5d7f3a`  
		Last Modified: Thu, 30 Jan 2020 23:37:58 GMT  
		Size: 4.9 KB (4880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef40a45729664f63076da68020d602f8388b6e56552e95eeada12628854176a7`  
		Last Modified: Thu, 30 Jan 2020 23:37:58 GMT  
		Size: 2.9 KB (2941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7`

```console
$ docker pull percona@sha256:b9d2bf785a43b122a109bf233b0ae18aa98e8bd9b86a3d2eecd7c1d70b3e4739
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7` - linux; amd64

```console
$ docker pull percona@sha256:d801123bbfaf750924f993f5c59189d144a93feb928b8aef95e541dd61c62881
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196408390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0128954d5b0faaf39b6ff058fbcbb9a2f07f6b60c663312fada05c826cc93b3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:34:15 GMT
RUN groupdel input && groupadd -g 999 mysql
# Thu, 30 Jan 2020 23:34:15 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:34:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Wed, 05 Feb 2020 23:35:34 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Wed, 05 Feb 2020 23:37:01 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 05 Feb 2020 23:37:02 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 05 Feb 2020 23:37:02 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 05 Feb 2020 23:37:03 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 05 Feb 2020 23:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Feb 2020 23:37:03 GMT
USER mysql
# Wed, 05 Feb 2020 23:37:03 GMT
EXPOSE 3306
# Wed, 05 Feb 2020 23:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41876e5543b58e7c452f162a531b7fed8fd228ab59ecd9f10bec3de5510092`  
		Last Modified: Thu, 30 Jan 2020 23:37:24 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ef0baa29ddb873dbc81a8f0a044e9bbd01dedde4adf9df51e79e2ede50d832`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ffcf5dd2e603082b9bd847b058b227c15955c7cd1fb07ab954a9c2413275b2`  
		Last Modified: Thu, 30 Jan 2020 23:37:25 GMT  
		Size: 6.4 MB (6438113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957e94b3b4fdf505a520f31b2923d37a6a00e2ff2a9a5f8a0a982391eed0f6e2`  
		Last Modified: Wed, 05 Feb 2020 23:38:07 GMT  
		Size: 114.2 MB (114183023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b87447119d4ac1b9281878658de608e732a0ece81b6eac05bb78dd69536268`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020903636e3080388f087f7db0cd4898b625066e37d7fde08aa9f329c1a33f85`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.29`

```console
$ docker pull percona@sha256:b9d2bf785a43b122a109bf233b0ae18aa98e8bd9b86a3d2eecd7c1d70b3e4739
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7.29` - linux; amd64

```console
$ docker pull percona@sha256:d801123bbfaf750924f993f5c59189d144a93feb928b8aef95e541dd61c62881
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196408390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0128954d5b0faaf39b6ff058fbcbb9a2f07f6b60c663312fada05c826cc93b3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:34:15 GMT
RUN groupdel input && groupadd -g 999 mysql
# Thu, 30 Jan 2020 23:34:15 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:34:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Wed, 05 Feb 2020 23:35:34 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Wed, 05 Feb 2020 23:37:01 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 05 Feb 2020 23:37:02 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 05 Feb 2020 23:37:02 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 05 Feb 2020 23:37:03 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 05 Feb 2020 23:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Feb 2020 23:37:03 GMT
USER mysql
# Wed, 05 Feb 2020 23:37:03 GMT
EXPOSE 3306
# Wed, 05 Feb 2020 23:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41876e5543b58e7c452f162a531b7fed8fd228ab59ecd9f10bec3de5510092`  
		Last Modified: Thu, 30 Jan 2020 23:37:24 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ef0baa29ddb873dbc81a8f0a044e9bbd01dedde4adf9df51e79e2ede50d832`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ffcf5dd2e603082b9bd847b058b227c15955c7cd1fb07ab954a9c2413275b2`  
		Last Modified: Thu, 30 Jan 2020 23:37:25 GMT  
		Size: 6.4 MB (6438113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957e94b3b4fdf505a520f31b2923d37a6a00e2ff2a9a5f8a0a982391eed0f6e2`  
		Last Modified: Wed, 05 Feb 2020 23:38:07 GMT  
		Size: 114.2 MB (114183023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b87447119d4ac1b9281878658de608e732a0ece81b6eac05bb78dd69536268`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020903636e3080388f087f7db0cd4898b625066e37d7fde08aa9f329c1a33f85`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.29-centos`

```console
$ docker pull percona@sha256:b9d2bf785a43b122a109bf233b0ae18aa98e8bd9b86a3d2eecd7c1d70b3e4739
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7.29-centos` - linux; amd64

```console
$ docker pull percona@sha256:d801123bbfaf750924f993f5c59189d144a93feb928b8aef95e541dd61c62881
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196408390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0128954d5b0faaf39b6ff058fbcbb9a2f07f6b60c663312fada05c826cc93b3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:34:15 GMT
RUN groupdel input && groupadd -g 999 mysql
# Thu, 30 Jan 2020 23:34:15 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:34:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Wed, 05 Feb 2020 23:35:34 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Wed, 05 Feb 2020 23:37:01 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 05 Feb 2020 23:37:02 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 05 Feb 2020 23:37:02 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 05 Feb 2020 23:37:03 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 05 Feb 2020 23:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Feb 2020 23:37:03 GMT
USER mysql
# Wed, 05 Feb 2020 23:37:03 GMT
EXPOSE 3306
# Wed, 05 Feb 2020 23:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41876e5543b58e7c452f162a531b7fed8fd228ab59ecd9f10bec3de5510092`  
		Last Modified: Thu, 30 Jan 2020 23:37:24 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ef0baa29ddb873dbc81a8f0a044e9bbd01dedde4adf9df51e79e2ede50d832`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ffcf5dd2e603082b9bd847b058b227c15955c7cd1fb07ab954a9c2413275b2`  
		Last Modified: Thu, 30 Jan 2020 23:37:25 GMT  
		Size: 6.4 MB (6438113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957e94b3b4fdf505a520f31b2923d37a6a00e2ff2a9a5f8a0a982391eed0f6e2`  
		Last Modified: Wed, 05 Feb 2020 23:38:07 GMT  
		Size: 114.2 MB (114183023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b87447119d4ac1b9281878658de608e732a0ece81b6eac05bb78dd69536268`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020903636e3080388f087f7db0cd4898b625066e37d7fde08aa9f329c1a33f85`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7-centos`

```console
$ docker pull percona@sha256:b9d2bf785a43b122a109bf233b0ae18aa98e8bd9b86a3d2eecd7c1d70b3e4739
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7-centos` - linux; amd64

```console
$ docker pull percona@sha256:d801123bbfaf750924f993f5c59189d144a93feb928b8aef95e541dd61c62881
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196408390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0128954d5b0faaf39b6ff058fbcbb9a2f07f6b60c663312fada05c826cc93b3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:34:15 GMT
RUN groupdel input && groupadd -g 999 mysql
# Thu, 30 Jan 2020 23:34:15 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:34:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Wed, 05 Feb 2020 23:35:34 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Wed, 05 Feb 2020 23:37:01 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 05 Feb 2020 23:37:02 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 05 Feb 2020 23:37:02 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 05 Feb 2020 23:37:03 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 05 Feb 2020 23:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Feb 2020 23:37:03 GMT
USER mysql
# Wed, 05 Feb 2020 23:37:03 GMT
EXPOSE 3306
# Wed, 05 Feb 2020 23:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41876e5543b58e7c452f162a531b7fed8fd228ab59ecd9f10bec3de5510092`  
		Last Modified: Thu, 30 Jan 2020 23:37:24 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ef0baa29ddb873dbc81a8f0a044e9bbd01dedde4adf9df51e79e2ede50d832`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ffcf5dd2e603082b9bd847b058b227c15955c7cd1fb07ab954a9c2413275b2`  
		Last Modified: Thu, 30 Jan 2020 23:37:25 GMT  
		Size: 6.4 MB (6438113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957e94b3b4fdf505a520f31b2923d37a6a00e2ff2a9a5f8a0a982391eed0f6e2`  
		Last Modified: Wed, 05 Feb 2020 23:38:07 GMT  
		Size: 114.2 MB (114183023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b87447119d4ac1b9281878658de608e732a0ece81b6eac05bb78dd69536268`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020903636e3080388f087f7db0cd4898b625066e37d7fde08aa9f329c1a33f85`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5-centos`

```console
$ docker pull percona@sha256:b9d2bf785a43b122a109bf233b0ae18aa98e8bd9b86a3d2eecd7c1d70b3e4739
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5-centos` - linux; amd64

```console
$ docker pull percona@sha256:d801123bbfaf750924f993f5c59189d144a93feb928b8aef95e541dd61c62881
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196408390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0128954d5b0faaf39b6ff058fbcbb9a2f07f6b60c663312fada05c826cc93b3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:34:15 GMT
RUN groupdel input && groupadd -g 999 mysql
# Thu, 30 Jan 2020 23:34:15 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:34:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Wed, 05 Feb 2020 23:35:34 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Wed, 05 Feb 2020 23:37:01 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 05 Feb 2020 23:37:02 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 05 Feb 2020 23:37:02 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 05 Feb 2020 23:37:03 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 05 Feb 2020 23:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Feb 2020 23:37:03 GMT
USER mysql
# Wed, 05 Feb 2020 23:37:03 GMT
EXPOSE 3306
# Wed, 05 Feb 2020 23:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41876e5543b58e7c452f162a531b7fed8fd228ab59ecd9f10bec3de5510092`  
		Last Modified: Thu, 30 Jan 2020 23:37:24 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ef0baa29ddb873dbc81a8f0a044e9bbd01dedde4adf9df51e79e2ede50d832`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ffcf5dd2e603082b9bd847b058b227c15955c7cd1fb07ab954a9c2413275b2`  
		Last Modified: Thu, 30 Jan 2020 23:37:25 GMT  
		Size: 6.4 MB (6438113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957e94b3b4fdf505a520f31b2923d37a6a00e2ff2a9a5f8a0a982391eed0f6e2`  
		Last Modified: Wed, 05 Feb 2020 23:38:07 GMT  
		Size: 114.2 MB (114183023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b87447119d4ac1b9281878658de608e732a0ece81b6eac05bb78dd69536268`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020903636e3080388f087f7db0cd4898b625066e37d7fde08aa9f329c1a33f85`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8`

```console
$ docker pull percona@sha256:95b64ef7f23021ea64ca8626bf04d7f9a052aa7481ee1f38e8fda6d5a98dae5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8` - linux; amd64

```console
$ docker pull percona@sha256:30f000dc85bd13397c346bf1e3a228e850a8869b1da00d6e987a2fa7a30fb448
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.5 MB (224496206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e269b673aa2af7f9d8abf157fc1460094bf886f0a4a1887842f45a8cf5d59262`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:33:00 GMT
RUN groupadd -g 1001 mysql
# Thu, 30 Jan 2020 23:33:01 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:33:05 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 23 Mar 2020 21:20:10 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Mon, 23 Mar 2020 21:21:02 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 23 Mar 2020 21:21:03 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 23 Mar 2020 21:21:04 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 23 Mar 2020 21:21:04 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 23 Mar 2020 21:21:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 23 Mar 2020 21:21:04 GMT
USER mysql
# Mon, 23 Mar 2020 21:21:04 GMT
EXPOSE 3306 33060
# Mon, 23 Mar 2020 21:21:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296eab8cb2767bf28303443e7bc3a4a0cbc14383b23c877b7b8c2f776fdf81b5`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed24ac5fd1f63a28eaf64c5435879cc6199b8433c5f68df137d2c364e1c11a3b`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303807e74badcc2b04a965236de0c98f0a8339a3525041b2cbe9e1b4a0ba16ed`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 6.4 MB (6438611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b90f167fb2a76e1742630dec20b9071a652cd47b9da24a39e19d1707478b470`  
		Last Modified: Mon, 23 Mar 2020 21:22:09 GMT  
		Size: 142.3 MB (142270573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962beccc99b2c7576801e02694f56db43953528e83fdee44aeb8138742b8de37`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c63f042185c82285c5bcd15c1624ab9de38042bca2b66748d7d1d4ef15f737`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0`

```console
$ docker pull percona@sha256:95b64ef7f23021ea64ca8626bf04d7f9a052aa7481ee1f38e8fda6d5a98dae5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0` - linux; amd64

```console
$ docker pull percona@sha256:30f000dc85bd13397c346bf1e3a228e850a8869b1da00d6e987a2fa7a30fb448
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.5 MB (224496206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e269b673aa2af7f9d8abf157fc1460094bf886f0a4a1887842f45a8cf5d59262`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:33:00 GMT
RUN groupadd -g 1001 mysql
# Thu, 30 Jan 2020 23:33:01 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:33:05 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 23 Mar 2020 21:20:10 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Mon, 23 Mar 2020 21:21:02 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 23 Mar 2020 21:21:03 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 23 Mar 2020 21:21:04 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 23 Mar 2020 21:21:04 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 23 Mar 2020 21:21:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 23 Mar 2020 21:21:04 GMT
USER mysql
# Mon, 23 Mar 2020 21:21:04 GMT
EXPOSE 3306 33060
# Mon, 23 Mar 2020 21:21:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296eab8cb2767bf28303443e7bc3a4a0cbc14383b23c877b7b8c2f776fdf81b5`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed24ac5fd1f63a28eaf64c5435879cc6199b8433c5f68df137d2c364e1c11a3b`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303807e74badcc2b04a965236de0c98f0a8339a3525041b2cbe9e1b4a0ba16ed`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 6.4 MB (6438611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b90f167fb2a76e1742630dec20b9071a652cd47b9da24a39e19d1707478b470`  
		Last Modified: Mon, 23 Mar 2020 21:22:09 GMT  
		Size: 142.3 MB (142270573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962beccc99b2c7576801e02694f56db43953528e83fdee44aeb8138742b8de37`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c63f042185c82285c5bcd15c1624ab9de38042bca2b66748d7d1d4ef15f737`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.19-10`

```console
$ docker pull percona@sha256:95b64ef7f23021ea64ca8626bf04d7f9a052aa7481ee1f38e8fda6d5a98dae5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0.19-10` - linux; amd64

```console
$ docker pull percona@sha256:30f000dc85bd13397c346bf1e3a228e850a8869b1da00d6e987a2fa7a30fb448
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.5 MB (224496206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e269b673aa2af7f9d8abf157fc1460094bf886f0a4a1887842f45a8cf5d59262`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:33:00 GMT
RUN groupadd -g 1001 mysql
# Thu, 30 Jan 2020 23:33:01 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:33:05 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 23 Mar 2020 21:20:10 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Mon, 23 Mar 2020 21:21:02 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 23 Mar 2020 21:21:03 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 23 Mar 2020 21:21:04 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 23 Mar 2020 21:21:04 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 23 Mar 2020 21:21:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 23 Mar 2020 21:21:04 GMT
USER mysql
# Mon, 23 Mar 2020 21:21:04 GMT
EXPOSE 3306 33060
# Mon, 23 Mar 2020 21:21:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296eab8cb2767bf28303443e7bc3a4a0cbc14383b23c877b7b8c2f776fdf81b5`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed24ac5fd1f63a28eaf64c5435879cc6199b8433c5f68df137d2c364e1c11a3b`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303807e74badcc2b04a965236de0c98f0a8339a3525041b2cbe9e1b4a0ba16ed`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 6.4 MB (6438611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b90f167fb2a76e1742630dec20b9071a652cd47b9da24a39e19d1707478b470`  
		Last Modified: Mon, 23 Mar 2020 21:22:09 GMT  
		Size: 142.3 MB (142270573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962beccc99b2c7576801e02694f56db43953528e83fdee44aeb8138742b8de37`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c63f042185c82285c5bcd15c1624ab9de38042bca2b66748d7d1d4ef15f737`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.19-10-centos`

```console
$ docker pull percona@sha256:95b64ef7f23021ea64ca8626bf04d7f9a052aa7481ee1f38e8fda6d5a98dae5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0.19-10-centos` - linux; amd64

```console
$ docker pull percona@sha256:30f000dc85bd13397c346bf1e3a228e850a8869b1da00d6e987a2fa7a30fb448
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.5 MB (224496206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e269b673aa2af7f9d8abf157fc1460094bf886f0a4a1887842f45a8cf5d59262`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:33:00 GMT
RUN groupadd -g 1001 mysql
# Thu, 30 Jan 2020 23:33:01 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:33:05 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 23 Mar 2020 21:20:10 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Mon, 23 Mar 2020 21:21:02 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 23 Mar 2020 21:21:03 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 23 Mar 2020 21:21:04 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 23 Mar 2020 21:21:04 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 23 Mar 2020 21:21:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 23 Mar 2020 21:21:04 GMT
USER mysql
# Mon, 23 Mar 2020 21:21:04 GMT
EXPOSE 3306 33060
# Mon, 23 Mar 2020 21:21:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296eab8cb2767bf28303443e7bc3a4a0cbc14383b23c877b7b8c2f776fdf81b5`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed24ac5fd1f63a28eaf64c5435879cc6199b8433c5f68df137d2c364e1c11a3b`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303807e74badcc2b04a965236de0c98f0a8339a3525041b2cbe9e1b4a0ba16ed`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 6.4 MB (6438611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b90f167fb2a76e1742630dec20b9071a652cd47b9da24a39e19d1707478b470`  
		Last Modified: Mon, 23 Mar 2020 21:22:09 GMT  
		Size: 142.3 MB (142270573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962beccc99b2c7576801e02694f56db43953528e83fdee44aeb8138742b8de37`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c63f042185c82285c5bcd15c1624ab9de38042bca2b66748d7d1d4ef15f737`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0-centos`

```console
$ docker pull percona@sha256:95b64ef7f23021ea64ca8626bf04d7f9a052aa7481ee1f38e8fda6d5a98dae5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0-centos` - linux; amd64

```console
$ docker pull percona@sha256:30f000dc85bd13397c346bf1e3a228e850a8869b1da00d6e987a2fa7a30fb448
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.5 MB (224496206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e269b673aa2af7f9d8abf157fc1460094bf886f0a4a1887842f45a8cf5d59262`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:33:00 GMT
RUN groupadd -g 1001 mysql
# Thu, 30 Jan 2020 23:33:01 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:33:05 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 23 Mar 2020 21:20:10 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Mon, 23 Mar 2020 21:21:02 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 23 Mar 2020 21:21:03 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 23 Mar 2020 21:21:04 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 23 Mar 2020 21:21:04 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 23 Mar 2020 21:21:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 23 Mar 2020 21:21:04 GMT
USER mysql
# Mon, 23 Mar 2020 21:21:04 GMT
EXPOSE 3306 33060
# Mon, 23 Mar 2020 21:21:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296eab8cb2767bf28303443e7bc3a4a0cbc14383b23c877b7b8c2f776fdf81b5`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed24ac5fd1f63a28eaf64c5435879cc6199b8433c5f68df137d2c364e1c11a3b`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303807e74badcc2b04a965236de0c98f0a8339a3525041b2cbe9e1b4a0ba16ed`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 6.4 MB (6438611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b90f167fb2a76e1742630dec20b9071a652cd47b9da24a39e19d1707478b470`  
		Last Modified: Mon, 23 Mar 2020 21:22:09 GMT  
		Size: 142.3 MB (142270573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962beccc99b2c7576801e02694f56db43953528e83fdee44aeb8138742b8de37`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c63f042185c82285c5bcd15c1624ab9de38042bca2b66748d7d1d4ef15f737`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8-centos`

```console
$ docker pull percona@sha256:95b64ef7f23021ea64ca8626bf04d7f9a052aa7481ee1f38e8fda6d5a98dae5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8-centos` - linux; amd64

```console
$ docker pull percona@sha256:30f000dc85bd13397c346bf1e3a228e850a8869b1da00d6e987a2fa7a30fb448
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.5 MB (224496206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e269b673aa2af7f9d8abf157fc1460094bf886f0a4a1887842f45a8cf5d59262`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:33:00 GMT
RUN groupadd -g 1001 mysql
# Thu, 30 Jan 2020 23:33:01 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:33:05 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 23 Mar 2020 21:20:10 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Mon, 23 Mar 2020 21:21:02 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 23 Mar 2020 21:21:03 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 23 Mar 2020 21:21:04 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 23 Mar 2020 21:21:04 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 23 Mar 2020 21:21:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 23 Mar 2020 21:21:04 GMT
USER mysql
# Mon, 23 Mar 2020 21:21:04 GMT
EXPOSE 3306 33060
# Mon, 23 Mar 2020 21:21:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296eab8cb2767bf28303443e7bc3a4a0cbc14383b23c877b7b8c2f776fdf81b5`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed24ac5fd1f63a28eaf64c5435879cc6199b8433c5f68df137d2c364e1c11a3b`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303807e74badcc2b04a965236de0c98f0a8339a3525041b2cbe9e1b4a0ba16ed`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 6.4 MB (6438611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b90f167fb2a76e1742630dec20b9071a652cd47b9da24a39e19d1707478b470`  
		Last Modified: Mon, 23 Mar 2020 21:22:09 GMT  
		Size: 142.3 MB (142270573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962beccc99b2c7576801e02694f56db43953528e83fdee44aeb8138742b8de37`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c63f042185c82285c5bcd15c1624ab9de38042bca2b66748d7d1d4ef15f737`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:centos`

```console
$ docker pull percona@sha256:b9d2bf785a43b122a109bf233b0ae18aa98e8bd9b86a3d2eecd7c1d70b3e4739
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:centos` - linux; amd64

```console
$ docker pull percona@sha256:d801123bbfaf750924f993f5c59189d144a93feb928b8aef95e541dd61c62881
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196408390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0128954d5b0faaf39b6ff058fbcbb9a2f07f6b60c663312fada05c826cc93b3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:34:15 GMT
RUN groupdel input && groupadd -g 999 mysql
# Thu, 30 Jan 2020 23:34:15 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:34:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Wed, 05 Feb 2020 23:35:34 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Wed, 05 Feb 2020 23:37:01 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 05 Feb 2020 23:37:02 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 05 Feb 2020 23:37:02 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 05 Feb 2020 23:37:03 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 05 Feb 2020 23:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Feb 2020 23:37:03 GMT
USER mysql
# Wed, 05 Feb 2020 23:37:03 GMT
EXPOSE 3306
# Wed, 05 Feb 2020 23:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41876e5543b58e7c452f162a531b7fed8fd228ab59ecd9f10bec3de5510092`  
		Last Modified: Thu, 30 Jan 2020 23:37:24 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ef0baa29ddb873dbc81a8f0a044e9bbd01dedde4adf9df51e79e2ede50d832`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ffcf5dd2e603082b9bd847b058b227c15955c7cd1fb07ab954a9c2413275b2`  
		Last Modified: Thu, 30 Jan 2020 23:37:25 GMT  
		Size: 6.4 MB (6438113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957e94b3b4fdf505a520f31b2923d37a6a00e2ff2a9a5f8a0a982391eed0f6e2`  
		Last Modified: Wed, 05 Feb 2020 23:38:07 GMT  
		Size: 114.2 MB (114183023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b87447119d4ac1b9281878658de608e732a0ece81b6eac05bb78dd69536268`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020903636e3080388f087f7db0cd4898b625066e37d7fde08aa9f329c1a33f85`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:latest`

```console
$ docker pull percona@sha256:b9d2bf785a43b122a109bf233b0ae18aa98e8bd9b86a3d2eecd7c1d70b3e4739
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:latest` - linux; amd64

```console
$ docker pull percona@sha256:d801123bbfaf750924f993f5c59189d144a93feb928b8aef95e541dd61c62881
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196408390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0128954d5b0faaf39b6ff058fbcbb9a2f07f6b60c663312fada05c826cc93b3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:34:15 GMT
RUN groupdel input && groupadd -g 999 mysql
# Thu, 30 Jan 2020 23:34:15 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:34:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Wed, 05 Feb 2020 23:35:34 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Wed, 05 Feb 2020 23:37:01 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 05 Feb 2020 23:37:02 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 05 Feb 2020 23:37:02 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 05 Feb 2020 23:37:03 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 05 Feb 2020 23:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Feb 2020 23:37:03 GMT
USER mysql
# Wed, 05 Feb 2020 23:37:03 GMT
EXPOSE 3306
# Wed, 05 Feb 2020 23:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41876e5543b58e7c452f162a531b7fed8fd228ab59ecd9f10bec3de5510092`  
		Last Modified: Thu, 30 Jan 2020 23:37:24 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ef0baa29ddb873dbc81a8f0a044e9bbd01dedde4adf9df51e79e2ede50d832`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ffcf5dd2e603082b9bd847b058b227c15955c7cd1fb07ab954a9c2413275b2`  
		Last Modified: Thu, 30 Jan 2020 23:37:25 GMT  
		Size: 6.4 MB (6438113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957e94b3b4fdf505a520f31b2923d37a6a00e2ff2a9a5f8a0a982391eed0f6e2`  
		Last Modified: Wed, 05 Feb 2020 23:38:07 GMT  
		Size: 114.2 MB (114183023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b87447119d4ac1b9281878658de608e732a0ece81b6eac05bb78dd69536268`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020903636e3080388f087f7db0cd4898b625066e37d7fde08aa9f329c1a33f85`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5`

```console
$ docker pull percona@sha256:b9d2bf785a43b122a109bf233b0ae18aa98e8bd9b86a3d2eecd7c1d70b3e4739
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5` - linux; amd64

```console
$ docker pull percona@sha256:d801123bbfaf750924f993f5c59189d144a93feb928b8aef95e541dd61c62881
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196408390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0128954d5b0faaf39b6ff058fbcbb9a2f07f6b60c663312fada05c826cc93b3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:34:15 GMT
RUN groupdel input && groupadd -g 999 mysql
# Thu, 30 Jan 2020 23:34:15 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:34:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Wed, 05 Feb 2020 23:35:34 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Wed, 05 Feb 2020 23:37:01 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 05 Feb 2020 23:37:02 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 05 Feb 2020 23:37:02 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 05 Feb 2020 23:37:03 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 05 Feb 2020 23:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Feb 2020 23:37:03 GMT
USER mysql
# Wed, 05 Feb 2020 23:37:03 GMT
EXPOSE 3306
# Wed, 05 Feb 2020 23:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41876e5543b58e7c452f162a531b7fed8fd228ab59ecd9f10bec3de5510092`  
		Last Modified: Thu, 30 Jan 2020 23:37:24 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ef0baa29ddb873dbc81a8f0a044e9bbd01dedde4adf9df51e79e2ede50d832`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ffcf5dd2e603082b9bd847b058b227c15955c7cd1fb07ab954a9c2413275b2`  
		Last Modified: Thu, 30 Jan 2020 23:37:25 GMT  
		Size: 6.4 MB (6438113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957e94b3b4fdf505a520f31b2923d37a6a00e2ff2a9a5f8a0a982391eed0f6e2`  
		Last Modified: Wed, 05 Feb 2020 23:38:07 GMT  
		Size: 114.2 MB (114183023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b87447119d4ac1b9281878658de608e732a0ece81b6eac05bb78dd69536268`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020903636e3080388f087f7db0cd4898b625066e37d7fde08aa9f329c1a33f85`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.6`

```console
$ docker pull percona@sha256:6e7663c302a2bae40ac5ed1cc66e1ebfaa6562fea488d7410d81ee4f5d3fc062
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.6` - linux; amd64

```console
$ docker pull percona@sha256:e77a18d8abe8c6a8b741b7ba58b6e020c283027807faf4d3b6c5c403b3631e4a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.8 MB (139805570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a00a0872b8df291f587ac74ba255a2a042fabd3a7bf530e5bfd86f80c6055ff`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:34:15 GMT
RUN groupdel input && groupadd -g 999 mysql
# Thu, 30 Jan 2020 23:34:15 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:35:32 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Thu, 30 Jan 2020 23:35:33 GMT
ENV PERCONA_VERSION=5.6.47-rel87.0.1.el7
# Thu, 30 Jan 2020 23:36:14 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:36:15 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Jan 2020 23:36:15 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:36:15 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:36:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:36:16 GMT
USER mysql
# Thu, 30 Jan 2020 23:36:16 GMT
EXPOSE 3306
# Thu, 30 Jan 2020 23:36:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41876e5543b58e7c452f162a531b7fed8fd228ab59ecd9f10bec3de5510092`  
		Last Modified: Thu, 30 Jan 2020 23:37:24 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ef0baa29ddb873dbc81a8f0a044e9bbd01dedde4adf9df51e79e2ede50d832`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5892fb24bbc2b3b3ac50cd99711500635a814cefd5185f7544c92cf9a5763c2`  
		Last Modified: Thu, 30 Jan 2020 23:38:00 GMT  
		Size: 6.4 MB (6438137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f269d97ff7c87de17f939b8d5b146b65dca30d6cfccf2b303b87fd32ce72971`  
		Last Modified: Thu, 30 Jan 2020 23:38:08 GMT  
		Size: 57.6 MB (57576805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977017066ad7b9b02060f04115cead186246564e814059f3c0063bdc9f5d7f3a`  
		Last Modified: Thu, 30 Jan 2020 23:37:58 GMT  
		Size: 4.9 KB (4880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef40a45729664f63076da68020d602f8388b6e56552e95eeada12628854176a7`  
		Last Modified: Thu, 30 Jan 2020 23:37:58 GMT  
		Size: 2.9 KB (2941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.6.47`

```console
$ docker pull percona@sha256:6e7663c302a2bae40ac5ed1cc66e1ebfaa6562fea488d7410d81ee4f5d3fc062
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.6.47` - linux; amd64

```console
$ docker pull percona@sha256:e77a18d8abe8c6a8b741b7ba58b6e020c283027807faf4d3b6c5c403b3631e4a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.8 MB (139805570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a00a0872b8df291f587ac74ba255a2a042fabd3a7bf530e5bfd86f80c6055ff`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:34:15 GMT
RUN groupdel input && groupadd -g 999 mysql
# Thu, 30 Jan 2020 23:34:15 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:35:32 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Thu, 30 Jan 2020 23:35:33 GMT
ENV PERCONA_VERSION=5.6.47-rel87.0.1.el7
# Thu, 30 Jan 2020 23:36:14 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:36:15 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Jan 2020 23:36:15 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:36:15 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:36:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:36:16 GMT
USER mysql
# Thu, 30 Jan 2020 23:36:16 GMT
EXPOSE 3306
# Thu, 30 Jan 2020 23:36:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41876e5543b58e7c452f162a531b7fed8fd228ab59ecd9f10bec3de5510092`  
		Last Modified: Thu, 30 Jan 2020 23:37:24 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ef0baa29ddb873dbc81a8f0a044e9bbd01dedde4adf9df51e79e2ede50d832`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5892fb24bbc2b3b3ac50cd99711500635a814cefd5185f7544c92cf9a5763c2`  
		Last Modified: Thu, 30 Jan 2020 23:38:00 GMT  
		Size: 6.4 MB (6438137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f269d97ff7c87de17f939b8d5b146b65dca30d6cfccf2b303b87fd32ce72971`  
		Last Modified: Thu, 30 Jan 2020 23:38:08 GMT  
		Size: 57.6 MB (57576805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977017066ad7b9b02060f04115cead186246564e814059f3c0063bdc9f5d7f3a`  
		Last Modified: Thu, 30 Jan 2020 23:37:58 GMT  
		Size: 4.9 KB (4880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef40a45729664f63076da68020d602f8388b6e56552e95eeada12628854176a7`  
		Last Modified: Thu, 30 Jan 2020 23:37:58 GMT  
		Size: 2.9 KB (2941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.7`

```console
$ docker pull percona@sha256:b9d2bf785a43b122a109bf233b0ae18aa98e8bd9b86a3d2eecd7c1d70b3e4739
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.7` - linux; amd64

```console
$ docker pull percona@sha256:d801123bbfaf750924f993f5c59189d144a93feb928b8aef95e541dd61c62881
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196408390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0128954d5b0faaf39b6ff058fbcbb9a2f07f6b60c663312fada05c826cc93b3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:34:15 GMT
RUN groupdel input && groupadd -g 999 mysql
# Thu, 30 Jan 2020 23:34:15 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:34:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Wed, 05 Feb 2020 23:35:34 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Wed, 05 Feb 2020 23:37:01 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 05 Feb 2020 23:37:02 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 05 Feb 2020 23:37:02 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 05 Feb 2020 23:37:03 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 05 Feb 2020 23:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Feb 2020 23:37:03 GMT
USER mysql
# Wed, 05 Feb 2020 23:37:03 GMT
EXPOSE 3306
# Wed, 05 Feb 2020 23:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41876e5543b58e7c452f162a531b7fed8fd228ab59ecd9f10bec3de5510092`  
		Last Modified: Thu, 30 Jan 2020 23:37:24 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ef0baa29ddb873dbc81a8f0a044e9bbd01dedde4adf9df51e79e2ede50d832`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ffcf5dd2e603082b9bd847b058b227c15955c7cd1fb07ab954a9c2413275b2`  
		Last Modified: Thu, 30 Jan 2020 23:37:25 GMT  
		Size: 6.4 MB (6438113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957e94b3b4fdf505a520f31b2923d37a6a00e2ff2a9a5f8a0a982391eed0f6e2`  
		Last Modified: Wed, 05 Feb 2020 23:38:07 GMT  
		Size: 114.2 MB (114183023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b87447119d4ac1b9281878658de608e732a0ece81b6eac05bb78dd69536268`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020903636e3080388f087f7db0cd4898b625066e37d7fde08aa9f329c1a33f85`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.7.29`

```console
$ docker pull percona@sha256:b9d2bf785a43b122a109bf233b0ae18aa98e8bd9b86a3d2eecd7c1d70b3e4739
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.7.29` - linux; amd64

```console
$ docker pull percona@sha256:d801123bbfaf750924f993f5c59189d144a93feb928b8aef95e541dd61c62881
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196408390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0128954d5b0faaf39b6ff058fbcbb9a2f07f6b60c663312fada05c826cc93b3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:34:15 GMT
RUN groupdel input && groupadd -g 999 mysql
# Thu, 30 Jan 2020 23:34:15 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:34:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Wed, 05 Feb 2020 23:35:34 GMT
ENV PERCONA_VERSION=5.7.29-32.1.el7
# Wed, 05 Feb 2020 23:37:01 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 05 Feb 2020 23:37:02 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 05 Feb 2020 23:37:02 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 05 Feb 2020 23:37:03 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 05 Feb 2020 23:37:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Feb 2020 23:37:03 GMT
USER mysql
# Wed, 05 Feb 2020 23:37:03 GMT
EXPOSE 3306
# Wed, 05 Feb 2020 23:37:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41876e5543b58e7c452f162a531b7fed8fd228ab59ecd9f10bec3de5510092`  
		Last Modified: Thu, 30 Jan 2020 23:37:24 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ef0baa29ddb873dbc81a8f0a044e9bbd01dedde4adf9df51e79e2ede50d832`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ffcf5dd2e603082b9bd847b058b227c15955c7cd1fb07ab954a9c2413275b2`  
		Last Modified: Thu, 30 Jan 2020 23:37:25 GMT  
		Size: 6.4 MB (6438113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957e94b3b4fdf505a520f31b2923d37a6a00e2ff2a9a5f8a0a982391eed0f6e2`  
		Last Modified: Wed, 05 Feb 2020 23:38:07 GMT  
		Size: 114.2 MB (114183023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b87447119d4ac1b9281878658de608e732a0ece81b6eac05bb78dd69536268`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020903636e3080388f087f7db0cd4898b625066e37d7fde08aa9f329c1a33f85`  
		Last Modified: Wed, 05 Feb 2020 23:37:42 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8`

```console
$ docker pull percona@sha256:95b64ef7f23021ea64ca8626bf04d7f9a052aa7481ee1f38e8fda6d5a98dae5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8` - linux; amd64

```console
$ docker pull percona@sha256:30f000dc85bd13397c346bf1e3a228e850a8869b1da00d6e987a2fa7a30fb448
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.5 MB (224496206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e269b673aa2af7f9d8abf157fc1460094bf886f0a4a1887842f45a8cf5d59262`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:33:00 GMT
RUN groupadd -g 1001 mysql
# Thu, 30 Jan 2020 23:33:01 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:33:05 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 23 Mar 2020 21:20:10 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Mon, 23 Mar 2020 21:21:02 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 23 Mar 2020 21:21:03 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 23 Mar 2020 21:21:04 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 23 Mar 2020 21:21:04 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 23 Mar 2020 21:21:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 23 Mar 2020 21:21:04 GMT
USER mysql
# Mon, 23 Mar 2020 21:21:04 GMT
EXPOSE 3306 33060
# Mon, 23 Mar 2020 21:21:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296eab8cb2767bf28303443e7bc3a4a0cbc14383b23c877b7b8c2f776fdf81b5`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed24ac5fd1f63a28eaf64c5435879cc6199b8433c5f68df137d2c364e1c11a3b`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303807e74badcc2b04a965236de0c98f0a8339a3525041b2cbe9e1b4a0ba16ed`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 6.4 MB (6438611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b90f167fb2a76e1742630dec20b9071a652cd47b9da24a39e19d1707478b470`  
		Last Modified: Mon, 23 Mar 2020 21:22:09 GMT  
		Size: 142.3 MB (142270573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962beccc99b2c7576801e02694f56db43953528e83fdee44aeb8138742b8de37`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c63f042185c82285c5bcd15c1624ab9de38042bca2b66748d7d1d4ef15f737`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0`

```console
$ docker pull percona@sha256:95b64ef7f23021ea64ca8626bf04d7f9a052aa7481ee1f38e8fda6d5a98dae5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8.0` - linux; amd64

```console
$ docker pull percona@sha256:30f000dc85bd13397c346bf1e3a228e850a8869b1da00d6e987a2fa7a30fb448
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.5 MB (224496206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e269b673aa2af7f9d8abf157fc1460094bf886f0a4a1887842f45a8cf5d59262`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:33:00 GMT
RUN groupadd -g 1001 mysql
# Thu, 30 Jan 2020 23:33:01 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:33:05 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 23 Mar 2020 21:20:10 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Mon, 23 Mar 2020 21:21:02 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 23 Mar 2020 21:21:03 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 23 Mar 2020 21:21:04 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 23 Mar 2020 21:21:04 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 23 Mar 2020 21:21:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 23 Mar 2020 21:21:04 GMT
USER mysql
# Mon, 23 Mar 2020 21:21:04 GMT
EXPOSE 3306 33060
# Mon, 23 Mar 2020 21:21:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296eab8cb2767bf28303443e7bc3a4a0cbc14383b23c877b7b8c2f776fdf81b5`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed24ac5fd1f63a28eaf64c5435879cc6199b8433c5f68df137d2c364e1c11a3b`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303807e74badcc2b04a965236de0c98f0a8339a3525041b2cbe9e1b4a0ba16ed`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 6.4 MB (6438611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b90f167fb2a76e1742630dec20b9071a652cd47b9da24a39e19d1707478b470`  
		Last Modified: Mon, 23 Mar 2020 21:22:09 GMT  
		Size: 142.3 MB (142270573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962beccc99b2c7576801e02694f56db43953528e83fdee44aeb8138742b8de37`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c63f042185c82285c5bcd15c1624ab9de38042bca2b66748d7d1d4ef15f737`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0.19-10`

```console
$ docker pull percona@sha256:95b64ef7f23021ea64ca8626bf04d7f9a052aa7481ee1f38e8fda6d5a98dae5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8.0.19-10` - linux; amd64

```console
$ docker pull percona@sha256:30f000dc85bd13397c346bf1e3a228e850a8869b1da00d6e987a2fa7a30fb448
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.5 MB (224496206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e269b673aa2af7f9d8abf157fc1460094bf886f0a4a1887842f45a8cf5d59262`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 30 Jan 2020 23:33:00 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jan 2020 23:33:00 GMT
RUN groupadd -g 1001 mysql
# Thu, 30 Jan 2020 23:33:01 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Thu, 30 Jan 2020 23:33:05 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 23 Mar 2020 21:20:10 GMT
ENV PERCONA_VERSION=8.0.19-10.1.el7
# Mon, 23 Mar 2020 21:21:02 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 23 Mar 2020 21:21:03 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 23 Mar 2020 21:21:04 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 23 Mar 2020 21:21:04 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 23 Mar 2020 21:21:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 23 Mar 2020 21:21:04 GMT
USER mysql
# Mon, 23 Mar 2020 21:21:04 GMT
EXPOSE 3306 33060
# Mon, 23 Mar 2020 21:21:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296eab8cb2767bf28303443e7bc3a4a0cbc14383b23c877b7b8c2f776fdf81b5`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed24ac5fd1f63a28eaf64c5435879cc6199b8433c5f68df137d2c364e1c11a3b`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303807e74badcc2b04a965236de0c98f0a8339a3525041b2cbe9e1b4a0ba16ed`  
		Last Modified: Thu, 30 Jan 2020 23:36:41 GMT  
		Size: 6.4 MB (6438611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b90f167fb2a76e1742630dec20b9071a652cd47b9da24a39e19d1707478b470`  
		Last Modified: Mon, 23 Mar 2020 21:22:09 GMT  
		Size: 142.3 MB (142270573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962beccc99b2c7576801e02694f56db43953528e83fdee44aeb8138742b8de37`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c63f042185c82285c5bcd15c1624ab9de38042bca2b66748d7d1d4ef15f737`  
		Last Modified: Mon, 23 Mar 2020 21:21:42 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-3.6`

```console
$ docker pull percona@sha256:dd5bfaa9be06fefdfb84811acb9e5e3c03047ac86773fa1c7381bce5ec90d598
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6` - linux; amd64

```console
$ docker pull percona@sha256:8d25c48d84055ee139945b8c2134b447ccf6b3785d4b996e0655fb4812fe1ab0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.3 MB (156272430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883a53a9e34d6aff5f88d4c7e1a5305962dc7d28a16d099d9a37c3dd6b0b8b8d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Wed, 29 Jan 2020 19:37:33 GMT
LABEL org.label-schema.schema-version=1.0
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.vendor=Percona
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.license=SSPLv1
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.opencontainers.image.vendor=Percona
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 15 Feb 2020 02:34:40 GMT
ENV PSMDB_VERSION=3.6.17-4.0
# Sat, 15 Feb 2020 02:34:40 GMT
LABEL org.label-schema.schema-version=3.6.17-4.0
# Sat, 15 Feb 2020 02:34:40 GMT
LABEL org.opencontainers.image.version=3.6.17-4.0
# Sat, 15 Feb 2020 02:34:44 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 15 Feb 2020 02:34:44 GMT
ENV OS_VER=el7
# Sat, 15 Feb 2020 02:34:45 GMT
ENV FULL_PERCONA_VERSION=3.6.17-4.0.el7
# Sat, 15 Feb 2020 02:34:45 GMT
ENV K8S_TOOLS_VERSION=0.4.2
# Sat, 15 Feb 2020 02:34:53 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Sat, 15 Feb 2020 02:35:49 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         yum-utils         shadow-utils         curl         procps-ng         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         yum clean all;         rm -rf /var/cache/yum /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Sat, 15 Feb 2020 02:35:50 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Sat, 15 Feb 2020 02:35:50 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 15 Feb 2020 02:35:51 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 15 Feb 2020 02:35:54 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 15 Feb 2020 02:35:54 GMT
VOLUME [/data/db]
# Sat, 15 Feb 2020 02:35:54 GMT
COPY file:85995e73e1e4d284ba65fabe65ed1e96fcb9c00ac0d328edb8b0b48749d784e1 in /entrypoint.sh 
# Sat, 15 Feb 2020 02:35:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 15 Feb 2020 02:35:55 GMT
EXPOSE 27017
# Sat, 15 Feb 2020 02:35:55 GMT
USER 1001
# Sat, 15 Feb 2020 02:35:55 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8f6987cdb938d0c2d7dabb952a4b2da195e5718c7abfa905b856b44d3f0f11`  
		Last Modified: Sat, 15 Feb 2020 02:36:29 GMT  
		Size: 6.4 MB (6380108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b368bc523806afffa36ef648c085dca9220781e35672c4918d9a9eb7dce3c664`  
		Last Modified: Sat, 15 Feb 2020 02:36:29 GMT  
		Size: 6.7 MB (6714918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb925f51e9fbbd8f697cabdbdac4e7269e42e1d4ecad85d68904979bdf31ec9`  
		Last Modified: Sat, 15 Feb 2020 02:36:38 GMT  
		Size: 59.8 MB (59811064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53d05cb4345d8123226acbff3db4bf637d57ed84fc828164d08b6dbc6cddd3f`  
		Last Modified: Sat, 15 Feb 2020 02:36:26 GMT  
		Size: 1.6 KB (1593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01051e0b33b5505b62bc9b1528cb4f8559346eb9a1e4b087d353c30383783220`  
		Last Modified: Sat, 15 Feb 2020 02:36:26 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cadad8163185f9a431fab412987e2794ea61e37c75f9d422dc171115dfc3435`  
		Last Modified: Sat, 15 Feb 2020 02:36:27 GMT  
		Size: 10.6 KB (10575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6eb624038abdab1f46d6d46afe5bcbb7962932b306bc66ea8a6034092256c99`  
		Last Modified: Sat, 15 Feb 2020 02:36:28 GMT  
		Size: 7.6 MB (7565368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c3be571e044284c5f520de72c1f89fe9ade2fb38621d85bcfd516d852aeb8f`  
		Last Modified: Sat, 15 Feb 2020 02:36:26 GMT  
		Size: 4.0 KB (4018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-3.6.17`

```console
$ docker pull percona@sha256:dd5bfaa9be06fefdfb84811acb9e5e3c03047ac86773fa1c7381bce5ec90d598
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6.17` - linux; amd64

```console
$ docker pull percona@sha256:8d25c48d84055ee139945b8c2134b447ccf6b3785d4b996e0655fb4812fe1ab0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.3 MB (156272430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883a53a9e34d6aff5f88d4c7e1a5305962dc7d28a16d099d9a37c3dd6b0b8b8d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Wed, 29 Jan 2020 19:37:33 GMT
LABEL org.label-schema.schema-version=1.0
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.vendor=Percona
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.license=SSPLv1
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.opencontainers.image.vendor=Percona
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 15 Feb 2020 02:34:40 GMT
ENV PSMDB_VERSION=3.6.17-4.0
# Sat, 15 Feb 2020 02:34:40 GMT
LABEL org.label-schema.schema-version=3.6.17-4.0
# Sat, 15 Feb 2020 02:34:40 GMT
LABEL org.opencontainers.image.version=3.6.17-4.0
# Sat, 15 Feb 2020 02:34:44 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 15 Feb 2020 02:34:44 GMT
ENV OS_VER=el7
# Sat, 15 Feb 2020 02:34:45 GMT
ENV FULL_PERCONA_VERSION=3.6.17-4.0.el7
# Sat, 15 Feb 2020 02:34:45 GMT
ENV K8S_TOOLS_VERSION=0.4.2
# Sat, 15 Feb 2020 02:34:53 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Sat, 15 Feb 2020 02:35:49 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         yum-utils         shadow-utils         curl         procps-ng         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         yum clean all;         rm -rf /var/cache/yum /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Sat, 15 Feb 2020 02:35:50 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Sat, 15 Feb 2020 02:35:50 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 15 Feb 2020 02:35:51 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 15 Feb 2020 02:35:54 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 15 Feb 2020 02:35:54 GMT
VOLUME [/data/db]
# Sat, 15 Feb 2020 02:35:54 GMT
COPY file:85995e73e1e4d284ba65fabe65ed1e96fcb9c00ac0d328edb8b0b48749d784e1 in /entrypoint.sh 
# Sat, 15 Feb 2020 02:35:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 15 Feb 2020 02:35:55 GMT
EXPOSE 27017
# Sat, 15 Feb 2020 02:35:55 GMT
USER 1001
# Sat, 15 Feb 2020 02:35:55 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8f6987cdb938d0c2d7dabb952a4b2da195e5718c7abfa905b856b44d3f0f11`  
		Last Modified: Sat, 15 Feb 2020 02:36:29 GMT  
		Size: 6.4 MB (6380108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b368bc523806afffa36ef648c085dca9220781e35672c4918d9a9eb7dce3c664`  
		Last Modified: Sat, 15 Feb 2020 02:36:29 GMT  
		Size: 6.7 MB (6714918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb925f51e9fbbd8f697cabdbdac4e7269e42e1d4ecad85d68904979bdf31ec9`  
		Last Modified: Sat, 15 Feb 2020 02:36:38 GMT  
		Size: 59.8 MB (59811064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53d05cb4345d8123226acbff3db4bf637d57ed84fc828164d08b6dbc6cddd3f`  
		Last Modified: Sat, 15 Feb 2020 02:36:26 GMT  
		Size: 1.6 KB (1593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01051e0b33b5505b62bc9b1528cb4f8559346eb9a1e4b087d353c30383783220`  
		Last Modified: Sat, 15 Feb 2020 02:36:26 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cadad8163185f9a431fab412987e2794ea61e37c75f9d422dc171115dfc3435`  
		Last Modified: Sat, 15 Feb 2020 02:36:27 GMT  
		Size: 10.6 KB (10575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6eb624038abdab1f46d6d46afe5bcbb7962932b306bc66ea8a6034092256c99`  
		Last Modified: Sat, 15 Feb 2020 02:36:28 GMT  
		Size: 7.6 MB (7565368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c3be571e044284c5f520de72c1f89fe9ade2fb38621d85bcfd516d852aeb8f`  
		Last Modified: Sat, 15 Feb 2020 02:36:26 GMT  
		Size: 4.0 KB (4018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.0`

```console
$ docker pull percona@sha256:c937b9a6696162910a3b1e5c851b9d3335700a50f9a9cf042bc6826ac0ba041f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0` - linux; amd64

```console
$ docker pull percona@sha256:1011c0e4100498c48b392842fed8b161e7a7ade0480764c1b356147196d3fb69
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.1 MB (160142768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a383bc18c37f73a3304fd9edbe81f189f9b761e1e01b75b7974aa9f12bf60096`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Wed, 29 Jan 2020 19:37:33 GMT
LABEL org.label-schema.schema-version=1.0
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.vendor=Percona
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.license=SSPLv1
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.opencontainers.image.vendor=Percona
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Apr 2020 19:34:59 GMT
ENV PSMDB_VERSION=4.0.18-11
# Thu, 30 Apr 2020 19:34:59 GMT
LABEL org.label-schema.schema-version=4.0.18-11
# Thu, 30 Apr 2020 19:34:59 GMT
LABEL org.opencontainers.image.version=4.0.18-11
# Thu, 30 Apr 2020 19:35:07 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-40 release
# Thu, 30 Apr 2020 19:35:07 GMT
ENV OS_VER=el7
# Thu, 30 Apr 2020 19:35:07 GMT
ENV FULL_PERCONA_VERSION=4.0.18-11.el7
# Thu, 30 Apr 2020 19:35:08 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 30 Apr 2020 19:35:13 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Thu, 30 Apr 2020 19:35:38 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 30 Apr 2020 19:35:39 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 30 Apr 2020 19:35:39 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 30 Apr 2020 19:35:40 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 30 Apr 2020 19:35:40 GMT
ENV GOSU_VERSION=1.11
# Thu, 30 Apr 2020 19:35:43 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 30 Apr 2020 19:35:45 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 30 Apr 2020 19:35:46 GMT
VOLUME [/data/db]
# Thu, 30 Apr 2020 19:35:46 GMT
COPY file:85995e73e1e4d284ba65fabe65ed1e96fcb9c00ac0d328edb8b0b48749d784e1 in /entrypoint.sh 
# Thu, 30 Apr 2020 19:35:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Apr 2020 19:35:46 GMT
EXPOSE 27017
# Thu, 30 Apr 2020 19:35:46 GMT
USER 1001
# Thu, 30 Apr 2020 19:35:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b430acd1012a6145fca50e4b059b9307dcc8959d2c9e975ebbd76f6b1f65618c`  
		Last Modified: Thu, 30 Apr 2020 19:36:15 GMT  
		Size: 6.4 MB (6381258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30eb48b75d742d4f4aebdd11257c39b2bbe788fe200df2cfdaa3c9bea1c9276b`  
		Last Modified: Thu, 30 Apr 2020 19:36:13 GMT  
		Size: 6.7 MB (6717491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1c37e185840ccaf8ede879c828e0b40d2d41918732a40503c2123b25e0cfa0`  
		Last Modified: Thu, 30 Apr 2020 19:36:23 GMT  
		Size: 62.2 MB (62188704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b808070801fd1b3b62094e7a00b9f5a7b8f483f29dedbc2f14d647d623e4bd11`  
		Last Modified: Thu, 30 Apr 2020 19:36:11 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1b9f03806b07e3fbcdd9d67b2c9ab29187674817751db7d50d8a137791c202`  
		Last Modified: Thu, 30 Apr 2020 19:36:10 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9fd51567b713434cde6fd33e37fbc79086df6f26ad2540b9303c047be00792b`  
		Last Modified: Thu, 30 Apr 2020 19:36:10 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ac4931be0a6e11c200d7edd6d820bf1b31aae950254c849510a2491e5f3377`  
		Last Modified: Thu, 30 Apr 2020 19:36:12 GMT  
		Size: 915.5 KB (915462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc31f4768b13c510a17cd9a9ac4a0628dc10046f7a37dfc32e9d9a232a6ef6c`  
		Last Modified: Thu, 30 Apr 2020 19:36:20 GMT  
		Size: 8.1 MB (8138875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d165a06d912a28fbd137298247e5e2262194e350c0bd748d763c523e5321b361`  
		Last Modified: Thu, 30 Apr 2020 19:36:10 GMT  
		Size: 4.0 KB (4017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.0.18`

```console
$ docker pull percona@sha256:c937b9a6696162910a3b1e5c851b9d3335700a50f9a9cf042bc6826ac0ba041f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0.18` - linux; amd64

```console
$ docker pull percona@sha256:1011c0e4100498c48b392842fed8b161e7a7ade0480764c1b356147196d3fb69
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.1 MB (160142768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a383bc18c37f73a3304fd9edbe81f189f9b761e1e01b75b7974aa9f12bf60096`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Wed, 29 Jan 2020 19:37:33 GMT
LABEL org.label-schema.schema-version=1.0
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.vendor=Percona
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.license=SSPLv1
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.opencontainers.image.vendor=Percona
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Apr 2020 19:34:59 GMT
ENV PSMDB_VERSION=4.0.18-11
# Thu, 30 Apr 2020 19:34:59 GMT
LABEL org.label-schema.schema-version=4.0.18-11
# Thu, 30 Apr 2020 19:34:59 GMT
LABEL org.opencontainers.image.version=4.0.18-11
# Thu, 30 Apr 2020 19:35:07 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-40 release
# Thu, 30 Apr 2020 19:35:07 GMT
ENV OS_VER=el7
# Thu, 30 Apr 2020 19:35:07 GMT
ENV FULL_PERCONA_VERSION=4.0.18-11.el7
# Thu, 30 Apr 2020 19:35:08 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 30 Apr 2020 19:35:13 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Thu, 30 Apr 2020 19:35:38 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 30 Apr 2020 19:35:39 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 30 Apr 2020 19:35:39 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 30 Apr 2020 19:35:40 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 30 Apr 2020 19:35:40 GMT
ENV GOSU_VERSION=1.11
# Thu, 30 Apr 2020 19:35:43 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 30 Apr 2020 19:35:45 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 30 Apr 2020 19:35:46 GMT
VOLUME [/data/db]
# Thu, 30 Apr 2020 19:35:46 GMT
COPY file:85995e73e1e4d284ba65fabe65ed1e96fcb9c00ac0d328edb8b0b48749d784e1 in /entrypoint.sh 
# Thu, 30 Apr 2020 19:35:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Apr 2020 19:35:46 GMT
EXPOSE 27017
# Thu, 30 Apr 2020 19:35:46 GMT
USER 1001
# Thu, 30 Apr 2020 19:35:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b430acd1012a6145fca50e4b059b9307dcc8959d2c9e975ebbd76f6b1f65618c`  
		Last Modified: Thu, 30 Apr 2020 19:36:15 GMT  
		Size: 6.4 MB (6381258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30eb48b75d742d4f4aebdd11257c39b2bbe788fe200df2cfdaa3c9bea1c9276b`  
		Last Modified: Thu, 30 Apr 2020 19:36:13 GMT  
		Size: 6.7 MB (6717491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1c37e185840ccaf8ede879c828e0b40d2d41918732a40503c2123b25e0cfa0`  
		Last Modified: Thu, 30 Apr 2020 19:36:23 GMT  
		Size: 62.2 MB (62188704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b808070801fd1b3b62094e7a00b9f5a7b8f483f29dedbc2f14d647d623e4bd11`  
		Last Modified: Thu, 30 Apr 2020 19:36:11 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1b9f03806b07e3fbcdd9d67b2c9ab29187674817751db7d50d8a137791c202`  
		Last Modified: Thu, 30 Apr 2020 19:36:10 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9fd51567b713434cde6fd33e37fbc79086df6f26ad2540b9303c047be00792b`  
		Last Modified: Thu, 30 Apr 2020 19:36:10 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ac4931be0a6e11c200d7edd6d820bf1b31aae950254c849510a2491e5f3377`  
		Last Modified: Thu, 30 Apr 2020 19:36:12 GMT  
		Size: 915.5 KB (915462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc31f4768b13c510a17cd9a9ac4a0628dc10046f7a37dfc32e9d9a232a6ef6c`  
		Last Modified: Thu, 30 Apr 2020 19:36:20 GMT  
		Size: 8.1 MB (8138875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d165a06d912a28fbd137298247e5e2262194e350c0bd748d763c523e5321b361`  
		Last Modified: Thu, 30 Apr 2020 19:36:10 GMT  
		Size: 4.0 KB (4017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:f4c8ffe4c5f94bc423c9109919f880f6bc49791fb5becf48632ec6213128cbd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:b51e170e9fd6409c696aaa5e4241c28f92366a8f10543918fe08581d35f506a5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.5 MB (169489840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c02b22bd30e8b8380ab55231749f340eecf99b48458a094d864fa68823f3620`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Wed, 29 Jan 2020 19:37:33 GMT
LABEL org.label-schema.schema-version=1.0
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.vendor=Percona
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.license=SSPLv1
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.opencontainers.image.vendor=Percona
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 02 Apr 2020 22:20:54 GMT
ENV PSMDB_VERSION=4.2.5-5
# Thu, 02 Apr 2020 22:20:54 GMT
LABEL org.label-schema.schema-version=4.2.5-5
# Thu, 02 Apr 2020 22:20:54 GMT
LABEL org.opencontainers.image.version=4.2.5-5
# Thu, 02 Apr 2020 22:22:54 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Thu, 02 Apr 2020 22:22:55 GMT
ENV OS_VER=el7
# Thu, 02 Apr 2020 22:22:55 GMT
ENV FULL_PERCONA_VERSION=4.2.5-5.el7
# Thu, 02 Apr 2020 22:22:55 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 02 Apr 2020 22:23:01 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Thu, 02 Apr 2020 22:23:27 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 02 Apr 2020 22:23:28 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 02 Apr 2020 22:23:28 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 02 Apr 2020 22:23:29 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 02 Apr 2020 22:23:29 GMT
ENV GOSU_VERSION=1.11
# Thu, 02 Apr 2020 22:23:31 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 02 Apr 2020 22:23:34 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 02 Apr 2020 22:23:34 GMT
VOLUME [/data/db]
# Thu, 02 Apr 2020 22:23:34 GMT
COPY file:d143ecb7a542d31ae4c95807064d8fad35f488059238d10fcd8b10f214d58331 in /entrypoint.sh 
# Thu, 02 Apr 2020 22:23:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Apr 2020 22:23:35 GMT
EXPOSE 27017
# Thu, 02 Apr 2020 22:23:35 GMT
USER 1001
# Thu, 02 Apr 2020 22:23:35 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc521f011e82a88e6d0a3188d1d9a2079c720f8a8700c163c7c5e41b13fb6599`  
		Last Modified: Thu, 02 Apr 2020 22:24:05 GMT  
		Size: 6.4 MB (6380271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c233308c343801e65aee2d70e54fca3ebd2c471e4a4c8dd22549207843c90beb`  
		Last Modified: Thu, 02 Apr 2020 22:24:05 GMT  
		Size: 6.7 MB (6717242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09053abfb58eab845e595666537f1cf050f052d031686b75dffc19c11f464a85`  
		Last Modified: Thu, 02 Apr 2020 22:24:18 GMT  
		Size: 71.5 MB (71536593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7006efe00012c9d9fcaecfa36574d24c3c6cd6c3e600f7388e65c979468eaabc`  
		Last Modified: Thu, 02 Apr 2020 22:24:03 GMT  
		Size: 1.6 KB (1592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cafae1bfce6f869d0dab1f8fa6c1f77db63503b1cb3408b3686c2aefbe482a`  
		Last Modified: Thu, 02 Apr 2020 22:24:02 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a358bfb1df2d674f3705449fe2e7a0bf3d7bea42b9b4355b6c9a1ad2c3e100a7`  
		Last Modified: Thu, 02 Apr 2020 22:24:02 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665d90b302ab0f42d9f40a01639e897665ef17a8a4de72d2c3d8238a56451a00`  
		Last Modified: Thu, 02 Apr 2020 22:24:02 GMT  
		Size: 915.5 KB (915467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a4206b014321ed9ae0150e800becc8db002e8047e425d40391233b91cd7df0`  
		Last Modified: Thu, 02 Apr 2020 22:24:04 GMT  
		Size: 8.1 MB (8138872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1d721b826f2468fd2fa4e6df9506cb766fb1b79909c2ad87ece0b109fa06b0`  
		Last Modified: Thu, 02 Apr 2020 22:24:02 GMT  
		Size: 4.4 KB (4437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2.5`

```console
$ docker pull percona@sha256:f4c8ffe4c5f94bc423c9109919f880f6bc49791fb5becf48632ec6213128cbd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.2.5` - linux; amd64

```console
$ docker pull percona@sha256:b51e170e9fd6409c696aaa5e4241c28f92366a8f10543918fe08581d35f506a5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.5 MB (169489840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c02b22bd30e8b8380ab55231749f340eecf99b48458a094d864fa68823f3620`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Wed, 29 Jan 2020 19:37:33 GMT
LABEL org.label-schema.schema-version=1.0
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.vendor=Percona
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.license=SSPLv1
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.opencontainers.image.vendor=Percona
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 02 Apr 2020 22:20:54 GMT
ENV PSMDB_VERSION=4.2.5-5
# Thu, 02 Apr 2020 22:20:54 GMT
LABEL org.label-schema.schema-version=4.2.5-5
# Thu, 02 Apr 2020 22:20:54 GMT
LABEL org.opencontainers.image.version=4.2.5-5
# Thu, 02 Apr 2020 22:22:54 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Thu, 02 Apr 2020 22:22:55 GMT
ENV OS_VER=el7
# Thu, 02 Apr 2020 22:22:55 GMT
ENV FULL_PERCONA_VERSION=4.2.5-5.el7
# Thu, 02 Apr 2020 22:22:55 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 02 Apr 2020 22:23:01 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Thu, 02 Apr 2020 22:23:27 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 02 Apr 2020 22:23:28 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 02 Apr 2020 22:23:28 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 02 Apr 2020 22:23:29 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 02 Apr 2020 22:23:29 GMT
ENV GOSU_VERSION=1.11
# Thu, 02 Apr 2020 22:23:31 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 02 Apr 2020 22:23:34 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 02 Apr 2020 22:23:34 GMT
VOLUME [/data/db]
# Thu, 02 Apr 2020 22:23:34 GMT
COPY file:d143ecb7a542d31ae4c95807064d8fad35f488059238d10fcd8b10f214d58331 in /entrypoint.sh 
# Thu, 02 Apr 2020 22:23:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Apr 2020 22:23:35 GMT
EXPOSE 27017
# Thu, 02 Apr 2020 22:23:35 GMT
USER 1001
# Thu, 02 Apr 2020 22:23:35 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc521f011e82a88e6d0a3188d1d9a2079c720f8a8700c163c7c5e41b13fb6599`  
		Last Modified: Thu, 02 Apr 2020 22:24:05 GMT  
		Size: 6.4 MB (6380271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c233308c343801e65aee2d70e54fca3ebd2c471e4a4c8dd22549207843c90beb`  
		Last Modified: Thu, 02 Apr 2020 22:24:05 GMT  
		Size: 6.7 MB (6717242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09053abfb58eab845e595666537f1cf050f052d031686b75dffc19c11f464a85`  
		Last Modified: Thu, 02 Apr 2020 22:24:18 GMT  
		Size: 71.5 MB (71536593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7006efe00012c9d9fcaecfa36574d24c3c6cd6c3e600f7388e65c979468eaabc`  
		Last Modified: Thu, 02 Apr 2020 22:24:03 GMT  
		Size: 1.6 KB (1592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cafae1bfce6f869d0dab1f8fa6c1f77db63503b1cb3408b3686c2aefbe482a`  
		Last Modified: Thu, 02 Apr 2020 22:24:02 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a358bfb1df2d674f3705449fe2e7a0bf3d7bea42b9b4355b6c9a1ad2c3e100a7`  
		Last Modified: Thu, 02 Apr 2020 22:24:02 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665d90b302ab0f42d9f40a01639e897665ef17a8a4de72d2c3d8238a56451a00`  
		Last Modified: Thu, 02 Apr 2020 22:24:02 GMT  
		Size: 915.5 KB (915467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a4206b014321ed9ae0150e800becc8db002e8047e425d40391233b91cd7df0`  
		Last Modified: Thu, 02 Apr 2020 22:24:04 GMT  
		Size: 8.1 MB (8138872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1d721b826f2468fd2fa4e6df9506cb766fb1b79909c2ad87ece0b109fa06b0`  
		Last Modified: Thu, 02 Apr 2020 22:24:02 GMT  
		Size: 4.4 KB (4437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
