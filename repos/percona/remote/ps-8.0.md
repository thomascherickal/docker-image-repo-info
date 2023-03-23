## `percona:ps-8.0`

```console
$ docker pull percona@sha256:1b4414376c0d9aafe5b621bd139f8d4452562f00dbb3a5393c3f04dbe6d042d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:ps-8.0` - linux; amd64

```console
$ docker pull percona@sha256:42c91a15a436e2ab2feb0332c26a46a19ca896f3a81cb417b481931e8a36e554
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **444.1 MB (444147257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:162a782e16231d7f5640bc0ef51deab9f52cc8c5528e399543c2222b3077b9ae`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 22 Mar 2023 23:55:09 GMT
ADD file:9545a60b93a26aad3efb7cb70c1d2099f15bf3adf38467dc56f286ff438b89b2 in / 
# Wed, 22 Mar 2023 23:55:10 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:20:39 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 23 Mar 2023 00:20:40 GMT
RUN set -ex;     groupdel input;     userdel systemd-coredump;     groupadd -g 1001 mysql;     useradd -u 1001 -r -g 1001 -s /sbin/nologin         -c "Default Application User" mysql
# Thu, 23 Mar 2023 00:21:12 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     dnf -y module disable mysql;     percona-release disable all;     percona-release enable ps-80 release
# Thu, 23 Mar 2023 00:21:12 GMT
ENV PS_VERSION=8.0.29-21.1
# Thu, 23 Mar 2023 00:21:12 GMT
ENV OS_VER=el8
# Thu, 23 Mar 2023 00:21:12 GMT
ENV FULL_PERCONA_VERSION=8.0.29-21.1.el8
# Thu, 23 Mar 2023 00:21:47 GMT
RUN set -ex;     rpm -e --nodeps tzdata;     dnf -y install         hostname         tzdata         jemalloc         which         cracklib-dicts         tar         policycoreutils;         dnf -y install         percona-server-server-${FULL_PERCONA_VERSION}         percona-server-devel-${FULL_PERCONA_VERSION}         percona-server-rocksdb-${FULL_PERCONA_VERSION};     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /var/lib/mysql
# Thu, 23 Mar 2023 00:21:49 GMT
RUN set -ex;     /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d; 	find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/'; 	echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf; 	printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf; 	/usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql; 	echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql; 	echo "THP_SETTING=never" >> /etc/sysconfig/mysql; 	chown -R mysql:root /etc/my.cnf /etc/my.cnf.d; 	chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Thu, 23 Mar 2023 00:21:49 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Thu, 23 Mar 2023 00:21:49 GMT
COPY file:8e394b40e5593ab1fb7ffd68ce2a3169f41e4e257f96ad515f6af4567362a3c5 in /docker-entrypoint.sh 
# Thu, 23 Mar 2023 00:21:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 00:21:49 GMT
USER mysql
# Thu, 23 Mar 2023 00:21:50 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 00:21:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5e8dcb5e56c183e88ba77bcc578f740c99b9e24522804c3588c46eda8f5cbdc1`  
		Last Modified: Wed, 22 Mar 2023 23:55:55 GMT  
		Size: 88.4 MB (88426082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f559f38a35981e9d54cccc047113059cc66917d58aaa6ee202f5ec20395d32c`  
		Last Modified: Thu, 23 Mar 2023 00:25:07 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bd93b69f8fe1d1223b20053e6a90bab33aaa80693b8cf70cfbec4506c241a8`  
		Last Modified: Thu, 23 Mar 2023 00:25:16 GMT  
		Size: 176.2 MB (176238489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202cd834ae4db37b6fbdb859d443ffe5a06e8e334939bfc1e53d3f9de5d10701`  
		Last Modified: Thu, 23 Mar 2023 00:25:32 GMT  
		Size: 179.5 MB (179477262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b27154872416218e3d01d3aedc9f60c1452bc5229a1495d4c3d180d4f43e0d2`  
		Last Modified: Thu, 23 Mar 2023 00:25:07 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b37133fc7fcecea5bd14d3e7d36a1a3bd55b446a3da3765f7429febf1756cc`  
		Last Modified: Thu, 23 Mar 2023 00:25:07 GMT  
		Size: 3.1 KB (3091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
