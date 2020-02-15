## `percona:psmdb-3.6.17`

```console
$ docker pull percona@sha256:dd5bfaa9be06fefdfb84811acb9e5e3c03047ac86773fa1c7381bce5ec90d598
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6.17` - linux; amd64

```console
$ docker pull percona@sha256:8d25c48d84055ee139945b8c2134b447ccf6b3785d4b996e0655fb4812fe1ab0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.3 MB (156272430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883a53a9e34d6aff5f88d4c7e1a5305962dc7d28a16d099d9a37c3dd6b0b8b8d`
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
# Sat, 15 Feb 2020 02:34:40 GMT
ENV PSMDB_VERSION=3.6.17-4.0
# Sat, 15 Feb 2020 02:34:40 GMT
LABEL org.label-schema.schema-version=3.6.17-4.0
# Sat, 15 Feb 2020 02:34:40 GMT
LABEL org.opencontainers.image.version=3.6.17-4.0
# Sat, 15 Feb 2020 02:34:44 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 15 Feb 2020 02:34:44 GMT
ENV OS_VER=el7
# Sat, 15 Feb 2020 02:34:45 GMT
ENV FULL_PERCONA_VERSION=3.6.17-4.0.el7
# Sat, 15 Feb 2020 02:34:45 GMT
ENV K8S_TOOLS_VERSION=0.4.2
# Sat, 15 Feb 2020 02:34:53 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Sat, 15 Feb 2020 02:35:49 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         yum-utils         shadow-utils         curl         procps-ng         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         yum clean all;         rm -rf /var/cache/yum /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Sat, 15 Feb 2020 02:35:50 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Sat, 15 Feb 2020 02:35:50 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 15 Feb 2020 02:35:51 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 15 Feb 2020 02:35:54 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 15 Feb 2020 02:35:54 GMT
VOLUME [/data/db]
# Sat, 15 Feb 2020 02:35:54 GMT
COPY file:85995e73e1e4d284ba65fabe65ed1e96fcb9c00ac0d328edb8b0b48749d784e1 in /entrypoint.sh 
# Sat, 15 Feb 2020 02:35:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 15 Feb 2020 02:35:55 GMT
EXPOSE 27017
# Sat, 15 Feb 2020 02:35:55 GMT
USER 1001
# Sat, 15 Feb 2020 02:35:55 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8f6987cdb938d0c2d7dabb952a4b2da195e5718c7abfa905b856b44d3f0f11`  
		Last Modified: Sat, 15 Feb 2020 02:36:29 GMT  
		Size: 6.4 MB (6380108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b368bc523806afffa36ef648c085dca9220781e35672c4918d9a9eb7dce3c664`  
		Last Modified: Sat, 15 Feb 2020 02:36:29 GMT  
		Size: 6.7 MB (6714918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb925f51e9fbbd8f697cabdbdac4e7269e42e1d4ecad85d68904979bdf31ec9`  
		Last Modified: Sat, 15 Feb 2020 02:36:38 GMT  
		Size: 59.8 MB (59811064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53d05cb4345d8123226acbff3db4bf637d57ed84fc828164d08b6dbc6cddd3f`  
		Last Modified: Sat, 15 Feb 2020 02:36:26 GMT  
		Size: 1.6 KB (1593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01051e0b33b5505b62bc9b1528cb4f8559346eb9a1e4b087d353c30383783220`  
		Last Modified: Sat, 15 Feb 2020 02:36:26 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cadad8163185f9a431fab412987e2794ea61e37c75f9d422dc171115dfc3435`  
		Last Modified: Sat, 15 Feb 2020 02:36:27 GMT  
		Size: 10.6 KB (10575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6eb624038abdab1f46d6d46afe5bcbb7962932b306bc66ea8a6034092256c99`  
		Last Modified: Sat, 15 Feb 2020 02:36:28 GMT  
		Size: 7.6 MB (7565368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c3be571e044284c5f520de72c1f89fe9ade2fb38621d85bcfd516d852aeb8f`  
		Last Modified: Sat, 15 Feb 2020 02:36:26 GMT  
		Size: 4.0 KB (4018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
