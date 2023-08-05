## `percona:ps-5.7.39`

```console
$ docker pull percona@sha256:917e909741490967eb1dcddaf4ae532591553af1d9d899f838a13a2451e13104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-5.7.39` - linux; amd64

```console
$ docker pull percona@sha256:7a227334ec43908ce406b2008cd5bd0ac404a89943e79b5f18857fb19e22c0e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.0 MB (419019729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600b9ba8d1577af9fa44e0765ca47fc45ffb6b41b52198fbeaa782fd841d9ea2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:37:14 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 05 Aug 2023 02:37:47 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 05 Aug 2023 02:37:48 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 05 Aug 2023 02:37:48 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:37:48 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 05 Aug 2023 02:38:24 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 05 Aug 2023 02:38:26 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 05 Aug 2023 02:38:26 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 05 Aug 2023 02:38:26 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 05 Aug 2023 02:38:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Aug 2023 02:38:26 GMT
USER mysql
# Sat, 05 Aug 2023 02:38:26 GMT
EXPOSE 3306
# Sat, 05 Aug 2023 02:38:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c336c62cff80b45ee85a0fa59f487562fb97a60b6a378466408a5339184788`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246478ec69e60b803e615bd1822bbc541da434fc39e827e4b729e66087d6d4f2`  
		Last Modified: Sat, 05 Aug 2023 02:44:27 GMT  
		Size: 192.6 MB (192560961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128fd83d981eaadfa0f79125eda4a3644b513d6b30fb18221054437407088974`  
		Last Modified: Sat, 05 Aug 2023 02:44:33 GMT  
		Size: 137.5 MB (137531359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e43ed1f0be0a87de5bf18ece0d8c06c0102e487c244cd8a5a2a0fd21e7274a8`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b658c06491156c996cd6d918fb83f6d134df292838612393a3333d154d653d5`  
		Last Modified: Sat, 05 Aug 2023 02:44:16 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
