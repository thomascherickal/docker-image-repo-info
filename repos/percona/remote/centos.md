## `percona:centos`

```console
$ docker pull percona@sha256:c6cec5f9c14edc620a6b12fbba50a3a8dffa21fc7724c37503044432c904b482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:centos` - linux; amd64

```console
$ docker pull percona@sha256:a73b5048c98576f126077b4ac202a16caf66abebe08b330615e46eac6f3990e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422738287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef9ed4d199cd1798ea6627a94cc29fc7580824bf0cf5e39f9132dcee8b5dc50`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:19:29 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Sat, 16 Sep 2023 03:20:04 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Sat, 16 Sep 2023 03:20:05 GMT
ENV PS_VERSION=5.7.39-42.1
# Sat, 16 Sep 2023 03:20:05 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:20:05 GMT
ENV FULL_PERCONA_VERSION=5.7.39-42.1.el8
# Sat, 16 Sep 2023 03:20:44 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Sat, 16 Sep 2023 03:20:45 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Sat, 16 Sep 2023 03:20:45 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Sat, 16 Sep 2023 03:20:45 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Sat, 16 Sep 2023 03:20:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Sep 2023 03:20:46 GMT
USER mysql
# Sat, 16 Sep 2023 03:20:46 GMT
EXPOSE 3306
# Sat, 16 Sep 2023 03:20:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f444e97db0bf5d50f5015a158a00bd5e453060943342f50cd305119e04ecc3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f512ea8d3aec4fe796c01a42c138a1865db0af5bbb181535f7b815db30908aa8`  
		Last Modified: Sat, 16 Sep 2023 03:27:23 GMT  
		Size: 196.3 MB (196271669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5017199f5cf25acfe2e4bf52f8ad3b297c2299ab04b85ddd2f2390bb12d13bb3`  
		Last Modified: Sat, 16 Sep 2023 03:27:21 GMT  
		Size: 137.5 MB (137541712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b594fad71442b6e1ab26f111cacaec4f79a1b00589d5a9e795a0b797e8b36a82`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b7a9503470801e82fdbfdd3b7346e4301ac0e879acd895b1281b7e039ffa3f`  
		Last Modified: Sat, 16 Sep 2023 03:27:03 GMT  
		Size: 3.1 KB (3062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
