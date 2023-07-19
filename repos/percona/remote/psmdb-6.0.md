## `percona:psmdb-6.0`

```console
$ docker pull percona@sha256:5bb1c8564947411895126da1fcfadadc30364bc2b214afe88e8c41305f49821a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-6.0` - linux; amd64

```console
$ docker pull percona@sha256:7f91269828cc2ed58d8fe8210b5aa6a1645d4a240d9384aeb6a76fef21a2c439
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.2 MB (273186119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e37c582bb7788d9ecc2d37753578bd9af9aeebad57479b20892f7cf4b1b5834c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:56:40 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 19 Jul 2023 20:56:40 GMT
ENV PSMDB_VERSION=6.0.6-5
# Wed, 19 Jul 2023 20:56:40 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:56:40 GMT
ENV FULL_PERCONA_VERSION=6.0.6-5.el8
# Wed, 19 Jul 2023 20:56:40 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 19 Jul 2023 20:56:40 GMT
ENV PSMDB_REPO=release
# Wed, 19 Jul 2023 20:57:39 GMT
RUN set -ex;     percona-release enable psmdb-60 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         percona-mongodb-mongosh         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-60/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 19 Jul 2023 20:57:41 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Wed, 19 Jul 2023 20:57:41 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 19 Jul 2023 20:57:41 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 19 Jul 2023 20:57:41 GMT
ENV GOSU_VERSION=1.11
# Wed, 19 Jul 2023 20:57:45 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 19 Jul 2023 20:57:47 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 19 Jul 2023 20:57:48 GMT
VOLUME [/data/db]
# Wed, 19 Jul 2023 20:57:48 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 19 Jul 2023 20:57:49 GMT
COPY file:7ab35f422fd362616b84e1dc71329cc9be05b7f834182c48bf98ceb92ee28956 in /entrypoint.sh 
# Wed, 19 Jul 2023 20:57:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Jul 2023 20:57:49 GMT
EXPOSE 27017
# Wed, 19 Jul 2023 20:57:49 GMT
USER 1001
# Wed, 19 Jul 2023 20:57:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfeeb16bf8999edb45d62d837e2ffada6ed220395b6a998d1464045211c00cb`  
		Last Modified: Wed, 19 Jul 2023 21:02:46 GMT  
		Size: 3.8 MB (3780725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316344c17489e6f24318a372aeabb2d69181e56930416ad2cada081290cadd50`  
		Last Modified: Wed, 19 Jul 2023 21:03:06 GMT  
		Size: 171.5 MB (171450441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92094b053c0f1f80800052550f0e6f3f6988f148b2c80b4c51f2a8878f465623`  
		Last Modified: Wed, 19 Jul 2023 21:02:44 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41275153d1746fbbe646d3bf79dc294d80b55de662b194e0d43e999719748e22`  
		Last Modified: Wed, 19 Jul 2023 21:02:44 GMT  
		Size: 4.1 KB (4100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3795d4cc5379a200b3afdca151e3ddabb483e87f95b83c918f5d2a9f19897a60`  
		Last Modified: Wed, 19 Jul 2023 21:02:43 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3312a928ce66eda2f07167075f8088f2a8f3c02f18e57b250794f13765a557d6`  
		Last Modified: Wed, 19 Jul 2023 21:02:43 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a1b596804d4930da784910045c7117c486912da3f5e9d1887d7219c7393227`  
		Last Modified: Wed, 19 Jul 2023 21:02:44 GMT  
		Size: 8.1 MB (8137887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f651bbf31dce44f34e25d7fffe16390f36c2838563751c1c4607b38a56bb33ba`  
		Last Modified: Wed, 19 Jul 2023 21:02:42 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad0fd0917bc890a07ed660e7ae80ad226dae255264663ed603ef832d22a8776`  
		Last Modified: Wed, 19 Jul 2023 21:02:43 GMT  
		Size: 4.6 KB (4566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
