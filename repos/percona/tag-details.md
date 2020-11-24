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
-	[`percona:8.0.21-12`](#percona8021-12)
-	[`percona:8.0.21-12-centos`](#percona8021-12-centos)
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
-	[`percona:ps-8.0.21-12`](#perconaps-8021-12)
-	[`percona:psmdb-3.6`](#perconapsmdb-36)
-	[`percona:psmdb-3.6.20`](#perconapsmdb-3620)
-	[`percona:psmdb-4.0`](#perconapsmdb-40)
-	[`percona:psmdb-4.0.21`](#perconapsmdb-4021)
-	[`percona:psmdb-4.2`](#perconapsmdb-42)
-	[`percona:psmdb-4.2.10`](#perconapsmdb-4210)
-	[`percona:psmdb-4.4`](#perconapsmdb-44)
-	[`percona:psmdb-4.4.1`](#perconapsmdb-441)

## `percona:5`

```console
$ docker pull percona@sha256:45fcbae875813c481b2a8512baab655f0fba95dd53effb965f2a9c4af095921a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5` - linux; amd64

```console
$ docker pull percona@sha256:9c8ac645edf99c63fd0e10e7b1a646492ff88d2606dfa315171e9c5c82abb8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.3 MB (198252191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:864a2ef94e17e2cfc4a3f14eddd58281dfb36bae929923c3aff4e38fe253b8e8`
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
# Sat, 14 Nov 2020 00:45:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Sat, 14 Nov 2020 00:45:47 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Sat, 14 Nov 2020 00:46:43 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Sat, 14 Nov 2020 00:46:44 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 14 Nov 2020 00:46:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 14 Nov 2020 00:46:44 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 00:46:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:46:45 GMT
USER mysql
# Sat, 14 Nov 2020 00:46:45 GMT
EXPOSE 3306
# Sat, 14 Nov 2020 00:46:45 GMT
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
	-	`sha256:208fefe84162bbe35a2b6b6fe4cfa93ede795d9e9259091ce5935121ebeeb43f`  
		Last Modified: Sat, 14 Nov 2020 00:47:51 GMT  
		Size: 6.6 MB (6562445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c666fd48cbd7079df09d1bdb3dd2294c903a34e893876d853302720e123be7ef`  
		Last Modified: Sat, 14 Nov 2020 00:48:10 GMT  
		Size: 115.6 MB (115586047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47590bf1cafc3c6f87fa677a7d278d6b1c820f34b1329443bc96fdf61b73a58`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed93bade8b45184b4511ecf7dec76939db7b6199bc4807bc0ae779d74275cde`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
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
$ docker pull percona@sha256:45fcbae875813c481b2a8512baab655f0fba95dd53effb965f2a9c4af095921a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7` - linux; amd64

```console
$ docker pull percona@sha256:9c8ac645edf99c63fd0e10e7b1a646492ff88d2606dfa315171e9c5c82abb8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.3 MB (198252191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:864a2ef94e17e2cfc4a3f14eddd58281dfb36bae929923c3aff4e38fe253b8e8`
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
# Sat, 14 Nov 2020 00:45:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Sat, 14 Nov 2020 00:45:47 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Sat, 14 Nov 2020 00:46:43 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Sat, 14 Nov 2020 00:46:44 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 14 Nov 2020 00:46:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 14 Nov 2020 00:46:44 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 00:46:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:46:45 GMT
USER mysql
# Sat, 14 Nov 2020 00:46:45 GMT
EXPOSE 3306
# Sat, 14 Nov 2020 00:46:45 GMT
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
	-	`sha256:208fefe84162bbe35a2b6b6fe4cfa93ede795d9e9259091ce5935121ebeeb43f`  
		Last Modified: Sat, 14 Nov 2020 00:47:51 GMT  
		Size: 6.6 MB (6562445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c666fd48cbd7079df09d1bdb3dd2294c903a34e893876d853302720e123be7ef`  
		Last Modified: Sat, 14 Nov 2020 00:48:10 GMT  
		Size: 115.6 MB (115586047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47590bf1cafc3c6f87fa677a7d278d6b1c820f34b1329443bc96fdf61b73a58`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed93bade8b45184b4511ecf7dec76939db7b6199bc4807bc0ae779d74275cde`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.31`

```console
$ docker pull percona@sha256:45fcbae875813c481b2a8512baab655f0fba95dd53effb965f2a9c4af095921a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7.31` - linux; amd64

```console
$ docker pull percona@sha256:9c8ac645edf99c63fd0e10e7b1a646492ff88d2606dfa315171e9c5c82abb8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.3 MB (198252191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:864a2ef94e17e2cfc4a3f14eddd58281dfb36bae929923c3aff4e38fe253b8e8`
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
# Sat, 14 Nov 2020 00:45:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Sat, 14 Nov 2020 00:45:47 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Sat, 14 Nov 2020 00:46:43 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Sat, 14 Nov 2020 00:46:44 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 14 Nov 2020 00:46:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 14 Nov 2020 00:46:44 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 00:46:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:46:45 GMT
USER mysql
# Sat, 14 Nov 2020 00:46:45 GMT
EXPOSE 3306
# Sat, 14 Nov 2020 00:46:45 GMT
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
	-	`sha256:208fefe84162bbe35a2b6b6fe4cfa93ede795d9e9259091ce5935121ebeeb43f`  
		Last Modified: Sat, 14 Nov 2020 00:47:51 GMT  
		Size: 6.6 MB (6562445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c666fd48cbd7079df09d1bdb3dd2294c903a34e893876d853302720e123be7ef`  
		Last Modified: Sat, 14 Nov 2020 00:48:10 GMT  
		Size: 115.6 MB (115586047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47590bf1cafc3c6f87fa677a7d278d6b1c820f34b1329443bc96fdf61b73a58`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed93bade8b45184b4511ecf7dec76939db7b6199bc4807bc0ae779d74275cde`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7.31-centos`

```console
$ docker pull percona@sha256:45fcbae875813c481b2a8512baab655f0fba95dd53effb965f2a9c4af095921a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7.31-centos` - linux; amd64

```console
$ docker pull percona@sha256:9c8ac645edf99c63fd0e10e7b1a646492ff88d2606dfa315171e9c5c82abb8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.3 MB (198252191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:864a2ef94e17e2cfc4a3f14eddd58281dfb36bae929923c3aff4e38fe253b8e8`
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
# Sat, 14 Nov 2020 00:45:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Sat, 14 Nov 2020 00:45:47 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Sat, 14 Nov 2020 00:46:43 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Sat, 14 Nov 2020 00:46:44 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 14 Nov 2020 00:46:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 14 Nov 2020 00:46:44 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 00:46:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:46:45 GMT
USER mysql
# Sat, 14 Nov 2020 00:46:45 GMT
EXPOSE 3306
# Sat, 14 Nov 2020 00:46:45 GMT
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
	-	`sha256:208fefe84162bbe35a2b6b6fe4cfa93ede795d9e9259091ce5935121ebeeb43f`  
		Last Modified: Sat, 14 Nov 2020 00:47:51 GMT  
		Size: 6.6 MB (6562445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c666fd48cbd7079df09d1bdb3dd2294c903a34e893876d853302720e123be7ef`  
		Last Modified: Sat, 14 Nov 2020 00:48:10 GMT  
		Size: 115.6 MB (115586047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47590bf1cafc3c6f87fa677a7d278d6b1c820f34b1329443bc96fdf61b73a58`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed93bade8b45184b4511ecf7dec76939db7b6199bc4807bc0ae779d74275cde`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5.7-centos`

```console
$ docker pull percona@sha256:45fcbae875813c481b2a8512baab655f0fba95dd53effb965f2a9c4af095921a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5.7-centos` - linux; amd64

```console
$ docker pull percona@sha256:9c8ac645edf99c63fd0e10e7b1a646492ff88d2606dfa315171e9c5c82abb8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.3 MB (198252191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:864a2ef94e17e2cfc4a3f14eddd58281dfb36bae929923c3aff4e38fe253b8e8`
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
# Sat, 14 Nov 2020 00:45:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Sat, 14 Nov 2020 00:45:47 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Sat, 14 Nov 2020 00:46:43 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Sat, 14 Nov 2020 00:46:44 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 14 Nov 2020 00:46:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 14 Nov 2020 00:46:44 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 00:46:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:46:45 GMT
USER mysql
# Sat, 14 Nov 2020 00:46:45 GMT
EXPOSE 3306
# Sat, 14 Nov 2020 00:46:45 GMT
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
	-	`sha256:208fefe84162bbe35a2b6b6fe4cfa93ede795d9e9259091ce5935121ebeeb43f`  
		Last Modified: Sat, 14 Nov 2020 00:47:51 GMT  
		Size: 6.6 MB (6562445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c666fd48cbd7079df09d1bdb3dd2294c903a34e893876d853302720e123be7ef`  
		Last Modified: Sat, 14 Nov 2020 00:48:10 GMT  
		Size: 115.6 MB (115586047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47590bf1cafc3c6f87fa677a7d278d6b1c820f34b1329443bc96fdf61b73a58`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed93bade8b45184b4511ecf7dec76939db7b6199bc4807bc0ae779d74275cde`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:5-centos`

```console
$ docker pull percona@sha256:45fcbae875813c481b2a8512baab655f0fba95dd53effb965f2a9c4af095921a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:5-centos` - linux; amd64

```console
$ docker pull percona@sha256:9c8ac645edf99c63fd0e10e7b1a646492ff88d2606dfa315171e9c5c82abb8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.3 MB (198252191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:864a2ef94e17e2cfc4a3f14eddd58281dfb36bae929923c3aff4e38fe253b8e8`
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
# Sat, 14 Nov 2020 00:45:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Sat, 14 Nov 2020 00:45:47 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Sat, 14 Nov 2020 00:46:43 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Sat, 14 Nov 2020 00:46:44 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 14 Nov 2020 00:46:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 14 Nov 2020 00:46:44 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 00:46:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:46:45 GMT
USER mysql
# Sat, 14 Nov 2020 00:46:45 GMT
EXPOSE 3306
# Sat, 14 Nov 2020 00:46:45 GMT
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
	-	`sha256:208fefe84162bbe35a2b6b6fe4cfa93ede795d9e9259091ce5935121ebeeb43f`  
		Last Modified: Sat, 14 Nov 2020 00:47:51 GMT  
		Size: 6.6 MB (6562445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c666fd48cbd7079df09d1bdb3dd2294c903a34e893876d853302720e123be7ef`  
		Last Modified: Sat, 14 Nov 2020 00:48:10 GMT  
		Size: 115.6 MB (115586047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47590bf1cafc3c6f87fa677a7d278d6b1c820f34b1329443bc96fdf61b73a58`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed93bade8b45184b4511ecf7dec76939db7b6199bc4807bc0ae779d74275cde`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8`

```console
$ docker pull percona@sha256:a1273d6f72b5da3bae9fcdcb656616d8bc38d08105b828320fc79dd21c8dba92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8` - linux; amd64

```console
$ docker pull percona@sha256:c57cf0f624a9a4416554f6c200903c8b79cd0309289382e6a7872e5545b28575
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236751548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9185ad0f0d944c2c61a5f755c90405eab75c6a24873c5cc790c0d9175c482abf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Mon, 16 Nov 2020 19:39:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 16 Nov 2020 19:39:13 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 16 Nov 2020 19:39:21 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 16 Nov 2020 19:39:22 GMT
ENV PS_VERSION=8.0.21-12.2
# Mon, 16 Nov 2020 19:39:22 GMT
ENV OS_VER=el8
# Mon, 16 Nov 2020 19:39:22 GMT
ENV FULL_PERCONA_VERSION=8.0.21-12.2.el8
# Mon, 16 Nov 2020 19:39:54 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 16 Nov 2020 19:39:55 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 16 Nov 2020 19:39:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 16 Nov 2020 19:39:56 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 16 Nov 2020 19:39:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Nov 2020 19:39:56 GMT
USER mysql
# Mon, 16 Nov 2020 19:39:56 GMT
EXPOSE 3306 33060
# Mon, 16 Nov 2020 19:39:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5c21c8dd23951725264770525357311c5f99842bd0cffd423ac391a1c67c2c`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.6 KB (1573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91115ecbd4e79b56593edf14b0bf32e3c0787a11f6236bb02f561be7f9b3778f`  
		Last Modified: Mon, 16 Nov 2020 19:41:05 GMT  
		Size: 18.5 MB (18520881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68ad7472ceb873e420ccc67142748f9c5c14abbe924cfb5bb2e9c1925f9f381`  
		Last Modified: Mon, 16 Nov 2020 19:41:27 GMT  
		Size: 143.4 MB (143356788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c045fe6e096e00950bcff0644cd62ad34e0ce90dde58b4121a204d050e26dbc`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b212ebb3894defef05a2e5b2d9b3ebf6fdeba266e9808ff6871c944ffacc71`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0`

```console
$ docker pull percona@sha256:a1273d6f72b5da3bae9fcdcb656616d8bc38d08105b828320fc79dd21c8dba92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0` - linux; amd64

```console
$ docker pull percona@sha256:c57cf0f624a9a4416554f6c200903c8b79cd0309289382e6a7872e5545b28575
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236751548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9185ad0f0d944c2c61a5f755c90405eab75c6a24873c5cc790c0d9175c482abf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Mon, 16 Nov 2020 19:39:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 16 Nov 2020 19:39:13 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 16 Nov 2020 19:39:21 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 16 Nov 2020 19:39:22 GMT
ENV PS_VERSION=8.0.21-12.2
# Mon, 16 Nov 2020 19:39:22 GMT
ENV OS_VER=el8
# Mon, 16 Nov 2020 19:39:22 GMT
ENV FULL_PERCONA_VERSION=8.0.21-12.2.el8
# Mon, 16 Nov 2020 19:39:54 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 16 Nov 2020 19:39:55 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 16 Nov 2020 19:39:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 16 Nov 2020 19:39:56 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 16 Nov 2020 19:39:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Nov 2020 19:39:56 GMT
USER mysql
# Mon, 16 Nov 2020 19:39:56 GMT
EXPOSE 3306 33060
# Mon, 16 Nov 2020 19:39:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5c21c8dd23951725264770525357311c5f99842bd0cffd423ac391a1c67c2c`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.6 KB (1573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91115ecbd4e79b56593edf14b0bf32e3c0787a11f6236bb02f561be7f9b3778f`  
		Last Modified: Mon, 16 Nov 2020 19:41:05 GMT  
		Size: 18.5 MB (18520881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68ad7472ceb873e420ccc67142748f9c5c14abbe924cfb5bb2e9c1925f9f381`  
		Last Modified: Mon, 16 Nov 2020 19:41:27 GMT  
		Size: 143.4 MB (143356788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c045fe6e096e00950bcff0644cd62ad34e0ce90dde58b4121a204d050e26dbc`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b212ebb3894defef05a2e5b2d9b3ebf6fdeba266e9808ff6871c944ffacc71`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.21-12`

```console
$ docker pull percona@sha256:a1273d6f72b5da3bae9fcdcb656616d8bc38d08105b828320fc79dd21c8dba92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0.21-12` - linux; amd64

```console
$ docker pull percona@sha256:c57cf0f624a9a4416554f6c200903c8b79cd0309289382e6a7872e5545b28575
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236751548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9185ad0f0d944c2c61a5f755c90405eab75c6a24873c5cc790c0d9175c482abf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Mon, 16 Nov 2020 19:39:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 16 Nov 2020 19:39:13 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 16 Nov 2020 19:39:21 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 16 Nov 2020 19:39:22 GMT
ENV PS_VERSION=8.0.21-12.2
# Mon, 16 Nov 2020 19:39:22 GMT
ENV OS_VER=el8
# Mon, 16 Nov 2020 19:39:22 GMT
ENV FULL_PERCONA_VERSION=8.0.21-12.2.el8
# Mon, 16 Nov 2020 19:39:54 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 16 Nov 2020 19:39:55 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 16 Nov 2020 19:39:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 16 Nov 2020 19:39:56 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 16 Nov 2020 19:39:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Nov 2020 19:39:56 GMT
USER mysql
# Mon, 16 Nov 2020 19:39:56 GMT
EXPOSE 3306 33060
# Mon, 16 Nov 2020 19:39:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5c21c8dd23951725264770525357311c5f99842bd0cffd423ac391a1c67c2c`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.6 KB (1573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91115ecbd4e79b56593edf14b0bf32e3c0787a11f6236bb02f561be7f9b3778f`  
		Last Modified: Mon, 16 Nov 2020 19:41:05 GMT  
		Size: 18.5 MB (18520881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68ad7472ceb873e420ccc67142748f9c5c14abbe924cfb5bb2e9c1925f9f381`  
		Last Modified: Mon, 16 Nov 2020 19:41:27 GMT  
		Size: 143.4 MB (143356788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c045fe6e096e00950bcff0644cd62ad34e0ce90dde58b4121a204d050e26dbc`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b212ebb3894defef05a2e5b2d9b3ebf6fdeba266e9808ff6871c944ffacc71`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0.21-12-centos`

```console
$ docker pull percona@sha256:a1273d6f72b5da3bae9fcdcb656616d8bc38d08105b828320fc79dd21c8dba92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0.21-12-centos` - linux; amd64

```console
$ docker pull percona@sha256:c57cf0f624a9a4416554f6c200903c8b79cd0309289382e6a7872e5545b28575
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236751548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9185ad0f0d944c2c61a5f755c90405eab75c6a24873c5cc790c0d9175c482abf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Mon, 16 Nov 2020 19:39:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 16 Nov 2020 19:39:13 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 16 Nov 2020 19:39:21 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 16 Nov 2020 19:39:22 GMT
ENV PS_VERSION=8.0.21-12.2
# Mon, 16 Nov 2020 19:39:22 GMT
ENV OS_VER=el8
# Mon, 16 Nov 2020 19:39:22 GMT
ENV FULL_PERCONA_VERSION=8.0.21-12.2.el8
# Mon, 16 Nov 2020 19:39:54 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 16 Nov 2020 19:39:55 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 16 Nov 2020 19:39:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 16 Nov 2020 19:39:56 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 16 Nov 2020 19:39:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Nov 2020 19:39:56 GMT
USER mysql
# Mon, 16 Nov 2020 19:39:56 GMT
EXPOSE 3306 33060
# Mon, 16 Nov 2020 19:39:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5c21c8dd23951725264770525357311c5f99842bd0cffd423ac391a1c67c2c`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.6 KB (1573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91115ecbd4e79b56593edf14b0bf32e3c0787a11f6236bb02f561be7f9b3778f`  
		Last Modified: Mon, 16 Nov 2020 19:41:05 GMT  
		Size: 18.5 MB (18520881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68ad7472ceb873e420ccc67142748f9c5c14abbe924cfb5bb2e9c1925f9f381`  
		Last Modified: Mon, 16 Nov 2020 19:41:27 GMT  
		Size: 143.4 MB (143356788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c045fe6e096e00950bcff0644cd62ad34e0ce90dde58b4121a204d050e26dbc`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b212ebb3894defef05a2e5b2d9b3ebf6fdeba266e9808ff6871c944ffacc71`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8.0-centos`

```console
$ docker pull percona@sha256:a1273d6f72b5da3bae9fcdcb656616d8bc38d08105b828320fc79dd21c8dba92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8.0-centos` - linux; amd64

```console
$ docker pull percona@sha256:c57cf0f624a9a4416554f6c200903c8b79cd0309289382e6a7872e5545b28575
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236751548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9185ad0f0d944c2c61a5f755c90405eab75c6a24873c5cc790c0d9175c482abf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Mon, 16 Nov 2020 19:39:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 16 Nov 2020 19:39:13 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 16 Nov 2020 19:39:21 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 16 Nov 2020 19:39:22 GMT
ENV PS_VERSION=8.0.21-12.2
# Mon, 16 Nov 2020 19:39:22 GMT
ENV OS_VER=el8
# Mon, 16 Nov 2020 19:39:22 GMT
ENV FULL_PERCONA_VERSION=8.0.21-12.2.el8
# Mon, 16 Nov 2020 19:39:54 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 16 Nov 2020 19:39:55 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 16 Nov 2020 19:39:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 16 Nov 2020 19:39:56 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 16 Nov 2020 19:39:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Nov 2020 19:39:56 GMT
USER mysql
# Mon, 16 Nov 2020 19:39:56 GMT
EXPOSE 3306 33060
# Mon, 16 Nov 2020 19:39:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5c21c8dd23951725264770525357311c5f99842bd0cffd423ac391a1c67c2c`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.6 KB (1573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91115ecbd4e79b56593edf14b0bf32e3c0787a11f6236bb02f561be7f9b3778f`  
		Last Modified: Mon, 16 Nov 2020 19:41:05 GMT  
		Size: 18.5 MB (18520881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68ad7472ceb873e420ccc67142748f9c5c14abbe924cfb5bb2e9c1925f9f381`  
		Last Modified: Mon, 16 Nov 2020 19:41:27 GMT  
		Size: 143.4 MB (143356788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c045fe6e096e00950bcff0644cd62ad34e0ce90dde58b4121a204d050e26dbc`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b212ebb3894defef05a2e5b2d9b3ebf6fdeba266e9808ff6871c944ffacc71`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:8-centos`

```console
$ docker pull percona@sha256:a1273d6f72b5da3bae9fcdcb656616d8bc38d08105b828320fc79dd21c8dba92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8-centos` - linux; amd64

```console
$ docker pull percona@sha256:c57cf0f624a9a4416554f6c200903c8b79cd0309289382e6a7872e5545b28575
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236751548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9185ad0f0d944c2c61a5f755c90405eab75c6a24873c5cc790c0d9175c482abf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Mon, 16 Nov 2020 19:39:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 16 Nov 2020 19:39:13 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 16 Nov 2020 19:39:21 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 16 Nov 2020 19:39:22 GMT
ENV PS_VERSION=8.0.21-12.2
# Mon, 16 Nov 2020 19:39:22 GMT
ENV OS_VER=el8
# Mon, 16 Nov 2020 19:39:22 GMT
ENV FULL_PERCONA_VERSION=8.0.21-12.2.el8
# Mon, 16 Nov 2020 19:39:54 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 16 Nov 2020 19:39:55 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 16 Nov 2020 19:39:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 16 Nov 2020 19:39:56 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 16 Nov 2020 19:39:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Nov 2020 19:39:56 GMT
USER mysql
# Mon, 16 Nov 2020 19:39:56 GMT
EXPOSE 3306 33060
# Mon, 16 Nov 2020 19:39:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5c21c8dd23951725264770525357311c5f99842bd0cffd423ac391a1c67c2c`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.6 KB (1573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91115ecbd4e79b56593edf14b0bf32e3c0787a11f6236bb02f561be7f9b3778f`  
		Last Modified: Mon, 16 Nov 2020 19:41:05 GMT  
		Size: 18.5 MB (18520881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68ad7472ceb873e420ccc67142748f9c5c14abbe924cfb5bb2e9c1925f9f381`  
		Last Modified: Mon, 16 Nov 2020 19:41:27 GMT  
		Size: 143.4 MB (143356788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c045fe6e096e00950bcff0644cd62ad34e0ce90dde58b4121a204d050e26dbc`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b212ebb3894defef05a2e5b2d9b3ebf6fdeba266e9808ff6871c944ffacc71`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:centos`

```console
$ docker pull percona@sha256:45fcbae875813c481b2a8512baab655f0fba95dd53effb965f2a9c4af095921a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:centos` - linux; amd64

```console
$ docker pull percona@sha256:9c8ac645edf99c63fd0e10e7b1a646492ff88d2606dfa315171e9c5c82abb8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.3 MB (198252191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:864a2ef94e17e2cfc4a3f14eddd58281dfb36bae929923c3aff4e38fe253b8e8`
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
# Sat, 14 Nov 2020 00:45:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Sat, 14 Nov 2020 00:45:47 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Sat, 14 Nov 2020 00:46:43 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Sat, 14 Nov 2020 00:46:44 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 14 Nov 2020 00:46:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 14 Nov 2020 00:46:44 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 00:46:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:46:45 GMT
USER mysql
# Sat, 14 Nov 2020 00:46:45 GMT
EXPOSE 3306
# Sat, 14 Nov 2020 00:46:45 GMT
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
	-	`sha256:208fefe84162bbe35a2b6b6fe4cfa93ede795d9e9259091ce5935121ebeeb43f`  
		Last Modified: Sat, 14 Nov 2020 00:47:51 GMT  
		Size: 6.6 MB (6562445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c666fd48cbd7079df09d1bdb3dd2294c903a34e893876d853302720e123be7ef`  
		Last Modified: Sat, 14 Nov 2020 00:48:10 GMT  
		Size: 115.6 MB (115586047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47590bf1cafc3c6f87fa677a7d278d6b1c820f34b1329443bc96fdf61b73a58`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed93bade8b45184b4511ecf7dec76939db7b6199bc4807bc0ae779d74275cde`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:latest`

```console
$ docker pull percona@sha256:45fcbae875813c481b2a8512baab655f0fba95dd53effb965f2a9c4af095921a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:latest` - linux; amd64

```console
$ docker pull percona@sha256:9c8ac645edf99c63fd0e10e7b1a646492ff88d2606dfa315171e9c5c82abb8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.3 MB (198252191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:864a2ef94e17e2cfc4a3f14eddd58281dfb36bae929923c3aff4e38fe253b8e8`
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
# Sat, 14 Nov 2020 00:45:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Sat, 14 Nov 2020 00:45:47 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Sat, 14 Nov 2020 00:46:43 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Sat, 14 Nov 2020 00:46:44 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 14 Nov 2020 00:46:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 14 Nov 2020 00:46:44 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 00:46:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:46:45 GMT
USER mysql
# Sat, 14 Nov 2020 00:46:45 GMT
EXPOSE 3306
# Sat, 14 Nov 2020 00:46:45 GMT
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
	-	`sha256:208fefe84162bbe35a2b6b6fe4cfa93ede795d9e9259091ce5935121ebeeb43f`  
		Last Modified: Sat, 14 Nov 2020 00:47:51 GMT  
		Size: 6.6 MB (6562445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c666fd48cbd7079df09d1bdb3dd2294c903a34e893876d853302720e123be7ef`  
		Last Modified: Sat, 14 Nov 2020 00:48:10 GMT  
		Size: 115.6 MB (115586047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47590bf1cafc3c6f87fa677a7d278d6b1c820f34b1329443bc96fdf61b73a58`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed93bade8b45184b4511ecf7dec76939db7b6199bc4807bc0ae779d74275cde`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5`

```console
$ docker pull percona@sha256:45fcbae875813c481b2a8512baab655f0fba95dd53effb965f2a9c4af095921a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5` - linux; amd64

```console
$ docker pull percona@sha256:9c8ac645edf99c63fd0e10e7b1a646492ff88d2606dfa315171e9c5c82abb8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.3 MB (198252191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:864a2ef94e17e2cfc4a3f14eddd58281dfb36bae929923c3aff4e38fe253b8e8`
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
# Sat, 14 Nov 2020 00:45:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Sat, 14 Nov 2020 00:45:47 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Sat, 14 Nov 2020 00:46:43 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Sat, 14 Nov 2020 00:46:44 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 14 Nov 2020 00:46:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 14 Nov 2020 00:46:44 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 00:46:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:46:45 GMT
USER mysql
# Sat, 14 Nov 2020 00:46:45 GMT
EXPOSE 3306
# Sat, 14 Nov 2020 00:46:45 GMT
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
	-	`sha256:208fefe84162bbe35a2b6b6fe4cfa93ede795d9e9259091ce5935121ebeeb43f`  
		Last Modified: Sat, 14 Nov 2020 00:47:51 GMT  
		Size: 6.6 MB (6562445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c666fd48cbd7079df09d1bdb3dd2294c903a34e893876d853302720e123be7ef`  
		Last Modified: Sat, 14 Nov 2020 00:48:10 GMT  
		Size: 115.6 MB (115586047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47590bf1cafc3c6f87fa677a7d278d6b1c820f34b1329443bc96fdf61b73a58`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed93bade8b45184b4511ecf7dec76939db7b6199bc4807bc0ae779d74275cde`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
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
$ docker pull percona@sha256:45fcbae875813c481b2a8512baab655f0fba95dd53effb965f2a9c4af095921a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.7` - linux; amd64

```console
$ docker pull percona@sha256:9c8ac645edf99c63fd0e10e7b1a646492ff88d2606dfa315171e9c5c82abb8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.3 MB (198252191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:864a2ef94e17e2cfc4a3f14eddd58281dfb36bae929923c3aff4e38fe253b8e8`
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
# Sat, 14 Nov 2020 00:45:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Sat, 14 Nov 2020 00:45:47 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Sat, 14 Nov 2020 00:46:43 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Sat, 14 Nov 2020 00:46:44 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 14 Nov 2020 00:46:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 14 Nov 2020 00:46:44 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 00:46:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:46:45 GMT
USER mysql
# Sat, 14 Nov 2020 00:46:45 GMT
EXPOSE 3306
# Sat, 14 Nov 2020 00:46:45 GMT
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
	-	`sha256:208fefe84162bbe35a2b6b6fe4cfa93ede795d9e9259091ce5935121ebeeb43f`  
		Last Modified: Sat, 14 Nov 2020 00:47:51 GMT  
		Size: 6.6 MB (6562445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c666fd48cbd7079df09d1bdb3dd2294c903a34e893876d853302720e123be7ef`  
		Last Modified: Sat, 14 Nov 2020 00:48:10 GMT  
		Size: 115.6 MB (115586047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47590bf1cafc3c6f87fa677a7d278d6b1c820f34b1329443bc96fdf61b73a58`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed93bade8b45184b4511ecf7dec76939db7b6199bc4807bc0ae779d74275cde`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-5.7.31`

```console
$ docker pull percona@sha256:45fcbae875813c481b2a8512baab655f0fba95dd53effb965f2a9c4af095921a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.7.31` - linux; amd64

```console
$ docker pull percona@sha256:9c8ac645edf99c63fd0e10e7b1a646492ff88d2606dfa315171e9c5c82abb8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.3 MB (198252191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:864a2ef94e17e2cfc4a3f14eddd58281dfb36bae929923c3aff4e38fe253b8e8`
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
# Sat, 14 Nov 2020 00:45:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable original release
# Sat, 14 Nov 2020 00:45:47 GMT
ENV PERCONA_VERSION=5.7.31-34.1.el7
# Sat, 14 Nov 2020 00:46:43 GMT
RUN set -ex;     yum install -y         Percona-Server-server-57-${PERCONA_VERSION}         Percona-Server-devel-57-${PERCONA_VERSION}         Percona-Server-tokudb-57-${PERCONA_VERSION}         Percona-Server-rocksdb-57-${PERCONA_VERSION}         jemalloc         openssl         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Sat, 14 Nov 2020 00:46:44 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 14 Nov 2020 00:46:44 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 14 Nov 2020 00:46:44 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 00:46:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:46:45 GMT
USER mysql
# Sat, 14 Nov 2020 00:46:45 GMT
EXPOSE 3306
# Sat, 14 Nov 2020 00:46:45 GMT
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
	-	`sha256:208fefe84162bbe35a2b6b6fe4cfa93ede795d9e9259091ce5935121ebeeb43f`  
		Last Modified: Sat, 14 Nov 2020 00:47:51 GMT  
		Size: 6.6 MB (6562445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c666fd48cbd7079df09d1bdb3dd2294c903a34e893876d853302720e123be7ef`  
		Last Modified: Sat, 14 Nov 2020 00:48:10 GMT  
		Size: 115.6 MB (115586047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47590bf1cafc3c6f87fa677a7d278d6b1c820f34b1329443bc96fdf61b73a58`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed93bade8b45184b4511ecf7dec76939db7b6199bc4807bc0ae779d74275cde`  
		Last Modified: Sat, 14 Nov 2020 00:47:49 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8`

```console
$ docker pull percona@sha256:a1273d6f72b5da3bae9fcdcb656616d8bc38d08105b828320fc79dd21c8dba92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8` - linux; amd64

```console
$ docker pull percona@sha256:c57cf0f624a9a4416554f6c200903c8b79cd0309289382e6a7872e5545b28575
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236751548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9185ad0f0d944c2c61a5f755c90405eab75c6a24873c5cc790c0d9175c482abf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Mon, 16 Nov 2020 19:39:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 16 Nov 2020 19:39:13 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 16 Nov 2020 19:39:21 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 16 Nov 2020 19:39:22 GMT
ENV PS_VERSION=8.0.21-12.2
# Mon, 16 Nov 2020 19:39:22 GMT
ENV OS_VER=el8
# Mon, 16 Nov 2020 19:39:22 GMT
ENV FULL_PERCONA_VERSION=8.0.21-12.2.el8
# Mon, 16 Nov 2020 19:39:54 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 16 Nov 2020 19:39:55 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 16 Nov 2020 19:39:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 16 Nov 2020 19:39:56 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 16 Nov 2020 19:39:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Nov 2020 19:39:56 GMT
USER mysql
# Mon, 16 Nov 2020 19:39:56 GMT
EXPOSE 3306 33060
# Mon, 16 Nov 2020 19:39:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5c21c8dd23951725264770525357311c5f99842bd0cffd423ac391a1c67c2c`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.6 KB (1573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91115ecbd4e79b56593edf14b0bf32e3c0787a11f6236bb02f561be7f9b3778f`  
		Last Modified: Mon, 16 Nov 2020 19:41:05 GMT  
		Size: 18.5 MB (18520881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68ad7472ceb873e420ccc67142748f9c5c14abbe924cfb5bb2e9c1925f9f381`  
		Last Modified: Mon, 16 Nov 2020 19:41:27 GMT  
		Size: 143.4 MB (143356788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c045fe6e096e00950bcff0644cd62ad34e0ce90dde58b4121a204d050e26dbc`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b212ebb3894defef05a2e5b2d9b3ebf6fdeba266e9808ff6871c944ffacc71`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0`

```console
$ docker pull percona@sha256:a1273d6f72b5da3bae9fcdcb656616d8bc38d08105b828320fc79dd21c8dba92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8.0` - linux; amd64

```console
$ docker pull percona@sha256:c57cf0f624a9a4416554f6c200903c8b79cd0309289382e6a7872e5545b28575
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236751548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9185ad0f0d944c2c61a5f755c90405eab75c6a24873c5cc790c0d9175c482abf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Mon, 16 Nov 2020 19:39:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 16 Nov 2020 19:39:13 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 16 Nov 2020 19:39:21 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 16 Nov 2020 19:39:22 GMT
ENV PS_VERSION=8.0.21-12.2
# Mon, 16 Nov 2020 19:39:22 GMT
ENV OS_VER=el8
# Mon, 16 Nov 2020 19:39:22 GMT
ENV FULL_PERCONA_VERSION=8.0.21-12.2.el8
# Mon, 16 Nov 2020 19:39:54 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 16 Nov 2020 19:39:55 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 16 Nov 2020 19:39:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 16 Nov 2020 19:39:56 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 16 Nov 2020 19:39:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Nov 2020 19:39:56 GMT
USER mysql
# Mon, 16 Nov 2020 19:39:56 GMT
EXPOSE 3306 33060
# Mon, 16 Nov 2020 19:39:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5c21c8dd23951725264770525357311c5f99842bd0cffd423ac391a1c67c2c`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.6 KB (1573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91115ecbd4e79b56593edf14b0bf32e3c0787a11f6236bb02f561be7f9b3778f`  
		Last Modified: Mon, 16 Nov 2020 19:41:05 GMT  
		Size: 18.5 MB (18520881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68ad7472ceb873e420ccc67142748f9c5c14abbe924cfb5bb2e9c1925f9f381`  
		Last Modified: Mon, 16 Nov 2020 19:41:27 GMT  
		Size: 143.4 MB (143356788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c045fe6e096e00950bcff0644cd62ad34e0ce90dde58b4121a204d050e26dbc`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b212ebb3894defef05a2e5b2d9b3ebf6fdeba266e9808ff6871c944ffacc71`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:ps-8.0.21-12`

```console
$ docker pull percona@sha256:a1273d6f72b5da3bae9fcdcb656616d8bc38d08105b828320fc79dd21c8dba92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8.0.21-12` - linux; amd64

```console
$ docker pull percona@sha256:c57cf0f624a9a4416554f6c200903c8b79cd0309289382e6a7872e5545b28575
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236751548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9185ad0f0d944c2c61a5f755c90405eab75c6a24873c5cc790c0d9175c482abf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Mon, 16 Nov 2020 19:39:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 16 Nov 2020 19:39:13 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Mon, 16 Nov 2020 19:39:21 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 16 Nov 2020 19:39:22 GMT
ENV PS_VERSION=8.0.21-12.2
# Mon, 16 Nov 2020 19:39:22 GMT
ENV OS_VER=el8
# Mon, 16 Nov 2020 19:39:22 GMT
ENV FULL_PERCONA_VERSION=8.0.21-12.2.el8
# Mon, 16 Nov 2020 19:39:54 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 16 Nov 2020 19:39:55 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 16 Nov 2020 19:39:55 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 16 Nov 2020 19:39:56 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 16 Nov 2020 19:39:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Nov 2020 19:39:56 GMT
USER mysql
# Mon, 16 Nov 2020 19:39:56 GMT
EXPOSE 3306 33060
# Mon, 16 Nov 2020 19:39:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5c21c8dd23951725264770525357311c5f99842bd0cffd423ac391a1c67c2c`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.6 KB (1573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91115ecbd4e79b56593edf14b0bf32e3c0787a11f6236bb02f561be7f9b3778f`  
		Last Modified: Mon, 16 Nov 2020 19:41:05 GMT  
		Size: 18.5 MB (18520881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68ad7472ceb873e420ccc67142748f9c5c14abbe924cfb5bb2e9c1925f9f381`  
		Last Modified: Mon, 16 Nov 2020 19:41:27 GMT  
		Size: 143.4 MB (143356788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c045fe6e096e00950bcff0644cd62ad34e0ce90dde58b4121a204d050e26dbc`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b212ebb3894defef05a2e5b2d9b3ebf6fdeba266e9808ff6871c944ffacc71`  
		Last Modified: Mon, 16 Nov 2020 19:41:03 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-3.6`

```console
$ docker pull percona@sha256:ac265b4ec8fed1766dc22260cdc52fdbdf2bedd529ab621abcf9b20f8717178d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6` - linux; amd64

```console
$ docker pull percona@sha256:021a211cedfb0683d3594d6309a19a1eb2f817435bb2e33d3b90d332963f6075
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.7 MB (157653105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638083383fc6ffa940c5a98ec2fbc9b2cce9a3244d00eaf266c00c07f0732121`
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
# Mon, 26 Oct 2020 17:24:28 GMT
ENV PSMDB_VERSION=3.6.20-9.0
# Mon, 26 Oct 2020 17:24:28 GMT
ENV OS_VER=el8
# Mon, 26 Oct 2020 17:24:28 GMT
ENV FULL_PERCONA_VERSION=3.6.20-9.0.el8
# Mon, 26 Oct 2020 17:24:28 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 26 Oct 2020 17:24:28 GMT
LABEL org.label-schema.schema-version=3.6.20-9.0
# Mon, 26 Oct 2020 17:24:29 GMT
LABEL org.opencontainers.image.version=3.6.20-9.0
# Mon, 26 Oct 2020 17:24:35 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Mon, 26 Oct 2020 17:24:50 GMT
RUN set -ex;     dnf install -y         dnf-utils         shadow-utils         curl         procps-ng         jq         oniguruma         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         dnf remove -y dnf-utils;         dnf clean all;         rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Mon, 26 Oct 2020 17:24:50 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 26 Oct 2020 17:24:51 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 26 Oct 2020 17:24:51 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 26 Oct 2020 17:24:53 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 26 Oct 2020 17:24:54 GMT
VOLUME [/data/db]
# Mon, 26 Oct 2020 17:24:54 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Mon, 26 Oct 2020 17:24:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Oct 2020 17:24:54 GMT
EXPOSE 27017
# Mon, 26 Oct 2020 17:24:54 GMT
USER 1001
# Mon, 26 Oct 2020 17:24:54 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fc827a496eb3c077fcef59e088800bc6f1cbe54185087987e552096bf8e49a`  
		Last Modified: Mon, 26 Oct 2020 17:25:29 GMT  
		Size: 18.5 MB (18498764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b1b93cdcac2da2df8793a9ded026af624430baa62e7e242d7715d5fbc2c376`  
		Last Modified: Mon, 26 Oct 2020 17:25:36 GMT  
		Size: 56.1 MB (56127594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb0bf69fb72ec24a3c6ea3918a369693b9f22048e24b09d6d605a5f59b2a1ee`  
		Last Modified: Mon, 26 Oct 2020 17:25:26 GMT  
		Size: 1.5 KB (1545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acc9f9ac9b27006e9d64b494581a0db18c4a42887de0db19c972e0bbc696400`  
		Last Modified: Mon, 26 Oct 2020 17:25:26 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0120f731f7d28eae0430bd6d7a3e579bdcee8f03f0c283c6fb90338ba5f6558`  
		Last Modified: Mon, 26 Oct 2020 17:25:26 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040f7b053d9753e7f7f28c49ddafc840415d9f8f85e6aee3095828e5168d5f4`  
		Last Modified: Mon, 26 Oct 2020 17:25:42 GMT  
		Size: 8.1 MB (8137888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599d792bd8774760855965a0257b798170d683054b6c043d9b3b1116fba33306`  
		Last Modified: Mon, 26 Oct 2020 17:25:26 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-3.6.20`

```console
$ docker pull percona@sha256:ac265b4ec8fed1766dc22260cdc52fdbdf2bedd529ab621abcf9b20f8717178d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6.20` - linux; amd64

```console
$ docker pull percona@sha256:021a211cedfb0683d3594d6309a19a1eb2f817435bb2e33d3b90d332963f6075
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.7 MB (157653105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638083383fc6ffa940c5a98ec2fbc9b2cce9a3244d00eaf266c00c07f0732121`
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
# Mon, 26 Oct 2020 17:24:28 GMT
ENV PSMDB_VERSION=3.6.20-9.0
# Mon, 26 Oct 2020 17:24:28 GMT
ENV OS_VER=el8
# Mon, 26 Oct 2020 17:24:28 GMT
ENV FULL_PERCONA_VERSION=3.6.20-9.0.el8
# Mon, 26 Oct 2020 17:24:28 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 26 Oct 2020 17:24:28 GMT
LABEL org.label-schema.schema-version=3.6.20-9.0
# Mon, 26 Oct 2020 17:24:29 GMT
LABEL org.opencontainers.image.version=3.6.20-9.0
# Mon, 26 Oct 2020 17:24:35 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Mon, 26 Oct 2020 17:24:50 GMT
RUN set -ex;     dnf install -y         dnf-utils         shadow-utils         curl         procps-ng         jq         oniguruma         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         dnf remove -y dnf-utils;         dnf clean all;         rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Mon, 26 Oct 2020 17:24:50 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 26 Oct 2020 17:24:51 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 26 Oct 2020 17:24:51 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 26 Oct 2020 17:24:53 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 26 Oct 2020 17:24:54 GMT
VOLUME [/data/db]
# Mon, 26 Oct 2020 17:24:54 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Mon, 26 Oct 2020 17:24:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Oct 2020 17:24:54 GMT
EXPOSE 27017
# Mon, 26 Oct 2020 17:24:54 GMT
USER 1001
# Mon, 26 Oct 2020 17:24:54 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fc827a496eb3c077fcef59e088800bc6f1cbe54185087987e552096bf8e49a`  
		Last Modified: Mon, 26 Oct 2020 17:25:29 GMT  
		Size: 18.5 MB (18498764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b1b93cdcac2da2df8793a9ded026af624430baa62e7e242d7715d5fbc2c376`  
		Last Modified: Mon, 26 Oct 2020 17:25:36 GMT  
		Size: 56.1 MB (56127594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb0bf69fb72ec24a3c6ea3918a369693b9f22048e24b09d6d605a5f59b2a1ee`  
		Last Modified: Mon, 26 Oct 2020 17:25:26 GMT  
		Size: 1.5 KB (1545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acc9f9ac9b27006e9d64b494581a0db18c4a42887de0db19c972e0bbc696400`  
		Last Modified: Mon, 26 Oct 2020 17:25:26 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0120f731f7d28eae0430bd6d7a3e579bdcee8f03f0c283c6fb90338ba5f6558`  
		Last Modified: Mon, 26 Oct 2020 17:25:26 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040f7b053d9753e7f7f28c49ddafc840415d9f8f85e6aee3095828e5168d5f4`  
		Last Modified: Mon, 26 Oct 2020 17:25:42 GMT  
		Size: 8.1 MB (8137888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599d792bd8774760855965a0257b798170d683054b6c043d9b3b1116fba33306`  
		Last Modified: Mon, 26 Oct 2020 17:25:26 GMT  
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

## `percona:psmdb-4.0.21`

**does not exist** (yet?)

## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:567bbc7872000933691b398569790072d9b5464f70c7ccd13ce88a5334785d55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:e204a0d86606576f921908435860b254896f6d0d3831692a4f4ea752cb1e7529
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.2 MB (169189396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cb7f52eddfa973547cc74232d4227e394ed8e3dd325aa8f614e6689af7755b7`
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
# Tue, 03 Nov 2020 23:21:09 GMT
ENV PSMDB_VERSION=4.2.10-11
# Tue, 03 Nov 2020 23:21:09 GMT
ENV OS_VER=el8
# Tue, 03 Nov 2020 23:21:09 GMT
ENV FULL_PERCONA_VERSION=4.2.10-11.el8
# Tue, 03 Nov 2020 23:21:09 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 03 Nov 2020 23:21:09 GMT
LABEL org.label-schema.schema-version=4.2.10-11
# Tue, 03 Nov 2020 23:21:09 GMT
LABEL org.opencontainers.image.version=4.2.10-11
# Tue, 03 Nov 2020 23:21:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Tue, 03 Nov 2020 23:21:34 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Tue, 03 Nov 2020 23:21:35 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 03 Nov 2020 23:21:35 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 03 Nov 2020 23:21:36 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 03 Nov 2020 23:21:36 GMT
ENV GOSU_VERSION=1.11
# Tue, 03 Nov 2020 23:21:38 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Tue, 03 Nov 2020 23:21:40 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 03 Nov 2020 23:21:40 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Tue, 03 Nov 2020 23:21:40 GMT
VOLUME [/data/db]
# Tue, 03 Nov 2020 23:21:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 03 Nov 2020 23:21:41 GMT
EXPOSE 27017
# Tue, 03 Nov 2020 23:21:41 GMT
USER 1001
# Tue, 03 Nov 2020 23:21:41 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da01c2fc3cfff16379ffd5555289af91cb20d6696f6c0cbe27cb99fd13895a81`  
		Last Modified: Tue, 03 Nov 2020 23:22:25 GMT  
		Size: 18.5 MB (18495331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec401bb7b362df6a450c0be33166d19dc7dba759c890a80a7c58ede17c268a3`  
		Last Modified: Tue, 03 Nov 2020 23:22:33 GMT  
		Size: 66.8 MB (66752765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b50cc6a3ac78b5540ea71e70e2637aeae688e5649b39b51abfd9eb9dbe74ff7`  
		Last Modified: Tue, 03 Nov 2020 23:22:22 GMT  
		Size: 1.5 KB (1543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b2e351bde6e945b711b5f4eac838ca2e5771c11f9f31914b0c33a3621b25de`  
		Last Modified: Tue, 03 Nov 2020 23:22:21 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda0dd0014df116890dcab7661b78904eef4046c92d423dcf328cde87bfc78be`  
		Last Modified: Tue, 03 Nov 2020 23:22:21 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66549f9f43f56db666e334fb84f963a8d0f670c697156aa7f5db03c97cdb8fcb`  
		Last Modified: Tue, 03 Nov 2020 23:22:22 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9532eede094afb7369f38132e57a1dba79f510a6cca66130f9c54aed77fecbc`  
		Last Modified: Tue, 03 Nov 2020 23:22:22 GMT  
		Size: 8.1 MB (8137891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a50901e060c07b462ea399e612384271eb73313a2b4273dc49c556bf707475`  
		Last Modified: Tue, 03 Nov 2020 23:22:21 GMT  
		Size: 4.5 KB (4543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `percona:psmdb-4.2.10`

```console
$ docker pull percona@sha256:567bbc7872000933691b398569790072d9b5464f70c7ccd13ce88a5334785d55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.2.10` - linux; amd64

```console
$ docker pull percona@sha256:e204a0d86606576f921908435860b254896f6d0d3831692a4f4ea752cb1e7529
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.2 MB (169189396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cb7f52eddfa973547cc74232d4227e394ed8e3dd325aa8f614e6689af7755b7`
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
# Tue, 03 Nov 2020 23:21:09 GMT
ENV PSMDB_VERSION=4.2.10-11
# Tue, 03 Nov 2020 23:21:09 GMT
ENV OS_VER=el8
# Tue, 03 Nov 2020 23:21:09 GMT
ENV FULL_PERCONA_VERSION=4.2.10-11.el8
# Tue, 03 Nov 2020 23:21:09 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 03 Nov 2020 23:21:09 GMT
LABEL org.label-schema.schema-version=4.2.10-11
# Tue, 03 Nov 2020 23:21:09 GMT
LABEL org.opencontainers.image.version=4.2.10-11
# Tue, 03 Nov 2020 23:21:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Tue, 03 Nov 2020 23:21:34 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Tue, 03 Nov 2020 23:21:35 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 03 Nov 2020 23:21:35 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 03 Nov 2020 23:21:36 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 03 Nov 2020 23:21:36 GMT
ENV GOSU_VERSION=1.11
# Tue, 03 Nov 2020 23:21:38 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Tue, 03 Nov 2020 23:21:40 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 03 Nov 2020 23:21:40 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Tue, 03 Nov 2020 23:21:40 GMT
VOLUME [/data/db]
# Tue, 03 Nov 2020 23:21:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 03 Nov 2020 23:21:41 GMT
EXPOSE 27017
# Tue, 03 Nov 2020 23:21:41 GMT
USER 1001
# Tue, 03 Nov 2020 23:21:41 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da01c2fc3cfff16379ffd5555289af91cb20d6696f6c0cbe27cb99fd13895a81`  
		Last Modified: Tue, 03 Nov 2020 23:22:25 GMT  
		Size: 18.5 MB (18495331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec401bb7b362df6a450c0be33166d19dc7dba759c890a80a7c58ede17c268a3`  
		Last Modified: Tue, 03 Nov 2020 23:22:33 GMT  
		Size: 66.8 MB (66752765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b50cc6a3ac78b5540ea71e70e2637aeae688e5649b39b51abfd9eb9dbe74ff7`  
		Last Modified: Tue, 03 Nov 2020 23:22:22 GMT  
		Size: 1.5 KB (1543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b2e351bde6e945b711b5f4eac838ca2e5771c11f9f31914b0c33a3621b25de`  
		Last Modified: Tue, 03 Nov 2020 23:22:21 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda0dd0014df116890dcab7661b78904eef4046c92d423dcf328cde87bfc78be`  
		Last Modified: Tue, 03 Nov 2020 23:22:21 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66549f9f43f56db666e334fb84f963a8d0f670c697156aa7f5db03c97cdb8fcb`  
		Last Modified: Tue, 03 Nov 2020 23:22:22 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9532eede094afb7369f38132e57a1dba79f510a6cca66130f9c54aed77fecbc`  
		Last Modified: Tue, 03 Nov 2020 23:22:22 GMT  
		Size: 8.1 MB (8137891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a50901e060c07b462ea399e612384271eb73313a2b4273dc49c556bf707475`  
		Last Modified: Tue, 03 Nov 2020 23:22:21 GMT  
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
