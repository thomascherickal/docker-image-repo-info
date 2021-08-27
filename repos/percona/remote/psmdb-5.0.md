## `percona:psmdb-5.0`

```console
$ docker pull percona@sha256:1df29b4d605f5f9b08c0abc691c1d7dc3a8a8a66f676f8a27f195873455a66db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0` - linux; amd64

```console
$ docker pull percona@sha256:6f4472465369db5a80e7fcbc68f06006e79f6ac51b2bce18ad1733fda9aaac5e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.2 MB (224214997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0263932ca807632aab876d74e7b9cdfd7bff2e4c0ee4667c805c434306cf1850`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Sat, 06 Mar 2021 01:08:18 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 27 Aug 2021 17:28:12 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-50 release
# Fri, 27 Aug 2021 17:28:12 GMT
ENV PSMDB_VERSION=5.0.2-1
# Fri, 27 Aug 2021 17:28:12 GMT
ENV OS_VER=el8
# Fri, 27 Aug 2021 17:28:13 GMT
ENV FULL_PERCONA_VERSION=5.0.2-1.el8
# Fri, 27 Aug 2021 17:28:13 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Fri, 27 Aug 2021 17:28:39 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Fri, 27 Aug 2021 17:28:40 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Fri, 27 Aug 2021 17:28:40 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Fri, 27 Aug 2021 17:28:41 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Fri, 27 Aug 2021 17:28:41 GMT
ENV GOSU_VERSION=1.11
# Fri, 27 Aug 2021 17:28:44 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Fri, 27 Aug 2021 17:28:47 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Fri, 27 Aug 2021 17:28:48 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Fri, 27 Aug 2021 17:28:48 GMT
COPY file:394bf652dd75af51e6216e50638da41e532899a18a493ab4508cbae71e5b28cd in /entrypoint.sh 
# Fri, 27 Aug 2021 17:28:48 GMT
VOLUME [/data/db]
# Fri, 27 Aug 2021 17:28:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 27 Aug 2021 17:28:49 GMT
EXPOSE 27017
# Fri, 27 Aug 2021 17:28:49 GMT
USER 1001
# Fri, 27 Aug 2021 17:28:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6176b1c12262b187a60dcc82b2cd8e61a48ce45b8069ae83ee41dd3467b878c5`  
		Last Modified: Fri, 27 Aug 2021 17:30:03 GMT  
		Size: 27.6 MB (27584268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c2e8bbf5a85801ed288804eb00c999ac5b7a2059cd0629d6b74a4ae29b056c`  
		Last Modified: Fri, 27 Aug 2021 17:30:14 GMT  
		Size: 112.4 MB (112362299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e6c3a78242e88dfaa061d636d86208a49fff0911d1b79d8361b3edc61ab566`  
		Last Modified: Fri, 27 Aug 2021 17:30:00 GMT  
		Size: 1.5 KB (1547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d20ac6292f2cb7382e8650620c0501b4be6adc912252bacd6de1f30026a566`  
		Last Modified: Fri, 27 Aug 2021 17:29:59 GMT  
		Size: 4.1 KB (4102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6d63a7f20a7f3d71235ac73319e6e8aa50a37110542c77bea2bf3f175d5b4c`  
		Last Modified: Fri, 27 Aug 2021 17:29:57 GMT  
		Size: 10.6 KB (10577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b750d2ad6b40d9078eb2affc1234d871e0f4e56dde0ade71d9f17a7dda9f5969`  
		Last Modified: Fri, 27 Aug 2021 17:29:58 GMT  
		Size: 914.6 KB (914552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2336a574d7c1bad0ff26956f146d2feaf18e63e2bf1df13bf447431a21b8462e`  
		Last Modified: Fri, 27 Aug 2021 17:29:59 GMT  
		Size: 8.1 MB (8137900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fd2ccf61a914006cddbf4b71d803f55d85f1119d21e75a06c8105fb4a1246e`  
		Last Modified: Fri, 27 Aug 2021 17:29:57 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dec9b513876fc83d6de9dae58f551fa8bac15971ec2c9a6216a43504de5c877`  
		Last Modified: Fri, 27 Aug 2021 17:29:57 GMT  
		Size: 4.5 KB (4549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
