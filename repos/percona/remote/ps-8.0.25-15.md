## `percona:ps-8.0.25-15`

```console
$ docker pull percona@sha256:33fc5903e824530a8a987a926dea1ab73f2390749efcf5146bf2ff08d50c822e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-8.0.25-15` - linux; amd64

```console
$ docker pull percona@sha256:9a22dfee411523126a0bfabddc327640cfb0ab3dc3fe340c9a8b1bbef3cbccef
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.0 MB (265991382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:349779085ece8ff91a458638558ad82c13813151d5bab5de0131af3c8cad04af`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:04 GMT
ADD file:805cb5e15fb6e0bb0326ca33fd2942e068863ce2a8491bb71522c652f31fb466 in / 
# Wed, 15 Sep 2021 18:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 18:20:05 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 18:56:15 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 15 Sep 2021 18:56:15 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Wed, 15 Sep 2021 18:56:41 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Wed, 15 Sep 2021 18:56:41 GMT
ENV PS_VERSION=8.0.25-15.1
# Wed, 15 Sep 2021 18:56:41 GMT
ENV OS_VER=el8
# Wed, 15 Sep 2021 18:56:41 GMT
ENV FULL_PERCONA_VERSION=8.0.25-15.1.el8
# Wed, 15 Sep 2021 18:57:12 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Wed, 15 Sep 2021 18:57:14 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Wed, 15 Sep 2021 18:57:14 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 15 Sep 2021 18:57:14 GMT
COPY file:fcc7e1ba857456cd0be5e7e73c551fe742d4b08d93a5cc538710f4731b28e602 in /docker-entrypoint.sh 
# Wed, 15 Sep 2021 18:57:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 15 Sep 2021 18:57:15 GMT
USER mysql
# Wed, 15 Sep 2021 18:57:15 GMT
EXPOSE 3306 33060
# Wed, 15 Sep 2021 18:57:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8422329e860c8ce0b890dec827973631ba413cfa8f0923e3766871a3c60e9485`  
		Last Modified: Wed, 15 Sep 2021 19:04:05 GMT  
		Size: 1.6 KB (1566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6f5e6e9cdbcb3b0282c5330869314057d22860b84c26b715fc679ad6a53a46`  
		Last Modified: Wed, 15 Sep 2021 19:04:11 GMT  
		Size: 29.0 MB (29015949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d8096664166bea54c265b33f0ab234b73fb37010aeab9f0caaf46f185b1beb`  
		Last Modified: Wed, 15 Sep 2021 19:04:28 GMT  
		Size: 153.5 MB (153451531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5f720509903bfbcef90d9ecf798dc53af1c4743d420f3928d707b41a3fad39`  
		Last Modified: Wed, 15 Sep 2021 19:04:06 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf49cee1b40237bf0193b90f27aa45f868bd139f1550433207ea44c15f32f20`  
		Last Modified: Wed, 15 Sep 2021 19:04:05 GMT  
		Size: 3.1 KB (3089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
