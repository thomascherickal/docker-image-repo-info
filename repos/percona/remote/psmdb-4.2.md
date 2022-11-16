## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:64603942a24c6a8caeeb36e785c0ba1b94a39c8879865b679cc45b491e71645b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:25cb9c545b5744709f56500a8ab01f384b06e981159f9247c3079a38a22811ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.9 MB (177857556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9442358cb9c71e68e0898bd43707dba9f256f15c95ac40bc88a5ec17ecc73f9f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 16 Nov 2022 07:52:18 GMT
ADD file:95e25b6cc4a22c4ecb537bc949b3636ae408264d293c1c32a3ad180e54f80ae9 in / 
# Wed, 16 Nov 2022 07:52:19 GMT
CMD ["/bin/bash"]
# Wed, 16 Nov 2022 08:52:25 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 16 Nov 2022 08:55:50 GMT
ENV PSMDB_VERSION=4.2.21-21
# Wed, 16 Nov 2022 08:55:50 GMT
ENV OS_VER=el8
# Wed, 16 Nov 2022 08:55:50 GMT
ENV FULL_PERCONA_VERSION=4.2.21-21.el8
# Wed, 16 Nov 2022 08:55:50 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 16 Nov 2022 08:55:53 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Wed, 16 Nov 2022 08:56:29 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 16 Nov 2022 08:56:30 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 16 Nov 2022 08:56:30 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 16 Nov 2022 08:56:30 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 16 Nov 2022 08:56:31 GMT
ENV GOSU_VERSION=1.11
# Wed, 16 Nov 2022 08:56:33 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 16 Nov 2022 08:56:37 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 16 Nov 2022 08:56:37 GMT
VOLUME [/data/db]
# Wed, 16 Nov 2022 08:56:37 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Wed, 16 Nov 2022 08:56:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 08:56:37 GMT
EXPOSE 27017
# Wed, 16 Nov 2022 08:56:37 GMT
USER 1001
# Wed, 16 Nov 2022 08:56:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:df958f680f30541ef9f464f2f49bd4366e5904477b5ca521a78a4c68db2aa858`  
		Last Modified: Wed, 16 Nov 2022 07:53:09 GMT  
		Size: 87.4 MB (87435022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c722957e212954222d1b494fbff4cc74b3ac66db19f8f5e140cd3cb0e422216a`  
		Last Modified: Wed, 16 Nov 2022 08:59:39 GMT  
		Size: 3.8 MB (3767694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448399e3c034ac8c91975047de8a2c8261d3a8b84c9a05ca56c4ddef7f487e2e`  
		Last Modified: Wed, 16 Nov 2022 08:59:48 GMT  
		Size: 77.6 MB (77581994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd5fc0fc78734de737398440b8ac2c3d9b6415efeef96d82c7a3b2b805d06fe`  
		Last Modified: Wed, 16 Nov 2022 08:59:38 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4af81d982fe4e6cf775db76c43ba358eb11ba12fade2c6771ba3638ec8af82`  
		Last Modified: Wed, 16 Nov 2022 08:59:36 GMT  
		Size: 4.1 KB (4101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b33560d47d38d4cede3bb1944dcb78154185f1063912c380f4523a1af7cdcee`  
		Last Modified: Wed, 16 Nov 2022 08:59:36 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6fa2f68e73336e07dedbe7278e89383e05282a1f23ce479a91c9588d1391ef0`  
		Last Modified: Wed, 16 Nov 2022 08:59:36 GMT  
		Size: 914.6 KB (914552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803af0ec48c9a69d81f45ff9099b6801c9652a25d5d26b90afdea5c49173d69e`  
		Last Modified: Wed, 16 Nov 2022 08:59:37 GMT  
		Size: 8.1 MB (8137893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c75d276e7471a643523e10ba34502edd7316253770589871159873eaa50122a`  
		Last Modified: Wed, 16 Nov 2022 08:59:36 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
