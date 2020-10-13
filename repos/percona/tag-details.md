<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `percona`

-	[`percona:5`](#percona5)
-	[`percona:5.6`](#percona56)
-	[`percona:5.6.49`](#percona5649)
-	[`percona:5.6.49-centos`](#percona5649-centos)
-	[`percona:5.6-centos`](#percona56-centos)
-	[`percona:5.7`](#percona57)
-	[`percona:5.7.31`](#percona5731)
-	[`percona:5.7.31-centos`](#percona5731-centos)
-	[`percona:5.7-centos`](#percona57-centos)
-	[`percona:5-centos`](#percona5-centos)
-	[`percona:8`](#percona8)
-	[`percona:8.0`](#percona80)
-	[`percona:8.0.20-11`](#percona8020-11)
-	[`percona:8.0.20-11-centos`](#percona8020-11-centos)
-	[`percona:8.0-centos`](#percona80-centos)
-	[`percona:8-centos`](#percona8-centos)
-	[`percona:centos`](#perconacentos)
-	[`percona:latest`](#perconalatest)
-	[`percona:ps-5`](#perconaps-5)
-	[`percona:ps-5.6`](#perconaps-56)
-	[`percona:ps-5.6.49`](#perconaps-5649)
-	[`percona:ps-5.7`](#perconaps-57)
-	[`percona:ps-5.7.31`](#perconaps-5731)
-	[`percona:ps-8`](#perconaps-8)
-	[`percona:ps-8.0`](#perconaps-80)
-	[`percona:ps-8.0.20-11`](#perconaps-8020-11)
-	[`percona:psmdb-3.6`](#perconapsmdb-36)
-	[`percona:psmdb-3.6.19`](#perconapsmdb-3619)
-	[`percona:psmdb-4.0`](#perconapsmdb-40)
-	[`percona:psmdb-4.0.20`](#perconapsmdb-4020)
-	[`percona:psmdb-4.2`](#perconapsmdb-42)
-	[`percona:psmdb-4.2.9`](#perconapsmdb-429)
-	[`percona:psmdb-4.4`](#perconapsmdb-44)
-	[`percona:psmdb-4.4.1`](#perconapsmdb-441)

## `percona:5`

```console
$ docker pull percona@sha256:34c453b0c796d184df0f5049c3ff47aa3d6c6db0b344c6170b5fef5bfb615ea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5` - linux; amd64

```console
$ docker pull percona@sha256:68dad5e2efeb6893e2d7d116a1eae144f2c641c17d00e7869397395590c91651
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.0 MB (197968054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb49da8a7d3c22eb92a4de93d43ede592bb5487ac89ad866211a4f9ef8d11a3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:41:04 GMT
RUN groupdel input && groupadd -g 999 mysql
# Mon, 10 Aug 2020 18:41:05 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:41:08 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Tue, 25 Aug 2020 18:29:22 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Tue, 25 Aug 2020 18:30:16 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 25 Aug 2020 18:30:17 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 25 Aug 2020 18:30:17 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 25 Aug 2020 18:30:18 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 25 Aug 2020 18:30:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 Aug 2020 18:30:18 GMT
USER mysql
# Tue, 25 Aug 2020 18:30:18 GMT
EXPOSE 3306
# Tue, 25 Aug 2020 18:30:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14bc3f760dd091dd563d2ef48f1147f72762a2b31109b475d8dcb60d351993a`  
		Last Modified: Mon, 10 Aug 2020 18:46:17 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd29505baaec9c24f65109881fc6c0d6d097e1d3973e08df81965f3d7bbdeef`  
		Last Modified: Mon, 10 Aug 2020 18:46:15 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35af5ab9a3507b90b1780d5c5f6f67c87bf9ab542ff82c91768593541302d95d`  
		Last Modified: Mon, 10 Aug 2020 18:46:16 GMT  
		Size: 6.5 MB (6520666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c120071707bdce8a2c097ec51e0ba326faf19d324fe2344135d47a195382e7a3`  
		Last Modified: Tue, 25 Aug 2020 18:31:15 GMT  
		Size: 115.6 MB (115577656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36714b45d31e2c0d3060533bb22b194773c2314f76087bcd85c7ce01680688`  
		Last Modified: Tue, 25 Aug 2020 18:30:56 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd1024e5c88aa4f5f0ce9960f3c2c77fc1bd423cc2e240926b3d69c3bfdc58`  
		Last Modified: Tue, 25 Aug 2020 18:30:55 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6`

```console
$ docker pull percona@sha256:5c31992eec3a97d45d56430231b3bd63ab41ac42098bbb86cfbbf38cfda7ee8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.6` - linux; amd64

```console
$ docker pull percona@sha256:b205120a44c4ab52257c781178c14c1028cccae1a7b37eeb3be763663614c9c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140400649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3de140c1e4106683bdf83d5b26297e55f62e814d4e50298c55b55c05d90846a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:41:04 GMT
RUN groupdel input && groupadd -g 999 mysql
# Mon, 10 Aug 2020 18:41:05 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:42:24 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Mon, 10 Aug 2020 18:42:24 GMT
ENV PERCONA_VERSION=5.6.49-rel89.0.1.el7
# Mon, 10 Aug 2020 18:43:05 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 10 Aug 2020 18:43:06 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 10 Aug 2020 18:43:06 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 10 Aug 2020 18:43:06 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Mon, 10 Aug 2020 18:43:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:43:07 GMT
USER mysql
# Mon, 10 Aug 2020 18:43:07 GMT
EXPOSE 3306
# Mon, 10 Aug 2020 18:43:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14bc3f760dd091dd563d2ef48f1147f72762a2b31109b475d8dcb60d351993a`  
		Last Modified: Mon, 10 Aug 2020 18:46:17 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd29505baaec9c24f65109881fc6c0d6d097e1d3973e08df81965f3d7bbdeef`  
		Last Modified: Mon, 10 Aug 2020 18:46:15 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf289b643b5657c22f720bb6138c36e1e2281247fc899762743dac9417e6ec2`  
		Last Modified: Mon, 10 Aug 2020 18:46:47 GMT  
		Size: 6.5 MB (6520701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77772238b545fcdd030d3e20f9c6441c74c66147c096a061cb25064868730c5`  
		Last Modified: Mon, 10 Aug 2020 18:46:56 GMT  
		Size: 58.0 MB (58006846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360da840cd215f1383e6c585004609079a5026d68f032a1325f849491517baa4`  
		Last Modified: Mon, 10 Aug 2020 18:46:46 GMT  
		Size: 4.9 KB (4879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adc09e8de6b047ccbbb8c4524bc7c8557cb92f82d87f2331b52eee2a3a9523a`  
		Last Modified: Mon, 10 Aug 2020 18:46:46 GMT  
		Size: 2.9 KB (2941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6.49`

```console
$ docker pull percona@sha256:5c31992eec3a97d45d56430231b3bd63ab41ac42098bbb86cfbbf38cfda7ee8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.6.49` - linux; amd64

```console
$ docker pull percona@sha256:b205120a44c4ab52257c781178c14c1028cccae1a7b37eeb3be763663614c9c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140400649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3de140c1e4106683bdf83d5b26297e55f62e814d4e50298c55b55c05d90846a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:41:04 GMT
RUN groupdel input && groupadd -g 999 mysql
# Mon, 10 Aug 2020 18:41:05 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:42:24 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Mon, 10 Aug 2020 18:42:24 GMT
ENV PERCONA_VERSION=5.6.49-rel89.0.1.el7
# Mon, 10 Aug 2020 18:43:05 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 10 Aug 2020 18:43:06 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 10 Aug 2020 18:43:06 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 10 Aug 2020 18:43:06 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Mon, 10 Aug 2020 18:43:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:43:07 GMT
USER mysql
# Mon, 10 Aug 2020 18:43:07 GMT
EXPOSE 3306
# Mon, 10 Aug 2020 18:43:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14bc3f760dd091dd563d2ef48f1147f72762a2b31109b475d8dcb60d351993a`  
		Last Modified: Mon, 10 Aug 2020 18:46:17 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd29505baaec9c24f65109881fc6c0d6d097e1d3973e08df81965f3d7bbdeef`  
		Last Modified: Mon, 10 Aug 2020 18:46:15 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf289b643b5657c22f720bb6138c36e1e2281247fc899762743dac9417e6ec2`  
		Last Modified: Mon, 10 Aug 2020 18:46:47 GMT  
		Size: 6.5 MB (6520701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77772238b545fcdd030d3e20f9c6441c74c66147c096a061cb25064868730c5`  
		Last Modified: Mon, 10 Aug 2020 18:46:56 GMT  
		Size: 58.0 MB (58006846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360da840cd215f1383e6c585004609079a5026d68f032a1325f849491517baa4`  
		Last Modified: Mon, 10 Aug 2020 18:46:46 GMT  
		Size: 4.9 KB (4879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adc09e8de6b047ccbbb8c4524bc7c8557cb92f82d87f2331b52eee2a3a9523a`  
		Last Modified: Mon, 10 Aug 2020 18:46:46 GMT  
		Size: 2.9 KB (2941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6.49-centos`

```console
$ docker pull percona@sha256:5c31992eec3a97d45d56430231b3bd63ab41ac42098bbb86cfbbf38cfda7ee8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.6.49-centos` - linux; amd64

```console
$ docker pull percona@sha256:b205120a44c4ab52257c781178c14c1028cccae1a7b37eeb3be763663614c9c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140400649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3de140c1e4106683bdf83d5b26297e55f62e814d4e50298c55b55c05d90846a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:41:04 GMT
RUN groupdel input && groupadd -g 999 mysql
# Mon, 10 Aug 2020 18:41:05 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:42:24 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Mon, 10 Aug 2020 18:42:24 GMT
ENV PERCONA_VERSION=5.6.49-rel89.0.1.el7
# Mon, 10 Aug 2020 18:43:05 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 10 Aug 2020 18:43:06 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 10 Aug 2020 18:43:06 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 10 Aug 2020 18:43:06 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Mon, 10 Aug 2020 18:43:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:43:07 GMT
USER mysql
# Mon, 10 Aug 2020 18:43:07 GMT
EXPOSE 3306
# Mon, 10 Aug 2020 18:43:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14bc3f760dd091dd563d2ef48f1147f72762a2b31109b475d8dcb60d351993a`  
		Last Modified: Mon, 10 Aug 2020 18:46:17 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd29505baaec9c24f65109881fc6c0d6d097e1d3973e08df81965f3d7bbdeef`  
		Last Modified: Mon, 10 Aug 2020 18:46:15 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf289b643b5657c22f720bb6138c36e1e2281247fc899762743dac9417e6ec2`  
		Last Modified: Mon, 10 Aug 2020 18:46:47 GMT  
		Size: 6.5 MB (6520701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77772238b545fcdd030d3e20f9c6441c74c66147c096a061cb25064868730c5`  
		Last Modified: Mon, 10 Aug 2020 18:46:56 GMT  
		Size: 58.0 MB (58006846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360da840cd215f1383e6c585004609079a5026d68f032a1325f849491517baa4`  
		Last Modified: Mon, 10 Aug 2020 18:46:46 GMT  
		Size: 4.9 KB (4879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adc09e8de6b047ccbbb8c4524bc7c8557cb92f82d87f2331b52eee2a3a9523a`  
		Last Modified: Mon, 10 Aug 2020 18:46:46 GMT  
		Size: 2.9 KB (2941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.6-centos`

```console
$ docker pull percona@sha256:5c31992eec3a97d45d56430231b3bd63ab41ac42098bbb86cfbbf38cfda7ee8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.6-centos` - linux; amd64

```console
$ docker pull percona@sha256:b205120a44c4ab52257c781178c14c1028cccae1a7b37eeb3be763663614c9c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140400649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3de140c1e4106683bdf83d5b26297e55f62e814d4e50298c55b55c05d90846a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:41:04 GMT
RUN groupdel input && groupadd -g 999 mysql
# Mon, 10 Aug 2020 18:41:05 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:42:24 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Mon, 10 Aug 2020 18:42:24 GMT
ENV PERCONA_VERSION=5.6.49-rel89.0.1.el7
# Mon, 10 Aug 2020 18:43:05 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 10 Aug 2020 18:43:06 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 10 Aug 2020 18:43:06 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 10 Aug 2020 18:43:06 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Mon, 10 Aug 2020 18:43:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:43:07 GMT
USER mysql
# Mon, 10 Aug 2020 18:43:07 GMT
EXPOSE 3306
# Mon, 10 Aug 2020 18:43:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14bc3f760dd091dd563d2ef48f1147f72762a2b31109b475d8dcb60d351993a`  
		Last Modified: Mon, 10 Aug 2020 18:46:17 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd29505baaec9c24f65109881fc6c0d6d097e1d3973e08df81965f3d7bbdeef`  
		Last Modified: Mon, 10 Aug 2020 18:46:15 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf289b643b5657c22f720bb6138c36e1e2281247fc899762743dac9417e6ec2`  
		Last Modified: Mon, 10 Aug 2020 18:46:47 GMT  
		Size: 6.5 MB (6520701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77772238b545fcdd030d3e20f9c6441c74c66147c096a061cb25064868730c5`  
		Last Modified: Mon, 10 Aug 2020 18:46:56 GMT  
		Size: 58.0 MB (58006846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360da840cd215f1383e6c585004609079a5026d68f032a1325f849491517baa4`  
		Last Modified: Mon, 10 Aug 2020 18:46:46 GMT  
		Size: 4.9 KB (4879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adc09e8de6b047ccbbb8c4524bc7c8557cb92f82d87f2331b52eee2a3a9523a`  
		Last Modified: Mon, 10 Aug 2020 18:46:46 GMT  
		Size: 2.9 KB (2941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7`

```console
$ docker pull percona@sha256:34c453b0c796d184df0f5049c3ff47aa3d6c6db0b344c6170b5fef5bfb615ea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7` - linux; amd64

```console
$ docker pull percona@sha256:68dad5e2efeb6893e2d7d116a1eae144f2c641c17d00e7869397395590c91651
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.0 MB (197968054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb49da8a7d3c22eb92a4de93d43ede592bb5487ac89ad866211a4f9ef8d11a3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:41:04 GMT
RUN groupdel input && groupadd -g 999 mysql
# Mon, 10 Aug 2020 18:41:05 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:41:08 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Tue, 25 Aug 2020 18:29:22 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Tue, 25 Aug 2020 18:30:16 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 25 Aug 2020 18:30:17 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 25 Aug 2020 18:30:17 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 25 Aug 2020 18:30:18 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 25 Aug 2020 18:30:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 Aug 2020 18:30:18 GMT
USER mysql
# Tue, 25 Aug 2020 18:30:18 GMT
EXPOSE 3306
# Tue, 25 Aug 2020 18:30:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14bc3f760dd091dd563d2ef48f1147f72762a2b31109b475d8dcb60d351993a`  
		Last Modified: Mon, 10 Aug 2020 18:46:17 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd29505baaec9c24f65109881fc6c0d6d097e1d3973e08df81965f3d7bbdeef`  
		Last Modified: Mon, 10 Aug 2020 18:46:15 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35af5ab9a3507b90b1780d5c5f6f67c87bf9ab542ff82c91768593541302d95d`  
		Last Modified: Mon, 10 Aug 2020 18:46:16 GMT  
		Size: 6.5 MB (6520666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c120071707bdce8a2c097ec51e0ba326faf19d324fe2344135d47a195382e7a3`  
		Last Modified: Tue, 25 Aug 2020 18:31:15 GMT  
		Size: 115.6 MB (115577656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36714b45d31e2c0d3060533bb22b194773c2314f76087bcd85c7ce01680688`  
		Last Modified: Tue, 25 Aug 2020 18:30:56 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd1024e5c88aa4f5f0ce9960f3c2c77fc1bd423cc2e240926b3d69c3bfdc58`  
		Last Modified: Tue, 25 Aug 2020 18:30:55 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.31`

```console
$ docker pull percona@sha256:34c453b0c796d184df0f5049c3ff47aa3d6c6db0b344c6170b5fef5bfb615ea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7.31` - linux; amd64

```console
$ docker pull percona@sha256:68dad5e2efeb6893e2d7d116a1eae144f2c641c17d00e7869397395590c91651
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.0 MB (197968054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb49da8a7d3c22eb92a4de93d43ede592bb5487ac89ad866211a4f9ef8d11a3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:41:04 GMT
RUN groupdel input && groupadd -g 999 mysql
# Mon, 10 Aug 2020 18:41:05 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:41:08 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Tue, 25 Aug 2020 18:29:22 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Tue, 25 Aug 2020 18:30:16 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 25 Aug 2020 18:30:17 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 25 Aug 2020 18:30:17 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 25 Aug 2020 18:30:18 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 25 Aug 2020 18:30:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 Aug 2020 18:30:18 GMT
USER mysql
# Tue, 25 Aug 2020 18:30:18 GMT
EXPOSE 3306
# Tue, 25 Aug 2020 18:30:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14bc3f760dd091dd563d2ef48f1147f72762a2b31109b475d8dcb60d351993a`  
		Last Modified: Mon, 10 Aug 2020 18:46:17 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd29505baaec9c24f65109881fc6c0d6d097e1d3973e08df81965f3d7bbdeef`  
		Last Modified: Mon, 10 Aug 2020 18:46:15 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35af5ab9a3507b90b1780d5c5f6f67c87bf9ab542ff82c91768593541302d95d`  
		Last Modified: Mon, 10 Aug 2020 18:46:16 GMT  
		Size: 6.5 MB (6520666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c120071707bdce8a2c097ec51e0ba326faf19d324fe2344135d47a195382e7a3`  
		Last Modified: Tue, 25 Aug 2020 18:31:15 GMT  
		Size: 115.6 MB (115577656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36714b45d31e2c0d3060533bb22b194773c2314f76087bcd85c7ce01680688`  
		Last Modified: Tue, 25 Aug 2020 18:30:56 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd1024e5c88aa4f5f0ce9960f3c2c77fc1bd423cc2e240926b3d69c3bfdc58`  
		Last Modified: Tue, 25 Aug 2020 18:30:55 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.31-centos`

```console
$ docker pull percona@sha256:34c453b0c796d184df0f5049c3ff47aa3d6c6db0b344c6170b5fef5bfb615ea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7.31-centos` - linux; amd64

```console
$ docker pull percona@sha256:68dad5e2efeb6893e2d7d116a1eae144f2c641c17d00e7869397395590c91651
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.0 MB (197968054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb49da8a7d3c22eb92a4de93d43ede592bb5487ac89ad866211a4f9ef8d11a3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:41:04 GMT
RUN groupdel input && groupadd -g 999 mysql
# Mon, 10 Aug 2020 18:41:05 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:41:08 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Tue, 25 Aug 2020 18:29:22 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Tue, 25 Aug 2020 18:30:16 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 25 Aug 2020 18:30:17 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 25 Aug 2020 18:30:17 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 25 Aug 2020 18:30:18 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 25 Aug 2020 18:30:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 Aug 2020 18:30:18 GMT
USER mysql
# Tue, 25 Aug 2020 18:30:18 GMT
EXPOSE 3306
# Tue, 25 Aug 2020 18:30:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14bc3f760dd091dd563d2ef48f1147f72762a2b31109b475d8dcb60d351993a`  
		Last Modified: Mon, 10 Aug 2020 18:46:17 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd29505baaec9c24f65109881fc6c0d6d097e1d3973e08df81965f3d7bbdeef`  
		Last Modified: Mon, 10 Aug 2020 18:46:15 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35af5ab9a3507b90b1780d5c5f6f67c87bf9ab542ff82c91768593541302d95d`  
		Last Modified: Mon, 10 Aug 2020 18:46:16 GMT  
		Size: 6.5 MB (6520666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c120071707bdce8a2c097ec51e0ba326faf19d324fe2344135d47a195382e7a3`  
		Last Modified: Tue, 25 Aug 2020 18:31:15 GMT  
		Size: 115.6 MB (115577656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36714b45d31e2c0d3060533bb22b194773c2314f76087bcd85c7ce01680688`  
		Last Modified: Tue, 25 Aug 2020 18:30:56 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd1024e5c88aa4f5f0ce9960f3c2c77fc1bd423cc2e240926b3d69c3bfdc58`  
		Last Modified: Tue, 25 Aug 2020 18:30:55 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7-centos`

```console
$ docker pull percona@sha256:34c453b0c796d184df0f5049c3ff47aa3d6c6db0b344c6170b5fef5bfb615ea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7-centos` - linux; amd64

```console
$ docker pull percona@sha256:68dad5e2efeb6893e2d7d116a1eae144f2c641c17d00e7869397395590c91651
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.0 MB (197968054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb49da8a7d3c22eb92a4de93d43ede592bb5487ac89ad866211a4f9ef8d11a3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:41:04 GMT
RUN groupdel input && groupadd -g 999 mysql
# Mon, 10 Aug 2020 18:41:05 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:41:08 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Tue, 25 Aug 2020 18:29:22 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Tue, 25 Aug 2020 18:30:16 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 25 Aug 2020 18:30:17 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 25 Aug 2020 18:30:17 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 25 Aug 2020 18:30:18 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 25 Aug 2020 18:30:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 Aug 2020 18:30:18 GMT
USER mysql
# Tue, 25 Aug 2020 18:30:18 GMT
EXPOSE 3306
# Tue, 25 Aug 2020 18:30:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14bc3f760dd091dd563d2ef48f1147f72762a2b31109b475d8dcb60d351993a`  
		Last Modified: Mon, 10 Aug 2020 18:46:17 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd29505baaec9c24f65109881fc6c0d6d097e1d3973e08df81965f3d7bbdeef`  
		Last Modified: Mon, 10 Aug 2020 18:46:15 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35af5ab9a3507b90b1780d5c5f6f67c87bf9ab542ff82c91768593541302d95d`  
		Last Modified: Mon, 10 Aug 2020 18:46:16 GMT  
		Size: 6.5 MB (6520666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c120071707bdce8a2c097ec51e0ba326faf19d324fe2344135d47a195382e7a3`  
		Last Modified: Tue, 25 Aug 2020 18:31:15 GMT  
		Size: 115.6 MB (115577656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36714b45d31e2c0d3060533bb22b194773c2314f76087bcd85c7ce01680688`  
		Last Modified: Tue, 25 Aug 2020 18:30:56 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd1024e5c88aa4f5f0ce9960f3c2c77fc1bd423cc2e240926b3d69c3bfdc58`  
		Last Modified: Tue, 25 Aug 2020 18:30:55 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5-centos`

```console
$ docker pull percona@sha256:34c453b0c796d184df0f5049c3ff47aa3d6c6db0b344c6170b5fef5bfb615ea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5-centos` - linux; amd64

```console
$ docker pull percona@sha256:68dad5e2efeb6893e2d7d116a1eae144f2c641c17d00e7869397395590c91651
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.0 MB (197968054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb49da8a7d3c22eb92a4de93d43ede592bb5487ac89ad866211a4f9ef8d11a3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:41:04 GMT
RUN groupdel input && groupadd -g 999 mysql
# Mon, 10 Aug 2020 18:41:05 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:41:08 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Tue, 25 Aug 2020 18:29:22 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Tue, 25 Aug 2020 18:30:16 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 25 Aug 2020 18:30:17 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 25 Aug 2020 18:30:17 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 25 Aug 2020 18:30:18 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 25 Aug 2020 18:30:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 Aug 2020 18:30:18 GMT
USER mysql
# Tue, 25 Aug 2020 18:30:18 GMT
EXPOSE 3306
# Tue, 25 Aug 2020 18:30:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14bc3f760dd091dd563d2ef48f1147f72762a2b31109b475d8dcb60d351993a`  
		Last Modified: Mon, 10 Aug 2020 18:46:17 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd29505baaec9c24f65109881fc6c0d6d097e1d3973e08df81965f3d7bbdeef`  
		Last Modified: Mon, 10 Aug 2020 18:46:15 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35af5ab9a3507b90b1780d5c5f6f67c87bf9ab542ff82c91768593541302d95d`  
		Last Modified: Mon, 10 Aug 2020 18:46:16 GMT  
		Size: 6.5 MB (6520666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c120071707bdce8a2c097ec51e0ba326faf19d324fe2344135d47a195382e7a3`  
		Last Modified: Tue, 25 Aug 2020 18:31:15 GMT  
		Size: 115.6 MB (115577656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36714b45d31e2c0d3060533bb22b194773c2314f76087bcd85c7ce01680688`  
		Last Modified: Tue, 25 Aug 2020 18:30:56 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd1024e5c88aa4f5f0ce9960f3c2c77fc1bd423cc2e240926b3d69c3bfdc58`  
		Last Modified: Tue, 25 Aug 2020 18:30:55 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8`

```console
$ docker pull percona@sha256:0a954add058176ff9e4b32e89add0e1c1f823b00bb84409bbd6a1dc64c17f8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8` - linux; amd64

```console
$ docker pull percona@sha256:6d4524eccd26af7bd7fb623c567159dfbd7f3d9a0e2f7bebd54af1e9ca9903dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226844917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83b637a6bfeda06bc2257037ca71fc122be1c537f8f12df59dd2149e6f005bb0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:39:48 GMT
RUN groupadd -g 1001 mysql
# Mon, 10 Aug 2020 18:39:48 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:39:53 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 10 Aug 2020 18:39:53 GMT
ENV PERCONA_VERSION=8.0.20-11.1.el7
# Mon, 10 Aug 2020 18:40:54 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 10 Aug 2020 18:40:55 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 10 Aug 2020 18:40:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 10 Aug 2020 18:40:55 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 10 Aug 2020 18:40:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:40:55 GMT
USER mysql
# Mon, 10 Aug 2020 18:40:56 GMT
EXPOSE 3306 33060
# Mon, 10 Aug 2020 18:40:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccd1831dd4a3e5ec4ae656d64d4a1c8fb826ae337a6b00de7839dbf4cd488f`  
		Last Modified: Mon, 10 Aug 2020 18:45:40 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aee8410d07aafe258c6360a478e295f77844d2f917d7c776fb3d87167a81ed4`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f7209a3389898cb2d9b5fd402161071eb7922beee2e4ef1a2ff601651a01a9`  
		Last Modified: Mon, 10 Aug 2020 18:45:41 GMT  
		Size: 6.5 MB (6520691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191d50365cd568082ca8e49128338cfd176fbc1449a8517b410659d67559783d`  
		Last Modified: Mon, 10 Aug 2020 18:46:05 GMT  
		Size: 144.5 MB (144454731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50eb93a060eaeedb4838ed7507bd9be5c0dbe716df655dd6db2ea974fa18b412`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f8232756960001c90ded8711d2fbc94030556d14ba2b90b12659663f26b94a`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0`

```console
$ docker pull percona@sha256:0a954add058176ff9e4b32e89add0e1c1f823b00bb84409bbd6a1dc64c17f8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0` - linux; amd64

```console
$ docker pull percona@sha256:6d4524eccd26af7bd7fb623c567159dfbd7f3d9a0e2f7bebd54af1e9ca9903dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226844917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83b637a6bfeda06bc2257037ca71fc122be1c537f8f12df59dd2149e6f005bb0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:39:48 GMT
RUN groupadd -g 1001 mysql
# Mon, 10 Aug 2020 18:39:48 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:39:53 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 10 Aug 2020 18:39:53 GMT
ENV PERCONA_VERSION=8.0.20-11.1.el7
# Mon, 10 Aug 2020 18:40:54 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 10 Aug 2020 18:40:55 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 10 Aug 2020 18:40:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 10 Aug 2020 18:40:55 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 10 Aug 2020 18:40:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:40:55 GMT
USER mysql
# Mon, 10 Aug 2020 18:40:56 GMT
EXPOSE 3306 33060
# Mon, 10 Aug 2020 18:40:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccd1831dd4a3e5ec4ae656d64d4a1c8fb826ae337a6b00de7839dbf4cd488f`  
		Last Modified: Mon, 10 Aug 2020 18:45:40 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aee8410d07aafe258c6360a478e295f77844d2f917d7c776fb3d87167a81ed4`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f7209a3389898cb2d9b5fd402161071eb7922beee2e4ef1a2ff601651a01a9`  
		Last Modified: Mon, 10 Aug 2020 18:45:41 GMT  
		Size: 6.5 MB (6520691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191d50365cd568082ca8e49128338cfd176fbc1449a8517b410659d67559783d`  
		Last Modified: Mon, 10 Aug 2020 18:46:05 GMT  
		Size: 144.5 MB (144454731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50eb93a060eaeedb4838ed7507bd9be5c0dbe716df655dd6db2ea974fa18b412`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f8232756960001c90ded8711d2fbc94030556d14ba2b90b12659663f26b94a`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.20-11`

```console
$ docker pull percona@sha256:0a954add058176ff9e4b32e89add0e1c1f823b00bb84409bbd6a1dc64c17f8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0.20-11` - linux; amd64

```console
$ docker pull percona@sha256:6d4524eccd26af7bd7fb623c567159dfbd7f3d9a0e2f7bebd54af1e9ca9903dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226844917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83b637a6bfeda06bc2257037ca71fc122be1c537f8f12df59dd2149e6f005bb0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:39:48 GMT
RUN groupadd -g 1001 mysql
# Mon, 10 Aug 2020 18:39:48 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:39:53 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 10 Aug 2020 18:39:53 GMT
ENV PERCONA_VERSION=8.0.20-11.1.el7
# Mon, 10 Aug 2020 18:40:54 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 10 Aug 2020 18:40:55 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 10 Aug 2020 18:40:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 10 Aug 2020 18:40:55 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 10 Aug 2020 18:40:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:40:55 GMT
USER mysql
# Mon, 10 Aug 2020 18:40:56 GMT
EXPOSE 3306 33060
# Mon, 10 Aug 2020 18:40:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccd1831dd4a3e5ec4ae656d64d4a1c8fb826ae337a6b00de7839dbf4cd488f`  
		Last Modified: Mon, 10 Aug 2020 18:45:40 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aee8410d07aafe258c6360a478e295f77844d2f917d7c776fb3d87167a81ed4`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f7209a3389898cb2d9b5fd402161071eb7922beee2e4ef1a2ff601651a01a9`  
		Last Modified: Mon, 10 Aug 2020 18:45:41 GMT  
		Size: 6.5 MB (6520691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191d50365cd568082ca8e49128338cfd176fbc1449a8517b410659d67559783d`  
		Last Modified: Mon, 10 Aug 2020 18:46:05 GMT  
		Size: 144.5 MB (144454731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50eb93a060eaeedb4838ed7507bd9be5c0dbe716df655dd6db2ea974fa18b412`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f8232756960001c90ded8711d2fbc94030556d14ba2b90b12659663f26b94a`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.20-11-centos`

```console
$ docker pull percona@sha256:0a954add058176ff9e4b32e89add0e1c1f823b00bb84409bbd6a1dc64c17f8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0.20-11-centos` - linux; amd64

```console
$ docker pull percona@sha256:6d4524eccd26af7bd7fb623c567159dfbd7f3d9a0e2f7bebd54af1e9ca9903dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226844917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83b637a6bfeda06bc2257037ca71fc122be1c537f8f12df59dd2149e6f005bb0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:39:48 GMT
RUN groupadd -g 1001 mysql
# Mon, 10 Aug 2020 18:39:48 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:39:53 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 10 Aug 2020 18:39:53 GMT
ENV PERCONA_VERSION=8.0.20-11.1.el7
# Mon, 10 Aug 2020 18:40:54 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 10 Aug 2020 18:40:55 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 10 Aug 2020 18:40:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 10 Aug 2020 18:40:55 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 10 Aug 2020 18:40:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:40:55 GMT
USER mysql
# Mon, 10 Aug 2020 18:40:56 GMT
EXPOSE 3306 33060
# Mon, 10 Aug 2020 18:40:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccd1831dd4a3e5ec4ae656d64d4a1c8fb826ae337a6b00de7839dbf4cd488f`  
		Last Modified: Mon, 10 Aug 2020 18:45:40 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aee8410d07aafe258c6360a478e295f77844d2f917d7c776fb3d87167a81ed4`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f7209a3389898cb2d9b5fd402161071eb7922beee2e4ef1a2ff601651a01a9`  
		Last Modified: Mon, 10 Aug 2020 18:45:41 GMT  
		Size: 6.5 MB (6520691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191d50365cd568082ca8e49128338cfd176fbc1449a8517b410659d67559783d`  
		Last Modified: Mon, 10 Aug 2020 18:46:05 GMT  
		Size: 144.5 MB (144454731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50eb93a060eaeedb4838ed7507bd9be5c0dbe716df655dd6db2ea974fa18b412`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f8232756960001c90ded8711d2fbc94030556d14ba2b90b12659663f26b94a`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0-centos`

```console
$ docker pull percona@sha256:0a954add058176ff9e4b32e89add0e1c1f823b00bb84409bbd6a1dc64c17f8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0-centos` - linux; amd64

```console
$ docker pull percona@sha256:6d4524eccd26af7bd7fb623c567159dfbd7f3d9a0e2f7bebd54af1e9ca9903dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226844917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83b637a6bfeda06bc2257037ca71fc122be1c537f8f12df59dd2149e6f005bb0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:39:48 GMT
RUN groupadd -g 1001 mysql
# Mon, 10 Aug 2020 18:39:48 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:39:53 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 10 Aug 2020 18:39:53 GMT
ENV PERCONA_VERSION=8.0.20-11.1.el7
# Mon, 10 Aug 2020 18:40:54 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 10 Aug 2020 18:40:55 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 10 Aug 2020 18:40:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 10 Aug 2020 18:40:55 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 10 Aug 2020 18:40:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:40:55 GMT
USER mysql
# Mon, 10 Aug 2020 18:40:56 GMT
EXPOSE 3306 33060
# Mon, 10 Aug 2020 18:40:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccd1831dd4a3e5ec4ae656d64d4a1c8fb826ae337a6b00de7839dbf4cd488f`  
		Last Modified: Mon, 10 Aug 2020 18:45:40 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aee8410d07aafe258c6360a478e295f77844d2f917d7c776fb3d87167a81ed4`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f7209a3389898cb2d9b5fd402161071eb7922beee2e4ef1a2ff601651a01a9`  
		Last Modified: Mon, 10 Aug 2020 18:45:41 GMT  
		Size: 6.5 MB (6520691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191d50365cd568082ca8e49128338cfd176fbc1449a8517b410659d67559783d`  
		Last Modified: Mon, 10 Aug 2020 18:46:05 GMT  
		Size: 144.5 MB (144454731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50eb93a060eaeedb4838ed7507bd9be5c0dbe716df655dd6db2ea974fa18b412`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f8232756960001c90ded8711d2fbc94030556d14ba2b90b12659663f26b94a`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8-centos`

```console
$ docker pull percona@sha256:0a954add058176ff9e4b32e89add0e1c1f823b00bb84409bbd6a1dc64c17f8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8-centos` - linux; amd64

```console
$ docker pull percona@sha256:6d4524eccd26af7bd7fb623c567159dfbd7f3d9a0e2f7bebd54af1e9ca9903dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226844917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83b637a6bfeda06bc2257037ca71fc122be1c537f8f12df59dd2149e6f005bb0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:39:48 GMT
RUN groupadd -g 1001 mysql
# Mon, 10 Aug 2020 18:39:48 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:39:53 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 10 Aug 2020 18:39:53 GMT
ENV PERCONA_VERSION=8.0.20-11.1.el7
# Mon, 10 Aug 2020 18:40:54 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 10 Aug 2020 18:40:55 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 10 Aug 2020 18:40:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 10 Aug 2020 18:40:55 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 10 Aug 2020 18:40:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:40:55 GMT
USER mysql
# Mon, 10 Aug 2020 18:40:56 GMT
EXPOSE 3306 33060
# Mon, 10 Aug 2020 18:40:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccd1831dd4a3e5ec4ae656d64d4a1c8fb826ae337a6b00de7839dbf4cd488f`  
		Last Modified: Mon, 10 Aug 2020 18:45:40 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aee8410d07aafe258c6360a478e295f77844d2f917d7c776fb3d87167a81ed4`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f7209a3389898cb2d9b5fd402161071eb7922beee2e4ef1a2ff601651a01a9`  
		Last Modified: Mon, 10 Aug 2020 18:45:41 GMT  
		Size: 6.5 MB (6520691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191d50365cd568082ca8e49128338cfd176fbc1449a8517b410659d67559783d`  
		Last Modified: Mon, 10 Aug 2020 18:46:05 GMT  
		Size: 144.5 MB (144454731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50eb93a060eaeedb4838ed7507bd9be5c0dbe716df655dd6db2ea974fa18b412`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f8232756960001c90ded8711d2fbc94030556d14ba2b90b12659663f26b94a`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:centos`

```console
$ docker pull percona@sha256:34c453b0c796d184df0f5049c3ff47aa3d6c6db0b344c6170b5fef5bfb615ea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:centos` - linux; amd64

```console
$ docker pull percona@sha256:68dad5e2efeb6893e2d7d116a1eae144f2c641c17d00e7869397395590c91651
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.0 MB (197968054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb49da8a7d3c22eb92a4de93d43ede592bb5487ac89ad866211a4f9ef8d11a3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:41:04 GMT
RUN groupdel input && groupadd -g 999 mysql
# Mon, 10 Aug 2020 18:41:05 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:41:08 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Tue, 25 Aug 2020 18:29:22 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Tue, 25 Aug 2020 18:30:16 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 25 Aug 2020 18:30:17 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 25 Aug 2020 18:30:17 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 25 Aug 2020 18:30:18 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 25 Aug 2020 18:30:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 Aug 2020 18:30:18 GMT
USER mysql
# Tue, 25 Aug 2020 18:30:18 GMT
EXPOSE 3306
# Tue, 25 Aug 2020 18:30:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14bc3f760dd091dd563d2ef48f1147f72762a2b31109b475d8dcb60d351993a`  
		Last Modified: Mon, 10 Aug 2020 18:46:17 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd29505baaec9c24f65109881fc6c0d6d097e1d3973e08df81965f3d7bbdeef`  
		Last Modified: Mon, 10 Aug 2020 18:46:15 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35af5ab9a3507b90b1780d5c5f6f67c87bf9ab542ff82c91768593541302d95d`  
		Last Modified: Mon, 10 Aug 2020 18:46:16 GMT  
		Size: 6.5 MB (6520666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c120071707bdce8a2c097ec51e0ba326faf19d324fe2344135d47a195382e7a3`  
		Last Modified: Tue, 25 Aug 2020 18:31:15 GMT  
		Size: 115.6 MB (115577656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36714b45d31e2c0d3060533bb22b194773c2314f76087bcd85c7ce01680688`  
		Last Modified: Tue, 25 Aug 2020 18:30:56 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd1024e5c88aa4f5f0ce9960f3c2c77fc1bd423cc2e240926b3d69c3bfdc58`  
		Last Modified: Tue, 25 Aug 2020 18:30:55 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:latest`

```console
$ docker pull percona@sha256:34c453b0c796d184df0f5049c3ff47aa3d6c6db0b344c6170b5fef5bfb615ea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:latest` - linux; amd64

```console
$ docker pull percona@sha256:68dad5e2efeb6893e2d7d116a1eae144f2c641c17d00e7869397395590c91651
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.0 MB (197968054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb49da8a7d3c22eb92a4de93d43ede592bb5487ac89ad866211a4f9ef8d11a3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:41:04 GMT
RUN groupdel input && groupadd -g 999 mysql
# Mon, 10 Aug 2020 18:41:05 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:41:08 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Tue, 25 Aug 2020 18:29:22 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Tue, 25 Aug 2020 18:30:16 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 25 Aug 2020 18:30:17 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 25 Aug 2020 18:30:17 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 25 Aug 2020 18:30:18 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 25 Aug 2020 18:30:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 Aug 2020 18:30:18 GMT
USER mysql
# Tue, 25 Aug 2020 18:30:18 GMT
EXPOSE 3306
# Tue, 25 Aug 2020 18:30:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14bc3f760dd091dd563d2ef48f1147f72762a2b31109b475d8dcb60d351993a`  
		Last Modified: Mon, 10 Aug 2020 18:46:17 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd29505baaec9c24f65109881fc6c0d6d097e1d3973e08df81965f3d7bbdeef`  
		Last Modified: Mon, 10 Aug 2020 18:46:15 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35af5ab9a3507b90b1780d5c5f6f67c87bf9ab542ff82c91768593541302d95d`  
		Last Modified: Mon, 10 Aug 2020 18:46:16 GMT  
		Size: 6.5 MB (6520666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c120071707bdce8a2c097ec51e0ba326faf19d324fe2344135d47a195382e7a3`  
		Last Modified: Tue, 25 Aug 2020 18:31:15 GMT  
		Size: 115.6 MB (115577656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36714b45d31e2c0d3060533bb22b194773c2314f76087bcd85c7ce01680688`  
		Last Modified: Tue, 25 Aug 2020 18:30:56 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd1024e5c88aa4f5f0ce9960f3c2c77fc1bd423cc2e240926b3d69c3bfdc58`  
		Last Modified: Tue, 25 Aug 2020 18:30:55 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5`

```console
$ docker pull percona@sha256:34c453b0c796d184df0f5049c3ff47aa3d6c6db0b344c6170b5fef5bfb615ea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5` - linux; amd64

```console
$ docker pull percona@sha256:68dad5e2efeb6893e2d7d116a1eae144f2c641c17d00e7869397395590c91651
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.0 MB (197968054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb49da8a7d3c22eb92a4de93d43ede592bb5487ac89ad866211a4f9ef8d11a3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:41:04 GMT
RUN groupdel input && groupadd -g 999 mysql
# Mon, 10 Aug 2020 18:41:05 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:41:08 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Tue, 25 Aug 2020 18:29:22 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Tue, 25 Aug 2020 18:30:16 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 25 Aug 2020 18:30:17 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 25 Aug 2020 18:30:17 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 25 Aug 2020 18:30:18 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 25 Aug 2020 18:30:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 Aug 2020 18:30:18 GMT
USER mysql
# Tue, 25 Aug 2020 18:30:18 GMT
EXPOSE 3306
# Tue, 25 Aug 2020 18:30:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14bc3f760dd091dd563d2ef48f1147f72762a2b31109b475d8dcb60d351993a`  
		Last Modified: Mon, 10 Aug 2020 18:46:17 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd29505baaec9c24f65109881fc6c0d6d097e1d3973e08df81965f3d7bbdeef`  
		Last Modified: Mon, 10 Aug 2020 18:46:15 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35af5ab9a3507b90b1780d5c5f6f67c87bf9ab542ff82c91768593541302d95d`  
		Last Modified: Mon, 10 Aug 2020 18:46:16 GMT  
		Size: 6.5 MB (6520666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c120071707bdce8a2c097ec51e0ba326faf19d324fe2344135d47a195382e7a3`  
		Last Modified: Tue, 25 Aug 2020 18:31:15 GMT  
		Size: 115.6 MB (115577656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36714b45d31e2c0d3060533bb22b194773c2314f76087bcd85c7ce01680688`  
		Last Modified: Tue, 25 Aug 2020 18:30:56 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd1024e5c88aa4f5f0ce9960f3c2c77fc1bd423cc2e240926b3d69c3bfdc58`  
		Last Modified: Tue, 25 Aug 2020 18:30:55 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.6`

```console
$ docker pull percona@sha256:5c31992eec3a97d45d56430231b3bd63ab41ac42098bbb86cfbbf38cfda7ee8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.6` - linux; amd64

```console
$ docker pull percona@sha256:b205120a44c4ab52257c781178c14c1028cccae1a7b37eeb3be763663614c9c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140400649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3de140c1e4106683bdf83d5b26297e55f62e814d4e50298c55b55c05d90846a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:41:04 GMT
RUN groupdel input && groupadd -g 999 mysql
# Mon, 10 Aug 2020 18:41:05 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:42:24 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Mon, 10 Aug 2020 18:42:24 GMT
ENV PERCONA_VERSION=5.6.49-rel89.0.1.el7
# Mon, 10 Aug 2020 18:43:05 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 10 Aug 2020 18:43:06 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 10 Aug 2020 18:43:06 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 10 Aug 2020 18:43:06 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Mon, 10 Aug 2020 18:43:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:43:07 GMT
USER mysql
# Mon, 10 Aug 2020 18:43:07 GMT
EXPOSE 3306
# Mon, 10 Aug 2020 18:43:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14bc3f760dd091dd563d2ef48f1147f72762a2b31109b475d8dcb60d351993a`  
		Last Modified: Mon, 10 Aug 2020 18:46:17 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd29505baaec9c24f65109881fc6c0d6d097e1d3973e08df81965f3d7bbdeef`  
		Last Modified: Mon, 10 Aug 2020 18:46:15 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf289b643b5657c22f720bb6138c36e1e2281247fc899762743dac9417e6ec2`  
		Last Modified: Mon, 10 Aug 2020 18:46:47 GMT  
		Size: 6.5 MB (6520701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77772238b545fcdd030d3e20f9c6441c74c66147c096a061cb25064868730c5`  
		Last Modified: Mon, 10 Aug 2020 18:46:56 GMT  
		Size: 58.0 MB (58006846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360da840cd215f1383e6c585004609079a5026d68f032a1325f849491517baa4`  
		Last Modified: Mon, 10 Aug 2020 18:46:46 GMT  
		Size: 4.9 KB (4879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adc09e8de6b047ccbbb8c4524bc7c8557cb92f82d87f2331b52eee2a3a9523a`  
		Last Modified: Mon, 10 Aug 2020 18:46:46 GMT  
		Size: 2.9 KB (2941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.6.49`

```console
$ docker pull percona@sha256:5c31992eec3a97d45d56430231b3bd63ab41ac42098bbb86cfbbf38cfda7ee8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.6.49` - linux; amd64

```console
$ docker pull percona@sha256:b205120a44c4ab52257c781178c14c1028cccae1a7b37eeb3be763663614c9c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140400649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3de140c1e4106683bdf83d5b26297e55f62e814d4e50298c55b55c05d90846a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:41:04 GMT
RUN groupdel input && groupadd -g 999 mysql
# Mon, 10 Aug 2020 18:41:05 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:42:24 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;         rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;         percona-release disable all;     percona-release enable original release
# Mon, 10 Aug 2020 18:42:24 GMT
ENV PERCONA_VERSION=5.6.49-rel89.0.1.el7
# Mon, 10 Aug 2020 18:43:05 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 10 Aug 2020 18:43:06 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 10 Aug 2020 18:43:06 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 10 Aug 2020 18:43:06 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Mon, 10 Aug 2020 18:43:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:43:07 GMT
USER mysql
# Mon, 10 Aug 2020 18:43:07 GMT
EXPOSE 3306
# Mon, 10 Aug 2020 18:43:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14bc3f760dd091dd563d2ef48f1147f72762a2b31109b475d8dcb60d351993a`  
		Last Modified: Mon, 10 Aug 2020 18:46:17 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd29505baaec9c24f65109881fc6c0d6d097e1d3973e08df81965f3d7bbdeef`  
		Last Modified: Mon, 10 Aug 2020 18:46:15 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf289b643b5657c22f720bb6138c36e1e2281247fc899762743dac9417e6ec2`  
		Last Modified: Mon, 10 Aug 2020 18:46:47 GMT  
		Size: 6.5 MB (6520701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77772238b545fcdd030d3e20f9c6441c74c66147c096a061cb25064868730c5`  
		Last Modified: Mon, 10 Aug 2020 18:46:56 GMT  
		Size: 58.0 MB (58006846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360da840cd215f1383e6c585004609079a5026d68f032a1325f849491517baa4`  
		Last Modified: Mon, 10 Aug 2020 18:46:46 GMT  
		Size: 4.9 KB (4879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adc09e8de6b047ccbbb8c4524bc7c8557cb92f82d87f2331b52eee2a3a9523a`  
		Last Modified: Mon, 10 Aug 2020 18:46:46 GMT  
		Size: 2.9 KB (2941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.7`

```console
$ docker pull percona@sha256:34c453b0c796d184df0f5049c3ff47aa3d6c6db0b344c6170b5fef5bfb615ea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.7` - linux; amd64

```console
$ docker pull percona@sha256:68dad5e2efeb6893e2d7d116a1eae144f2c641c17d00e7869397395590c91651
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.0 MB (197968054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb49da8a7d3c22eb92a4de93d43ede592bb5487ac89ad866211a4f9ef8d11a3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:41:04 GMT
RUN groupdel input && groupadd -g 999 mysql
# Mon, 10 Aug 2020 18:41:05 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:41:08 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Tue, 25 Aug 2020 18:29:22 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Tue, 25 Aug 2020 18:30:16 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 25 Aug 2020 18:30:17 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 25 Aug 2020 18:30:17 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 25 Aug 2020 18:30:18 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 25 Aug 2020 18:30:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 Aug 2020 18:30:18 GMT
USER mysql
# Tue, 25 Aug 2020 18:30:18 GMT
EXPOSE 3306
# Tue, 25 Aug 2020 18:30:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14bc3f760dd091dd563d2ef48f1147f72762a2b31109b475d8dcb60d351993a`  
		Last Modified: Mon, 10 Aug 2020 18:46:17 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd29505baaec9c24f65109881fc6c0d6d097e1d3973e08df81965f3d7bbdeef`  
		Last Modified: Mon, 10 Aug 2020 18:46:15 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35af5ab9a3507b90b1780d5c5f6f67c87bf9ab542ff82c91768593541302d95d`  
		Last Modified: Mon, 10 Aug 2020 18:46:16 GMT  
		Size: 6.5 MB (6520666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c120071707bdce8a2c097ec51e0ba326faf19d324fe2344135d47a195382e7a3`  
		Last Modified: Tue, 25 Aug 2020 18:31:15 GMT  
		Size: 115.6 MB (115577656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36714b45d31e2c0d3060533bb22b194773c2314f76087bcd85c7ce01680688`  
		Last Modified: Tue, 25 Aug 2020 18:30:56 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd1024e5c88aa4f5f0ce9960f3c2c77fc1bd423cc2e240926b3d69c3bfdc58`  
		Last Modified: Tue, 25 Aug 2020 18:30:55 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.7.31`

```console
$ docker pull percona@sha256:34c453b0c796d184df0f5049c3ff47aa3d6c6db0b344c6170b5fef5bfb615ea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.7.31` - linux; amd64

```console
$ docker pull percona@sha256:68dad5e2efeb6893e2d7d116a1eae144f2c641c17d00e7869397395590c91651
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.0 MB (197968054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb49da8a7d3c22eb92a4de93d43ede592bb5487ac89ad866211a4f9ef8d11a3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:41:04 GMT
RUN groupdel input && groupadd -g 999 mysql
# Mon, 10 Aug 2020 18:41:05 GMT
RUN useradd -u 999 -r -g 999 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:41:08 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Tue, 25 Aug 2020 18:29:22 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Tue, 25 Aug 2020 18:30:16 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 25 Aug 2020 18:30:17 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Tue, 25 Aug 2020 18:30:17 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 25 Aug 2020 18:30:18 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Tue, 25 Aug 2020 18:30:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 Aug 2020 18:30:18 GMT
USER mysql
# Tue, 25 Aug 2020 18:30:18 GMT
EXPOSE 3306
# Tue, 25 Aug 2020 18:30:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14bc3f760dd091dd563d2ef48f1147f72762a2b31109b475d8dcb60d351993a`  
		Last Modified: Mon, 10 Aug 2020 18:46:17 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd29505baaec9c24f65109881fc6c0d6d097e1d3973e08df81965f3d7bbdeef`  
		Last Modified: Mon, 10 Aug 2020 18:46:15 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35af5ab9a3507b90b1780d5c5f6f67c87bf9ab542ff82c91768593541302d95d`  
		Last Modified: Mon, 10 Aug 2020 18:46:16 GMT  
		Size: 6.5 MB (6520666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c120071707bdce8a2c097ec51e0ba326faf19d324fe2344135d47a195382e7a3`  
		Last Modified: Tue, 25 Aug 2020 18:31:15 GMT  
		Size: 115.6 MB (115577656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36714b45d31e2c0d3060533bb22b194773c2314f76087bcd85c7ce01680688`  
		Last Modified: Tue, 25 Aug 2020 18:30:56 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd1024e5c88aa4f5f0ce9960f3c2c77fc1bd423cc2e240926b3d69c3bfdc58`  
		Last Modified: Tue, 25 Aug 2020 18:30:55 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8`

```console
$ docker pull percona@sha256:0a954add058176ff9e4b32e89add0e1c1f823b00bb84409bbd6a1dc64c17f8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8` - linux; amd64

```console
$ docker pull percona@sha256:6d4524eccd26af7bd7fb623c567159dfbd7f3d9a0e2f7bebd54af1e9ca9903dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226844917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83b637a6bfeda06bc2257037ca71fc122be1c537f8f12df59dd2149e6f005bb0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:39:48 GMT
RUN groupadd -g 1001 mysql
# Mon, 10 Aug 2020 18:39:48 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:39:53 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 10 Aug 2020 18:39:53 GMT
ENV PERCONA_VERSION=8.0.20-11.1.el7
# Mon, 10 Aug 2020 18:40:54 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 10 Aug 2020 18:40:55 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 10 Aug 2020 18:40:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 10 Aug 2020 18:40:55 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 10 Aug 2020 18:40:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:40:55 GMT
USER mysql
# Mon, 10 Aug 2020 18:40:56 GMT
EXPOSE 3306 33060
# Mon, 10 Aug 2020 18:40:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccd1831dd4a3e5ec4ae656d64d4a1c8fb826ae337a6b00de7839dbf4cd488f`  
		Last Modified: Mon, 10 Aug 2020 18:45:40 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aee8410d07aafe258c6360a478e295f77844d2f917d7c776fb3d87167a81ed4`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f7209a3389898cb2d9b5fd402161071eb7922beee2e4ef1a2ff601651a01a9`  
		Last Modified: Mon, 10 Aug 2020 18:45:41 GMT  
		Size: 6.5 MB (6520691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191d50365cd568082ca8e49128338cfd176fbc1449a8517b410659d67559783d`  
		Last Modified: Mon, 10 Aug 2020 18:46:05 GMT  
		Size: 144.5 MB (144454731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50eb93a060eaeedb4838ed7507bd9be5c0dbe716df655dd6db2ea974fa18b412`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f8232756960001c90ded8711d2fbc94030556d14ba2b90b12659663f26b94a`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0`

```console
$ docker pull percona@sha256:0a954add058176ff9e4b32e89add0e1c1f823b00bb84409bbd6a1dc64c17f8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8.0` - linux; amd64

```console
$ docker pull percona@sha256:6d4524eccd26af7bd7fb623c567159dfbd7f3d9a0e2f7bebd54af1e9ca9903dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226844917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83b637a6bfeda06bc2257037ca71fc122be1c537f8f12df59dd2149e6f005bb0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:39:48 GMT
RUN groupadd -g 1001 mysql
# Mon, 10 Aug 2020 18:39:48 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:39:53 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 10 Aug 2020 18:39:53 GMT
ENV PERCONA_VERSION=8.0.20-11.1.el7
# Mon, 10 Aug 2020 18:40:54 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 10 Aug 2020 18:40:55 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 10 Aug 2020 18:40:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 10 Aug 2020 18:40:55 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 10 Aug 2020 18:40:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:40:55 GMT
USER mysql
# Mon, 10 Aug 2020 18:40:56 GMT
EXPOSE 3306 33060
# Mon, 10 Aug 2020 18:40:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccd1831dd4a3e5ec4ae656d64d4a1c8fb826ae337a6b00de7839dbf4cd488f`  
		Last Modified: Mon, 10 Aug 2020 18:45:40 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aee8410d07aafe258c6360a478e295f77844d2f917d7c776fb3d87167a81ed4`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f7209a3389898cb2d9b5fd402161071eb7922beee2e4ef1a2ff601651a01a9`  
		Last Modified: Mon, 10 Aug 2020 18:45:41 GMT  
		Size: 6.5 MB (6520691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191d50365cd568082ca8e49128338cfd176fbc1449a8517b410659d67559783d`  
		Last Modified: Mon, 10 Aug 2020 18:46:05 GMT  
		Size: 144.5 MB (144454731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50eb93a060eaeedb4838ed7507bd9be5c0dbe716df655dd6db2ea974fa18b412`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f8232756960001c90ded8711d2fbc94030556d14ba2b90b12659663f26b94a`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0.20-11`

```console
$ docker pull percona@sha256:0a954add058176ff9e4b32e89add0e1c1f823b00bb84409bbd6a1dc64c17f8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8.0.20-11` - linux; amd64

```console
$ docker pull percona@sha256:6d4524eccd26af7bd7fb623c567159dfbd7f3d9a0e2f7bebd54af1e9ca9903dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226844917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83b637a6bfeda06bc2257037ca71fc122be1c537f8f12df59dd2149e6f005bb0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:39:48 GMT
RUN groupadd -g 1001 mysql
# Mon, 10 Aug 2020 18:39:48 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 10 Aug 2020 18:39:53 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Mon, 10 Aug 2020 18:39:53 GMT
ENV PERCONA_VERSION=8.0.20-11.1.el7
# Mon, 10 Aug 2020 18:40:54 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Mon, 10 Aug 2020 18:40:55 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 10 Aug 2020 18:40:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 10 Aug 2020 18:40:55 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 10 Aug 2020 18:40:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:40:55 GMT
USER mysql
# Mon, 10 Aug 2020 18:40:56 GMT
EXPOSE 3306 33060
# Mon, 10 Aug 2020 18:40:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccd1831dd4a3e5ec4ae656d64d4a1c8fb826ae337a6b00de7839dbf4cd488f`  
		Last Modified: Mon, 10 Aug 2020 18:45:40 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aee8410d07aafe258c6360a478e295f77844d2f917d7c776fb3d87167a81ed4`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f7209a3389898cb2d9b5fd402161071eb7922beee2e4ef1a2ff601651a01a9`  
		Last Modified: Mon, 10 Aug 2020 18:45:41 GMT  
		Size: 6.5 MB (6520691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191d50365cd568082ca8e49128338cfd176fbc1449a8517b410659d67559783d`  
		Last Modified: Mon, 10 Aug 2020 18:46:05 GMT  
		Size: 144.5 MB (144454731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50eb93a060eaeedb4838ed7507bd9be5c0dbe716df655dd6db2ea974fa18b412`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f8232756960001c90ded8711d2fbc94030556d14ba2b90b12659663f26b94a`  
		Last Modified: Mon, 10 Aug 2020 18:45:39 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-3.6`

```console
$ docker pull percona@sha256:9cb3697a01eb0004ecdf50148f158689765a472ed587851e9315802ba12ad6cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6` - linux; amd64

```console
$ docker pull percona@sha256:b99eb8da53225288ec57217d7dc12147fc3ab23be0c31d6aef0128c6aefb2357
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.5 MB (157475795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:389f77c209ee832872f3a8af694538c0d180511d5066a1fe85d2868d305aa60e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.schema-version=1.0
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.vendor=Percona
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.license=SSPLv1
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.vendor=Percona
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 12 Oct 2020 23:27:35 GMT
ENV PSMDB_VERSION=3.6.19-8.0
# Mon, 12 Oct 2020 23:27:35 GMT
ENV OS_VER=el8
# Mon, 12 Oct 2020 23:27:35 GMT
ENV FULL_PERCONA_VERSION=3.6.19-8.0.el8
# Mon, 12 Oct 2020 23:27:35 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 12 Oct 2020 23:27:35 GMT
LABEL org.label-schema.schema-version=3.6.19-8.0
# Mon, 12 Oct 2020 23:27:36 GMT
LABEL org.opencontainers.image.version=3.6.19-8.0
# Mon, 12 Oct 2020 23:27:41 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Mon, 12 Oct 2020 23:29:07 GMT
RUN set -ex;     dnf install -y         dnf-utils         shadow-utils         curl         procps-ng         jq         oniguruma         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         dnf remove -y dnf-utils;         dnf clean all;         rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Mon, 12 Oct 2020 23:29:08 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 12 Oct 2020 23:29:08 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 12 Oct 2020 23:29:09 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 12 Oct 2020 23:29:11 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 12 Oct 2020 23:29:11 GMT
VOLUME [/data/db]
# Mon, 12 Oct 2020 23:29:11 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Mon, 12 Oct 2020 23:29:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Oct 2020 23:29:11 GMT
EXPOSE 27017
# Mon, 12 Oct 2020 23:29:12 GMT
USER 1001
# Mon, 12 Oct 2020 23:29:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026fd142135cccc902939200d9ef4958d0906f35ecd2e6281d78ea772bfbc263`  
		Last Modified: Mon, 12 Oct 2020 23:30:45 GMT  
		Size: 18.5 MB (18498753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc08ed7425d14c5f9a43044b3a0fda9cc0404dd2e47b1885aaa1dde677cb429b`  
		Last Modified: Mon, 12 Oct 2020 23:30:52 GMT  
		Size: 56.0 MB (55950293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee31f98cc7d6171c1cf63c3d64d534a21f96dd0f8c51b16e641fd4b0e081e1d`  
		Last Modified: Mon, 12 Oct 2020 23:30:42 GMT  
		Size: 1.5 KB (1546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa6bdf439054511291388a32d93c4c9b9226afa4633b44cd8044ab9c7b5ac1c`  
		Last Modified: Mon, 12 Oct 2020 23:30:42 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef8e1eaeebdede0689bfcf5c45b8c3ef26388b535e1a4154bf245f9f19e4705`  
		Last Modified: Mon, 12 Oct 2020 23:30:42 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b8e9f0e4c69ddb2a653381a51ed85851aa0f81fffcd7e1bb4ddd5e43014666`  
		Last Modified: Mon, 12 Oct 2020 23:30:45 GMT  
		Size: 8.1 MB (8137888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f371c8ee58424503974b0cb045958d785aedb4657d990dea7f97683d394a09`  
		Last Modified: Mon, 12 Oct 2020 23:30:42 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-3.6.19`

```console
$ docker pull percona@sha256:9cb3697a01eb0004ecdf50148f158689765a472ed587851e9315802ba12ad6cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6.19` - linux; amd64

```console
$ docker pull percona@sha256:b99eb8da53225288ec57217d7dc12147fc3ab23be0c31d6aef0128c6aefb2357
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.5 MB (157475795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:389f77c209ee832872f3a8af694538c0d180511d5066a1fe85d2868d305aa60e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.schema-version=1.0
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.vendor=Percona
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.license=SSPLv1
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.vendor=Percona
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 12 Oct 2020 23:27:35 GMT
ENV PSMDB_VERSION=3.6.19-8.0
# Mon, 12 Oct 2020 23:27:35 GMT
ENV OS_VER=el8
# Mon, 12 Oct 2020 23:27:35 GMT
ENV FULL_PERCONA_VERSION=3.6.19-8.0.el8
# Mon, 12 Oct 2020 23:27:35 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 12 Oct 2020 23:27:35 GMT
LABEL org.label-schema.schema-version=3.6.19-8.0
# Mon, 12 Oct 2020 23:27:36 GMT
LABEL org.opencontainers.image.version=3.6.19-8.0
# Mon, 12 Oct 2020 23:27:41 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Mon, 12 Oct 2020 23:29:07 GMT
RUN set -ex;     dnf install -y         dnf-utils         shadow-utils         curl         procps-ng         jq         oniguruma         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         dnf remove -y dnf-utils;         dnf clean all;         rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Mon, 12 Oct 2020 23:29:08 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 12 Oct 2020 23:29:08 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 12 Oct 2020 23:29:09 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 12 Oct 2020 23:29:11 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 12 Oct 2020 23:29:11 GMT
VOLUME [/data/db]
# Mon, 12 Oct 2020 23:29:11 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Mon, 12 Oct 2020 23:29:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Oct 2020 23:29:11 GMT
EXPOSE 27017
# Mon, 12 Oct 2020 23:29:12 GMT
USER 1001
# Mon, 12 Oct 2020 23:29:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026fd142135cccc902939200d9ef4958d0906f35ecd2e6281d78ea772bfbc263`  
		Last Modified: Mon, 12 Oct 2020 23:30:45 GMT  
		Size: 18.5 MB (18498753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc08ed7425d14c5f9a43044b3a0fda9cc0404dd2e47b1885aaa1dde677cb429b`  
		Last Modified: Mon, 12 Oct 2020 23:30:52 GMT  
		Size: 56.0 MB (55950293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee31f98cc7d6171c1cf63c3d64d534a21f96dd0f8c51b16e641fd4b0e081e1d`  
		Last Modified: Mon, 12 Oct 2020 23:30:42 GMT  
		Size: 1.5 KB (1546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa6bdf439054511291388a32d93c4c9b9226afa4633b44cd8044ab9c7b5ac1c`  
		Last Modified: Mon, 12 Oct 2020 23:30:42 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef8e1eaeebdede0689bfcf5c45b8c3ef26388b535e1a4154bf245f9f19e4705`  
		Last Modified: Mon, 12 Oct 2020 23:30:42 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b8e9f0e4c69ddb2a653381a51ed85851aa0f81fffcd7e1bb4ddd5e43014666`  
		Last Modified: Mon, 12 Oct 2020 23:30:45 GMT  
		Size: 8.1 MB (8137888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f371c8ee58424503974b0cb045958d785aedb4657d990dea7f97683d394a09`  
		Last Modified: Mon, 12 Oct 2020 23:30:42 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.0`

```console
$ docker pull percona@sha256:fae1681a81476b2e05b13dc7c76dae3993ad04c74f4506a6dc3f05c2abbb38b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0` - linux; amd64

```console
$ docker pull percona@sha256:be4c733aa9b5f9dae5d9316d137a39a025cf068fda74b1180e0bfc2c06c768cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.3 MB (160266575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec000be1f954e4d46b2ecfcfaa23bbe31310864df65029fc3686d4fb82396ee5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.schema-version=1.0
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.vendor=Percona
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.license=SSPLv1
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.vendor=Percona
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 12 Oct 2020 23:26:30 GMT
ENV PSMDB_VERSION=4.0.20-14
# Mon, 12 Oct 2020 23:26:30 GMT
ENV OS_VER=el8
# Mon, 12 Oct 2020 23:26:30 GMT
ENV FULL_PERCONA_VERSION=4.0.20-14.el8
# Mon, 12 Oct 2020 23:26:31 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 12 Oct 2020 23:26:31 GMT
LABEL org.label-schema.schema-version=4.0.20-14
# Mon, 12 Oct 2020 23:26:31 GMT
LABEL org.opencontainers.image.version=4.0.20-14
# Mon, 12 Oct 2020 23:26:36 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-40 release
# Mon, 12 Oct 2020 23:27:20 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Mon, 12 Oct 2020 23:27:21 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 12 Oct 2020 23:27:21 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 12 Oct 2020 23:27:22 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 12 Oct 2020 23:27:22 GMT
ENV GOSU_VERSION=1.11
# Mon, 12 Oct 2020 23:27:24 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Mon, 12 Oct 2020 23:27:25 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 12 Oct 2020 23:27:26 GMT
VOLUME [/data/db]
# Mon, 12 Oct 2020 23:27:26 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Mon, 12 Oct 2020 23:27:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Oct 2020 23:27:26 GMT
EXPOSE 27017
# Mon, 12 Oct 2020 23:27:26 GMT
USER 1001
# Mon, 12 Oct 2020 23:27:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5ba7e151e324f42f2d84f8f6670ec672ab147c0483f434abc0b8ea35419ad2`  
		Last Modified: Mon, 12 Oct 2020 23:30:30 GMT  
		Size: 18.5 MB (18498836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdd7b3aa8765c02b2a621c893088ac5998bbdd3f50a91ce884be44add1a783b`  
		Last Modified: Mon, 12 Oct 2020 23:30:37 GMT  
		Size: 57.8 MB (57826439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8735f7fc9e83dd3f93199e99049b70425c22cdba8434595048db8c60d9fbee1`  
		Last Modified: Mon, 12 Oct 2020 23:30:28 GMT  
		Size: 1.5 KB (1546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781b2a376e49acc8ae8c427c65629c85ea72465a7c18aa44c4786970e9158a7f`  
		Last Modified: Mon, 12 Oct 2020 23:30:27 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d93ef50d7cfad10ff84cc60e5cf5a965e012e1524c704a9e6c40a7000879610`  
		Last Modified: Mon, 12 Oct 2020 23:30:27 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca332f12de04fb6361b7b24591a9f9639adef8e0153e40e9547bab8158428460`  
		Last Modified: Mon, 12 Oct 2020 23:30:27 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84567a8925d51ba2547a805e0606c5a05548501405b82731bd40a794410a252e`  
		Last Modified: Mon, 12 Oct 2020 23:30:28 GMT  
		Size: 8.1 MB (8137890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872ef8548d10bc94f27bc0af1d9b0cf928efb674f7411717deba17420a7c6390`  
		Last Modified: Mon, 12 Oct 2020 23:30:27 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.0.20`

```console
$ docker pull percona@sha256:fae1681a81476b2e05b13dc7c76dae3993ad04c74f4506a6dc3f05c2abbb38b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0.20` - linux; amd64

```console
$ docker pull percona@sha256:be4c733aa9b5f9dae5d9316d137a39a025cf068fda74b1180e0bfc2c06c768cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.3 MB (160266575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec000be1f954e4d46b2ecfcfaa23bbe31310864df65029fc3686d4fb82396ee5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.schema-version=1.0
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.vendor=Percona
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.license=SSPLv1
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.vendor=Percona
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 12 Oct 2020 23:26:30 GMT
ENV PSMDB_VERSION=4.0.20-14
# Mon, 12 Oct 2020 23:26:30 GMT
ENV OS_VER=el8
# Mon, 12 Oct 2020 23:26:30 GMT
ENV FULL_PERCONA_VERSION=4.0.20-14.el8
# Mon, 12 Oct 2020 23:26:31 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 12 Oct 2020 23:26:31 GMT
LABEL org.label-schema.schema-version=4.0.20-14
# Mon, 12 Oct 2020 23:26:31 GMT
LABEL org.opencontainers.image.version=4.0.20-14
# Mon, 12 Oct 2020 23:26:36 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-40 release
# Mon, 12 Oct 2020 23:27:20 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Mon, 12 Oct 2020 23:27:21 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 12 Oct 2020 23:27:21 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 12 Oct 2020 23:27:22 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 12 Oct 2020 23:27:22 GMT
ENV GOSU_VERSION=1.11
# Mon, 12 Oct 2020 23:27:24 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Mon, 12 Oct 2020 23:27:25 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 12 Oct 2020 23:27:26 GMT
VOLUME [/data/db]
# Mon, 12 Oct 2020 23:27:26 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Mon, 12 Oct 2020 23:27:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Oct 2020 23:27:26 GMT
EXPOSE 27017
# Mon, 12 Oct 2020 23:27:26 GMT
USER 1001
# Mon, 12 Oct 2020 23:27:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5ba7e151e324f42f2d84f8f6670ec672ab147c0483f434abc0b8ea35419ad2`  
		Last Modified: Mon, 12 Oct 2020 23:30:30 GMT  
		Size: 18.5 MB (18498836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdd7b3aa8765c02b2a621c893088ac5998bbdd3f50a91ce884be44add1a783b`  
		Last Modified: Mon, 12 Oct 2020 23:30:37 GMT  
		Size: 57.8 MB (57826439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8735f7fc9e83dd3f93199e99049b70425c22cdba8434595048db8c60d9fbee1`  
		Last Modified: Mon, 12 Oct 2020 23:30:28 GMT  
		Size: 1.5 KB (1546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781b2a376e49acc8ae8c427c65629c85ea72465a7c18aa44c4786970e9158a7f`  
		Last Modified: Mon, 12 Oct 2020 23:30:27 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d93ef50d7cfad10ff84cc60e5cf5a965e012e1524c704a9e6c40a7000879610`  
		Last Modified: Mon, 12 Oct 2020 23:30:27 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca332f12de04fb6361b7b24591a9f9639adef8e0153e40e9547bab8158428460`  
		Last Modified: Mon, 12 Oct 2020 23:30:27 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84567a8925d51ba2547a805e0606c5a05548501405b82731bd40a794410a252e`  
		Last Modified: Mon, 12 Oct 2020 23:30:28 GMT  
		Size: 8.1 MB (8137890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872ef8548d10bc94f27bc0af1d9b0cf928efb674f7411717deba17420a7c6390`  
		Last Modified: Mon, 12 Oct 2020 23:30:27 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:93b6fe9e73f94207bcc8e528aa3fced37aa0aa6bb1432c366abdc8fe88355165
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:ca976ddd693bef566f9473b5c4075e6df5f4691dcc0ec00da80aa3c479e88800
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (168994723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48a9d253dbbc2fd29e7ab1d4157deb3dd0764fcb18878b87a76d82c9e60805e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.schema-version=1.0
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.vendor=Percona
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.license=SSPLv1
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.vendor=Percona
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 12 Oct 2020 23:24:44 GMT
ENV PSMDB_VERSION=4.2.9-10
# Mon, 12 Oct 2020 23:24:45 GMT
ENV OS_VER=el8
# Mon, 12 Oct 2020 23:24:45 GMT
ENV FULL_PERCONA_VERSION=4.2.9-10.el8
# Mon, 12 Oct 2020 23:24:45 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 12 Oct 2020 23:24:45 GMT
LABEL org.label-schema.schema-version=4.2.9-10
# Mon, 12 Oct 2020 23:24:45 GMT
LABEL org.opencontainers.image.version=4.2.9-10
# Mon, 12 Oct 2020 23:24:51 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Mon, 12 Oct 2020 23:26:13 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Mon, 12 Oct 2020 23:26:13 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 12 Oct 2020 23:26:14 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 12 Oct 2020 23:26:14 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 12 Oct 2020 23:26:15 GMT
ENV GOSU_VERSION=1.11
# Mon, 12 Oct 2020 23:26:16 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Mon, 12 Oct 2020 23:26:18 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 12 Oct 2020 23:26:19 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Mon, 12 Oct 2020 23:26:19 GMT
VOLUME [/data/db]
# Mon, 12 Oct 2020 23:26:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Oct 2020 23:26:19 GMT
EXPOSE 27017
# Mon, 12 Oct 2020 23:26:19 GMT
USER 1001
# Mon, 12 Oct 2020 23:26:19 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4598eb37c9c92a69c27788e3c557d4df713ee2ade165501d8781e778913ac0bb`  
		Last Modified: Mon, 12 Oct 2020 23:29:57 GMT  
		Size: 18.5 MB (18498855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cb35f9d56a11fd0809d61775f302f061b446e8a49e5516cdcdf0aa11ea84af`  
		Last Modified: Mon, 12 Oct 2020 23:30:23 GMT  
		Size: 66.6 MB (66554560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a88565e32967faea4be03ab125bace54b0c9429f42d50709fc65b30fdc25780`  
		Last Modified: Mon, 12 Oct 2020 23:29:54 GMT  
		Size: 1.5 KB (1543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb375f5b7464cd2d653ceacddba35a29d5e94aae4e6df264f0a893a63442fe4`  
		Last Modified: Mon, 12 Oct 2020 23:29:53 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f8e304c448d217a038390662e8a4c0c1f286753e5fb4825623488edfe89a80`  
		Last Modified: Mon, 12 Oct 2020 23:29:53 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4a1a1870451501ac7e97bb0651a3b714f8278b11f178eb8a152776d3ef47bf`  
		Last Modified: Mon, 12 Oct 2020 23:29:53 GMT  
		Size: 914.6 KB (914552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5f602fae06280037fbc89395ddd867e4a88689cd61128f017f3c2cb0020521`  
		Last Modified: Mon, 12 Oct 2020 23:29:54 GMT  
		Size: 8.1 MB (8137896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1583766639f8302631572f0a153688752759d73c8f5b5479671faa28bccc8`  
		Last Modified: Mon, 12 Oct 2020 23:29:53 GMT  
		Size: 4.5 KB (4543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2.9`

```console
$ docker pull percona@sha256:93b6fe9e73f94207bcc8e528aa3fced37aa0aa6bb1432c366abdc8fe88355165
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.2.9` - linux; amd64

```console
$ docker pull percona@sha256:ca976ddd693bef566f9473b5c4075e6df5f4691dcc0ec00da80aa3c479e88800
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (168994723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48a9d253dbbc2fd29e7ab1d4157deb3dd0764fcb18878b87a76d82c9e60805e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.schema-version=1.0
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.vendor=Percona
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.license=SSPLv1
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.vendor=Percona
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 12 Oct 2020 23:24:44 GMT
ENV PSMDB_VERSION=4.2.9-10
# Mon, 12 Oct 2020 23:24:45 GMT
ENV OS_VER=el8
# Mon, 12 Oct 2020 23:24:45 GMT
ENV FULL_PERCONA_VERSION=4.2.9-10.el8
# Mon, 12 Oct 2020 23:24:45 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 12 Oct 2020 23:24:45 GMT
LABEL org.label-schema.schema-version=4.2.9-10
# Mon, 12 Oct 2020 23:24:45 GMT
LABEL org.opencontainers.image.version=4.2.9-10
# Mon, 12 Oct 2020 23:24:51 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Mon, 12 Oct 2020 23:26:13 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Mon, 12 Oct 2020 23:26:13 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 12 Oct 2020 23:26:14 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 12 Oct 2020 23:26:14 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 12 Oct 2020 23:26:15 GMT
ENV GOSU_VERSION=1.11
# Mon, 12 Oct 2020 23:26:16 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Mon, 12 Oct 2020 23:26:18 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 12 Oct 2020 23:26:19 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Mon, 12 Oct 2020 23:26:19 GMT
VOLUME [/data/db]
# Mon, 12 Oct 2020 23:26:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Oct 2020 23:26:19 GMT
EXPOSE 27017
# Mon, 12 Oct 2020 23:26:19 GMT
USER 1001
# Mon, 12 Oct 2020 23:26:19 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4598eb37c9c92a69c27788e3c557d4df713ee2ade165501d8781e778913ac0bb`  
		Last Modified: Mon, 12 Oct 2020 23:29:57 GMT  
		Size: 18.5 MB (18498855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cb35f9d56a11fd0809d61775f302f061b446e8a49e5516cdcdf0aa11ea84af`  
		Last Modified: Mon, 12 Oct 2020 23:30:23 GMT  
		Size: 66.6 MB (66554560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a88565e32967faea4be03ab125bace54b0c9429f42d50709fc65b30fdc25780`  
		Last Modified: Mon, 12 Oct 2020 23:29:54 GMT  
		Size: 1.5 KB (1543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb375f5b7464cd2d653ceacddba35a29d5e94aae4e6df264f0a893a63442fe4`  
		Last Modified: Mon, 12 Oct 2020 23:29:53 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f8e304c448d217a038390662e8a4c0c1f286753e5fb4825623488edfe89a80`  
		Last Modified: Mon, 12 Oct 2020 23:29:53 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4a1a1870451501ac7e97bb0651a3b714f8278b11f178eb8a152776d3ef47bf`  
		Last Modified: Mon, 12 Oct 2020 23:29:53 GMT  
		Size: 914.6 KB (914552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5f602fae06280037fbc89395ddd867e4a88689cd61128f017f3c2cb0020521`  
		Last Modified: Mon, 12 Oct 2020 23:29:54 GMT  
		Size: 8.1 MB (8137896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1583766639f8302631572f0a153688752759d73c8f5b5479671faa28bccc8`  
		Last Modified: Mon, 12 Oct 2020 23:29:53 GMT  
		Size: 4.5 KB (4543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.4`

```console
$ docker pull percona@sha256:62006f0224906a408e4b20eecfc0fb5611d251544c2dd1d5792c6378cd0f4628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.4` - linux; amd64

```console
$ docker pull percona@sha256:2b12bb1628e54016a3d025dec8ce96cf1962cdd86f9f492f523260109f5dd782
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.7 MB (180688237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a25db8e909c45a6a62756c2232d085f99dc01ab9253fbfd9c25fed71579b16e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.schema-version=1.0
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.vendor=Percona
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.license=SSPLv1
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.vendor=Percona
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 12 Oct 2020 23:23:14 GMT
ENV PSMDB_VERSION=4.4.1-3
# Mon, 12 Oct 2020 23:23:14 GMT
ENV OS_VER=el8
# Mon, 12 Oct 2020 23:23:15 GMT
ENV FULL_PERCONA_VERSION=4.4.1-3.el8
# Mon, 12 Oct 2020 23:23:15 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 12 Oct 2020 23:23:15 GMT
LABEL org.label-schema.schema-version=4.4.1-3
# Mon, 12 Oct 2020 23:23:15 GMT
LABEL org.opencontainers.image.version=4.4.1-3
# Mon, 12 Oct 2020 23:23:21 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Mon, 12 Oct 2020 23:24:28 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Mon, 12 Oct 2020 23:24:29 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 12 Oct 2020 23:24:29 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 12 Oct 2020 23:24:30 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 12 Oct 2020 23:24:30 GMT
ENV GOSU_VERSION=1.11
# Mon, 12 Oct 2020 23:24:33 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Mon, 12 Oct 2020 23:24:35 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 12 Oct 2020 23:24:35 GMT
COPY file:1e164890dbc426ff0038117af76a47815ae534b64e95a15a83e6e5d7f79a4d77 in /entrypoint.sh 
# Mon, 12 Oct 2020 23:24:35 GMT
VOLUME [/data/db]
# Mon, 12 Oct 2020 23:24:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Oct 2020 23:24:35 GMT
EXPOSE 27017
# Mon, 12 Oct 2020 23:24:36 GMT
USER 1001
# Mon, 12 Oct 2020 23:24:36 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc34f3aca9d2f036f9140f3ef335ef7c6ec172b6f0ed8837ab62b0ce75ace79d`  
		Last Modified: Mon, 12 Oct 2020 23:29:41 GMT  
		Size: 18.5 MB (18498894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661990b80b0e4bc92dd584034d8e23962c2f4fa86a3b6a8368afa6c3f7eaf0be`  
		Last Modified: Mon, 12 Oct 2020 23:29:49 GMT  
		Size: 78.2 MB (78248039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5419b2bcb04f58ca0f7476c60cf049187a18a9460ece20a3c5d31a5fe55e3064`  
		Last Modified: Mon, 12 Oct 2020 23:29:37 GMT  
		Size: 1.5 KB (1547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4cc68c5a569b4632a25f119662405c89a141144ad073974d8869f67b1bed92`  
		Last Modified: Mon, 12 Oct 2020 23:29:36 GMT  
		Size: 4.1 KB (4072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fc31a7d2488eb4aece31ee79bf05111e4ec0de1c867f5e452bba946a62bdcd`  
		Last Modified: Mon, 12 Oct 2020 23:29:36 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c89251882d386c3fe869d6892f289eecada40a707b14eeb8f5b4fdbac84cc2b`  
		Last Modified: Mon, 12 Oct 2020 23:29:36 GMT  
		Size: 914.6 KB (914552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0647c7f051a652c92200ff19f0314e6e10b1b30b829bef27c26f6c61d9362c13`  
		Last Modified: Mon, 12 Oct 2020 23:29:38 GMT  
		Size: 8.1 MB (8137889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3395ad19ebde4f582c20d8dfa2390746c97df7a1d96d09b9c5e05b9a5fba7b`  
		Last Modified: Mon, 12 Oct 2020 23:29:36 GMT  
		Size: 4.5 KB (4545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.4.1`

```console
$ docker pull percona@sha256:62006f0224906a408e4b20eecfc0fb5611d251544c2dd1d5792c6378cd0f4628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.4.1` - linux; amd64

```console
$ docker pull percona@sha256:2b12bb1628e54016a3d025dec8ce96cf1962cdd86f9f492f523260109f5dd782
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.7 MB (180688237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a25db8e909c45a6a62756c2232d085f99dc01ab9253fbfd9c25fed71579b16e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.schema-version=1.0
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.vendor=Percona
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.license=SSPLv1
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.vendor=Percona
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 12 Oct 2020 23:23:14 GMT
ENV PSMDB_VERSION=4.4.1-3
# Mon, 12 Oct 2020 23:23:14 GMT
ENV OS_VER=el8
# Mon, 12 Oct 2020 23:23:15 GMT
ENV FULL_PERCONA_VERSION=4.4.1-3.el8
# Mon, 12 Oct 2020 23:23:15 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 12 Oct 2020 23:23:15 GMT
LABEL org.label-schema.schema-version=4.4.1-3
# Mon, 12 Oct 2020 23:23:15 GMT
LABEL org.opencontainers.image.version=4.4.1-3
# Mon, 12 Oct 2020 23:23:21 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Mon, 12 Oct 2020 23:24:28 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Mon, 12 Oct 2020 23:24:29 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 12 Oct 2020 23:24:29 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 12 Oct 2020 23:24:30 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 12 Oct 2020 23:24:30 GMT
ENV GOSU_VERSION=1.11
# Mon, 12 Oct 2020 23:24:33 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Mon, 12 Oct 2020 23:24:35 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 12 Oct 2020 23:24:35 GMT
COPY file:1e164890dbc426ff0038117af76a47815ae534b64e95a15a83e6e5d7f79a4d77 in /entrypoint.sh 
# Mon, 12 Oct 2020 23:24:35 GMT
VOLUME [/data/db]
# Mon, 12 Oct 2020 23:24:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Oct 2020 23:24:35 GMT
EXPOSE 27017
# Mon, 12 Oct 2020 23:24:36 GMT
USER 1001
# Mon, 12 Oct 2020 23:24:36 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc34f3aca9d2f036f9140f3ef335ef7c6ec172b6f0ed8837ab62b0ce75ace79d`  
		Last Modified: Mon, 12 Oct 2020 23:29:41 GMT  
		Size: 18.5 MB (18498894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661990b80b0e4bc92dd584034d8e23962c2f4fa86a3b6a8368afa6c3f7eaf0be`  
		Last Modified: Mon, 12 Oct 2020 23:29:49 GMT  
		Size: 78.2 MB (78248039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5419b2bcb04f58ca0f7476c60cf049187a18a9460ece20a3c5d31a5fe55e3064`  
		Last Modified: Mon, 12 Oct 2020 23:29:37 GMT  
		Size: 1.5 KB (1547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4cc68c5a569b4632a25f119662405c89a141144ad073974d8869f67b1bed92`  
		Last Modified: Mon, 12 Oct 2020 23:29:36 GMT  
		Size: 4.1 KB (4072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fc31a7d2488eb4aece31ee79bf05111e4ec0de1c867f5e452bba946a62bdcd`  
		Last Modified: Mon, 12 Oct 2020 23:29:36 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c89251882d386c3fe869d6892f289eecada40a707b14eeb8f5b4fdbac84cc2b`  
		Last Modified: Mon, 12 Oct 2020 23:29:36 GMT  
		Size: 914.6 KB (914552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0647c7f051a652c92200ff19f0314e6e10b1b30b829bef27c26f6c61d9362c13`  
		Last Modified: Mon, 12 Oct 2020 23:29:38 GMT  
		Size: 8.1 MB (8137889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3395ad19ebde4f582c20d8dfa2390746c97df7a1d96d09b9c5e05b9a5fba7b`  
		Last Modified: Mon, 12 Oct 2020 23:29:36 GMT  
		Size: 4.5 KB (4545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
