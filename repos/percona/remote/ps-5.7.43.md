## `percona:ps-5.7.43`

```console
$ docker pull percona@sha256:12af58903c65ade02145fef87dc9444cc8f7b61bf2e97b7daeee82dfcae29f65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-5.7.43` - linux; amd64

```console
$ docker pull percona@sha256:a55696457b0d3b2364b207444bf240b30cf2f8a5b3fde94f09654749fdbcf021
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **445.1 MB (445094994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ef8d2d22b330787d164aa7c20a2199db7682724eee4f7bf6e8ec4643d6fae62`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:23:06 GMT
ADD file:56e00fc237c2b28dde03c72a85001f865f02c455f532215409ee621993dcfe98 in / 
# Wed, 06 Dec 2023 19:23:07 GMT
CMD ["/bin/bash"]
# Wed, 06 Dec 2023 19:50:10 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 06 Dec 2023 19:50:11 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Wed, 06 Dec 2023 19:50:51 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Wed, 06 Dec 2023 19:50:52 GMT
ENV PS_VERSION=5.7.43-47.1
# Wed, 06 Dec 2023 19:50:52 GMT
ENV OS_VER=el8
# Wed, 06 Dec 2023 19:50:52 GMT
ENV FULL_PERCONA_VERSION=5.7.43-47.1.el8
# Wed, 06 Dec 2023 19:51:34 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Wed, 06 Dec 2023 19:51:36 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Wed, 06 Dec 2023 19:51:36 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 06 Dec 2023 19:51:36 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Wed, 06 Dec 2023 19:51:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 06 Dec 2023 19:51:36 GMT
USER mysql
# Wed, 06 Dec 2023 19:51:36 GMT
EXPOSE 3306
# Wed, 06 Dec 2023 19:51:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f1712686323e0a6cedaa7c814b922f2a093bf3a9181c622641857175f4d864e`  
		Last Modified: Wed, 06 Dec 2023 19:24:12 GMT  
		Size: 95.5 MB (95493114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64f7cb30340b0f5354a06d984c662dbc624e20c0a5207012f61807eb08aca81`  
		Last Modified: Wed, 06 Dec 2023 19:57:05 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ea107b04449e7d6c243306dc049e94b38360f675f2bce822111294793fe8e5`  
		Last Modified: Wed, 06 Dec 2023 19:57:16 GMT  
		Size: 210.9 MB (210868521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066a819ce0bc075b7762b268173abfa1812203e39baaac6dc091f9585ebfbccf`  
		Last Modified: Wed, 06 Dec 2023 19:57:23 GMT  
		Size: 138.7 MB (138727691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932039c62e520ae261dd7f9cbd1f4d4e38bf9b94146f97c5594c005871865d04`  
		Last Modified: Wed, 06 Dec 2023 19:57:05 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793cd0cfaa0abbf0e47fc74dc8bff50de98940b4eab401016ef43a3eaf74a522`  
		Last Modified: Wed, 06 Dec 2023 19:57:05 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
