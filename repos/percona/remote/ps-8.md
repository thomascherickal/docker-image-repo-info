## `percona:ps-8`

```console
$ docker pull percona@sha256:152a753966cc97d970334a6bbee77eb8bbc8ff175e2a9e7989427d024acd785b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-8` - linux; amd64

```console
$ docker pull percona@sha256:8a5fc13dae6518cbd3d8453cd29cd88932fabd84b8f0a15257b7fbd2ba1a9266
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.9 MB (384890197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9ff8bc01f73ca6a94dd334c3c32d715c560e846deb32c8bbfeb88e2747cc35`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Feb 2022 02:07:03 GMT
ADD file:22d2bf309f3ff2ffd43267be3876b00e3dab021977498a24e8fa6410730dffe1 in / 
# Fri, 25 Feb 2022 02:07:04 GMT
CMD ["/bin/bash"]
# Thu, 03 Mar 2022 07:13:37 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 03 Mar 2022 07:13:38 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -c "Default Application User" mysql
# Thu, 03 Mar 2022 07:14:31 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql;     percona-release disable all;     percona-release enable ps-80 release
# Thu, 03 Mar 2022 07:14:31 GMT
ENV PS_VERSION=8.0.27-18.1
# Thu, 03 Mar 2022 07:14:31 GMT
ENV OS_VER=el8
# Thu, 03 Mar 2022 07:14:32 GMT
ENV FULL_PERCONA_VERSION=8.0.27-18.1.el8
# Thu, 03 Mar 2022 07:15:08 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Thu, 03 Mar 2022 07:15:10 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 03 Mar 2022 07:15:10 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 03 Mar 2022 07:15:10 GMT
COPY file:fcc7e1ba857456cd0be5e7e73c551fe742d4b08d93a5cc538710f4731b28e602 in /docker-entrypoint.sh 
# Thu, 03 Mar 2022 07:15:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 03 Mar 2022 07:15:10 GMT
USER mysql
# Thu, 03 Mar 2022 07:15:10 GMT
EXPOSE 3306 33060
# Thu, 03 Mar 2022 07:15:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7ab19aacdb2faec097aea292a4f3191d996d24aafdc2cf79d4673237a48fe828`  
		Last Modified: Fri, 25 Feb 2022 02:08:16 GMT  
		Size: 87.3 MB (87254130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b1f98322dcf7dbc9e7195563de4148b12e05282568398d5685fcec75a52545`  
		Last Modified: Thu, 03 Mar 2022 07:16:06 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ce0fad3cf388354482043e77824557fc32dcbe10aa6691725586982fcd794a`  
		Last Modified: Thu, 03 Mar 2022 07:16:15 GMT  
		Size: 135.3 MB (135338453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6d947328dbc4cd0eb34da6fd2f544d0fad57f37b0f3f5b3d9993b3505f6192`  
		Last Modified: Thu, 03 Mar 2022 07:16:34 GMT  
		Size: 162.3 MB (162292187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96acfec8c7604b9001eeac4cb0e514476b94c405274f198cc89447e2699dd092`  
		Last Modified: Thu, 03 Mar 2022 07:16:06 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83f430e0956d74935adc5668a698ebefd83ae7d3b5a45cfebe5a74172100400`  
		Last Modified: Thu, 03 Mar 2022 07:16:06 GMT  
		Size: 3.1 KB (3089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
