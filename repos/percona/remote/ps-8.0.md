## `percona:ps-8.0`

```console
$ docker pull percona@sha256:7f7c9884cf1a67ce3e181f2eb4e708c440d4d9c7402f9ad9e326ecda68e3e437
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-8.0` - linux; amd64

```console
$ docker pull percona@sha256:bae75430cb515663492a2065bf15490c3ba5f08132eddc70775ee2b4a8fd0aa4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.3 MB (383334811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f13778994e5b9087f796c00f48ec93c9b6543a8abd5541da3b67f6a517d710cf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 16 Jun 2023 00:20:10 GMT
ADD file:4d6795a06ab65ed16d9773d6062cfb26d1cc84e8d1d57a4ab57acc3ad355bc28 in / 
# Fri, 16 Jun 2023 00:20:11 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:44:39 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 16 Jun 2023 00:44:40 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Wed, 21 Jun 2023 19:27:21 GMT
ENV PS_VERSION=8.0.33-25.1
# Wed, 21 Jun 2023 19:27:21 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Wed, 21 Jun 2023 19:27:21 GMT
ENV OS_VER=el9
# Wed, 21 Jun 2023 19:27:21 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Wed, 21 Jun 2023 19:27:21 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Wed, 21 Jun 2023 19:27:21 GMT
ENV PS_REPO=testing
# Wed, 21 Jun 2023 19:27:25 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Wed, 21 Jun 2023 19:28:16 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Wed, 21 Jun 2023 19:28:20 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Wed, 21 Jun 2023 19:28:20 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 21 Jun 2023 19:28:20 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Wed, 21 Jun 2023 19:28:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 21 Jun 2023 19:28:20 GMT
USER mysql
# Wed, 21 Jun 2023 19:28:20 GMT
EXPOSE 3306 33060
# Wed, 21 Jun 2023 19:28:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bd3a74881334e44c59cd7aa126040b4e8f5429f27370e87c3bf0857becd84786`  
		Last Modified: Fri, 16 Jun 2023 00:21:29 GMT  
		Size: 88.0 MB (87963873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe174e5edf9341715af80f2f73266079ce90b84b1293a6e2878004eca2dae3e`  
		Last Modified: Fri, 16 Jun 2023 00:49:01 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b85468f85eabc42f48fa8556dab774d62e3eaf47800c3ddcdd3e2fd40084bb2`  
		Last Modified: Wed, 21 Jun 2023 19:29:05 GMT  
		Size: 7.3 MB (7330224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3209472199971fec4c70ef59a11e3aa6b804800c5b7a3da09b2c33001a5a4e1`  
		Last Modified: Wed, 21 Jun 2023 19:29:44 GMT  
		Size: 288.0 MB (288034823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865629cf7d8c2aefc7d9c8706f257543617cea8e9ac1580bad31971cf35a2488`  
		Last Modified: Wed, 21 Jun 2023 19:29:04 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e842c56807c8a7f125f608dcbdca957ba1c889440d94de6af25b45a5c3d5e4`  
		Last Modified: Wed, 21 Jun 2023 19:29:04 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
