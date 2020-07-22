## `percona:8-centos`

```console
$ docker pull percona@sha256:7f2b7709f85a4b77d612e7cbb518372f439bbc2dec80567bdf01793676c8ad66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:8-centos` - linux; amd64

```console
$ docker pull percona@sha256:c28fa0801bd23c97cfb16f669b15fd66446780ec899a07831e1e2addd96cd6de
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226846380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:413400f31bb523d51ef5609617ac531d53959cdbd034fc781b9333829c1ae857`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:39:06 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 05 May 2020 21:39:07 GMT
RUN groupadd -g 1001 mysql
# Tue, 05 May 2020 21:39:08 GMT
RUN useradd -u 1001 -r -g 1001 -s /sbin/nologin 		-c "Default Application User" mysql
# Tue, 05 May 2020 21:39:13 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     yum install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release disable all;     percona-release setup ps80
# Wed, 22 Jul 2020 01:15:22 GMT
ENV PERCONA_VERSION=8.0.20-11.1.el7
# Wed, 22 Jul 2020 01:16:40 GMT
RUN set -ex;     yum install -y         percona-server-server-${PERCONA_VERSION}         percona-server-tokudb-${PERCONA_VERSION}         percona-server-devel-${PERCONA_VERSION}         percona-server-rocksdb-${PERCONA_VERSION}         jemalloc         which         policycoreutils;         yum clean all;     rm -rf /var/cache/yum /var/lib/mysql
# Wed, 22 Jul 2020 01:16:42 GMT
RUN /usr/bin/install -m 0775 -o mysql -g root -d /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d 	&& find /etc/my.cnf /etc/my.cnf.d -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user)/#&/' 	&& echo '!includedir /etc/my.cnf.d' >> /etc/my.cnf 	&& printf '[mysqld]\nskip-host-cache\nskip-name-resolve\n' > /etc/my.cnf.d/docker.cnf 	&& /usr/bin/install -m 0664 -o mysql -g root /dev/null /etc/sysconfig/mysql 	&& echo "LD_PRELOAD=/usr/lib64/libjemalloc.so.1" >> /etc/sysconfig/mysql 	&& echo "THP_SETTING=never" >> /etc/sysconfig/mysql 	&& chown -R mysql:root /etc/my.cnf /etc/my.cnf.d 	&& chmod -R ug+rwX /etc/my.cnf /etc/my.cnf.d
# Wed, 22 Jul 2020 01:16:42 GMT
VOLUME [/var/lib/mysql /var/log/mysql]
# Wed, 22 Jul 2020 01:16:43 GMT
COPY file:98315a3cdd5c008868bca89eff8d9037073d3b25d79ce0bfce9220868c87243b in /docker-entrypoint.sh 
# Wed, 22 Jul 2020 01:16:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jul 2020 01:16:43 GMT
USER mysql
# Wed, 22 Jul 2020 01:16:44 GMT
EXPOSE 3306 33060
# Wed, 22 Jul 2020 01:16:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e386a719ceae0f0238e80a8fbcd5e5144f3c4675860fc1677674d224a4f043`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b0b666a45f4b0619d873f8a797c2e1c0451a196871908efd2d3442c506e6ef`  
		Last Modified: Tue, 05 May 2020 21:44:33 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b1a9d6f75e0d0123edeb268d2aa760548242a912592232d7b1d93ae8f9f1d6`  
		Last Modified: Tue, 05 May 2020 21:44:34 GMT  
		Size: 6.5 MB (6516428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6466b5cc6fc95faae6a65b204af5bbb271324bc41e3520b95cea1dc0372ebd7b`  
		Last Modified: Wed, 22 Jul 2020 01:18:19 GMT  
		Size: 144.4 MB (144443506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff707b7c5fab2483a29cca043035a0d1127ac6d0887f6d50c6d8034c99fb7eff`  
		Last Modified: Wed, 22 Jul 2020 01:17:45 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f48980d0f84b985b4689b7fddafa95da937aa4ce11774b638459b1d5011096`  
		Last Modified: Wed, 22 Jul 2020 01:17:45 GMT  
		Size: 3.1 KB (3067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
