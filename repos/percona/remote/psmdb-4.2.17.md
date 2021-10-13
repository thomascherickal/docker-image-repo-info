## `percona:psmdb-4.2.17`

```console
$ docker pull percona@sha256:8080c8c01f67ca63637baa1c34fdfdd7cd71909b0e6437495d73852cfb0a0b08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2.17` - linux; amd64

```console
$ docker pull percona@sha256:4c88074ca33e56ed9e8c868a9c19eb195f513dde25723c6e2b23912958e3c68e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.4 MB (199395593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edaad76fee8fdbd6510a8f705956d7b3c3e5241775ffe009fafe7f68d1a70d96`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:04 GMT
ADD file:805cb5e15fb6e0bb0326ca33fd2942e068863ce2a8491bb71522c652f31fb466 in / 
# Wed, 15 Sep 2021 18:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 18:20:05 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 18:56:15 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 15 Sep 2021 19:01:18 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Wed, 13 Oct 2021 15:53:23 GMT
ENV PSMDB_VERSION=4.2.17-17
# Wed, 13 Oct 2021 15:53:23 GMT
ENV OS_VER=el8
# Wed, 13 Oct 2021 15:53:23 GMT
ENV FULL_PERCONA_VERSION=4.2.17-17.el8
# Wed, 13 Oct 2021 15:53:23 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 13 Oct 2021 15:53:54 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 13 Oct 2021 15:53:55 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 13 Oct 2021 15:53:55 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 13 Oct 2021 15:53:56 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 13 Oct 2021 15:53:56 GMT
ENV GOSU_VERSION=1.11
# Wed, 13 Oct 2021 15:54:01 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 13 Oct 2021 15:54:03 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 13 Oct 2021 15:54:04 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Wed, 13 Oct 2021 15:54:04 GMT
VOLUME [/data/db]
# Wed, 13 Oct 2021 15:54:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 15:54:04 GMT
EXPOSE 27017
# Wed, 13 Oct 2021 15:54:04 GMT
USER 1001
# Wed, 13 Oct 2021 15:54:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1519da890e410793d93550cb3ae60e5c86f9e3ef8e41b93487820a6970140b`  
		Last Modified: Wed, 15 Sep 2021 19:07:42 GMT  
		Size: 29.0 MB (28996742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee9f3465e1ea8abebe7151b5881399c91d0cfacde81e71df760d84bf59cb1fe`  
		Last Modified: Wed, 13 Oct 2021 15:55:12 GMT  
		Size: 77.8 MB (77807545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2718bd0e58bdcbd19b778632c889fbf7aca4073abae5be5fc2528e3f6f6243ae`  
		Last Modified: Wed, 13 Oct 2021 15:55:02 GMT  
		Size: 1.5 KB (1547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89154d76f3722710225815f9832f83cb377417be4845a258d350e2d0efc48f41`  
		Last Modified: Wed, 13 Oct 2021 15:55:01 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52aef1e7aeaaa0418115c680b644f7a4d9e0660fc3a69e11653d3f65825b7c2`  
		Last Modified: Wed, 13 Oct 2021 15:55:00 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc40752dabba7e1dc5c128fe52b9caa52a65070c598e00b2ac65e5ece97f832`  
		Last Modified: Wed, 13 Oct 2021 15:55:01 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f8e2b7c1cb272f0d01e92911b47fc482747cb4c127eb73ec06c44b1d9fa1b1`  
		Last Modified: Wed, 13 Oct 2021 15:55:02 GMT  
		Size: 8.1 MB (8137888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40cf3a0cc5b5bec4d7007db0d68ede74ed6da9f0c034b4659ded6a9b9a1a85a`  
		Last Modified: Wed, 13 Oct 2021 15:55:00 GMT  
		Size: 4.6 KB (4554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
