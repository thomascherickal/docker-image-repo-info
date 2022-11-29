## `percona:ps-8`

```console
$ docker pull percona@sha256:a1e2fd2efa4140bbe10fcfd8e4625c60fc620a38d9f9c3e8a771c54788ef099b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-8` - linux; amd64

```console
$ docker pull percona@sha256:1f39fd6f2dd51b70689bf1e7fa858a112abdf91d9fcf72286b0e951bf6ed80a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **435.2 MB (435178169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d7ea08792fb056df4a15a3927d89c82f6707ebecc41665f878184b87ebc2743`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Nov 2022 19:20:47 GMT
ADD file:0b5cd2f93e1c6f939d535c707f7dda5d950091382d18cdd7cf32ded784e057fc in / 
# Tue, 29 Nov 2022 19:20:48 GMT
CMD ["/bin/bash"]
# Tue, 29 Nov 2022 19:51:48 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 29 Nov 2022 19:51:49 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -c "Default Application User" mysql
# Tue, 29 Nov 2022 19:52:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql;     percona-release disable all;     percona-release enable ps-80 release
# Tue, 29 Nov 2022 19:52:20 GMT
ENV PS_VERSION=8.0.29-21.1
# Tue, 29 Nov 2022 19:52:20 GMT
ENV OS_VER=el8
# Tue, 29 Nov 2022 19:52:20 GMT
ENV FULL_PERCONA_VERSION=8.0.29-21.1.el8
# Tue, 29 Nov 2022 19:52:54 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Tue, 29 Nov 2022 19:52:57 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Tue, 29 Nov 2022 19:52:57 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Tue, 29 Nov 2022 19:52:57 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Tue, 29 Nov 2022 19:52:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 29 Nov 2022 19:52:57 GMT
USER mysql
# Tue, 29 Nov 2022 19:52:57 GMT
EXPOSE 3306 33060
# Tue, 29 Nov 2022 19:52:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d0409ace7ea3bb98342dc30153bf50a92eeb0872d0474ef4fb0eabf9aba2390c`  
		Last Modified: Tue, 29 Nov 2022 19:22:26 GMT  
		Size: 87.4 MB (87437780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c655454d4eedbc3848b716d3742c8668c38127f34622a8a5228edea0c17ad04`  
		Last Modified: Tue, 29 Nov 2022 19:56:39 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743409f6465f83f993a340b279dfa5eff74a0f721cb1fb4ea96afd3960376b5a`  
		Last Modified: Tue, 29 Nov 2022 19:56:49 GMT  
		Size: 169.4 MB (169362351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82694018381e3b69a0a6c27a8998a9a6bc164fd362eafaedc8167e4730e678b7`  
		Last Modified: Tue, 29 Nov 2022 19:57:05 GMT  
		Size: 178.4 MB (178372616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1f2137a0b3a94a3579832e7685b20f9c5f460daac42bd6d262cc8150d5e30a`  
		Last Modified: Tue, 29 Nov 2022 19:56:39 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144698dc97f9347b72f6c68c59d5836e6770a646e3c0635a5ddf8f77664b32aa`  
		Last Modified: Tue, 29 Nov 2022 19:56:38 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
