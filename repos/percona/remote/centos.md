## `percona:centos`

```console
$ docker pull percona@sha256:617b6c0625293c53757a43d43c942176c761bb4010496792b40358e6ef77fde9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:centos` - linux; amd64

```console
$ docker pull percona@sha256:6e926ef0e4d61cef91c1e909fecd7240d7b65147471939fb7caf570aad9feb2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **425.8 MB (425751675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb655b90660ab1e12cab46856bf2d3615584d5b5d1287d5bdb8780b50e332bdd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 12 Oct 2023 21:28:19 GMT
ADD file:08ccec25d0d1459d4c27b2b0354bb526203faac57f1570a94b91c0d83e7474db in / 
# Thu, 12 Oct 2023 21:28:20 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 22:22:31 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 12 Oct 2023 22:22:32 GMT
RUN set -ex;     groupdel ssh_keys;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Thu, 12 Oct 2023 22:23:09 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Thu, 12 Oct 2023 22:23:10 GMT
ENV PS_VERSION=5.7.43-47.1
# Thu, 12 Oct 2023 22:23:10 GMT
ENV OS_VER=el8
# Thu, 12 Oct 2023 22:23:10 GMT
ENV FULL_PERCONA_VERSION=5.7.43-47.1.el8
# Thu, 12 Oct 2023 22:23:50 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         tzdata         jemalloc         which         cracklib-dicts         policycoreutils;         dnf -y install         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Thu, 12 Oct 2023 22:23:52 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 12 Oct 2023 22:23:52 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 12 Oct 2023 22:23:52 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 12 Oct 2023 22:23:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 12 Oct 2023 22:23:52 GMT
USER mysql
# Thu, 12 Oct 2023 22:23:53 GMT
EXPOSE 3306
# Thu, 12 Oct 2023 22:23:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:eeccb7e6dc78cf3d674adcfebd1e8ff22148cf87ec3d731d3cd73eff435f6d9f`  
		Last Modified: Thu, 12 Oct 2023 21:29:47 GMT  
		Size: 88.0 MB (88009290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872779aafb948f3169e8540be1b8447f5f88bd16eede9a7d9437817d434033a7`  
		Last Modified: Thu, 12 Oct 2023 22:29:30 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa41e0ef46795250c0dd5ed35aa741dc7db6830af4b75bb53c1f953c762ca7b9`  
		Last Modified: Thu, 12 Oct 2023 22:29:43 GMT  
		Size: 200.1 MB (200052698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d507677b32d02fa348d1b5b95711f687daad7e0d9be98fee55057397c07d50b`  
		Last Modified: Thu, 12 Oct 2023 22:29:48 GMT  
		Size: 137.7 MB (137684021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500c272969405fcecac5fa26f75abef9bd200ad6fa0bce23c691b7dd479aa209`  
		Last Modified: Thu, 12 Oct 2023 22:29:30 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ccb4b2ba89126286f19dff20ec6f953e190d2fd4e59540e09359dd097acfdd`  
		Last Modified: Thu, 12 Oct 2023 22:29:30 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
