## `percona:psmdb-4.4.15`

```console
$ docker pull percona@sha256:e657d18472702da6004bb0902823c8b9ad3108cc6193ed89097df43329de5cbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4.15` - linux; amd64

```console
$ docker pull percona@sha256:ab90ebc8e1fae544f1a4733cac4d2d9daac3756fc4a012d88c2be60d9a25104b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.2 MB (197209511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d431e542f4ae7c5fe6f0c76657f34fea14a5e7549fdcd5f6f6f7a320038d03`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:14 GMT
ADD file:5a832f5300f589b7f2a820f29d0655906164c4946d5fcd467921017c28a26bee in / 
# Wed, 07 Dec 2022 01:51:15 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:14:45 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 07 Dec 2022 02:17:15 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Wed, 07 Dec 2022 02:17:15 GMT
ENV PSMDB_VERSION=4.4.15-15
# Wed, 07 Dec 2022 02:17:15 GMT
ENV OS_VER=el8
# Wed, 07 Dec 2022 02:17:15 GMT
ENV FULL_PERCONA_VERSION=4.4.15-15.el8
# Wed, 07 Dec 2022 02:17:15 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 07 Dec 2022 02:17:54 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 07 Dec 2022 02:17:55 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 07 Dec 2022 02:17:55 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 07 Dec 2022 02:17:55 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 07 Dec 2022 02:17:55 GMT
ENV GOSU_VERSION=1.11
# Wed, 07 Dec 2022 02:17:59 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 07 Dec 2022 02:18:01 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 07 Dec 2022 02:18:01 GMT
VOLUME [/data/db]
# Wed, 07 Dec 2022 02:18:02 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 07 Dec 2022 02:18:02 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Wed, 07 Dec 2022 02:18:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 07 Dec 2022 02:18:02 GMT
EXPOSE 27017
# Wed, 07 Dec 2022 02:18:02 GMT
USER 1001
# Wed, 07 Dec 2022 02:18:02 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4c770e098606ecfd5b78f4d61fc5e11b92fdde43d07825e543f04fe64aaa62eb`  
		Last Modified: Wed, 07 Dec 2022 01:52:57 GMT  
		Size: 87.4 MB (87445275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b87caba5d450bedc5f577f79e35433ae14506eaf199b3f8d6b46a2527f792e`  
		Last Modified: Wed, 07 Dec 2022 02:21:06 GMT  
		Size: 3.8 MB (3778985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6534f6b02c4c1b90dbe692a4736c9f30983e46b99883d97c5fbd22b3f28dcd3a`  
		Last Modified: Wed, 07 Dec 2022 02:21:17 GMT  
		Size: 96.9 MB (96899205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28562ced64a9a1726a553799cddaa6334140ac0e4e03cf53c91c43a75933a99d`  
		Last Modified: Wed, 07 Dec 2022 02:21:05 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4d9bba7b2170b29bafac0d90fd59abff6a1b3db2fa9c90aa9aee89d764dd7c`  
		Last Modified: Wed, 07 Dec 2022 02:21:05 GMT  
		Size: 4.1 KB (4102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c38d66642c21f71fc2aca01355c7f00f30cebeb79893cf5fe4f0f25584cfaa`  
		Last Modified: Wed, 07 Dec 2022 02:21:03 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8817f90fd06efef2d240831bc58f12e2fec20e7d7f6edcca40bf88730cd684a0`  
		Last Modified: Wed, 07 Dec 2022 02:21:03 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e20db943aacafccf227f8bacabdd497860f80b2afa48fd43141598215ceff6`  
		Last Modified: Wed, 07 Dec 2022 02:21:05 GMT  
		Size: 8.1 MB (8137886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afc8c7acbb0807906c77f2ec40b8143515a43f5da5e5448e5d963e4d5610583`  
		Last Modified: Wed, 07 Dec 2022 02:21:03 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849fc920ffcced490f7a19cf15e37930a2f9fd466e9f88f76f5e3335a2865cd4`  
		Last Modified: Wed, 07 Dec 2022 02:21:03 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
