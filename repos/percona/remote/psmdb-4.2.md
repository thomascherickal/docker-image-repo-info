## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:be8999379b6f9c1be9f2c68b864d5b446bf3b045edd9710ea39aae1afd7ff9bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:4135e49d7d29caf784039d4f239c9f9d03230bfb652d47e99955793e9bae7204
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.4 MB (176424821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af29533ff7800432dfea82a6dfdb97cbbdab023f4250d5c1220054c4d8c86bed`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Oct 2022 19:20:44 GMT
ADD file:13fd8e206cb28eeafe30eb7ce28aaa24652a47074e82b1229e25c3f07b525253 in / 
# Fri, 21 Oct 2022 19:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:38:52 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 21 Oct 2022 19:42:17 GMT
ENV PSMDB_VERSION=4.2.21-21
# Fri, 21 Oct 2022 19:42:17 GMT
ENV OS_VER=el8
# Fri, 21 Oct 2022 19:42:17 GMT
ENV FULL_PERCONA_VERSION=4.2.21-21.el8
# Fri, 21 Oct 2022 19:42:17 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Fri, 21 Oct 2022 19:42:20 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Fri, 21 Oct 2022 19:42:55 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Fri, 21 Oct 2022 19:42:56 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Fri, 21 Oct 2022 19:42:57 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Fri, 21 Oct 2022 19:42:57 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Fri, 21 Oct 2022 19:42:57 GMT
ENV GOSU_VERSION=1.11
# Fri, 21 Oct 2022 19:43:00 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Fri, 21 Oct 2022 19:43:02 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Fri, 21 Oct 2022 19:43:02 GMT
VOLUME [/data/db]
# Fri, 21 Oct 2022 19:43:02 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Fri, 21 Oct 2022 19:43:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Oct 2022 19:43:03 GMT
EXPOSE 27017
# Fri, 21 Oct 2022 19:43:03 GMT
USER 1001
# Fri, 21 Oct 2022 19:43:03 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:1580782cb014754e166fa2c701113af0e745dba59fb5fc368a1b676059545818`  
		Last Modified: Fri, 21 Oct 2022 19:22:23 GMT  
		Size: 86.0 MB (85966825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b8b39a80b4f29e4688e63d0dc175f28b8d0a748d479af04beba35bffe903fc`  
		Last Modified: Fri, 21 Oct 2022 19:45:42 GMT  
		Size: 3.8 MB (3775652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51fa8976d8ad69850b49c9f083acbcf43cc130d8b3fbddfda85d403c3546bbf5`  
		Last Modified: Fri, 21 Oct 2022 19:45:51 GMT  
		Size: 77.6 MB (77609512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9496f436738893e9acce976540ae048c2740f17a15431cb50984fcbcccde8fea`  
		Last Modified: Fri, 21 Oct 2022 19:45:41 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0c2b11986fd25fb2746863d8d1d793d4fce124ff8039b965a2a98d1b2f9b27`  
		Last Modified: Fri, 21 Oct 2022 19:45:39 GMT  
		Size: 4.1 KB (4101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8940395b288739da8b8880bf17c716c4d82dbc773c13c21d744788b455d7950c`  
		Last Modified: Fri, 21 Oct 2022 19:45:39 GMT  
		Size: 10.6 KB (10577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d105279afdb75952fe3967c2fcb00ca8ad5d0da43d52fc743380d1d89cf7a561`  
		Last Modified: Fri, 21 Oct 2022 19:45:39 GMT  
		Size: 914.5 KB (914545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d14f3d5c3da3b325e9a5af9a17710319d50e416ce48a02004d7ce7a12a183af`  
		Last Modified: Fri, 21 Oct 2022 19:45:41 GMT  
		Size: 8.1 MB (8137887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec55fd9f11bc58fcd8603dfc4fc9b892ab49344eba3b36639d81fb3cc316f9c`  
		Last Modified: Fri, 21 Oct 2022 19:45:39 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
