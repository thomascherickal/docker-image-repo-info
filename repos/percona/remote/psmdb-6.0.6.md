## `percona:psmdb-6.0.6`

```console
$ docker pull percona@sha256:e441d67543960d0bc89653ed0f6b862308e5630f4afa448e57208e2aba0dd571
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-6.0.6` - linux; amd64

```console
$ docker pull percona@sha256:9171645f625909cb21cdfe4f9a82c764db0c56a5e867d35124b71b4bd4030c79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.3 MB (273255826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c80a33a0620016638ccbbf4d6502980a515ebad6e92c28160fbc24b7e58f331`
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
# Sat, 05 Aug 2023 02:38:43 GMT
ENV PSMDB_VERSION=6.0.6-5
# Sat, 05 Aug 2023 02:38:43 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:38:43 GMT
ENV FULL_PERCONA_VERSION=6.0.6-5.el8
# Sat, 05 Aug 2023 02:38:43 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 05 Aug 2023 02:38:44 GMT
ENV PSMDB_REPO=release
# Sat, 05 Aug 2023 02:39:35 GMT
RUN set -ex;     percona-release enable psmdb-60 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         percona-mongodb-mongosh         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-60/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 05 Aug 2023 02:39:36 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 05 Aug 2023 02:39:36 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 05 Aug 2023 02:39:37 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 05 Aug 2023 02:39:37 GMT
ENV GOSU_VERSION=1.11
# Sat, 05 Aug 2023 02:39:40 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 05 Aug 2023 02:39:43 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 05 Aug 2023 02:39:43 GMT
VOLUME [/data/db]
# Sat, 05 Aug 2023 02:39:44 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 05 Aug 2023 02:39:44 GMT
COPY file:7ab35f422fd362616b84e1dc71329cc9be05b7f834182c48bf98ceb92ee28956 in /entrypoint.sh 
# Sat, 05 Aug 2023 02:39:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Aug 2023 02:39:44 GMT
EXPOSE 27017
# Sat, 05 Aug 2023 02:39:44 GMT
USER 1001
# Sat, 05 Aug 2023 02:39:44 GMT
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
	-	`sha256:aada92cc74feabd7f036fa62e92d7486494fd7eeb32169853eac63d89d6cc335`  
		Last Modified: Sat, 05 Aug 2023 02:45:22 GMT  
		Size: 171.5 MB (171457076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04091c0a0ca708cb0ba5127fd18ab25fbad57b6735a713e8888add8aff01b73`  
		Last Modified: Sat, 05 Aug 2023 02:45:03 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f53c502f4e69265cde9d852c4c107370c73890d5f6c4e04e68775e54764320`  
		Last Modified: Sat, 05 Aug 2023 02:45:02 GMT  
		Size: 4.1 KB (4101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d680fb10eb2b8edb9087f6b54e0cbda82b44c99d7e5b8c96af70ca5ac109af65`  
		Last Modified: Sat, 05 Aug 2023 02:45:00 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1d81e265209e98a17d5a2bd518098eafed7b24a37e0db6200be56cdcec6eef`  
		Last Modified: Sat, 05 Aug 2023 02:45:01 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b298a09d7027f47a37aae68afd38aab9540bc2730aff175879fcb54455099146`  
		Last Modified: Sat, 05 Aug 2023 02:45:02 GMT  
		Size: 8.1 MB (8137886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5d18c9bb10f213c9777681b384dc42ef80aaa2001307b3ec9fff2a7362b675`  
		Last Modified: Sat, 05 Aug 2023 02:45:00 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fde879b52bc4bb68759c5dfe55bc96ed550e74f89b87a50e51c12effa26c787`  
		Last Modified: Sat, 05 Aug 2023 02:45:00 GMT  
		Size: 4.6 KB (4567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
