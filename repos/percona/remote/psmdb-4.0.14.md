## `percona:psmdb-4.0.14`

```console
$ docker pull percona@sha256:079ce316f3f2d4b71c53b4f5318c6d68c4f193297f6d2af0c7c24393ae79000a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0.14` - linux; amd64

```console
$ docker pull percona@sha256:7894e16d2c35804adeaa889e23f39c8c3beda8812bbaa20c6cefa70f901b35d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (158962129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dad05fffb9bc15ab6fa0b1d52645ff6b5f90b025fbd7e1dec243dea12382e38`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Wed, 29 Jan 2020 19:37:33 GMT
LABEL org.label-schema.schema-version=1.0
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.vendor=Percona
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.license=SSPLv1
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.opencontainers.image.vendor=Percona
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 29 Jan 2020 19:37:35 GMT
ENV PSMDB_VERSION=4.0.14-8
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.label-schema.schema-version=4.0.14-8
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.version=4.0.14-8
# Wed, 29 Jan 2020 19:37:40 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-40 release
# Wed, 29 Jan 2020 19:37:40 GMT
ENV OS_VER=el7
# Wed, 29 Jan 2020 19:37:40 GMT
ENV FULL_PERCONA_VERSION=4.0.14-8.el7
# Wed, 29 Jan 2020 19:37:41 GMT
ENV K8S_TOOLS_VERSION=0.4.2
# Wed, 29 Jan 2020 19:37:46 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Wed, 29 Jan 2020 19:38:10 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 29 Jan 2020 19:38:11 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 29 Jan 2020 19:38:11 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 29 Jan 2020 19:38:12 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 29 Jan 2020 19:38:12 GMT
ENV GOSU_VERSION=1.11
# Wed, 29 Jan 2020 19:38:15 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 29 Jan 2020 19:38:17 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 29 Jan 2020 19:38:17 GMT
VOLUME [/data/db]
# Wed, 29 Jan 2020 19:38:18 GMT
COPY file:85995e73e1e4d284ba65fabe65ed1e96fcb9c00ac0d328edb8b0b48749d784e1 in /entrypoint.sh 
# Wed, 29 Jan 2020 19:38:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jan 2020 19:38:18 GMT
EXPOSE 27017
# Wed, 29 Jan 2020 19:38:18 GMT
USER 1001
# Wed, 29 Jan 2020 19:38:18 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e0ce77bf6153fbd690fb03eb3d42b9008411f9b97ed8a22154ef61d28d080a`  
		Last Modified: Wed, 29 Jan 2020 19:40:14 GMT  
		Size: 6.4 MB (6371262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a64cfd09ed5cff1b25acf8bd50ec6ac54b3fe2923885d8b17ae1613ba1088d`  
		Last Modified: Wed, 29 Jan 2020 19:40:14 GMT  
		Size: 6.7 MB (6693993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fafc1f651a2a537b76012523ec0737016d6e7a782a4d60786c0712d9ce354bce`  
		Last Modified: Wed, 29 Jan 2020 19:40:25 GMT  
		Size: 61.6 MB (61615064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b071a9fc3a03521f5e70f60e5df9db3e78ec9272536000918b88445e644d903`  
		Last Modified: Wed, 29 Jan 2020 19:40:11 GMT  
		Size: 1.6 KB (1591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df472d658ba7d39a94826ca133f38bf0207f70c9ea2336ff6cb1ef6d92cbf92b`  
		Last Modified: Wed, 29 Jan 2020 19:40:10 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29e055ad0d1fb34b76891468a719cf6dd405b1a285318aed9772a3a2ef14411`  
		Last Modified: Wed, 29 Jan 2020 19:40:09 GMT  
		Size: 10.6 KB (10577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88767c48922b736c64e5fcdbf6f257b4aee0003d9d12d7d23be12cba18d7f524`  
		Last Modified: Wed, 29 Jan 2020 19:40:10 GMT  
		Size: 915.5 KB (915468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5666d291ae7585a1cac26a076e091582c3685ceafa04085d4863cb1b7c23feb`  
		Last Modified: Wed, 29 Jan 2020 19:40:12 GMT  
		Size: 7.6 MB (7565373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d76452c8dcfa27e0eeee766d647a78a2384081b4528837c95a797b032ae0b`  
		Last Modified: Wed, 29 Jan 2020 19:40:09 GMT  
		Size: 4.0 KB (4014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
