## `percona:psmdb-3.6`

```console
$ docker pull percona@sha256:6f4839cff36fb816beab56a69f8acfb428f1043769f275d2f213708ddc4b9661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6` - linux; amd64

```console
$ docker pull percona@sha256:147f999d6a931565f8812e9bc3387862040d9e1f3be06479ded81734af24f42d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.0 MB (156955012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6007e785e971302c5d50954833bc5c79c3422c509f8232f61b18611904e9e4e7`
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
# Tue, 26 May 2020 21:45:48 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Tue, 26 May 2020 21:46:12 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         yum-utils         shadow-utils         curl         procps-ng         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         yum clean all;         rm -rf /var/cache/yum /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Tue, 26 May 2020 21:46:14 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 26 May 2020 21:46:15 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 26 May 2020 21:46:16 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 26 May 2020 21:46:21 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 26 May 2020 21:46:21 GMT
VOLUME [/data/db]
# Tue, 26 May 2020 21:46:21 GMT
COPY file:85995e73e1e4d284ba65fabe65ed1e96fcb9c00ac0d328edb8b0b48749d784e1 in /entrypoint.sh 
# Tue, 26 May 2020 21:46:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 26 May 2020 21:46:22 GMT
EXPOSE 27017
# Tue, 26 May 2020 21:46:23 GMT
USER 1001
# Tue, 26 May 2020 21:46:23 GMT
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
	-	`sha256:f6d53e4d6470b9e7a55ea4d656570c7d7b1630d4e36da4a75cb758551ffba777`  
		Last Modified: Tue, 26 May 2020 21:47:12 GMT  
		Size: 6.8 MB (6794740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2487bc853ed7b533d7232c6bb4496349f515dee5974139c8c5f0ef7b779ef2fa`  
		Last Modified: Tue, 26 May 2020 21:47:25 GMT  
		Size: 59.7 MB (59650682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dadb527369af8261ce449cedd3ec6af481947a0695bb450adf73de206be4feb`  
		Last Modified: Tue, 26 May 2020 21:47:07 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8949220cddbb6332cb6b9e8171f990b98f93a9e19209ae55361027347c9439a3`  
		Last Modified: Tue, 26 May 2020 21:47:07 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0369cbd1fb50d2e24a30d691d263566f12d72783e20acf23696c26906dfbcd94`  
		Last Modified: Tue, 26 May 2020 21:47:07 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924b240b4cb54c9df68c61d44eac4b3345fa0e050bdfde7374790cafa9c4f460`  
		Last Modified: Tue, 26 May 2020 21:47:12 GMT  
		Size: 8.1 MB (8138879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2850bf614f384c3501d51222981386b44270240e20116ecc7fc0e1fe02c3c86`  
		Last Modified: Tue, 26 May 2020 21:47:07 GMT  
		Size: 4.0 KB (4013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
