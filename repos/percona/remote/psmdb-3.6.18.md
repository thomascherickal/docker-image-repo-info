## `percona:psmdb-3.6.18`

```console
$ docker pull percona@sha256:295d360a85dc46ee443cd340dfcadcbc406d119c29700784eb1c5afe8de37b26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6.18` - linux; amd64

```console
$ docker pull percona@sha256:5bb2e2fa02ba7570561ad727c5ad45b61986dcc88efbde3447cb4a904a1c08c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.0 MB (157035853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bb0898e4443c69e665418e86e273338005e2d89b1666a8ac7c9ffab515a3729`
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
# Tue, 26 May 2020 21:45:33 GMT
ENV PSMDB_VERSION=3.6.18-6.0
# Tue, 26 May 2020 21:45:34 GMT
LABEL org.label-schema.schema-version=3.6.18-6.0
# Tue, 26 May 2020 21:45:34 GMT
LABEL org.opencontainers.image.version=3.6.18-6.0
# Tue, 26 May 2020 21:45:40 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Tue, 26 May 2020 21:45:40 GMT
ENV OS_VER=el7
# Tue, 26 May 2020 21:45:41 GMT
ENV FULL_PERCONA_VERSION=3.6.18-6.0.el7
# Tue, 26 May 2020 21:45:41 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 02 Jul 2020 17:21:14 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-2.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-6.8.2-1.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Thu, 02 Jul 2020 17:21:32 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         yum-utils         shadow-utils         curl         procps-ng         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         yum clean all;         rm -rf /var/cache/yum /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Thu, 02 Jul 2020 17:21:32 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 02 Jul 2020 17:21:33 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 02 Jul 2020 17:21:33 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 02 Jul 2020 17:21:35 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 02 Jul 2020 17:21:36 GMT
VOLUME [/data/db]
# Thu, 02 Jul 2020 17:21:36 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Thu, 02 Jul 2020 17:21:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Jul 2020 17:21:36 GMT
EXPOSE 27017
# Thu, 02 Jul 2020 17:21:36 GMT
USER 1001
# Thu, 02 Jul 2020 17:21:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b9cf95a40ddab7409d772516d80954ddbf1ea23d0b61ad382f8cfc15eb086b`  
		Last Modified: Tue, 26 May 2020 21:47:12 GMT  
		Size: 6.5 MB (6470308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224b3b313dda5e5a1d45077b7a7380fe3616b6b1f9993a464b0f0742503a5ef6`  
		Last Modified: Thu, 02 Jul 2020 17:22:19 GMT  
		Size: 6.9 MB (6866852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e9f32fd306993d08b51cfbc4c17d20a137743d3d3633b37d9ccf7ef8ca5f28`  
		Last Modified: Thu, 02 Jul 2020 17:22:27 GMT  
		Size: 59.7 MB (59658881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e683bdb8b3e4e93c793d57b71c3a1ec06e4a2f0a41ab3d33917c1a6741f800ce`  
		Last Modified: Thu, 02 Jul 2020 17:22:16 GMT  
		Size: 1.6 KB (1593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e012d00cdfac70ed89214d6c727457048aa09261a226f16a77f672cd68d5ff0`  
		Last Modified: Thu, 02 Jul 2020 17:22:16 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f8729ed74d84ee001ebfad26a5c65e83ddfe7960e50404e021433067391c3a`  
		Last Modified: Thu, 02 Jul 2020 17:22:16 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6657db9ed2cf25bbd739123194bf42a6ea0a3e16e488add8ebb78fe01dcd61`  
		Last Modified: Thu, 02 Jul 2020 17:22:19 GMT  
		Size: 8.1 MB (8138884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91023628d75393aa573a82271a79e3d39e66c5ccd1dc62c683a51540e74a1407`  
		Last Modified: Thu, 02 Jul 2020 17:22:16 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
