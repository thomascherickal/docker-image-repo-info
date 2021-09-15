## `percona:psmdb-5.0.2`

```console
$ docker pull percona@sha256:f6aac479d669624396ec4880544ea455b00695503899ca37244d62af892464b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0.2` - linux; amd64

```console
$ docker pull percona@sha256:18b3d4c8fb8c06ac2bddc2d0a733bf6f8f56badcb9cccd2e3eaf5615fb15b0b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.2 MB (232235105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aed25d328744a2d25e3b336f391358ab8279700694bb7a87837fd13531cccf68`
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
# Wed, 15 Sep 2021 18:59:33 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-50 release
# Wed, 15 Sep 2021 18:59:33 GMT
ENV PSMDB_VERSION=5.0.2-1
# Wed, 15 Sep 2021 18:59:33 GMT
ENV OS_VER=el8
# Wed, 15 Sep 2021 18:59:33 GMT
ENV FULL_PERCONA_VERSION=5.0.2-1.el8
# Wed, 15 Sep 2021 18:59:34 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 15 Sep 2021 18:59:57 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 15 Sep 2021 18:59:58 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 15 Sep 2021 18:59:59 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 15 Sep 2021 18:59:59 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 15 Sep 2021 18:59:59 GMT
ENV GOSU_VERSION=1.11
# Wed, 15 Sep 2021 19:00:10 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 15 Sep 2021 19:00:13 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 15 Sep 2021 19:00:14 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 15 Sep 2021 19:00:14 GMT
COPY file:394bf652dd75af51e6216e50638da41e532899a18a493ab4508cbae71e5b28cd in /entrypoint.sh 
# Wed, 15 Sep 2021 19:00:14 GMT
VOLUME [/data/db]
# Wed, 15 Sep 2021 19:00:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Sep 2021 19:00:15 GMT
EXPOSE 27017
# Wed, 15 Sep 2021 19:00:15 GMT
USER 1001
# Wed, 15 Sep 2021 19:00:15 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f8cd82037d208b9dc1abf25558eea975627cf488e12ccacf896e4e4bb56f49`  
		Last Modified: Wed, 15 Sep 2021 19:06:45 GMT  
		Size: 29.0 MB (28996720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55087f72c28e104bf2948d3e459e6c92f9acc1ffc99cd435283f7cb894757181`  
		Last Modified: Wed, 15 Sep 2021 19:06:56 GMT  
		Size: 110.6 MB (110633896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df584bde14eebe973938aa5bd89b1ff3747d6e60af98bd207ee870425dad4a37`  
		Last Modified: Wed, 15 Sep 2021 19:06:42 GMT  
		Size: 1.5 KB (1534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920c9abecf28e4757bb6f01a4d070091158d34570629ed411039e6d0e8041929`  
		Last Modified: Wed, 15 Sep 2021 19:06:42 GMT  
		Size: 4.1 KB (4099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba70cb959bca8660fa02d8840567bc479b584b509d789aa1dc4b00bac7e2b0e9`  
		Last Modified: Wed, 15 Sep 2021 19:06:39 GMT  
		Size: 10.6 KB (10577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71f974256571ca77c8563094df7eb09888c5e2ee9cc5a8c228c64dfeefd4ad7`  
		Last Modified: Wed, 15 Sep 2021 19:06:40 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf27f6ba98fd560877c5f8e8420ba8f8f4fa9d0fcbf2ac0b9fc35aacee33819`  
		Last Modified: Wed, 15 Sep 2021 19:06:41 GMT  
		Size: 8.1 MB (8137892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546eb3aa28819ddf7ee64df90c735614768c6412926486e8bf203a40f2f74747`  
		Last Modified: Wed, 15 Sep 2021 19:06:39 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9f78af6a6d5471bf57d93ef7ae865471bdb6ba4769a71ab76bbd4609fda065`  
		Last Modified: Wed, 15 Sep 2021 19:06:39 GMT  
		Size: 4.5 KB (4548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
