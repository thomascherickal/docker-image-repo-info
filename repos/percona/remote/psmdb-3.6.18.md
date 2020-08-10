## `percona:psmdb-3.6.18`

```console
$ docker pull percona@sha256:32cc38eaf515a4e94844d3e4a1ed0f7a2db63c4ffa01e3476d10ec705a311422
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6.18` - linux; amd64

```console
$ docker pull percona@sha256:a25b309763927aea7ef3c048237f9f294c00712bbd94a3872ed16dbfed9de782
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.9 MB (156890386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:237ee5fdc8731de53675c3bf679827f1920cd4e9b1c3d23c48e3736b5a89ea3c`
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
# Mon, 10 Aug 2020 18:44:48 GMT
ENV PSMDB_VERSION=3.6.18-6.0
# Mon, 10 Aug 2020 18:44:48 GMT
LABEL org.label-schema.schema-version=3.6.18-6.0
# Mon, 10 Aug 2020 18:44:49 GMT
LABEL org.opencontainers.image.version=3.6.18-6.0
# Mon, 10 Aug 2020 18:44:52 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Mon, 10 Aug 2020 18:44:53 GMT
ENV OS_VER=el7
# Mon, 10 Aug 2020 18:44:53 GMT
ENV FULL_PERCONA_VERSION=3.6.18-6.0.el7
# Mon, 10 Aug 2020 18:44:53 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 10 Aug 2020 18:44:58 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-2.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-6.8.2-1.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Mon, 10 Aug 2020 18:45:15 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         yum-utils         shadow-utils         curl         procps-ng         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         yum clean all;         rm -rf /var/cache/yum /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Mon, 10 Aug 2020 18:45:16 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 10 Aug 2020 18:45:16 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 10 Aug 2020 18:45:17 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 10 Aug 2020 18:45:19 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 10 Aug 2020 18:45:19 GMT
VOLUME [/data/db]
# Mon, 10 Aug 2020 18:45:20 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Mon, 10 Aug 2020 18:45:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 10 Aug 2020 18:45:20 GMT
EXPOSE 27017
# Mon, 10 Aug 2020 18:45:20 GMT
USER 1001
# Mon, 10 Aug 2020 18:45:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c8a4d6ef109e6571ab4978cd6979334ff3abb265b0845847aa085c8300e480`  
		Last Modified: Mon, 10 Aug 2020 18:47:40 GMT  
		Size: 6.5 MB (6456631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c9baa45a4df2e6f04437b7b2d6e7f528be53bce987762bc4d46e58f91fbf97`  
		Last Modified: Mon, 10 Aug 2020 18:47:40 GMT  
		Size: 6.9 MB (6881373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21bbba4da4c46ba9fdd4851a09652edd376f5d797865c3d10e4f4c518a3134d4`  
		Last Modified: Mon, 10 Aug 2020 18:47:48 GMT  
		Size: 59.5 MB (59529528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb469ae1639d5054ec31d969fcbaa8056e7d12d4a23e01227c3675a5f198d926`  
		Last Modified: Mon, 10 Aug 2020 18:47:37 GMT  
		Size: 1.6 KB (1593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc6e4acce4c12f3a86b83e9dc2993772eebb0fe81ebb99aa9faa057cba5d7ff`  
		Last Modified: Mon, 10 Aug 2020 18:47:37 GMT  
		Size: 4.1 KB (4073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084b17505d413a7edf83d77811124d9746239ef6a7757ed205ed1327705c051c`  
		Last Modified: Mon, 10 Aug 2020 18:47:38 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc862384047c6a0bee8c3a196c749da020d1c79e891ae681b64aefe7958bb61a`  
		Last Modified: Mon, 10 Aug 2020 18:47:39 GMT  
		Size: 8.1 MB (8138880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8329ef7b9d766a55410da6d35ef753449844283038b93b5b9eeff6d24b6e8ce`  
		Last Modified: Mon, 10 Aug 2020 18:47:37 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
