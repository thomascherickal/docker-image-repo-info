## `percona:8-centos`

```console
$ docker pull percona@sha256:2181c1e57b3047853052fcf4f03c83ed28a3afefc07f9d9f262b56a86d4ffc37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:8-centos` - linux; amd64

```console
$ docker pull percona@sha256:7f6110d07dd03f94965f3dd6dc8e3257b6e1348c2e9d0f40ee7eb307ee7e5bb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **434.0 MB (434032468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e96381fe0ab15c3e24dfbaf656146a85d64246d941e7968fa1abfd0558cb9ae5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Nov 2022 07:52:18 GMT
ADD file:95e25b6cc4a22c4ecb537bc949b3636ae408264d293c1c32a3ad180e54f80ae9 in / 
# Wed, 16 Nov 2022 07:52:19 GMT
CMD ["/bin/bash"]
# Wed, 16 Nov 2022 08:52:25 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 16 Nov 2022 08:52:26 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -c "Default Application User" mysql
# Wed, 16 Nov 2022 08:52:58 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql;     percona-release disable all;     percona-release enable ps-80 release
# Wed, 16 Nov 2022 08:52:58 GMT
ENV PS_VERSION=8.0.29-21.1
# Wed, 16 Nov 2022 08:52:59 GMT
ENV OS_VER=el8
# Wed, 16 Nov 2022 08:52:59 GMT
ENV FULL_PERCONA_VERSION=8.0.29-21.1.el8
# Wed, 16 Nov 2022 08:53:34 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Wed, 16 Nov 2022 08:53:37 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Wed, 16 Nov 2022 08:53:37 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 16 Nov 2022 08:53:37 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Wed, 16 Nov 2022 08:53:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 16 Nov 2022 08:53:37 GMT
USER mysql
# Wed, 16 Nov 2022 08:53:37 GMT
EXPOSE 3306 33060
# Wed, 16 Nov 2022 08:53:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:df958f680f30541ef9f464f2f49bd4366e5904477b5ca521a78a4c68db2aa858`  
		Last Modified: Wed, 16 Nov 2022 07:53:09 GMT  
		Size: 87.4 MB (87435022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e327b8265c6c1799c6e2038dbd5ab5bc6a74da988fb2dc5b23e47d542f3b92`  
		Last Modified: Wed, 16 Nov 2022 08:57:29 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68586949955d3a69e69dcec7ab66ab5e24e0d16a9d0f66aa2d04f42fc6bfd73c`  
		Last Modified: Wed, 16 Nov 2022 08:57:38 GMT  
		Size: 168.1 MB (168147368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab8c2af6d8fd23c3967a35365510f0362621f759ab3da0abc07620f593f39c0`  
		Last Modified: Wed, 16 Nov 2022 08:57:55 GMT  
		Size: 178.4 MB (178444654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a53d133a1db29681f0fc4ae29c62990ab07993046b3450753c2281d2613ff8e`  
		Last Modified: Wed, 16 Nov 2022 08:57:29 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21156c61ec42993930fd1150ce6d5d24b47fd8d91b9ecd75089b240c16642b7c`  
		Last Modified: Wed, 16 Nov 2022 08:57:29 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
