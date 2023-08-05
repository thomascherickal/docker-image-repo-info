## `percona:psmdb-5.0.18`

```console
$ docker pull percona@sha256:eb5079ffe9e7a01187687e1a2ec18a07b814d583693885ac41bcb5353cb6584e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0.18` - linux; amd64

```console
$ docker pull percona@sha256:a157dce551d689ecaab2c3126142ef4e1dbca79e08624646cc08dd8d8edd8498
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.2 MB (250204467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61397b95e994a12ab05f0bb6e007a48cb82dbafe4fca0ab2589258bc5f809d1`
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
# Sat, 05 Aug 2023 02:39:49 GMT
ENV PSMDB_VERSION=5.0.18-15
# Sat, 05 Aug 2023 02:39:49 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:39:49 GMT
ENV FULL_PERCONA_VERSION=5.0.18-15.el8
# Sat, 05 Aug 2023 02:39:49 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 05 Aug 2023 02:39:49 GMT
ENV PSMDB_REPO=release
# Sat, 05 Aug 2023 02:40:38 GMT
RUN set -ex;     percona-release enable psmdb-50 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 05 Aug 2023 02:40:39 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 05 Aug 2023 02:40:39 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 05 Aug 2023 02:40:39 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 05 Aug 2023 02:40:40 GMT
ENV GOSU_VERSION=1.11
# Sat, 05 Aug 2023 02:40:43 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 05 Aug 2023 02:40:45 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 05 Aug 2023 02:40:45 GMT
VOLUME [/data/db]
# Sat, 05 Aug 2023 02:40:46 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 05 Aug 2023 02:40:46 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Sat, 05 Aug 2023 02:40:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Aug 2023 02:40:46 GMT
EXPOSE 27017
# Sat, 05 Aug 2023 02:40:46 GMT
USER 1001
# Sat, 05 Aug 2023 02:40:46 GMT
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
	-	`sha256:6cd92c276efa8e5b68b5b7fcecf6b58f4b7a20a6776d915b86975073cecb2822`  
		Last Modified: Sat, 05 Aug 2023 02:45:50 GMT  
		Size: 148.4 MB (148405720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f461e81d9f3700256e8b65d37bee411185b2ca5a1b3feff8a1d9b779c1e75b`  
		Last Modified: Sat, 05 Aug 2023 02:45:33 GMT  
		Size: 1.7 KB (1673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070f0d0b1c680ccf52cd9079aa3802ea0f39a5c34463143461c913bae028c3f2`  
		Last Modified: Sat, 05 Aug 2023 02:45:33 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e69f8b607deab0b234a92af126c63835c3b61f0d41f395e19623238991dd84`  
		Last Modified: Sat, 05 Aug 2023 02:45:31 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1cb4bea1eae352c8e86f6630ce34409b909aa021fe6cfd4b7c92e15297e7813`  
		Last Modified: Sat, 05 Aug 2023 02:45:31 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b92eb86ae980fb67b38d8230bdeeee45effe10199bab48b8d6fa73c8b788b`  
		Last Modified: Sat, 05 Aug 2023 02:45:33 GMT  
		Size: 8.1 MB (8137890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93c8d9477c278503c5bb8709cde113949dd5934e286b7bdc5a2d8f80f85ea09`  
		Last Modified: Sat, 05 Aug 2023 02:45:31 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18bd184a5acad57f4c6fba34f6871f9eeb6778de66a16d70cbd08c6e84da28b`  
		Last Modified: Sat, 05 Aug 2023 02:45:31 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
