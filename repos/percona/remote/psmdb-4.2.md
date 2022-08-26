## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:6ca4ec820ee99b9b32c9cd0bea8403631a5650b590d76587a7bb1f587bfea97b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:c875aea2841feef6ebe5786ef4bf91a922dc292e20617d69757ae93ec2a72f2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.3 MB (175255241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff9f7ae0ea9f4b119eba94f2413d404bf7af16f1013a55407779e77324ae8f32`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 26 Aug 2022 21:25:47 GMT
ADD file:67ab7eee8368c5d1cd71a8cfac5ea227da5b36ae49291c75dadb87506b1f1195 in / 
# Fri, 26 Aug 2022 21:25:48 GMT
CMD ["/bin/bash"]
# Fri, 26 Aug 2022 21:58:56 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 26 Aug 2022 22:02:21 GMT
ENV PSMDB_VERSION=4.2.21-21
# Fri, 26 Aug 2022 22:02:21 GMT
ENV OS_VER=el8
# Fri, 26 Aug 2022 22:02:21 GMT
ENV FULL_PERCONA_VERSION=4.2.21-21.el8
# Fri, 26 Aug 2022 22:02:21 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Fri, 26 Aug 2022 22:02:24 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Fri, 26 Aug 2022 22:02:58 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Fri, 26 Aug 2022 22:02:59 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Fri, 26 Aug 2022 22:02:59 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Fri, 26 Aug 2022 22:02:59 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Fri, 26 Aug 2022 22:03:00 GMT
ENV GOSU_VERSION=1.11
# Fri, 26 Aug 2022 22:03:02 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Fri, 26 Aug 2022 22:03:04 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Fri, 26 Aug 2022 22:03:04 GMT
VOLUME [/data/db]
# Fri, 26 Aug 2022 22:03:04 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Fri, 26 Aug 2022 22:03:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Aug 2022 22:03:05 GMT
EXPOSE 27017
# Fri, 26 Aug 2022 22:03:05 GMT
USER 1001
# Fri, 26 Aug 2022 22:03:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2c825b6c4689f5d76258b0f0f7f6a1e27cbbd03f813bf02abeca31d54bcc9fcf`  
		Last Modified: Fri, 26 Aug 2022 21:27:24 GMT  
		Size: 84.9 MB (84863365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd2a3269da2a46c6c59714c1a5a3a2b6cabcc91fc87e7494fb8be4f99068fcc`  
		Last Modified: Fri, 26 Aug 2022 22:05:43 GMT  
		Size: 3.7 MB (3749715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997716fa371bb4829e1dcc0cabd01c7d1e5359796ed16de11390e2b5576cccec`  
		Last Modified: Fri, 26 Aug 2022 22:05:52 GMT  
		Size: 77.6 MB (77569312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93eb31b6e8c371a5568d9df91710d7c285881b01881d48c80c9a835d96526277`  
		Last Modified: Fri, 26 Aug 2022 22:05:42 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb03d3cf9a143f5b6fe5b29bdab8604c0724e1100539619b973ae9ee49fe3adb`  
		Last Modified: Fri, 26 Aug 2022 22:05:40 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941f40c8e7476658e5225e3c18722a2dd138b53f28afc0fa3418a39353506cfb`  
		Last Modified: Fri, 26 Aug 2022 22:05:40 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed62646d6ac6f916d3c36a36af9b9edf54b0e817385349b8c0e0a48f150bcc1`  
		Last Modified: Fri, 26 Aug 2022 22:05:40 GMT  
		Size: 914.5 KB (914546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97157d087be64b9b146cf67b5a5f2aa1d640e16691ee03a1d885d454d5a88bc7`  
		Last Modified: Fri, 26 Aug 2022 22:05:42 GMT  
		Size: 8.1 MB (8137892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038559138e0aebe7ba002c2a79e947416e8079cd957c5302eba11384c9a3878b`  
		Last Modified: Fri, 26 Aug 2022 22:05:40 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
