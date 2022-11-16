## `percona:psmdb-4.4.15`

```console
$ docker pull percona@sha256:6ece8bf0a53feee8e22c390a74a4ed3958c770b468bae8851ed7f19c36d3edb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4.15` - linux; amd64

```console
$ docker pull percona@sha256:01fe4bc9f1a4dd561d2c9f9149798315fa4e20865e18a7f8af7f46ee51372642
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.2 MB (197175447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49bee36fa37e459270fe7fb4b484810d5f3138fdbebd899b6d681c88e2bed197`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 16 Nov 2022 07:52:18 GMT
ADD file:95e25b6cc4a22c4ecb537bc949b3636ae408264d293c1c32a3ad180e54f80ae9 in / 
# Wed, 16 Nov 2022 07:52:19 GMT
CMD ["/bin/bash"]
# Wed, 16 Nov 2022 08:52:25 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 16 Nov 2022 08:54:55 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Wed, 16 Nov 2022 08:54:55 GMT
ENV PSMDB_VERSION=4.4.15-15
# Wed, 16 Nov 2022 08:54:55 GMT
ENV OS_VER=el8
# Wed, 16 Nov 2022 08:54:55 GMT
ENV FULL_PERCONA_VERSION=4.4.15-15.el8
# Wed, 16 Nov 2022 08:54:55 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 16 Nov 2022 08:55:33 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 16 Nov 2022 08:55:34 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 16 Nov 2022 08:55:34 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 16 Nov 2022 08:55:35 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 16 Nov 2022 08:55:35 GMT
ENV GOSU_VERSION=1.11
# Wed, 16 Nov 2022 08:55:39 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 16 Nov 2022 08:55:42 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 16 Nov 2022 08:55:42 GMT
VOLUME [/data/db]
# Wed, 16 Nov 2022 08:55:43 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 16 Nov 2022 08:55:43 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Wed, 16 Nov 2022 08:55:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 08:55:43 GMT
EXPOSE 27017
# Wed, 16 Nov 2022 08:55:43 GMT
USER 1001
# Wed, 16 Nov 2022 08:55:44 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:df958f680f30541ef9f464f2f49bd4366e5904477b5ca521a78a4c68db2aa858`  
		Last Modified: Wed, 16 Nov 2022 07:53:09 GMT  
		Size: 87.4 MB (87435022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc279b5a84226f63d344b7d7230abfeecfaf210a4bad1271d8164d0ed25881e`  
		Last Modified: Wed, 16 Nov 2022 08:59:15 GMT  
		Size: 3.8 MB (3767707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc07e1f402d0ce613661d78a07ef9856868e821a7e98eb8dfb4e1b6a458e6b3`  
		Last Modified: Wed, 16 Nov 2022 08:59:26 GMT  
		Size: 96.9 MB (96886667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2ecaf72a5a15b9b44759222f57a521f422f5a13347b04d23d2c0c61892fae3`  
		Last Modified: Wed, 16 Nov 2022 08:59:14 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2bea338f2b9e81637d4e950e86d325f7fcdfdf634218c1b7c3c46964ef5111`  
		Last Modified: Wed, 16 Nov 2022 08:59:14 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e487a5b2d0b2b64af94e0d5b38e1a47ceadab964a9e2b9f8bc7df9d16e171db`  
		Last Modified: Wed, 16 Nov 2022 08:59:12 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad3dbe0e4fe9122823d09de2ad43c28a3119d2a57a951b6026e680fb3fdcd63`  
		Last Modified: Wed, 16 Nov 2022 08:59:13 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ceed0f4dd4c0dbd88a66d638b53ac014dba5f130be60969917b69f1592289d`  
		Last Modified: Wed, 16 Nov 2022 08:59:14 GMT  
		Size: 8.1 MB (8137890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb66a3691d53125bc4c60d6a9017ae3a445ae004b55570b3711036ad3211fca`  
		Last Modified: Wed, 16 Nov 2022 08:59:12 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f24d37c02462c83306e1cd4cb0c348b804b20378dd74a53f278440179afa7b`  
		Last Modified: Wed, 16 Nov 2022 08:59:12 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
