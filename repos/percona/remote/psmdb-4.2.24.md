## `percona:psmdb-4.2.24`

```console
$ docker pull percona@sha256:417a33e5efa24d070b09fb98686b87855a4407996e444bd0969e41d9d648e14e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2.24` - linux; amd64

```console
$ docker pull percona@sha256:9bf13f930154fb98ac8eb383ff4cb474b0c5e55e9f06d5bd61bd351e614e3ad9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.0 MB (218982875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96d6b644c893ebc4931a60b83039bd095a5e08478a77483afd5defe634249ae7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 21:00:21 GMT
ENV PSMDB_VERSION=4.2.24-24
# Wed, 19 Jul 2023 21:00:21 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 21:00:21 GMT
ENV FULL_PERCONA_VERSION=4.2.24-24.el8
# Wed, 19 Jul 2023 21:00:21 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 19 Jul 2023 21:00:21 GMT
ENV PSMDB_REPO=release
# Wed, 19 Jul 2023 21:00:24 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 19 Jul 2023 21:01:18 GMT
RUN set -ex;     percona-release enable psmdb-42 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 19 Jul 2023 21:01:19 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Wed, 19 Jul 2023 21:01:19 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 19 Jul 2023 21:01:19 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 19 Jul 2023 21:01:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 19 Jul 2023 21:01:22 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 19 Jul 2023 21:01:24 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -;     rm -f /tmp/SHA256SUMS;     chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 19 Jul 2023 21:01:24 GMT
VOLUME [/data/db]
# Wed, 19 Jul 2023 21:01:24 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Wed, 19 Jul 2023 21:01:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Jul 2023 21:01:25 GMT
EXPOSE 27017
# Wed, 19 Jul 2023 21:01:25 GMT
USER 1001
# Wed, 19 Jul 2023 21:01:25 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e9678bb5b7740544ef9b6e0adaf854ae190ff342cd33800e36552209b9afaf`  
		Last Modified: Wed, 19 Jul 2023 21:04:19 GMT  
		Size: 3.8 MB (3780726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e79f0731191b7de3b22ba64651251cbe013e731edaedacfbb1ffa162bca5164`  
		Last Modified: Wed, 19 Jul 2023 21:04:34 GMT  
		Size: 117.2 MB (117246830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cecf075293fa1b5edd9fa3857a3608f971d8dfeeaf99d24e6dd8bb43d1f1bbe`  
		Last Modified: Wed, 19 Jul 2023 21:04:19 GMT  
		Size: 1.7 KB (1674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dece26f0a5a06f593068ae57a27dac26d29cddfdbb432de7c7a4594979ede15`  
		Last Modified: Wed, 19 Jul 2023 21:04:17 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797db8c8348c835d01a7290c086fb7b29d5a0fddc16b7447b49456bf42e6c1a3`  
		Last Modified: Wed, 19 Jul 2023 21:04:17 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56511a35297055062106a03d16897e06ca36ce82e68384a91eebce60dc9445f9`  
		Last Modified: Wed, 19 Jul 2023 21:04:17 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1458c80147cf317e35fd4232c27d6ac19dfe40a39fa9037bcba5e014c8f21d`  
		Last Modified: Wed, 19 Jul 2023 21:04:18 GMT  
		Size: 8.2 MB (8151466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26833b6f777712a761f1b53a7a16fd211827b0d7330335b0fe583409906cf4e7`  
		Last Modified: Wed, 19 Jul 2023 21:04:17 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
