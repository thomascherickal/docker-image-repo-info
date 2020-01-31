<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `percona`

-	[`percona:5`](#percona5)
-	[`percona:5.6`](#percona56)
-	[`percona:5.6.47`](#percona5647)
-	[`percona:5.6.47-centos`](#percona5647-centos)
-	[`percona:5.6-centos`](#percona56-centos)
-	[`percona:5.7`](#percona57)
-	[`percona:5.7.28`](#percona5728)
-	[`percona:5.7.28-centos`](#percona5728-centos)
-	[`percona:5.7-centos`](#percona57-centos)
-	[`percona:5-centos`](#percona5-centos)
-	[`percona:8`](#percona8)
-	[`percona:8.0`](#percona80)
-	[`percona:8.0.18-9`](#percona8018-9)
-	[`percona:8.0.18-9-centos`](#percona8018-9-centos)
-	[`percona:8.0-centos`](#percona80-centos)
-	[`percona:8-centos`](#percona8-centos)
-	[`percona:centos`](#perconacentos)
-	[`percona:latest`](#perconalatest)
-	[`percona:ps-5`](#perconaps-5)
-	[`percona:ps-5.6`](#perconaps-56)
-	[`percona:ps-5.6.47`](#perconaps-5647)
-	[`percona:ps-5.7`](#perconaps-57)
-	[`percona:ps-5.7.28`](#perconaps-5728)
-	[`percona:ps-8`](#perconaps-8)
-	[`percona:ps-8.0`](#perconaps-80)
-	[`percona:ps-8.0.18-9`](#perconaps-8018-9)
-	[`percona:psmdb-3.6`](#perconapsmdb-36)
-	[`percona:psmdb-3.6.16`](#perconapsmdb-3616)
-	[`percona:psmdb-4.0`](#perconapsmdb-40)
-	[`percona:psmdb-4.0.14`](#perconapsmdb-4014)
-	[`percona:psmdb-4.2`](#perconapsmdb-42)
-	[`percona:psmdb-4.2.2`](#perconapsmdb-422)

## `percona:5`

```console
$ docker pull percona@sha256:657730edcb3c268b37360d9e3ecb7e776a83ebb9a6027688fb68e4b45ef40ffe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5` - linux; amd64

```console
$ docker pull percona@sha256:1de5f84148c22bf55ebb47d6507eed0c072e45a694d7841ed359773236b2bb01
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193935403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9525064c8e2527931e33be2c6ba6868aa28f948ad2cd91d7317ab5938f144cd`
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
# Thu, 30 Jan 2020 23:34:20 GMT
ENV PERCONA_VERSION=5.7.28-31.1.el7
# Thu, 30 Jan 2020 23:35:15 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:35:15 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 30 Jan 2020 23:35:16 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:35:16 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:35:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:35:16 GMT
USER mysql
# Thu, 30 Jan 2020 23:35:16 GMT
EXPOSE 3306
# Thu, 30 Jan 2020 23:35:17 GMT
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
	-	`sha256:2c4e76436340f27cb846339ac414b3ddc6aafab23726bf117e40d2b17988ff8b`  
		Last Modified: Thu, 30 Jan 2020 23:37:49 GMT  
		Size: 111.7 MB (111710030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf05bcd6eb9056238d6239f3d374cdbf4319a58b35949b8e4be17c4bfbc405a`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe05bc0d56e90717f9fd0de98c24521adc2f245537cb3363d088a9a6524e3438`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
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
$ docker pull percona@sha256:657730edcb3c268b37360d9e3ecb7e776a83ebb9a6027688fb68e4b45ef40ffe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7` - linux; amd64

```console
$ docker pull percona@sha256:1de5f84148c22bf55ebb47d6507eed0c072e45a694d7841ed359773236b2bb01
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193935403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9525064c8e2527931e33be2c6ba6868aa28f948ad2cd91d7317ab5938f144cd`
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
# Thu, 30 Jan 2020 23:34:20 GMT
ENV PERCONA_VERSION=5.7.28-31.1.el7
# Thu, 30 Jan 2020 23:35:15 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:35:15 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 30 Jan 2020 23:35:16 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:35:16 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:35:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:35:16 GMT
USER mysql
# Thu, 30 Jan 2020 23:35:16 GMT
EXPOSE 3306
# Thu, 30 Jan 2020 23:35:17 GMT
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
	-	`sha256:2c4e76436340f27cb846339ac414b3ddc6aafab23726bf117e40d2b17988ff8b`  
		Last Modified: Thu, 30 Jan 2020 23:37:49 GMT  
		Size: 111.7 MB (111710030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf05bcd6eb9056238d6239f3d374cdbf4319a58b35949b8e4be17c4bfbc405a`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe05bc0d56e90717f9fd0de98c24521adc2f245537cb3363d088a9a6524e3438`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.28`

```console
$ docker pull percona@sha256:657730edcb3c268b37360d9e3ecb7e776a83ebb9a6027688fb68e4b45ef40ffe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7.28` - linux; amd64

```console
$ docker pull percona@sha256:1de5f84148c22bf55ebb47d6507eed0c072e45a694d7841ed359773236b2bb01
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193935403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9525064c8e2527931e33be2c6ba6868aa28f948ad2cd91d7317ab5938f144cd`
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
# Thu, 30 Jan 2020 23:34:20 GMT
ENV PERCONA_VERSION=5.7.28-31.1.el7
# Thu, 30 Jan 2020 23:35:15 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:35:15 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 30 Jan 2020 23:35:16 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:35:16 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:35:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:35:16 GMT
USER mysql
# Thu, 30 Jan 2020 23:35:16 GMT
EXPOSE 3306
# Thu, 30 Jan 2020 23:35:17 GMT
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
	-	`sha256:2c4e76436340f27cb846339ac414b3ddc6aafab23726bf117e40d2b17988ff8b`  
		Last Modified: Thu, 30 Jan 2020 23:37:49 GMT  
		Size: 111.7 MB (111710030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf05bcd6eb9056238d6239f3d374cdbf4319a58b35949b8e4be17c4bfbc405a`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe05bc0d56e90717f9fd0de98c24521adc2f245537cb3363d088a9a6524e3438`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.28-centos`

```console
$ docker pull percona@sha256:657730edcb3c268b37360d9e3ecb7e776a83ebb9a6027688fb68e4b45ef40ffe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7.28-centos` - linux; amd64

```console
$ docker pull percona@sha256:1de5f84148c22bf55ebb47d6507eed0c072e45a694d7841ed359773236b2bb01
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193935403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9525064c8e2527931e33be2c6ba6868aa28f948ad2cd91d7317ab5938f144cd`
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
# Thu, 30 Jan 2020 23:34:20 GMT
ENV PERCONA_VERSION=5.7.28-31.1.el7
# Thu, 30 Jan 2020 23:35:15 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:35:15 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 30 Jan 2020 23:35:16 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:35:16 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:35:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:35:16 GMT
USER mysql
# Thu, 30 Jan 2020 23:35:16 GMT
EXPOSE 3306
# Thu, 30 Jan 2020 23:35:17 GMT
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
	-	`sha256:2c4e76436340f27cb846339ac414b3ddc6aafab23726bf117e40d2b17988ff8b`  
		Last Modified: Thu, 30 Jan 2020 23:37:49 GMT  
		Size: 111.7 MB (111710030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf05bcd6eb9056238d6239f3d374cdbf4319a58b35949b8e4be17c4bfbc405a`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe05bc0d56e90717f9fd0de98c24521adc2f245537cb3363d088a9a6524e3438`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7-centos`

```console
$ docker pull percona@sha256:657730edcb3c268b37360d9e3ecb7e776a83ebb9a6027688fb68e4b45ef40ffe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7-centos` - linux; amd64

```console
$ docker pull percona@sha256:1de5f84148c22bf55ebb47d6507eed0c072e45a694d7841ed359773236b2bb01
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193935403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9525064c8e2527931e33be2c6ba6868aa28f948ad2cd91d7317ab5938f144cd`
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
# Thu, 30 Jan 2020 23:34:20 GMT
ENV PERCONA_VERSION=5.7.28-31.1.el7
# Thu, 30 Jan 2020 23:35:15 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:35:15 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 30 Jan 2020 23:35:16 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:35:16 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:35:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:35:16 GMT
USER mysql
# Thu, 30 Jan 2020 23:35:16 GMT
EXPOSE 3306
# Thu, 30 Jan 2020 23:35:17 GMT
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
	-	`sha256:2c4e76436340f27cb846339ac414b3ddc6aafab23726bf117e40d2b17988ff8b`  
		Last Modified: Thu, 30 Jan 2020 23:37:49 GMT  
		Size: 111.7 MB (111710030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf05bcd6eb9056238d6239f3d374cdbf4319a58b35949b8e4be17c4bfbc405a`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe05bc0d56e90717f9fd0de98c24521adc2f245537cb3363d088a9a6524e3438`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5-centos`

```console
$ docker pull percona@sha256:657730edcb3c268b37360d9e3ecb7e776a83ebb9a6027688fb68e4b45ef40ffe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5-centos` - linux; amd64

```console
$ docker pull percona@sha256:1de5f84148c22bf55ebb47d6507eed0c072e45a694d7841ed359773236b2bb01
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193935403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9525064c8e2527931e33be2c6ba6868aa28f948ad2cd91d7317ab5938f144cd`
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
# Thu, 30 Jan 2020 23:34:20 GMT
ENV PERCONA_VERSION=5.7.28-31.1.el7
# Thu, 30 Jan 2020 23:35:15 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:35:15 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 30 Jan 2020 23:35:16 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:35:16 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:35:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:35:16 GMT
USER mysql
# Thu, 30 Jan 2020 23:35:16 GMT
EXPOSE 3306
# Thu, 30 Jan 2020 23:35:17 GMT
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
	-	`sha256:2c4e76436340f27cb846339ac414b3ddc6aafab23726bf117e40d2b17988ff8b`  
		Last Modified: Thu, 30 Jan 2020 23:37:49 GMT  
		Size: 111.7 MB (111710030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf05bcd6eb9056238d6239f3d374cdbf4319a58b35949b8e4be17c4bfbc405a`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe05bc0d56e90717f9fd0de98c24521adc2f245537cb3363d088a9a6524e3438`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8`

```console
$ docker pull percona@sha256:0678083552e17e751120ca35a1885321692265383a43bed9a7a695186354a1c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8` - linux; amd64

```console
$ docker pull percona@sha256:cddbde7e513e695789dc3d94d9b1ee571215930c8641c154e60dac22bf9aad81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217785444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9988e1470d5bdeaef521ccf2c3a6fc9f6fe5827bc55ff92e52c10148e0e1d9e7`
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
# Thu, 30 Jan 2020 23:33:06 GMT
ENV PERCONA_VERSION=8.0.18-9.1.el7
# Thu, 30 Jan 2020 23:33:59 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:33:59 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Jan 2020 23:34:00 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:34:00 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:34:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:34:00 GMT
USER mysql
# Thu, 30 Jan 2020 23:34:01 GMT
EXPOSE 3306 33060
# Thu, 30 Jan 2020 23:34:01 GMT
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
	-	`sha256:2931c8d2d38d06b1f32d044bc25c64beb904c15f99efa50b92994d4d13ca2dfe`  
		Last Modified: Thu, 30 Jan 2020 23:37:15 GMT  
		Size: 135.6 MB (135559806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d0980db83ca60593ce5c2e75c74d92e37749400fa42073794b407b8d51733f`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeb3deef6848372f7b69528fa4df46e15ce0af25a955e4042d32a2ba5920ad7`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0`

```console
$ docker pull percona@sha256:0678083552e17e751120ca35a1885321692265383a43bed9a7a695186354a1c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0` - linux; amd64

```console
$ docker pull percona@sha256:cddbde7e513e695789dc3d94d9b1ee571215930c8641c154e60dac22bf9aad81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217785444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9988e1470d5bdeaef521ccf2c3a6fc9f6fe5827bc55ff92e52c10148e0e1d9e7`
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
# Thu, 30 Jan 2020 23:33:06 GMT
ENV PERCONA_VERSION=8.0.18-9.1.el7
# Thu, 30 Jan 2020 23:33:59 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:33:59 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Jan 2020 23:34:00 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:34:00 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:34:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:34:00 GMT
USER mysql
# Thu, 30 Jan 2020 23:34:01 GMT
EXPOSE 3306 33060
# Thu, 30 Jan 2020 23:34:01 GMT
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
	-	`sha256:2931c8d2d38d06b1f32d044bc25c64beb904c15f99efa50b92994d4d13ca2dfe`  
		Last Modified: Thu, 30 Jan 2020 23:37:15 GMT  
		Size: 135.6 MB (135559806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d0980db83ca60593ce5c2e75c74d92e37749400fa42073794b407b8d51733f`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeb3deef6848372f7b69528fa4df46e15ce0af25a955e4042d32a2ba5920ad7`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.18-9`

```console
$ docker pull percona@sha256:0678083552e17e751120ca35a1885321692265383a43bed9a7a695186354a1c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0.18-9` - linux; amd64

```console
$ docker pull percona@sha256:cddbde7e513e695789dc3d94d9b1ee571215930c8641c154e60dac22bf9aad81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217785444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9988e1470d5bdeaef521ccf2c3a6fc9f6fe5827bc55ff92e52c10148e0e1d9e7`
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
# Thu, 30 Jan 2020 23:33:06 GMT
ENV PERCONA_VERSION=8.0.18-9.1.el7
# Thu, 30 Jan 2020 23:33:59 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:33:59 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Jan 2020 23:34:00 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:34:00 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:34:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:34:00 GMT
USER mysql
# Thu, 30 Jan 2020 23:34:01 GMT
EXPOSE 3306 33060
# Thu, 30 Jan 2020 23:34:01 GMT
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
	-	`sha256:2931c8d2d38d06b1f32d044bc25c64beb904c15f99efa50b92994d4d13ca2dfe`  
		Last Modified: Thu, 30 Jan 2020 23:37:15 GMT  
		Size: 135.6 MB (135559806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d0980db83ca60593ce5c2e75c74d92e37749400fa42073794b407b8d51733f`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeb3deef6848372f7b69528fa4df46e15ce0af25a955e4042d32a2ba5920ad7`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.18-9-centos`

```console
$ docker pull percona@sha256:0678083552e17e751120ca35a1885321692265383a43bed9a7a695186354a1c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0.18-9-centos` - linux; amd64

```console
$ docker pull percona@sha256:cddbde7e513e695789dc3d94d9b1ee571215930c8641c154e60dac22bf9aad81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217785444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9988e1470d5bdeaef521ccf2c3a6fc9f6fe5827bc55ff92e52c10148e0e1d9e7`
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
# Thu, 30 Jan 2020 23:33:06 GMT
ENV PERCONA_VERSION=8.0.18-9.1.el7
# Thu, 30 Jan 2020 23:33:59 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:33:59 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Jan 2020 23:34:00 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:34:00 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:34:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:34:00 GMT
USER mysql
# Thu, 30 Jan 2020 23:34:01 GMT
EXPOSE 3306 33060
# Thu, 30 Jan 2020 23:34:01 GMT
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
	-	`sha256:2931c8d2d38d06b1f32d044bc25c64beb904c15f99efa50b92994d4d13ca2dfe`  
		Last Modified: Thu, 30 Jan 2020 23:37:15 GMT  
		Size: 135.6 MB (135559806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d0980db83ca60593ce5c2e75c74d92e37749400fa42073794b407b8d51733f`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeb3deef6848372f7b69528fa4df46e15ce0af25a955e4042d32a2ba5920ad7`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0-centos`

```console
$ docker pull percona@sha256:0678083552e17e751120ca35a1885321692265383a43bed9a7a695186354a1c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0-centos` - linux; amd64

```console
$ docker pull percona@sha256:cddbde7e513e695789dc3d94d9b1ee571215930c8641c154e60dac22bf9aad81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217785444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9988e1470d5bdeaef521ccf2c3a6fc9f6fe5827bc55ff92e52c10148e0e1d9e7`
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
# Thu, 30 Jan 2020 23:33:06 GMT
ENV PERCONA_VERSION=8.0.18-9.1.el7
# Thu, 30 Jan 2020 23:33:59 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:33:59 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Jan 2020 23:34:00 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:34:00 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:34:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:34:00 GMT
USER mysql
# Thu, 30 Jan 2020 23:34:01 GMT
EXPOSE 3306 33060
# Thu, 30 Jan 2020 23:34:01 GMT
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
	-	`sha256:2931c8d2d38d06b1f32d044bc25c64beb904c15f99efa50b92994d4d13ca2dfe`  
		Last Modified: Thu, 30 Jan 2020 23:37:15 GMT  
		Size: 135.6 MB (135559806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d0980db83ca60593ce5c2e75c74d92e37749400fa42073794b407b8d51733f`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeb3deef6848372f7b69528fa4df46e15ce0af25a955e4042d32a2ba5920ad7`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8-centos`

```console
$ docker pull percona@sha256:0678083552e17e751120ca35a1885321692265383a43bed9a7a695186354a1c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8-centos` - linux; amd64

```console
$ docker pull percona@sha256:cddbde7e513e695789dc3d94d9b1ee571215930c8641c154e60dac22bf9aad81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217785444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9988e1470d5bdeaef521ccf2c3a6fc9f6fe5827bc55ff92e52c10148e0e1d9e7`
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
# Thu, 30 Jan 2020 23:33:06 GMT
ENV PERCONA_VERSION=8.0.18-9.1.el7
# Thu, 30 Jan 2020 23:33:59 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:33:59 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Jan 2020 23:34:00 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:34:00 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:34:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:34:00 GMT
USER mysql
# Thu, 30 Jan 2020 23:34:01 GMT
EXPOSE 3306 33060
# Thu, 30 Jan 2020 23:34:01 GMT
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
	-	`sha256:2931c8d2d38d06b1f32d044bc25c64beb904c15f99efa50b92994d4d13ca2dfe`  
		Last Modified: Thu, 30 Jan 2020 23:37:15 GMT  
		Size: 135.6 MB (135559806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d0980db83ca60593ce5c2e75c74d92e37749400fa42073794b407b8d51733f`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeb3deef6848372f7b69528fa4df46e15ce0af25a955e4042d32a2ba5920ad7`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:centos`

```console
$ docker pull percona@sha256:657730edcb3c268b37360d9e3ecb7e776a83ebb9a6027688fb68e4b45ef40ffe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:centos` - linux; amd64

```console
$ docker pull percona@sha256:1de5f84148c22bf55ebb47d6507eed0c072e45a694d7841ed359773236b2bb01
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193935403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9525064c8e2527931e33be2c6ba6868aa28f948ad2cd91d7317ab5938f144cd`
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
# Thu, 30 Jan 2020 23:34:20 GMT
ENV PERCONA_VERSION=5.7.28-31.1.el7
# Thu, 30 Jan 2020 23:35:15 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:35:15 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 30 Jan 2020 23:35:16 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:35:16 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:35:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:35:16 GMT
USER mysql
# Thu, 30 Jan 2020 23:35:16 GMT
EXPOSE 3306
# Thu, 30 Jan 2020 23:35:17 GMT
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
	-	`sha256:2c4e76436340f27cb846339ac414b3ddc6aafab23726bf117e40d2b17988ff8b`  
		Last Modified: Thu, 30 Jan 2020 23:37:49 GMT  
		Size: 111.7 MB (111710030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf05bcd6eb9056238d6239f3d374cdbf4319a58b35949b8e4be17c4bfbc405a`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe05bc0d56e90717f9fd0de98c24521adc2f245537cb3363d088a9a6524e3438`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:latest`

```console
$ docker pull percona@sha256:657730edcb3c268b37360d9e3ecb7e776a83ebb9a6027688fb68e4b45ef40ffe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:latest` - linux; amd64

```console
$ docker pull percona@sha256:1de5f84148c22bf55ebb47d6507eed0c072e45a694d7841ed359773236b2bb01
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193935403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9525064c8e2527931e33be2c6ba6868aa28f948ad2cd91d7317ab5938f144cd`
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
# Thu, 30 Jan 2020 23:34:20 GMT
ENV PERCONA_VERSION=5.7.28-31.1.el7
# Thu, 30 Jan 2020 23:35:15 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:35:15 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 30 Jan 2020 23:35:16 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:35:16 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:35:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:35:16 GMT
USER mysql
# Thu, 30 Jan 2020 23:35:16 GMT
EXPOSE 3306
# Thu, 30 Jan 2020 23:35:17 GMT
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
	-	`sha256:2c4e76436340f27cb846339ac414b3ddc6aafab23726bf117e40d2b17988ff8b`  
		Last Modified: Thu, 30 Jan 2020 23:37:49 GMT  
		Size: 111.7 MB (111710030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf05bcd6eb9056238d6239f3d374cdbf4319a58b35949b8e4be17c4bfbc405a`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe05bc0d56e90717f9fd0de98c24521adc2f245537cb3363d088a9a6524e3438`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5`

```console
$ docker pull percona@sha256:657730edcb3c268b37360d9e3ecb7e776a83ebb9a6027688fb68e4b45ef40ffe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5` - linux; amd64

```console
$ docker pull percona@sha256:1de5f84148c22bf55ebb47d6507eed0c072e45a694d7841ed359773236b2bb01
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193935403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9525064c8e2527931e33be2c6ba6868aa28f948ad2cd91d7317ab5938f144cd`
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
# Thu, 30 Jan 2020 23:34:20 GMT
ENV PERCONA_VERSION=5.7.28-31.1.el7
# Thu, 30 Jan 2020 23:35:15 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:35:15 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 30 Jan 2020 23:35:16 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:35:16 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:35:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:35:16 GMT
USER mysql
# Thu, 30 Jan 2020 23:35:16 GMT
EXPOSE 3306
# Thu, 30 Jan 2020 23:35:17 GMT
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
	-	`sha256:2c4e76436340f27cb846339ac414b3ddc6aafab23726bf117e40d2b17988ff8b`  
		Last Modified: Thu, 30 Jan 2020 23:37:49 GMT  
		Size: 111.7 MB (111710030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf05bcd6eb9056238d6239f3d374cdbf4319a58b35949b8e4be17c4bfbc405a`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe05bc0d56e90717f9fd0de98c24521adc2f245537cb3363d088a9a6524e3438`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
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
$ docker pull percona@sha256:657730edcb3c268b37360d9e3ecb7e776a83ebb9a6027688fb68e4b45ef40ffe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.7` - linux; amd64

```console
$ docker pull percona@sha256:1de5f84148c22bf55ebb47d6507eed0c072e45a694d7841ed359773236b2bb01
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193935403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9525064c8e2527931e33be2c6ba6868aa28f948ad2cd91d7317ab5938f144cd`
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
# Thu, 30 Jan 2020 23:34:20 GMT
ENV PERCONA_VERSION=5.7.28-31.1.el7
# Thu, 30 Jan 2020 23:35:15 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:35:15 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 30 Jan 2020 23:35:16 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:35:16 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:35:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:35:16 GMT
USER mysql
# Thu, 30 Jan 2020 23:35:16 GMT
EXPOSE 3306
# Thu, 30 Jan 2020 23:35:17 GMT
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
	-	`sha256:2c4e76436340f27cb846339ac414b3ddc6aafab23726bf117e40d2b17988ff8b`  
		Last Modified: Thu, 30 Jan 2020 23:37:49 GMT  
		Size: 111.7 MB (111710030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf05bcd6eb9056238d6239f3d374cdbf4319a58b35949b8e4be17c4bfbc405a`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe05bc0d56e90717f9fd0de98c24521adc2f245537cb3363d088a9a6524e3438`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.7.28`

```console
$ docker pull percona@sha256:657730edcb3c268b37360d9e3ecb7e776a83ebb9a6027688fb68e4b45ef40ffe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.7.28` - linux; amd64

```console
$ docker pull percona@sha256:1de5f84148c22bf55ebb47d6507eed0c072e45a694d7841ed359773236b2bb01
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193935403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9525064c8e2527931e33be2c6ba6868aa28f948ad2cd91d7317ab5938f144cd`
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
# Thu, 30 Jan 2020 23:34:20 GMT
ENV PERCONA_VERSION=5.7.28-31.1.el7
# Thu, 30 Jan 2020 23:35:15 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:35:15 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 30 Jan 2020 23:35:16 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:35:16 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:35:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:35:16 GMT
USER mysql
# Thu, 30 Jan 2020 23:35:16 GMT
EXPOSE 3306
# Thu, 30 Jan 2020 23:35:17 GMT
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
	-	`sha256:2c4e76436340f27cb846339ac414b3ddc6aafab23726bf117e40d2b17988ff8b`  
		Last Modified: Thu, 30 Jan 2020 23:37:49 GMT  
		Size: 111.7 MB (111710030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf05bcd6eb9056238d6239f3d374cdbf4319a58b35949b8e4be17c4bfbc405a`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe05bc0d56e90717f9fd0de98c24521adc2f245537cb3363d088a9a6524e3438`  
		Last Modified: Thu, 30 Jan 2020 23:37:23 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8`

```console
$ docker pull percona@sha256:0678083552e17e751120ca35a1885321692265383a43bed9a7a695186354a1c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8` - linux; amd64

```console
$ docker pull percona@sha256:cddbde7e513e695789dc3d94d9b1ee571215930c8641c154e60dac22bf9aad81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217785444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9988e1470d5bdeaef521ccf2c3a6fc9f6fe5827bc55ff92e52c10148e0e1d9e7`
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
# Thu, 30 Jan 2020 23:33:06 GMT
ENV PERCONA_VERSION=8.0.18-9.1.el7
# Thu, 30 Jan 2020 23:33:59 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:33:59 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Jan 2020 23:34:00 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:34:00 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:34:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:34:00 GMT
USER mysql
# Thu, 30 Jan 2020 23:34:01 GMT
EXPOSE 3306 33060
# Thu, 30 Jan 2020 23:34:01 GMT
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
	-	`sha256:2931c8d2d38d06b1f32d044bc25c64beb904c15f99efa50b92994d4d13ca2dfe`  
		Last Modified: Thu, 30 Jan 2020 23:37:15 GMT  
		Size: 135.6 MB (135559806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d0980db83ca60593ce5c2e75c74d92e37749400fa42073794b407b8d51733f`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeb3deef6848372f7b69528fa4df46e15ce0af25a955e4042d32a2ba5920ad7`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0`

```console
$ docker pull percona@sha256:0678083552e17e751120ca35a1885321692265383a43bed9a7a695186354a1c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8.0` - linux; amd64

```console
$ docker pull percona@sha256:cddbde7e513e695789dc3d94d9b1ee571215930c8641c154e60dac22bf9aad81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217785444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9988e1470d5bdeaef521ccf2c3a6fc9f6fe5827bc55ff92e52c10148e0e1d9e7`
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
# Thu, 30 Jan 2020 23:33:06 GMT
ENV PERCONA_VERSION=8.0.18-9.1.el7
# Thu, 30 Jan 2020 23:33:59 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:33:59 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Jan 2020 23:34:00 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:34:00 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:34:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:34:00 GMT
USER mysql
# Thu, 30 Jan 2020 23:34:01 GMT
EXPOSE 3306 33060
# Thu, 30 Jan 2020 23:34:01 GMT
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
	-	`sha256:2931c8d2d38d06b1f32d044bc25c64beb904c15f99efa50b92994d4d13ca2dfe`  
		Last Modified: Thu, 30 Jan 2020 23:37:15 GMT  
		Size: 135.6 MB (135559806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d0980db83ca60593ce5c2e75c74d92e37749400fa42073794b407b8d51733f`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeb3deef6848372f7b69528fa4df46e15ce0af25a955e4042d32a2ba5920ad7`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0.18-9`

```console
$ docker pull percona@sha256:0678083552e17e751120ca35a1885321692265383a43bed9a7a695186354a1c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8.0.18-9` - linux; amd64

```console
$ docker pull percona@sha256:cddbde7e513e695789dc3d94d9b1ee571215930c8641c154e60dac22bf9aad81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217785444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9988e1470d5bdeaef521ccf2c3a6fc9f6fe5827bc55ff92e52c10148e0e1d9e7`
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
# Thu, 30 Jan 2020 23:33:06 GMT
ENV PERCONA_VERSION=8.0.18-9.1.el7
# Thu, 30 Jan 2020 23:33:59 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Thu, 30 Jan 2020 23:33:59 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Jan 2020 23:34:00 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Jan 2020 23:34:00 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:34:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:34:00 GMT
USER mysql
# Thu, 30 Jan 2020 23:34:01 GMT
EXPOSE 3306 33060
# Thu, 30 Jan 2020 23:34:01 GMT
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
	-	`sha256:2931c8d2d38d06b1f32d044bc25c64beb904c15f99efa50b92994d4d13ca2dfe`  
		Last Modified: Thu, 30 Jan 2020 23:37:15 GMT  
		Size: 135.6 MB (135559806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d0980db83ca60593ce5c2e75c74d92e37749400fa42073794b407b8d51733f`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeb3deef6848372f7b69528fa4df46e15ce0af25a955e4042d32a2ba5920ad7`  
		Last Modified: Thu, 30 Jan 2020 23:36:40 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-3.6`

```console
$ docker pull percona@sha256:3b45ebe07a6e764f96b0cff8c2568a55512a68ae3d46cdc7e284d890aedf5c1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6` - linux; amd64

```console
$ docker pull percona@sha256:f840867a97e0a8f6c239faae8f9ee505f81eac4ce023e9b777a9b351deff60b4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.2 MB (156237561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c13f4a85937ed8fc5d1cf8ca167808ebf58987b27f278ec366517892eda1b05`
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
# Wed, 29 Jan 2020 19:38:27 GMT
ENV PSMDB_VERSION=3.6.16-3.6
# Wed, 29 Jan 2020 19:38:27 GMT
LABEL org.label-schema.schema-version=3.6.16-3.6
# Wed, 29 Jan 2020 19:38:27 GMT
LABEL org.opencontainers.image.version=3.6.16-3.6
# Wed, 29 Jan 2020 19:38:31 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 29 Jan 2020 19:38:31 GMT
ENV OS_VER=el7
# Wed, 29 Jan 2020 19:38:31 GMT
ENV FULL_PERCONA_VERSION=3.6.16-3.6.el7
# Wed, 29 Jan 2020 19:38:32 GMT
ENV K8S_TOOLS_VERSION=0.4.2
# Wed, 29 Jan 2020 19:38:37 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Wed, 29 Jan 2020 19:39:33 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         yum-utils         shadow-utils         curl         procps-ng         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         yum clean all;         rm -rf /var/cache/yum /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Wed, 29 Jan 2020 19:39:34 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 29 Jan 2020 19:39:34 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 29 Jan 2020 19:39:35 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 29 Jan 2020 19:39:38 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 29 Jan 2020 19:39:38 GMT
VOLUME [/data/db]
# Wed, 29 Jan 2020 19:39:38 GMT
COPY file:85995e73e1e4d284ba65fabe65ed1e96fcb9c00ac0d328edb8b0b48749d784e1 in /entrypoint.sh 
# Wed, 29 Jan 2020 19:39:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jan 2020 19:39:39 GMT
EXPOSE 27017
# Wed, 29 Jan 2020 19:39:39 GMT
USER 1001
# Wed, 29 Jan 2020 19:39:39 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fbe7d180ed89de6f48845a8efec93f14b170ee9de1c4843fe0a55e6c22947c`  
		Last Modified: Wed, 29 Jan 2020 19:40:34 GMT  
		Size: 6.4 MB (6373087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03f2b091cecd7b21c74ef437e20f83829ed002f85676ac67ad5cde9db056e17`  
		Last Modified: Wed, 29 Jan 2020 19:40:34 GMT  
		Size: 6.7 MB (6701948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f885049d322d8f846ce683718c61bcbeedbb1d7efb3520f8be6dbe3fb4fe74`  
		Last Modified: Wed, 29 Jan 2020 19:40:45 GMT  
		Size: 59.8 MB (59796187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0d5065db278bfcd88761044e018119b4188aa3c9b581ccab40a454f423ebff`  
		Last Modified: Wed, 29 Jan 2020 19:40:29 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd4b8352524372d9e80ed51147ba64189619c7b93334d73daf3207e6b626543`  
		Last Modified: Wed, 29 Jan 2020 19:40:29 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f364e83bd306717868204518f83ac9930f43778a9048fe6def86bb41c4532b41`  
		Last Modified: Wed, 29 Jan 2020 19:40:29 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c090b71c27de9ac8659f24929c6ef467459fbfcb5547024c5cf15d8749c4dd`  
		Last Modified: Wed, 29 Jan 2020 19:40:33 GMT  
		Size: 7.6 MB (7565360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809ab9a5e9e8bd1cc9a33fd286587c272d68e5667ce1764c301cd55d6e91caa1`  
		Last Modified: Wed, 29 Jan 2020 19:40:29 GMT  
		Size: 4.0 KB (4017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-3.6.16`

```console
$ docker pull percona@sha256:3b45ebe07a6e764f96b0cff8c2568a55512a68ae3d46cdc7e284d890aedf5c1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6.16` - linux; amd64

```console
$ docker pull percona@sha256:f840867a97e0a8f6c239faae8f9ee505f81eac4ce023e9b777a9b351deff60b4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.2 MB (156237561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c13f4a85937ed8fc5d1cf8ca167808ebf58987b27f278ec366517892eda1b05`
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
# Wed, 29 Jan 2020 19:38:27 GMT
ENV PSMDB_VERSION=3.6.16-3.6
# Wed, 29 Jan 2020 19:38:27 GMT
LABEL org.label-schema.schema-version=3.6.16-3.6
# Wed, 29 Jan 2020 19:38:27 GMT
LABEL org.opencontainers.image.version=3.6.16-3.6
# Wed, 29 Jan 2020 19:38:31 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 29 Jan 2020 19:38:31 GMT
ENV OS_VER=el7
# Wed, 29 Jan 2020 19:38:31 GMT
ENV FULL_PERCONA_VERSION=3.6.16-3.6.el7
# Wed, 29 Jan 2020 19:38:32 GMT
ENV K8S_TOOLS_VERSION=0.4.2
# Wed, 29 Jan 2020 19:38:37 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Wed, 29 Jan 2020 19:39:33 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         yum-utils         shadow-utils         curl         procps-ng         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         yum clean all;         rm -rf /var/cache/yum /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Wed, 29 Jan 2020 19:39:34 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 29 Jan 2020 19:39:34 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 29 Jan 2020 19:39:35 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 29 Jan 2020 19:39:38 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 29 Jan 2020 19:39:38 GMT
VOLUME [/data/db]
# Wed, 29 Jan 2020 19:39:38 GMT
COPY file:85995e73e1e4d284ba65fabe65ed1e96fcb9c00ac0d328edb8b0b48749d784e1 in /entrypoint.sh 
# Wed, 29 Jan 2020 19:39:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jan 2020 19:39:39 GMT
EXPOSE 27017
# Wed, 29 Jan 2020 19:39:39 GMT
USER 1001
# Wed, 29 Jan 2020 19:39:39 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fbe7d180ed89de6f48845a8efec93f14b170ee9de1c4843fe0a55e6c22947c`  
		Last Modified: Wed, 29 Jan 2020 19:40:34 GMT  
		Size: 6.4 MB (6373087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03f2b091cecd7b21c74ef437e20f83829ed002f85676ac67ad5cde9db056e17`  
		Last Modified: Wed, 29 Jan 2020 19:40:34 GMT  
		Size: 6.7 MB (6701948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f885049d322d8f846ce683718c61bcbeedbb1d7efb3520f8be6dbe3fb4fe74`  
		Last Modified: Wed, 29 Jan 2020 19:40:45 GMT  
		Size: 59.8 MB (59796187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0d5065db278bfcd88761044e018119b4188aa3c9b581ccab40a454f423ebff`  
		Last Modified: Wed, 29 Jan 2020 19:40:29 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd4b8352524372d9e80ed51147ba64189619c7b93334d73daf3207e6b626543`  
		Last Modified: Wed, 29 Jan 2020 19:40:29 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f364e83bd306717868204518f83ac9930f43778a9048fe6def86bb41c4532b41`  
		Last Modified: Wed, 29 Jan 2020 19:40:29 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c090b71c27de9ac8659f24929c6ef467459fbfcb5547024c5cf15d8749c4dd`  
		Last Modified: Wed, 29 Jan 2020 19:40:33 GMT  
		Size: 7.6 MB (7565360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809ab9a5e9e8bd1cc9a33fd286587c272d68e5667ce1764c301cd55d6e91caa1`  
		Last Modified: Wed, 29 Jan 2020 19:40:29 GMT  
		Size: 4.0 KB (4017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.0`

```console
$ docker pull percona@sha256:079ce316f3f2d4b71c53b4f5318c6d68c4f193297f6d2af0c7c24393ae79000a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0` - linux; amd64

```console
$ docker pull percona@sha256:7894e16d2c35804adeaa889e23f39c8c3beda8812bbaa20c6cefa70f901b35d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (158962129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dad05fffb9bc15ab6fa0b1d52645ff6b5f90b025fbd7e1dec243dea12382e38`
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
# Wed, 29 Jan 2020 19:37:35 GMT
ENV PSMDB_VERSION=4.0.14-8
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.label-schema.schema-version=4.0.14-8
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.version=4.0.14-8
# Wed, 29 Jan 2020 19:37:40 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-40 release
# Wed, 29 Jan 2020 19:37:40 GMT
ENV OS_VER=el7
# Wed, 29 Jan 2020 19:37:40 GMT
ENV FULL_PERCONA_VERSION=4.0.14-8.el7
# Wed, 29 Jan 2020 19:37:41 GMT
ENV K8S_TOOLS_VERSION=0.4.2
# Wed, 29 Jan 2020 19:37:46 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Wed, 29 Jan 2020 19:38:10 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 29 Jan 2020 19:38:11 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 29 Jan 2020 19:38:11 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 29 Jan 2020 19:38:12 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 29 Jan 2020 19:38:12 GMT
ENV GOSU_VERSION=1.11
# Wed, 29 Jan 2020 19:38:15 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 29 Jan 2020 19:38:17 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 29 Jan 2020 19:38:17 GMT
VOLUME [/data/db]
# Wed, 29 Jan 2020 19:38:18 GMT
COPY file:85995e73e1e4d284ba65fabe65ed1e96fcb9c00ac0d328edb8b0b48749d784e1 in /entrypoint.sh 
# Wed, 29 Jan 2020 19:38:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jan 2020 19:38:18 GMT
EXPOSE 27017
# Wed, 29 Jan 2020 19:38:18 GMT
USER 1001
# Wed, 29 Jan 2020 19:38:18 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e0ce77bf6153fbd690fb03eb3d42b9008411f9b97ed8a22154ef61d28d080a`  
		Last Modified: Wed, 29 Jan 2020 19:40:14 GMT  
		Size: 6.4 MB (6371262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a64cfd09ed5cff1b25acf8bd50ec6ac54b3fe2923885d8b17ae1613ba1088d`  
		Last Modified: Wed, 29 Jan 2020 19:40:14 GMT  
		Size: 6.7 MB (6693993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fafc1f651a2a537b76012523ec0737016d6e7a782a4d60786c0712d9ce354bce`  
		Last Modified: Wed, 29 Jan 2020 19:40:25 GMT  
		Size: 61.6 MB (61615064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b071a9fc3a03521f5e70f60e5df9db3e78ec9272536000918b88445e644d903`  
		Last Modified: Wed, 29 Jan 2020 19:40:11 GMT  
		Size: 1.6 KB (1591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df472d658ba7d39a94826ca133f38bf0207f70c9ea2336ff6cb1ef6d92cbf92b`  
		Last Modified: Wed, 29 Jan 2020 19:40:10 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29e055ad0d1fb34b76891468a719cf6dd405b1a285318aed9772a3a2ef14411`  
		Last Modified: Wed, 29 Jan 2020 19:40:09 GMT  
		Size: 10.6 KB (10577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88767c48922b736c64e5fcdbf6f257b4aee0003d9d12d7d23be12cba18d7f524`  
		Last Modified: Wed, 29 Jan 2020 19:40:10 GMT  
		Size: 915.5 KB (915468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5666d291ae7585a1cac26a076e091582c3685ceafa04085d4863cb1b7c23feb`  
		Last Modified: Wed, 29 Jan 2020 19:40:12 GMT  
		Size: 7.6 MB (7565373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d76452c8dcfa27e0eeee766d647a78a2384081b4528837c95a797b032ae0b`  
		Last Modified: Wed, 29 Jan 2020 19:40:09 GMT  
		Size: 4.0 KB (4014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.0.14`

```console
$ docker pull percona@sha256:079ce316f3f2d4b71c53b4f5318c6d68c4f193297f6d2af0c7c24393ae79000a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0.14` - linux; amd64

```console
$ docker pull percona@sha256:7894e16d2c35804adeaa889e23f39c8c3beda8812bbaa20c6cefa70f901b35d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (158962129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dad05fffb9bc15ab6fa0b1d52645ff6b5f90b025fbd7e1dec243dea12382e38`
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
# Wed, 29 Jan 2020 19:37:35 GMT
ENV PSMDB_VERSION=4.0.14-8
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.label-schema.schema-version=4.0.14-8
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.version=4.0.14-8
# Wed, 29 Jan 2020 19:37:40 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-40 release
# Wed, 29 Jan 2020 19:37:40 GMT
ENV OS_VER=el7
# Wed, 29 Jan 2020 19:37:40 GMT
ENV FULL_PERCONA_VERSION=4.0.14-8.el7
# Wed, 29 Jan 2020 19:37:41 GMT
ENV K8S_TOOLS_VERSION=0.4.2
# Wed, 29 Jan 2020 19:37:46 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Wed, 29 Jan 2020 19:38:10 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 29 Jan 2020 19:38:11 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 29 Jan 2020 19:38:11 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 29 Jan 2020 19:38:12 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 29 Jan 2020 19:38:12 GMT
ENV GOSU_VERSION=1.11
# Wed, 29 Jan 2020 19:38:15 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 29 Jan 2020 19:38:17 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 29 Jan 2020 19:38:17 GMT
VOLUME [/data/db]
# Wed, 29 Jan 2020 19:38:18 GMT
COPY file:85995e73e1e4d284ba65fabe65ed1e96fcb9c00ac0d328edb8b0b48749d784e1 in /entrypoint.sh 
# Wed, 29 Jan 2020 19:38:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jan 2020 19:38:18 GMT
EXPOSE 27017
# Wed, 29 Jan 2020 19:38:18 GMT
USER 1001
# Wed, 29 Jan 2020 19:38:18 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e0ce77bf6153fbd690fb03eb3d42b9008411f9b97ed8a22154ef61d28d080a`  
		Last Modified: Wed, 29 Jan 2020 19:40:14 GMT  
		Size: 6.4 MB (6371262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a64cfd09ed5cff1b25acf8bd50ec6ac54b3fe2923885d8b17ae1613ba1088d`  
		Last Modified: Wed, 29 Jan 2020 19:40:14 GMT  
		Size: 6.7 MB (6693993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fafc1f651a2a537b76012523ec0737016d6e7a782a4d60786c0712d9ce354bce`  
		Last Modified: Wed, 29 Jan 2020 19:40:25 GMT  
		Size: 61.6 MB (61615064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b071a9fc3a03521f5e70f60e5df9db3e78ec9272536000918b88445e644d903`  
		Last Modified: Wed, 29 Jan 2020 19:40:11 GMT  
		Size: 1.6 KB (1591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df472d658ba7d39a94826ca133f38bf0207f70c9ea2336ff6cb1ef6d92cbf92b`  
		Last Modified: Wed, 29 Jan 2020 19:40:10 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29e055ad0d1fb34b76891468a719cf6dd405b1a285318aed9772a3a2ef14411`  
		Last Modified: Wed, 29 Jan 2020 19:40:09 GMT  
		Size: 10.6 KB (10577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88767c48922b736c64e5fcdbf6f257b4aee0003d9d12d7d23be12cba18d7f524`  
		Last Modified: Wed, 29 Jan 2020 19:40:10 GMT  
		Size: 915.5 KB (915468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5666d291ae7585a1cac26a076e091582c3685ceafa04085d4863cb1b7c23feb`  
		Last Modified: Wed, 29 Jan 2020 19:40:12 GMT  
		Size: 7.6 MB (7565373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d76452c8dcfa27e0eeee766d647a78a2384081b4528837c95a797b032ae0b`  
		Last Modified: Wed, 29 Jan 2020 19:40:09 GMT  
		Size: 4.0 KB (4014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:5a671b03f9e7850e27fd9dacfe34cc50a0c5077c307f5a02c6ab0654f19a163a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:db2918bd5c4ada1bf975ac0ddd388c3a67675cd1391da943d3d6c4f724498b0f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168165379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b57096b2e53057e4399fe03706551a1fec26da302c752a80c854c344c49538c2`
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
# Fri, 31 Jan 2020 17:34:32 GMT
ENV PSMDB_VERSION=4.2.2-3
# Fri, 31 Jan 2020 17:34:32 GMT
LABEL org.label-schema.schema-version=4.2.2-3
# Fri, 31 Jan 2020 17:34:33 GMT
LABEL org.opencontainers.image.version=4.2.2-3
# Fri, 31 Jan 2020 17:34:37 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Fri, 31 Jan 2020 17:34:37 GMT
ENV OS_VER=el7
# Fri, 31 Jan 2020 17:34:37 GMT
ENV FULL_PERCONA_VERSION=4.2.2-3.el7
# Fri, 31 Jan 2020 17:34:38 GMT
ENV K8S_TOOLS_VERSION=0.4.2
# Fri, 31 Jan 2020 17:34:43 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Fri, 31 Jan 2020 17:35:08 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Fri, 31 Jan 2020 17:35:09 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Fri, 31 Jan 2020 17:35:09 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Fri, 31 Jan 2020 17:35:10 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Fri, 31 Jan 2020 17:35:10 GMT
ENV GOSU_VERSION=1.11
# Fri, 31 Jan 2020 17:35:13 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Fri, 31 Jan 2020 17:35:15 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Fri, 31 Jan 2020 17:35:16 GMT
VOLUME [/data/db]
# Fri, 31 Jan 2020 17:35:16 GMT
COPY file:d143ecb7a542d31ae4c95807064d8fad35f488059238d10fcd8b10f214d58331 in /entrypoint.sh 
# Fri, 31 Jan 2020 17:35:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 31 Jan 2020 17:35:16 GMT
EXPOSE 27017
# Fri, 31 Jan 2020 17:35:16 GMT
USER 1001
# Fri, 31 Jan 2020 17:35:17 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5bbd523abf2b326480ee5b2881545334404f8a97969b12df90a2cf04b6cd5c`  
		Last Modified: Fri, 31 Jan 2020 17:35:57 GMT  
		Size: 6.4 MB (6369761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a88959c6abc98af902a3befe62e40f8a71ba1895ec5f602b38465f2cc5d279`  
		Last Modified: Fri, 31 Jan 2020 17:35:57 GMT  
		Size: 6.7 MB (6701058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f049af6cdf020f931a6e4f5c01f9397bee8d83c47e1c12938e446ac239c8aa6`  
		Last Modified: Fri, 31 Jan 2020 17:36:08 GMT  
		Size: 70.8 MB (70812325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45638dc4485c5c2db3d9c2fd2b3887c6d72eedcef12406a03cfb7f24cfeed7eb`  
		Last Modified: Fri, 31 Jan 2020 17:35:55 GMT  
		Size: 1.6 KB (1592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfc182c99b9c2c67e0fb90be2637a749d7b81e015497e3211e0613cb809e65c`  
		Last Modified: Fri, 31 Jan 2020 17:35:54 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b146bb19c1ce27b5d842b0f7fc27018598e10f6ea433c785660bf4aba05c9f`  
		Last Modified: Fri, 31 Jan 2020 17:35:54 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf3acef48d9a80b1ea6109a1ea6b77af7dcb8e97cbd1e15d8ca005af7766fc6`  
		Last Modified: Fri, 31 Jan 2020 17:35:54 GMT  
		Size: 915.5 KB (915465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63741e185a978679663e21eca1d914601b1fb31d05a2994eb7efaa628eedd5fd`  
		Last Modified: Fri, 31 Jan 2020 17:35:56 GMT  
		Size: 7.6 MB (7565376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839b3539c40a7ef73e1b0edf8460bbcad00bb0ec8fd728f2bb9161338a0a4452`  
		Last Modified: Fri, 31 Jan 2020 17:35:54 GMT  
		Size: 4.4 KB (4437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2.2`

```console
$ docker pull percona@sha256:5a671b03f9e7850e27fd9dacfe34cc50a0c5077c307f5a02c6ab0654f19a163a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.2.2` - linux; amd64

```console
$ docker pull percona@sha256:db2918bd5c4ada1bf975ac0ddd388c3a67675cd1391da943d3d6c4f724498b0f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168165379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b57096b2e53057e4399fe03706551a1fec26da302c752a80c854c344c49538c2`
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
# Fri, 31 Jan 2020 17:34:32 GMT
ENV PSMDB_VERSION=4.2.2-3
# Fri, 31 Jan 2020 17:34:32 GMT
LABEL org.label-schema.schema-version=4.2.2-3
# Fri, 31 Jan 2020 17:34:33 GMT
LABEL org.opencontainers.image.version=4.2.2-3
# Fri, 31 Jan 2020 17:34:37 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Fri, 31 Jan 2020 17:34:37 GMT
ENV OS_VER=el7
# Fri, 31 Jan 2020 17:34:37 GMT
ENV FULL_PERCONA_VERSION=4.2.2-3.el7
# Fri, 31 Jan 2020 17:34:38 GMT
ENV K8S_TOOLS_VERSION=0.4.2
# Fri, 31 Jan 2020 17:34:43 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Fri, 31 Jan 2020 17:35:08 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Fri, 31 Jan 2020 17:35:09 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Fri, 31 Jan 2020 17:35:09 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Fri, 31 Jan 2020 17:35:10 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Fri, 31 Jan 2020 17:35:10 GMT
ENV GOSU_VERSION=1.11
# Fri, 31 Jan 2020 17:35:13 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Fri, 31 Jan 2020 17:35:15 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Fri, 31 Jan 2020 17:35:16 GMT
VOLUME [/data/db]
# Fri, 31 Jan 2020 17:35:16 GMT
COPY file:d143ecb7a542d31ae4c95807064d8fad35f488059238d10fcd8b10f214d58331 in /entrypoint.sh 
# Fri, 31 Jan 2020 17:35:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 31 Jan 2020 17:35:16 GMT
EXPOSE 27017
# Fri, 31 Jan 2020 17:35:16 GMT
USER 1001
# Fri, 31 Jan 2020 17:35:17 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5bbd523abf2b326480ee5b2881545334404f8a97969b12df90a2cf04b6cd5c`  
		Last Modified: Fri, 31 Jan 2020 17:35:57 GMT  
		Size: 6.4 MB (6369761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a88959c6abc98af902a3befe62e40f8a71ba1895ec5f602b38465f2cc5d279`  
		Last Modified: Fri, 31 Jan 2020 17:35:57 GMT  
		Size: 6.7 MB (6701058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f049af6cdf020f931a6e4f5c01f9397bee8d83c47e1c12938e446ac239c8aa6`  
		Last Modified: Fri, 31 Jan 2020 17:36:08 GMT  
		Size: 70.8 MB (70812325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45638dc4485c5c2db3d9c2fd2b3887c6d72eedcef12406a03cfb7f24cfeed7eb`  
		Last Modified: Fri, 31 Jan 2020 17:35:55 GMT  
		Size: 1.6 KB (1592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfc182c99b9c2c67e0fb90be2637a749d7b81e015497e3211e0613cb809e65c`  
		Last Modified: Fri, 31 Jan 2020 17:35:54 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b146bb19c1ce27b5d842b0f7fc27018598e10f6ea433c785660bf4aba05c9f`  
		Last Modified: Fri, 31 Jan 2020 17:35:54 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf3acef48d9a80b1ea6109a1ea6b77af7dcb8e97cbd1e15d8ca005af7766fc6`  
		Last Modified: Fri, 31 Jan 2020 17:35:54 GMT  
		Size: 915.5 KB (915465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63741e185a978679663e21eca1d914601b1fb31d05a2994eb7efaa628eedd5fd`  
		Last Modified: Fri, 31 Jan 2020 17:35:56 GMT  
		Size: 7.6 MB (7565376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839b3539c40a7ef73e1b0edf8460bbcad00bb0ec8fd728f2bb9161338a0a4452`  
		Last Modified: Fri, 31 Jan 2020 17:35:54 GMT  
		Size: 4.4 KB (4437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
