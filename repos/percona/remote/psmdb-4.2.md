## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:64b0fb28fdc9c9e5fa39cbb010288c005c98165af4734c6cea14bac3df38b3fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:cd5282bd064d8462ef2cfb3113b1d4011e782e0223632652af383096ada18fd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.3 MB (175257559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8587f5bce652f5ac53df6aa9b822410952b99e3aa7ee50702dfa58b6b6efdf6e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 30 Aug 2022 21:20:24 GMT
ADD file:89b329a9c0e7f31e805663a6efe50c116e65ed0b9ebe1afa97f66b3c29c95980 in / 
# Tue, 30 Aug 2022 21:20:25 GMT
CMD ["/bin/bash"]
# Tue, 30 Aug 2022 21:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 30 Aug 2022 21:43:12 GMT
ENV PSMDB_VERSION=4.2.21-21
# Tue, 30 Aug 2022 21:43:12 GMT
ENV OS_VER=el8
# Tue, 30 Aug 2022 21:43:12 GMT
ENV FULL_PERCONA_VERSION=4.2.21-21.el8
# Tue, 30 Aug 2022 21:43:12 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 30 Aug 2022 21:43:15 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Tue, 30 Aug 2022 21:43:50 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Tue, 30 Aug 2022 21:43:51 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 30 Aug 2022 21:43:51 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 30 Aug 2022 21:43:51 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 30 Aug 2022 21:43:52 GMT
ENV GOSU_VERSION=1.11
# Tue, 30 Aug 2022 21:43:54 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Tue, 30 Aug 2022 21:43:56 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 30 Aug 2022 21:43:56 GMT
VOLUME [/data/db]
# Tue, 30 Aug 2022 21:43:56 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Tue, 30 Aug 2022 21:43:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Aug 2022 21:43:57 GMT
EXPOSE 27017
# Tue, 30 Aug 2022 21:43:57 GMT
USER 1001
# Tue, 30 Aug 2022 21:43:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7266c81ed91338580bd46dbd5ea0787661dc5b416c63ed01711df0b108c861a4`  
		Last Modified: Tue, 30 Aug 2022 21:21:17 GMT  
		Size: 84.9 MB (84864369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed72fbd0aaf314115ee48efbf508283df2c1b8b35ef783ce008b53160ebedfd`  
		Last Modified: Tue, 30 Aug 2022 21:46:38 GMT  
		Size: 3.8 MB (3750907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c13cfa67f41b5b985d038f183163ad348e5bc528338f6257ecbc6b724cef4b8`  
		Last Modified: Tue, 30 Aug 2022 21:46:47 GMT  
		Size: 77.6 MB (77569433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d206a3bc6642f698b6b3c5d29fb512dd672ebb56a0ada1d335ed2c65aa55c2e3`  
		Last Modified: Tue, 30 Aug 2022 21:46:37 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2ff90ad49bb9b6b73bc1546c4408f67d33c502d406cbc98ccb11fc8e1215e1`  
		Last Modified: Tue, 30 Aug 2022 21:46:35 GMT  
		Size: 4.1 KB (4101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174650f582a9bda5e75393c64cb60bc55b20e13737e6aafbadff655f6fed0d31`  
		Last Modified: Tue, 30 Aug 2022 21:46:35 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f50384f068f4c6f3ccaa6b041291e18b9c964e3d103ea56e08bb3ebe058ea1`  
		Last Modified: Tue, 30 Aug 2022 21:46:36 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14417696923614570c676a0a5601a1c2b9ae10b702972a1c9e94b558b86119dd`  
		Last Modified: Tue, 30 Aug 2022 21:46:37 GMT  
		Size: 8.1 MB (8137897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbba97e4612e039f6a225579f1d87758a86d496a318d4cb003455956f6404873`  
		Last Modified: Tue, 30 Aug 2022 21:46:35 GMT  
		Size: 4.6 KB (4556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
