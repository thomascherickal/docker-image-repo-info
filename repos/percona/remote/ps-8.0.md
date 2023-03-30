## `percona:ps-8.0`

```console
$ docker pull percona@sha256:f4b3ff162ce29bd4552506222be6c948f1011997be8b444cca939839d79aa0f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-8.0` - linux; amd64

```console
$ docker pull percona@sha256:8fe7ab8963eec636131624cc4cf2f51fa0f46b35c0e118efcbea7727a78e86ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.3 MB (345344383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f400ad4fb9ef4bd1cc7d5a324a42232cc2a61b6b1f1f3bfcf65fd77d01b5a517`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 29 Mar 2023 00:21:07 GMT
ADD file:bbb779b34d70fa61dfa3a32a574754396befa0d010178d789b24ef2f7e54038a in / 
# Wed, 29 Mar 2023 00:21:07 GMT
CMD ["/bin/bash"]
# Thu, 30 Mar 2023 05:41:05 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Mar 2023 05:41:06 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -m -c "Default Application User" mysql
# Thu, 30 Mar 2023 05:41:06 GMT
ENV PS_VERSION=8.0.32-24.1
# Thu, 30 Mar 2023 05:41:06 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1
# Thu, 30 Mar 2023 05:41:06 GMT
ENV OS_VER=el9
# Thu, 30 Mar 2023 05:41:06 GMT
ENV FULL_PERCONA_VERSION=8.0.32-24.1.el9
# Thu, 30 Mar 2023 05:41:07 GMT
ENV FULL_MYSQL_SHELL_VERSION=8.0.32-1.el9
# Thu, 30 Mar 2023 05:41:07 GMT
ENV PS_REPO=testing
# Thu, 30 Mar 2023 05:41:10 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release enable ps-80 ${PS_REPO};     percona-release enable mysql-shell ${PS_REPO}
# Thu, 30 Mar 2023 05:41:49 GMT
RUN set -ex;     dnf -y install epel-release;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION}         percona-icu-data-files-${FULL_PERCONA_VERSION}         percona-mysql-shell-${FULL_MYSQL_SHELL_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Thu, 30 Mar 2023 05:41:52 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 30 Mar 2023 05:41:52 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 30 Mar 2023 05:41:52 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Thu, 30 Mar 2023 05:41:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 05:41:52 GMT
USER mysql
# Thu, 30 Mar 2023 05:41:52 GMT
EXPOSE 3306 33060
# Thu, 30 Mar 2023 05:41:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6ce6d5bf0ebdb5c3e381cb7bdfa874f93abbdca053dac29f85511fd690b132d8`  
		Last Modified: Wed, 29 Mar 2023 00:22:17 GMT  
		Size: 88.6 MB (88598609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca3b3b72db5fdba6c56997929eb101c4299695ee88e5c9159983315630fb101`  
		Last Modified: Thu, 30 Mar 2023 05:42:31 GMT  
		Size: 1.6 KB (1633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6654597cd407bfb00c3f4b6e54b55c883193a85dfd3e1303b1bf1d907c9c1aae`  
		Last Modified: Thu, 30 Mar 2023 05:42:32 GMT  
		Size: 7.4 MB (7373470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5595155e5bcf9456b0d077889f5135d51722c6ded1eb3124e7b2357b044c837f`  
		Last Modified: Thu, 30 Mar 2023 05:43:03 GMT  
		Size: 249.4 MB (249366417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39aafe0fbc05b348de3e0e09dc38063855b87a4fbf228ccd414261a3889f7f7`  
		Last Modified: Thu, 30 Mar 2023 05:42:31 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982995ce1e5765e9a107bf965a300474038fd4d90a55e28c98163d4759bccac1`  
		Last Modified: Thu, 30 Mar 2023 05:42:31 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
