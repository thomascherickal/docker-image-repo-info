## `percona:psmdb-4.4`

```console
$ docker pull percona@sha256:c239705bfb45d3d82192f25b0fc26a8852328d0582abe475e5a3448e30174aae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4` - linux; amd64

```console
$ docker pull percona@sha256:7a31f81f96296323ff033ba015cbdd8ab5654d604712a7c02939582861fb0d22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.6 MB (237595900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1977141cc927400819649d21421f58fa3c0b84847ac1d1118d5a905a128e33f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:38:43 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 05 Aug 2023 02:40:59 GMT
ENV PSMDB_VERSION=4.4.22-21
# Sat, 05 Aug 2023 02:40:59 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:40:59 GMT
ENV FULL_PERCONA_VERSION=4.4.22-21.el8
# Sat, 05 Aug 2023 02:40:59 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 05 Aug 2023 02:41:00 GMT
ENV PSMDB_REPO=release
# Sat, 05 Aug 2023 02:41:48 GMT
RUN set -ex;     percona-release enable psmdb-44 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 05 Aug 2023 02:41:49 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 05 Aug 2023 02:41:49 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 05 Aug 2023 02:41:49 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 05 Aug 2023 02:41:49 GMT
ENV GOSU_VERSION=1.11
# Sat, 05 Aug 2023 02:41:52 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 05 Aug 2023 02:41:54 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 05 Aug 2023 02:41:54 GMT
VOLUME [/data/db]
# Sat, 05 Aug 2023 02:41:54 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 05 Aug 2023 02:41:54 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Sat, 05 Aug 2023 02:41:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Aug 2023 02:41:54 GMT
EXPOSE 27017
# Sat, 05 Aug 2023 02:41:55 GMT
USER 1001
# Sat, 05 Aug 2023 02:41:55 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57009482fd55816f25227289cfc8b0a086fd3aecb1118cd78296a2812242a3ca`  
		Last Modified: Sat, 05 Aug 2023 02:45:04 GMT  
		Size: 3.8 MB (3790449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95079a3fccb2584b90e99d03c94ff892f7fa90ce47f053bf752dec80125a6fd0`  
		Last Modified: Sat, 05 Aug 2023 02:46:20 GMT  
		Size: 135.8 MB (135797189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c94088d172c64026a14b18b1be0de57bfe497ddebb4788b8d39c3e729e14085`  
		Last Modified: Sat, 05 Aug 2023 02:46:02 GMT  
		Size: 1.7 KB (1670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e0c1586df59510cd3716c2a61fed1258eccba381e591b58942cbddb577af77`  
		Last Modified: Sat, 05 Aug 2023 02:46:02 GMT  
		Size: 4.1 KB (4098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec741bb4f4c876f1d8340ce35a258a1d92fc80b7e4517be721f6f12d54d1484`  
		Last Modified: Sat, 05 Aug 2023 02:46:00 GMT  
		Size: 10.6 KB (10572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a59c6d7e5d11dc766bd0bb9e9e7e45cbf5ab33c25d1e5e679a301ad98fd6315`  
		Last Modified: Sat, 05 Aug 2023 02:46:00 GMT  
		Size: 914.5 KB (914541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e81ec4631c520e4e2de7bc046ac14a05fa9020321bea3dc2e73712df76a93cb`  
		Last Modified: Sat, 05 Aug 2023 02:46:01 GMT  
		Size: 8.1 MB (8137881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4442fac3f7f7776ebd35c06e49abd3e92c873983b0f1beedbc294b8076a69436`  
		Last Modified: Sat, 05 Aug 2023 02:46:00 GMT  
		Size: 13.2 KB (13203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe57b4cc3ec75b7e93ee684396b84fae979b66f5d974eef48a3808f41fed50ab`  
		Last Modified: Sat, 05 Aug 2023 02:46:00 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
