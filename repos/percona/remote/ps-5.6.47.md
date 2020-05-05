## `percona:ps-5.6.47`

```console
$ docker pull percona@sha256:3f5f47da029d71b2916a445bb69d37663e6c87fb5ed5938626773886ed6575d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-5.6.47` - linux; amd64

```console
$ docker pull percona@sha256:6b6443928425419101e7669708a3816c9c9427ff8e95b7b38598da2b2b562d68
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140090870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:471de329f78861ad4d68f73434e2a365ddf71e8105a27a767ac6b9dbf3085c77`
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
# Tue, 05 May 2020 21:41:20 GMT
ENV PERCONA_VERSION=5.6.47-rel87.0.1.el7
# Tue, 05 May 2020 21:41:56 GMT
RUN set -ex;     yum install -y         Percona-Server-server-56-${PERCONA_VERSION}         Percona-Server-tokudb-56-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Tue, 05 May 2020 21:41:57 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /etc/my.cnf.d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user|sql_mode)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user|sql_mode)/#&/' 	&& sed -i '/Make sure only root/,/fi/d' /usr/bin/ps_tokudb_admin 	&& echo "thp-setting=never" >> /etc/my.cnf 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& ln -s /etc/my.cnf.d /etc/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Tue, 05 May 2020 21:41:57 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 05 May 2020 21:41:57 GMT
COPY file:1d7c9d67c6f11e6632845ae6085c57582457d49c5e3d732f0b3bd3f40b8bf179 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:41:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:41:58 GMT
USER mysql
# Tue, 05 May 2020 21:41:58 GMT
EXPOSE 3306
# Tue, 05 May 2020 21:41:58 GMT
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
	-	`sha256:41e36abb65ce57419008701d1b729fee6bc44acdf6fb4461766a7c5a230df72f`  
		Last Modified: Tue, 05 May 2020 21:46:29 GMT  
		Size: 57.7 MB (57684537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a10198407188f3311699f81fc324f59efde57a1c1b20a7cc38064cbbab013c`  
		Last Modified: Tue, 05 May 2020 21:45:41 GMT  
		Size: 4.9 KB (4877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0847b6c89d46efe4c1d4e76db263163f92b559c7aa86f1644c2dcce0820cdb`  
		Last Modified: Tue, 05 May 2020 21:45:41 GMT  
		Size: 2.9 KB (2942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
