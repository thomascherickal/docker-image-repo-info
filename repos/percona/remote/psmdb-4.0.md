## `percona:psmdb-4.0`

```console
$ docker pull percona@sha256:50b2f422b1f59d3281f53346503046ce76cb2091f3101f2d6ad564a783d87bd5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0` - linux; amd64

```console
$ docker pull percona@sha256:4c8f0f472d747dbe9abec92bd7755b0ca9dbdcff855422e0f1932d2c3629421d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.8 MB (159807459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:283525e93531b3c2ee68229bd61450f57f03847c11c5bfff8cd9c7d81c74f93d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:42:02 GMT
LABEL org.label-schema.schema-version=1.0
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.vendor=Percona
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.label-schema.license=SSPLv1
# Tue, 05 May 2020 21:42:03 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.vendor=Percona
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Tue, 05 May 2020 21:42:04 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 02 Jul 2020 17:20:15 GMT
ENV PSMDB_VERSION=4.0.19-12
# Thu, 02 Jul 2020 17:20:15 GMT
LABEL org.label-schema.schema-version=4.0.19-12
# Thu, 02 Jul 2020 17:20:15 GMT
LABEL org.opencontainers.image.version=4.0.19-12
# Thu, 02 Jul 2020 17:20:20 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-40 release
# Thu, 02 Jul 2020 17:20:20 GMT
ENV OS_VER=el7
# Thu, 02 Jul 2020 17:20:20 GMT
ENV FULL_PERCONA_VERSION=4.0.19-12.el7
# Thu, 02 Jul 2020 17:20:20 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 02 Jul 2020 17:20:25 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-2.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-6.8.2-1.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Thu, 02 Jul 2020 17:20:57 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         yum-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     yum clean all;     rm -rf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 02 Jul 2020 17:20:57 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 02 Jul 2020 17:20:58 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 02 Jul 2020 17:20:58 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 02 Jul 2020 17:20:59 GMT
ENV GOSU_VERSION=1.11
# Thu, 02 Jul 2020 17:21:02 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 02 Jul 2020 17:21:04 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 02 Jul 2020 17:21:04 GMT
VOLUME [/data/db]
# Thu, 02 Jul 2020 17:21:04 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Thu, 02 Jul 2020 17:21:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Jul 2020 17:21:05 GMT
EXPOSE 27017
# Thu, 02 Jul 2020 17:21:05 GMT
USER 1001
# Thu, 02 Jul 2020 17:21:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5109611112125f79258a9f8d59c3ef11256cc2d34cdd8e1ebb9633d218bbdf08`  
		Last Modified: Thu, 02 Jul 2020 17:22:02 GMT  
		Size: 6.5 MB (6471413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018ff6fd1bd6bd93645c4e94b8a1ba0375eb0c9d95e74d7b77a38efe80fcd229`  
		Last Modified: Thu, 02 Jul 2020 17:22:02 GMT  
		Size: 6.9 MB (6867143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071041a0d2c46a1358a0c5c369b0f3796aca1a81cbdad7796ec7548d91435e17`  
		Last Modified: Thu, 02 Jul 2020 17:22:11 GMT  
		Size: 61.5 MB (61513630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ad5af3fc92236f0711c1051eaec699bcaaabba482bc0282b9fede2af93e209`  
		Last Modified: Thu, 02 Jul 2020 17:22:00 GMT  
		Size: 1.6 KB (1594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35750ebe5d0f1e9bc83635cd6642c1ff83bb20fb0bb9a27e16d1b024fa276609`  
		Last Modified: Thu, 02 Jul 2020 17:21:59 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d0904fab10023a2e21d916489eed4462bf884ed282ccc48e955adbf17ec208`  
		Last Modified: Thu, 02 Jul 2020 17:21:59 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c132430f30e0ce4bc221e0fcf7602010dad8fc66a0aae599a53f608b5daf39`  
		Last Modified: Thu, 02 Jul 2020 17:22:00 GMT  
		Size: 915.5 KB (915466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c37bfbfe55ca6cf935126e6c298df8654b7bece6811e1f673c9e09f27253e2`  
		Last Modified: Thu, 02 Jul 2020 17:22:01 GMT  
		Size: 8.1 MB (8138879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2485e5ab8ac8154cb077075aa9c2b59a46d2c76fe2898dbf5d8bce634fe3f926`  
		Last Modified: Thu, 02 Jul 2020 17:22:00 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
