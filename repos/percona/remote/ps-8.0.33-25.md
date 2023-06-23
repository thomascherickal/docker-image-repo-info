## `percona:ps-8.0.33-25`

```console
$ docker pull percona@sha256:6f60b35e5f518e0dd46237895a4dba83b8e3e76328197299ea972600caf7d7ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-8.0.33-25` - linux; amd64

```console
$ docker pull percona@sha256:8babb7b44f39864e7fc11374d93d3f852d2d1ec9a15a6a0f1cda14b020958419
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.3 MB (383335198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ce2b3c131386b54b83e7022b5128dece4a3f50b6fe41733f00a72a98aa69f1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Jun 2023 00:23:56 GMT
ADD file:a5dc577a850ef41488490ddc01c977760aaa7fc688e77923c15be6c9f12674af in / 
# Fri, 23 Jun 2023 00:23:56 GMT
CMD ["/bin/bash"]
# Fri, 23 Jun 2023 00:41:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 23 Jun 2023 00:41:13 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_VERSION=8.0.33-25.1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1
# Fri, 23 Jun 2023 00:41:13 GMT
ENV OS_VER=el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_PERCONA_VERSION=8.0.33-25.1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.33-1.el9
# Fri, 23 Jun 2023 00:41:13 GMT
ENV PS_REPO=testing
# Fri, 23 Jun 2023 00:41:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Fri, 23 Jun 2023 00:42:07 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Fri, 23 Jun 2023 00:42:11 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Fri, 23 Jun 2023 00:42:12 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Fri, 23 Jun 2023 00:42:12 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Fri, 23 Jun 2023 00:42:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jun 2023 00:42:12 GMT
USER mysql
# Fri, 23 Jun 2023 00:42:12 GMT
EXPOSE 3306 33060
# Fri, 23 Jun 2023 00:42:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:fd5367e01a11dce2026f7954fed19fca5829ed8a5816767ce069cda19e8b880e`  
		Last Modified: Fri, 23 Jun 2023 00:25:15 GMT  
		Size: 88.0 MB (87962811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bce2f5c31c83f94f136286aa47a15096ef1fe91e17aa8a4565af115549f15f`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.6 KB (1636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57914938b6feea2ca15088c32824fe36d315d524ba6143be76f4d1a1338b74a2`  
		Last Modified: Fri, 23 Jun 2023 00:42:58 GMT  
		Size: 7.3 MB (7326811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d313ab89a3ab23608351b5f778095610efdbc000dc174d4881221ce2ba4309`  
		Last Modified: Fri, 23 Jun 2023 00:43:37 GMT  
		Size: 288.0 MB (288039685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59e5e66ea115bc515f1cbadaf38bc07a1bfac33017e96ad729ea3443492fb2c`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0115118d13b5c42a3029767175c1727983b42050a09862aa94a51298d945e62`  
		Last Modified: Fri, 23 Jun 2023 00:42:57 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
