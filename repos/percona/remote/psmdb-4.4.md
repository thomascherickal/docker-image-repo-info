## `percona:psmdb-4.4`

```console
$ docker pull percona@sha256:f09d8b27b4f0692f79a8ee09e3e1cb0e369838f4dc36db9e8a58b9ef7f7eedd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4` - linux; amd64

```console
$ docker pull percona@sha256:ebcdbe61cab0d70e5da771d522a29f50d2dcc4b3290a52ca29d9df044ef127f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.5 MB (237524598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f05044b9788877ed284ee63ffb72151acccd2493a1dc4a3e22dd1f0ee1703c8b`
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
# Wed, 19 Jul 2023 20:59:11 GMT
ENV PSMDB_VERSION=4.4.22-21
# Wed, 19 Jul 2023 20:59:11 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:59:11 GMT
ENV FULL_PERCONA_VERSION=4.4.22-21.el8
# Wed, 19 Jul 2023 20:59:11 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 19 Jul 2023 20:59:11 GMT
ENV PSMDB_REPO=release
# Wed, 19 Jul 2023 21:00:06 GMT
RUN set -ex;     percona-release enable psmdb-44 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 19 Jul 2023 21:00:07 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Wed, 19 Jul 2023 21:00:07 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 19 Jul 2023 21:00:08 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 19 Jul 2023 21:00:08 GMT
ENV GOSU_VERSION=1.11
# Wed, 19 Jul 2023 21:00:11 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 19 Jul 2023 21:00:13 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 19 Jul 2023 21:00:13 GMT
VOLUME [/data/db]
# Wed, 19 Jul 2023 21:00:14 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 19 Jul 2023 21:00:14 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Wed, 19 Jul 2023 21:00:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Jul 2023 21:00:14 GMT
EXPOSE 27017
# Wed, 19 Jul 2023 21:00:14 GMT
USER 1001
# Wed, 19 Jul 2023 21:00:14 GMT
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
	-	`sha256:fc48270b12b6e8573229e85e54544765d38c5f1a5961123410a222fc68bf7246`  
		Last Modified: Wed, 19 Jul 2023 21:04:07 GMT  
		Size: 135.8 MB (135788927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522371c78b2da0c8d2d9da9e905d8a8e52a8f3dc35f8b743216d496062277025`  
		Last Modified: Wed, 19 Jul 2023 21:03:47 GMT  
		Size: 1.7 KB (1674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd5d48230675b0a33ac2c53354e00b5b6e441080cd6d6bfd7f90ffde89c391e`  
		Last Modified: Wed, 19 Jul 2023 21:03:47 GMT  
		Size: 4.1 KB (4102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0993c9297f19c4f1d108dc25cc516edf0bf734e0a2c82f89175b6d5239c2546a`  
		Last Modified: Wed, 19 Jul 2023 21:03:45 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558c1170e1df3360a090b3368c37cf155fbb0453a8cda4462ddefb273b7b46c8`  
		Last Modified: Wed, 19 Jul 2023 21:03:45 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730cf5236bbe8cab26bea91c358ec7d20b63ab39ffa77743875b2808d46b1284`  
		Last Modified: Wed, 19 Jul 2023 21:03:46 GMT  
		Size: 8.1 MB (8137888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688e3eec3c26f684042cce2cb26673808cee58dd28170b2aed5b513a4132764b`  
		Last Modified: Wed, 19 Jul 2023 21:03:45 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86519eb4bcbe8b48013addf85cee05112506ad5f03c6b17eb3bb61ab5e74b31a`  
		Last Modified: Wed, 19 Jul 2023 21:03:45 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
