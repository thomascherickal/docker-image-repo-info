## `percona:ps-8.0`

```console
$ docker pull percona@sha256:d9eed206e9a2aea60a33dfc37cab27af07f9b35ba16c7fa61f425e5abcabf8e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-8.0` - linux; amd64

```console
$ docker pull percona@sha256:2799c6b347cf13b52e5a1e6f247ebe6c65a7a8972666b4813c27dbe071c80952
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422677972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ed1e0ea9a2174109bea8ff281509a2e0a5e5a9d2e6dd15bf304db4b05c817e1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 14 Sep 2022 21:20:18 GMT
ADD file:e80b88eaaaff4337df2e280f39f05fa55901ffe34cce7c0e05597362c0e60f1d in / 
# Wed, 14 Sep 2022 21:20:18 GMT
CMD ["/bin/bash"]
# Wed, 14 Sep 2022 21:47:59 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 14 Sep 2022 21:47:59 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -c "Default Application User" mysql
# Wed, 14 Sep 2022 21:48:29 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql;     percona-release disable all;     percona-release enable ps-80 release
# Wed, 14 Sep 2022 21:48:29 GMT
ENV PS_VERSION=8.0.29-21.1
# Wed, 14 Sep 2022 21:48:29 GMT
ENV OS_VER=el8
# Wed, 14 Sep 2022 21:48:29 GMT
ENV FULL_PERCONA_VERSION=8.0.29-21.1.el8
# Wed, 14 Sep 2022 21:49:03 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Wed, 14 Sep 2022 21:49:05 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Wed, 14 Sep 2022 21:49:06 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 14 Sep 2022 21:49:06 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Wed, 14 Sep 2022 21:49:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Sep 2022 21:49:06 GMT
USER mysql
# Wed, 14 Sep 2022 21:49:06 GMT
EXPOSE 3306 33060
# Wed, 14 Sep 2022 21:49:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7cb069903b8a7a68536454971fb537ee41f021abcc75a62ee6b76efe61020d70`  
		Last Modified: Wed, 14 Sep 2022 21:21:09 GMT  
		Size: 86.0 MB (85955949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dfe4b2d7a2cea3c21c55bbd540b694bdfe604fdda838efc1d45628d12af519`  
		Last Modified: Wed, 14 Sep 2022 21:52:38 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3232bbde82b36072c97c787bd9dfa1a009aeb4d3ad24070fb0ba74daf087e251`  
		Last Modified: Wed, 14 Sep 2022 21:52:48 GMT  
		Size: 158.3 MB (158270286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e6a6f9b94897fcf89077977f0ef1425b0a1dcc60020af0e9c9628a969ce3a1`  
		Last Modified: Wed, 14 Sep 2022 21:53:05 GMT  
		Size: 178.4 MB (178446316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d4c7d536f771c8a180b20ba8539d8e7c8e07dde48954a42e10f74110cfe140`  
		Last Modified: Wed, 14 Sep 2022 21:52:38 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e00468757dc304a1139f45d0d4bddc133243c835e70fed562b532b1f4f1cd6`  
		Last Modified: Wed, 14 Sep 2022 21:52:38 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
