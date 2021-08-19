## `percona:ps-5.7.35`

```console
$ docker pull percona@sha256:b08af5453f8d9145053c126a7b15a43fff6be6213f2c07e4edf10f5db7fa97b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-5.7.35` - linux; amd64

```console
$ docker pull percona@sha256:6f8fe07a8610015cff7e054e16434df635c5d220384d3d57be8b50fef8500872
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.5 MB (244471863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c125f3d82264fb16effbda273540e116b732abcbb13022da55780d09dd6d0bcb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Sat, 06 Mar 2021 01:08:18 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 06 Mar 2021 01:09:11 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 999 mysql;     useradd -u 999 -r -g 999 -s /sbin/nologin         -c "Default Application User" mysql
# Thu, 19 Aug 2021 00:25:38 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql
# Thu, 19 Aug 2021 00:25:38 GMT
ENV PS_VERSION=5.7.35-38.1
# Thu, 19 Aug 2021 00:25:38 GMT
ENV OS_VER=el8
# Thu, 19 Aug 2021 00:25:38 GMT
ENV FULL_PERCONA_VERSION=5.7.35-38.1.el8
# Thu, 19 Aug 2021 00:26:06 GMT
RUN set -ex;     dnf install -y         dnf-utils         jemalloc         cracklib-dicts         which;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         selinux-policy             | xargs curl -Lf -o /tmp/selinux-policy.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm --nodeps;     rm -rf /tmp/policycoreutils.rpm /tmp/selinux-policy.rpm;         dnf install -y         Percona-Server-server-57-${FULL_PERCONA_VERSION}         Percona-Server-devel-57-${FULL_PERCONA_VERSION}         Percona-Server-tokudb-57-${FULL_PERCONA_VERSION}         Percona-Server-rocksdb-57-${FULL_PERCONA_VERSION};     dnf remove -y dnf-utils;     dnf clean all;     rm -rf /var/cache/dnf /var/lib/mysql
# Thu, 19 Aug 2021 00:26:07 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	ln -s /etc/my.cnf.d /etc/mysql; 	chown -R mysql:root /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d; 	chmod -R ug+rwX /etc/percona-server.cnf /etc/percona-server.conf.d /etc/my.cnf.d
# Thu, 19 Aug 2021 00:26:07 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 19 Aug 2021 00:26:08 GMT
COPY file:905f699d79b77ffbf7039a84326c28f490b5fbb94dacddae8e03ff2d2ee34360 in /docker-entrypoint.sh 
# Thu, 19 Aug 2021 00:26:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Aug 2021 00:26:08 GMT
USER mysql
# Thu, 19 Aug 2021 00:26:08 GMT
EXPOSE 3306
# Thu, 19 Aug 2021 00:26:08 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c93caa609cd1653cc648c7d0c921200ae458bce4299b00a2a256dfec67d2843`  
		Last Modified: Sat, 06 Mar 2021 01:15:28 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc7733b933f8551d0271a2a0f732a29d988d535bae1ff8f0a14fb88bcc5a39`  
		Last Modified: Thu, 19 Aug 2021 00:27:07 GMT  
		Size: 42.3 MB (42302018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd65ccf84b4f3d9e43c3c96a7a29fa652c2898bdd8e3292c70f6e4d71a0096d0`  
		Last Modified: Thu, 19 Aug 2021 00:27:21 GMT  
		Size: 127.0 MB (126981796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d134bfe2a3769ca9a87d326d800a110d1fc9a5a3cdc446dbffea407387db7c84`  
		Last Modified: Thu, 19 Aug 2021 00:27:03 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4417cb1a92e2c92178b3814d98f3e7f80399d1dd202d7415143745f919dfdae`  
		Last Modified: Thu, 19 Aug 2021 00:27:03 GMT  
		Size: 3.1 KB (3064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
