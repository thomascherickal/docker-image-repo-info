## `percona:psmdb-4.0`

```console
$ docker pull percona@sha256:c937b9a6696162910a3b1e5c851b9d3335700a50f9a9cf042bc6826ac0ba041f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0` - linux; amd64

```console
$ docker pull percona@sha256:1011c0e4100498c48b392842fed8b161e7a7ade0480764c1b356147196d3fb69
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.1 MB (160142768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a383bc18c37f73a3304fd9edbe81f189f9b761e1e01b75b7974aa9f12bf60096`
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
# Thu, 30 Apr 2020 19:34:59 GMT
ENV PSMDB_VERSION=4.0.18-11
# Thu, 30 Apr 2020 19:34:59 GMT
LABEL org.label-schema.schema-version=4.0.18-11
# Thu, 30 Apr 2020 19:34:59 GMT
LABEL org.opencontainers.image.version=4.0.18-11
# Thu, 30 Apr 2020 19:35:07 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-40 release
# Thu, 30 Apr 2020 19:35:07 GMT
ENV OS_VER=el7
# Thu, 30 Apr 2020 19:35:07 GMT
ENV FULL_PERCONA_VERSION=4.0.18-11.el7
# Thu, 30 Apr 2020 19:35:08 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 30 Apr 2020 19:35:13 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Thu, 30 Apr 2020 19:35:38 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 30 Apr 2020 19:35:39 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 30 Apr 2020 19:35:39 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 30 Apr 2020 19:35:40 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 30 Apr 2020 19:35:40 GMT
ENV GOSU_VERSION=1.11
# Thu, 30 Apr 2020 19:35:43 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 30 Apr 2020 19:35:45 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 30 Apr 2020 19:35:46 GMT
VOLUME [/data/db]
# Thu, 30 Apr 2020 19:35:46 GMT
COPY file:85995e73e1e4d284ba65fabe65ed1e96fcb9c00ac0d328edb8b0b48749d784e1 in /entrypoint.sh 
# Thu, 30 Apr 2020 19:35:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Apr 2020 19:35:46 GMT
EXPOSE 27017
# Thu, 30 Apr 2020 19:35:46 GMT
USER 1001
# Thu, 30 Apr 2020 19:35:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b430acd1012a6145fca50e4b059b9307dcc8959d2c9e975ebbd76f6b1f65618c`  
		Last Modified: Thu, 30 Apr 2020 19:36:15 GMT  
		Size: 6.4 MB (6381258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30eb48b75d742d4f4aebdd11257c39b2bbe788fe200df2cfdaa3c9bea1c9276b`  
		Last Modified: Thu, 30 Apr 2020 19:36:13 GMT  
		Size: 6.7 MB (6717491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1c37e185840ccaf8ede879c828e0b40d2d41918732a40503c2123b25e0cfa0`  
		Last Modified: Thu, 30 Apr 2020 19:36:23 GMT  
		Size: 62.2 MB (62188704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b808070801fd1b3b62094e7a00b9f5a7b8f483f29dedbc2f14d647d623e4bd11`  
		Last Modified: Thu, 30 Apr 2020 19:36:11 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1b9f03806b07e3fbcdd9d67b2c9ab29187674817751db7d50d8a137791c202`  
		Last Modified: Thu, 30 Apr 2020 19:36:10 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9fd51567b713434cde6fd33e37fbc79086df6f26ad2540b9303c047be00792b`  
		Last Modified: Thu, 30 Apr 2020 19:36:10 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ac4931be0a6e11c200d7edd6d820bf1b31aae950254c849510a2491e5f3377`  
		Last Modified: Thu, 30 Apr 2020 19:36:12 GMT  
		Size: 915.5 KB (915462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc31f4768b13c510a17cd9a9ac4a0628dc10046f7a37dfc32e9d9a232a6ef6c`  
		Last Modified: Thu, 30 Apr 2020 19:36:20 GMT  
		Size: 8.1 MB (8138875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d165a06d912a28fbd137298247e5e2262194e350c0bd748d763c523e5321b361`  
		Last Modified: Thu, 30 Apr 2020 19:36:10 GMT  
		Size: 4.0 KB (4017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
