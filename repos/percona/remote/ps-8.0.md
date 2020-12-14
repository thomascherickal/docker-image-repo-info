## `percona:ps-8.0`

```console
$ docker pull percona@sha256:d5d76334aa84c239fde43a2d2331d9bc268acec1702632d1741037a80419dda3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:ps-8.0` - linux; amd64

```console
$ docker pull percona@sha256:5bbb24c3ff580b9feebf71f4a2df037fa26adacc8cd73b52ff5911fd89fa2b6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.5 MB (239482162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef86f7cd16d0a330e95d544ac8d2972013aeea59202bf620660b1330103584f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:48:03 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 08 Dec 2020 00:48:04 GMT
RUN groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 08 Dec 2020 00:48:12 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup -y ps80
# Mon, 14 Dec 2020 21:36:41 GMT
ENV PS_VERSION=8.0.22-13.1
# Mon, 14 Dec 2020 21:36:41 GMT
ENV OS_VER=el8
# Mon, 14 Dec 2020 21:36:41 GMT
ENV FULL_PERCONA_VERSION=8.0.22-13.1.el8
# Mon, 14 Dec 2020 21:37:14 GMT
RUN set -ex;     dnf install -y         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-tokudb-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         jemalloc         which         cracklib-dicts         policycoreutils;         dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Mon, 14 Dec 2020 21:37:15 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Mon, 14 Dec 2020 21:37:15 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Mon, 14 Dec 2020 21:37:16 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Mon, 14 Dec 2020 21:37:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Dec 2020 21:37:16 GMT
USER mysql
# Mon, 14 Dec 2020 21:37:16 GMT
EXPOSE 3306 33060
# Mon, 14 Dec 2020 21:37:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ce9644bc2779e06cc0a9ac9a86e9f4981ba7c6f0274fb87a2d59b1e9f47f44`  
		Last Modified: Tue, 08 Dec 2020 00:53:09 GMT  
		Size: 1.6 KB (1568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980739941cb96072c34a82314491f555b66b9440b93eed4ef3b9c4b35a451b62`  
		Last Modified: Tue, 08 Dec 2020 00:53:13 GMT  
		Size: 19.3 MB (19323541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a089ee89f6043a60f32e44e5405ba3fdc61a0dd8403bc5082f7b188f6091cc`  
		Last Modified: Mon, 14 Dec 2020 21:38:38 GMT  
		Size: 145.0 MB (144970871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b068859f838cf3d9907c77ae252f18ac268163439c0de7e44867d7a5e68164a`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aec5f76445c9fd06a1652fcbf8d4cb0ae7924d1560149e5972c39eb39f3cff`  
		Last Modified: Mon, 14 Dec 2020 21:38:13 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
