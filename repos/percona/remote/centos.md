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
