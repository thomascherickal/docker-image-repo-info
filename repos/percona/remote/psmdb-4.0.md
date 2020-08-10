## `percona:psmdb-4.0`

```console
$ docker pull percona@sha256:0aeb8bc34d9d4c7dc2ba6dc5cf29cde9fdd09552176df94b21790f909e8837b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0` - linux; amd64

```console
$ docker pull percona@sha256:02737f9db4acd20f4dfcc28769b2430b4452d1e71b8880eba2165706219c6b8a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.7 MB (159674391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:485d19e252bdb9a908a2dabccd1eed001b549cf2db5506f307cdb2d9831febc3`
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
# Mon, 10 Aug 2020 18:44:01 GMT
ENV PSMDB_VERSION=4.0.19-12
# Mon, 10 Aug 2020 18:44:02 GMT
LABEL org.label-schema.schema-version=4.0.19-12
# Mon, 10 Aug 2020 18:44:02 GMT
LABEL org.opencontainers.image.version=4.0.19-12
# Mon, 10 Aug 2020 18:44:06 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-40 release
# Mon, 10 Aug 2020 18:44:06 GMT
ENV OS_VER=el7
# Mon, 10 Aug 2020 18:44:06 GMT
ENV FULL_PERCONA_VERSION=4.0.19-12.el7
# Mon, 10 Aug 2020 18:44:06 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 10 Aug 2020 18:44:11 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-2.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-6.8.2-1.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Mon, 10 Aug 2020 18:44:31 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Mon, 10 Aug 2020 18:44:32 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 10 Aug 2020 18:44:32 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 10 Aug 2020 18:44:33 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 10 Aug 2020 18:44:33 GMT
ENV GOSU_VERSION=1.11
# Mon, 10 Aug 2020 18:44:35 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Mon, 10 Aug 2020 18:44:37 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 10 Aug 2020 18:44:37 GMT
VOLUME [/data/db]
# Mon, 10 Aug 2020 18:44:37 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Mon, 10 Aug 2020 18:44:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 10 Aug 2020 18:44:38 GMT
EXPOSE 27017
# Mon, 10 Aug 2020 18:44:38 GMT
USER 1001
# Mon, 10 Aug 2020 18:44:38 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3a8445854757f7b44c1cdd7136da5bae99e9b59b67f5eb8085d51c22751fff`  
		Last Modified: Mon, 10 Aug 2020 18:47:23 GMT  
		Size: 6.5 MB (6456025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8baa023c9bdf2f3a728b954db6a161b738782067c6bcc563ebc942e8562a4cf6`  
		Last Modified: Mon, 10 Aug 2020 18:47:23 GMT  
		Size: 6.9 MB (6880940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352ffe9848310a6ea40b21fa67b9472b0722a4cda9b9874942eaf213fada6385`  
		Last Modified: Mon, 10 Aug 2020 18:47:32 GMT  
		Size: 61.4 MB (61399103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c95258e552e8fc2b1c9b0269936e83b08e69a8c1195a40f65343f3d397a506c`  
		Last Modified: Mon, 10 Aug 2020 18:47:21 GMT  
		Size: 1.6 KB (1591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9e343d704c2df2a2c0e3fd2a43b62b4b7ef669194762592e8f068ff2fa6828`  
		Last Modified: Mon, 10 Aug 2020 18:47:20 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707b7808844bad2411f0ca06e9007b59dd246166f8e389ae56ba4e49af83a3d2`  
		Last Modified: Mon, 10 Aug 2020 18:47:20 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a8a835895ed8d9f2a4b6727dd7864351204bbf5834acd5151805a5cde4e208`  
		Last Modified: Mon, 10 Aug 2020 18:47:20 GMT  
		Size: 915.5 KB (915474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff555784e82928591116666b00ef8da2439561ced468ee62087b6cc52a207d63`  
		Last Modified: Mon, 10 Aug 2020 18:47:22 GMT  
		Size: 8.1 MB (8138876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dbfc472fe8ecfe3ceb4966aabe3c0eb97381f813ca7a2ad3900341ac420700`  
		Last Modified: Mon, 10 Aug 2020 18:47:20 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
