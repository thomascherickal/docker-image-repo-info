## `percona:psmdb-3.6.19`

```console
$ docker pull percona@sha256:9cb3697a01eb0004ecdf50148f158689765a472ed587851e9315802ba12ad6cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6.19` - linux; amd64

```console
$ docker pull percona@sha256:b99eb8da53225288ec57217d7dc12147fc3ab23be0c31d6aef0128c6aefb2357
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.5 MB (157475795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:389f77c209ee832872f3a8af694538c0d180511d5066a1fe85d2868d305aa60e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.schema-version=1.0
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.vendor=Percona
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.label-schema.license=SSPLv1
# Fri, 04 Sep 2020 19:25:41 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.vendor=Percona
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Fri, 04 Sep 2020 19:25:42 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 12 Oct 2020 23:27:35 GMT
ENV PSMDB_VERSION=3.6.19-8.0
# Mon, 12 Oct 2020 23:27:35 GMT
ENV OS_VER=el8
# Mon, 12 Oct 2020 23:27:35 GMT
ENV FULL_PERCONA_VERSION=3.6.19-8.0.el8
# Mon, 12 Oct 2020 23:27:35 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 12 Oct 2020 23:27:35 GMT
LABEL org.label-schema.schema-version=3.6.19-8.0
# Mon, 12 Oct 2020 23:27:36 GMT
LABEL org.opencontainers.image.version=3.6.19-8.0
# Mon, 12 Oct 2020 23:27:41 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Mon, 12 Oct 2020 23:29:07 GMT
RUN set -ex;     dnf install -y         dnf-utils         shadow-utils         curl         procps-ng         jq         oniguruma         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         dnf remove -y dnf-utils;         dnf clean all;         rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Mon, 12 Oct 2020 23:29:08 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 12 Oct 2020 23:29:08 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 12 Oct 2020 23:29:09 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 12 Oct 2020 23:29:11 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 12 Oct 2020 23:29:11 GMT
VOLUME [/data/db]
# Mon, 12 Oct 2020 23:29:11 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Mon, 12 Oct 2020 23:29:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Oct 2020 23:29:11 GMT
EXPOSE 27017
# Mon, 12 Oct 2020 23:29:12 GMT
USER 1001
# Mon, 12 Oct 2020 23:29:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026fd142135cccc902939200d9ef4958d0906f35ecd2e6281d78ea772bfbc263`  
		Last Modified: Mon, 12 Oct 2020 23:30:45 GMT  
		Size: 18.5 MB (18498753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc08ed7425d14c5f9a43044b3a0fda9cc0404dd2e47b1885aaa1dde677cb429b`  
		Last Modified: Mon, 12 Oct 2020 23:30:52 GMT  
		Size: 56.0 MB (55950293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee31f98cc7d6171c1cf63c3d64d534a21f96dd0f8c51b16e641fd4b0e081e1d`  
		Last Modified: Mon, 12 Oct 2020 23:30:42 GMT  
		Size: 1.5 KB (1546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa6bdf439054511291388a32d93c4c9b9226afa4633b44cd8044ab9c7b5ac1c`  
		Last Modified: Mon, 12 Oct 2020 23:30:42 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef8e1eaeebdede0689bfcf5c45b8c3ef26388b535e1a4154bf245f9f19e4705`  
		Last Modified: Mon, 12 Oct 2020 23:30:42 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b8e9f0e4c69ddb2a653381a51ed85851aa0f81fffcd7e1bb4ddd5e43014666`  
		Last Modified: Mon, 12 Oct 2020 23:30:45 GMT  
		Size: 8.1 MB (8137888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f371c8ee58424503974b0cb045958d785aedb4657d990dea7f97683d394a09`  
		Last Modified: Mon, 12 Oct 2020 23:30:42 GMT  
		Size: 4.5 KB (4542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
