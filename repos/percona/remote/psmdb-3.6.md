## `percona:psmdb-3.6`

```console
$ docker pull percona@sha256:c08bd3daa8c0914e6f349370ff0f312eb4c87327515657e1ea7c200d784e372c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6` - linux; amd64

```console
$ docker pull percona@sha256:22e421512d4a63efc5aba7213f05accac3622031e20aa95f348ae2f87e352d6f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.9 MB (156918061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0a82035177d4bc2fd31a4360a6ca256330e60e8b7ee5c848aa96714fc5ec0c6`
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
# Mon, 17 Aug 2020 18:20:52 GMT
ENV PSMDB_VERSION=3.6.19-7.0
# Mon, 17 Aug 2020 18:20:52 GMT
LABEL org.label-schema.schema-version=3.6.19-7.0
# Mon, 17 Aug 2020 18:20:52 GMT
LABEL org.opencontainers.image.version=3.6.19-7.0
# Mon, 17 Aug 2020 18:20:57 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Mon, 17 Aug 2020 18:20:57 GMT
ENV OS_VER=el7
# Mon, 17 Aug 2020 18:20:57 GMT
ENV FULL_PERCONA_VERSION=3.6.19-7.0.el7
# Mon, 17 Aug 2020 18:20:57 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 17 Aug 2020 18:21:02 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-2.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-6.8.2-1.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Mon, 17 Aug 2020 18:21:20 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         yum-utils         shadow-utils         curl         procps-ng         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         yum clean all;         rm -rf /var/cache/yum /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Mon, 17 Aug 2020 18:21:20 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 17 Aug 2020 18:21:21 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 17 Aug 2020 18:21:22 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 17 Aug 2020 18:21:24 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 17 Aug 2020 18:21:24 GMT
VOLUME [/data/db]
# Mon, 17 Aug 2020 18:21:24 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Mon, 17 Aug 2020 18:21:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Aug 2020 18:21:25 GMT
EXPOSE 27017
# Mon, 17 Aug 2020 18:21:25 GMT
USER 1001
# Mon, 17 Aug 2020 18:21:25 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aad326dd31c40a1325d0fa1d3bc47c6e2d0d1f323dff9f9857714225321548c`  
		Last Modified: Mon, 17 Aug 2020 18:22:12 GMT  
		Size: 6.5 MB (6455957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa3f410784979b119425fb5f7374cb6f763f8246ee7fc99a8b0405c29213616`  
		Last Modified: Mon, 17 Aug 2020 18:22:12 GMT  
		Size: 6.9 MB (6881012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e469dce4bca7eea392f86b182fa3f88e62b98bd78023d7fe4e4b4b4533f1469`  
		Last Modified: Mon, 17 Aug 2020 18:22:20 GMT  
		Size: 59.6 MB (59558243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6af17410fe2bae960abafc8777911f1c10a5fa84caf9d7da938faaeb6afffc`  
		Last Modified: Mon, 17 Aug 2020 18:22:09 GMT  
		Size: 1.6 KB (1594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1c01e0019370e003856bf67e2413f49e09e64da331be1047c8f12c64b5f2be`  
		Last Modified: Mon, 17 Aug 2020 18:22:09 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be35b80070673c0d26151b0e8075fbb7c6853f1b3fdf4cd57f897288b150f51e`  
		Last Modified: Mon, 17 Aug 2020 18:22:09 GMT  
		Size: 10.6 KB (10575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede68323c438b69ccc3d5dfbc158c6e795bb54facf31dbffa2132c1ba2d61c74`  
		Last Modified: Mon, 17 Aug 2020 18:22:12 GMT  
		Size: 8.1 MB (8138875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50521073245dc9aed6648780e80fda638df8449bdb8c5e1ccb92b2aba22f95c`  
		Last Modified: Mon, 17 Aug 2020 18:22:09 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
