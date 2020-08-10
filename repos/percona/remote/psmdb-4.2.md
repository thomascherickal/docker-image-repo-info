## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:f235a60e1fec7bc5038d2d1384c102cc26638763ad87640b8032d69cbd00ebb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:f63b56c0ba6e553f6e4703d014abf5b5759a397c4ea2eab1c692fab48931b404
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.2 MB (169193717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05124bba7611945f91ccfaa8dd2941ec7d19def4cb2d47e77c1b7b32e47f3991`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:43:15 GMT
LABEL org.label-schema.schema-version=1.0
# Mon, 10 Aug 2020 18:43:15 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Mon, 10 Aug 2020 18:43:15 GMT
LABEL org.label-schema.vendor=Percona
# Mon, 10 Aug 2020 18:43:15 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Mon, 10 Aug 2020 18:43:15 GMT
LABEL org.label-schema.license=SSPLv1
# Mon, 10 Aug 2020 18:43:16 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Mon, 10 Aug 2020 18:43:16 GMT
LABEL org.opencontainers.image.vendor=Percona
# Mon, 10 Aug 2020 18:43:16 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Mon, 10 Aug 2020 18:43:16 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Mon, 10 Aug 2020 18:43:16 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 10 Aug 2020 18:43:16 GMT
ENV PSMDB_VERSION=4.2.8-8
# Mon, 10 Aug 2020 18:43:17 GMT
LABEL org.label-schema.schema-version=4.2.8-8
# Mon, 10 Aug 2020 18:43:17 GMT
LABEL org.opencontainers.image.version=4.2.8-8
# Mon, 10 Aug 2020 18:43:20 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Mon, 10 Aug 2020 18:43:21 GMT
ENV OS_VER=el7
# Mon, 10 Aug 2020 18:43:21 GMT
ENV FULL_PERCONA_VERSION=4.2.8-8.el7
# Mon, 10 Aug 2020 18:43:21 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 10 Aug 2020 18:43:26 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-2.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-6.8.2-1.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Mon, 10 Aug 2020 18:43:43 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;             repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Mon, 10 Aug 2020 18:43:44 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 10 Aug 2020 18:43:44 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 10 Aug 2020 18:43:45 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 10 Aug 2020 18:43:45 GMT
ENV GOSU_VERSION=1.11
# Mon, 10 Aug 2020 18:43:48 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Mon, 10 Aug 2020 18:43:50 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 10 Aug 2020 18:43:50 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Mon, 10 Aug 2020 18:43:50 GMT
VOLUME [/data/db]
# Mon, 10 Aug 2020 18:43:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 10 Aug 2020 18:43:51 GMT
EXPOSE 27017
# Mon, 10 Aug 2020 18:43:51 GMT
USER 1001
# Mon, 10 Aug 2020 18:43:51 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f478fedff42f32cbdeb4a5a6608401ffc5ffee4cf3dc682e0439feca623c9b`  
		Last Modified: Mon, 10 Aug 2020 18:47:07 GMT  
		Size: 6.5 MB (6456025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4018161a22daf012ae4b9264253712137bc71d2fc1ec55829fc34538b8eaac`  
		Last Modified: Mon, 10 Aug 2020 18:47:07 GMT  
		Size: 6.9 MB (6880922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b523008a3f4f3d5035362bd23b9ec9197d893792a1cc267f95448d525ea4207c`  
		Last Modified: Mon, 10 Aug 2020 18:47:16 GMT  
		Size: 70.9 MB (70918453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8192baf4c337abd72607a05591994106fad7344c9b9503d4629db2e54aaea6`  
		Last Modified: Mon, 10 Aug 2020 18:47:05 GMT  
		Size: 1.6 KB (1590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c92071bc6d3e78a6bd0e5c25598d7f884477288870c0c1bcf99f9f3dddbb1a4`  
		Last Modified: Mon, 10 Aug 2020 18:47:04 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0819e5f62bb5f38cdbe9a6b31aac3cdad527639747315378a6d4f24c7a0bcdac`  
		Last Modified: Mon, 10 Aug 2020 18:47:04 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b341fc2caab9b052cbe0aff6d2772bb72f7d9b26474ae5a1f61a2cb91f9bc960`  
		Last Modified: Mon, 10 Aug 2020 18:47:04 GMT  
		Size: 915.5 KB (915468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36f5a3034c1aa37aa2066a17c16946363d46d6a2a09b80bf2364b2c9fa37aa9`  
		Last Modified: Mon, 10 Aug 2020 18:47:05 GMT  
		Size: 8.1 MB (8138878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd44be8ac4536feccf76c3586dc6d1542f8bd01cad5ff12d3719c84a3cd0c8e`  
		Last Modified: Mon, 10 Aug 2020 18:47:04 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
