## `percona:psmdb-4.0.21`

```console
$ docker pull percona@sha256:f507e23047b740cf8a06afb83ae6f8217447f42e01bbc86f5e65b2fc089fac30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-4.0.21` - linux; amd64

```console
$ docker pull percona@sha256:36eef643c03a466091585ac095dbfb5fdec9b86557bf49b356e3e8d8a887ad5f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.5 MB (160494815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82735c0ba50a3f1f91e1c72af602b9dac32bd0ebdc582b455c771e0a40df909`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Mon, 16 Nov 2020 19:39:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 25 Nov 2020 01:53:33 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     dnf install -y /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-40 release
# Wed, 25 Nov 2020 01:53:34 GMT
ENV PSMDB_VERSION=4.0.21-15
# Wed, 25 Nov 2020 01:53:34 GMT
ENV OS_VER=el8
# Wed, 25 Nov 2020 01:53:34 GMT
ENV FULL_PERCONA_VERSION=4.0.21-15.el8
# Wed, 25 Nov 2020 01:53:35 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 25 Nov 2020 01:54:01 GMT
RUN set -ex;     dnf install -y         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         shadow-utils         curl         procps-ng         oniguruma         jq         dnf-utils;         repoquery -a --location         policycoreutils             | xargs curl -Lf -o /tmp/policycoreutils.rpm;     repoquery -a --location         percona-server-mongodb-server-${FULL_PERCONA_VERSION}             | xargs curl -Lf -o /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     rpm -iv /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm --nodeps;         rm -rf /tmp/policycoreutils.rpm /tmp/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.rpm;     dnf clean all;     dnf -y remove dnf-utils;     rm -rf /var/cache/dnf /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 25 Nov 2020 01:54:03 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 25 Nov 2020 01:54:03 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 25 Nov 2020 01:54:05 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 25 Nov 2020 01:54:05 GMT
ENV GOSU_VERSION=1.11
# Wed, 25 Nov 2020 01:54:09 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 25 Nov 2020 01:54:13 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 25 Nov 2020 01:54:13 GMT
VOLUME [/data/db]
# Wed, 25 Nov 2020 01:54:14 GMT
COPY file:36bd7798a7bd236f79a692385b6877519fd05ff40f92de87cb1d5c527c35d799 in /entrypoint.sh 
# Wed, 25 Nov 2020 01:54:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Nov 2020 01:54:14 GMT
EXPOSE 27017
# Wed, 25 Nov 2020 01:54:15 GMT
USER 1001
# Wed, 25 Nov 2020 01:54:15 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30199a0d1169e3b1a6084276700e5e994fdeb09aabe1be54821028d6484318e7`  
		Last Modified: Wed, 25 Nov 2020 01:55:12 GMT  
		Size: 18.5 MB (18495644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b421360427c3d8c1b67ded92b085ad422ada3311ea184d98082f3e3a90e8c320`  
		Last Modified: Wed, 25 Nov 2020 01:55:21 GMT  
		Size: 58.1 MB (58057878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1833e7fefec98fcd48747691f5333f694ba63db9ab47413908a996b07d4c2787`  
		Last Modified: Wed, 25 Nov 2020 01:55:10 GMT  
		Size: 1.5 KB (1546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4981fc3cbff9cd35b9de136108b42d822d809ea55228a9c4b790dfef9e135d0`  
		Last Modified: Wed, 25 Nov 2020 01:55:09 GMT  
		Size: 4.1 KB (4071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3536833245a595b102a3f32bf5ae5772e32113399cd615336fabe66b9e679a69`  
		Last Modified: Wed, 25 Nov 2020 01:55:08 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21365312d80276803a49972512a5dd7b43f2a23a689db22b211f27b03b5e1b78`  
		Last Modified: Wed, 25 Nov 2020 01:55:09 GMT  
		Size: 914.5 KB (914544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9522afddbb22f4fe863f498ae37733298f829c08d5894d7b2f96451c09f648fa`  
		Last Modified: Wed, 25 Nov 2020 01:55:10 GMT  
		Size: 8.1 MB (8137890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a1e7bb7c586e271ef9284eef0818c59cd9d15a24bb2bdac8f00a25a5a6e5ab`  
		Last Modified: Wed, 25 Nov 2020 01:55:08 GMT  
		Size: 4.5 KB (4543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
