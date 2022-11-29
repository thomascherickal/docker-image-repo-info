## `percona:psmdb-5.0`

```console
$ docker pull percona@sha256:7d8360f591dd075f9819770a8cc5487487fc652b16e743ed2a65b65f6a2953dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0` - linux; amd64

```console
$ docker pull percona@sha256:ee0ca4bb3447b6f2d2fb3eb4997ff419bd4a7d222f183d05f53d650220e72200
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.6 MB (212584576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdde233e4b41619ed2d1d0db877836911547f0db31dd3adebb80a2bc055781a1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 29 Nov 2022 19:20:47 GMT
ADD file:0b5cd2f93e1c6f939d535c707f7dda5d950091382d18cdd7cf32ded784e057fc in / 
# Tue, 29 Nov 2022 19:20:48 GMT
CMD ["/bin/bash"]
# Tue, 29 Nov 2022 19:51:48 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 29 Nov 2022 19:53:20 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-50 release
# Tue, 29 Nov 2022 19:53:20 GMT
ENV PSMDB_VERSION=5.0.10-9
# Tue, 29 Nov 2022 19:53:21 GMT
ENV OS_VER=el8
# Tue, 29 Nov 2022 19:53:21 GMT
ENV FULL_PERCONA_VERSION=5.0.10-9.el8
# Tue, 29 Nov 2022 19:53:21 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 29 Nov 2022 19:54:01 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Tue, 29 Nov 2022 19:54:02 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 29 Nov 2022 19:54:02 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 29 Nov 2022 19:54:02 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 29 Nov 2022 19:54:02 GMT
ENV GOSU_VERSION=1.11
# Tue, 29 Nov 2022 19:54:06 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Tue, 29 Nov 2022 19:54:11 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 29 Nov 2022 19:54:11 GMT
VOLUME [/data/db]
# Tue, 29 Nov 2022 19:54:12 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Tue, 29 Nov 2022 19:54:12 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Tue, 29 Nov 2022 19:54:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Nov 2022 19:54:12 GMT
EXPOSE 27017
# Tue, 29 Nov 2022 19:54:13 GMT
USER 1001
# Tue, 29 Nov 2022 19:54:13 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d0409ace7ea3bb98342dc30153bf50a92eeb0872d0474ef4fb0eabf9aba2390c`  
		Last Modified: Tue, 29 Nov 2022 19:22:26 GMT  
		Size: 87.4 MB (87437780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c49cb05c0106634e61af804c476285c0db118793e7cae73dede775685297913`  
		Last Modified: Tue, 29 Nov 2022 19:57:40 GMT  
		Size: 3.8 MB (3774974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03c6c18da9ad7e47cc9f1827f8d537172afc36ffea18a0ab50a2ce7576e1c61`  
		Last Modified: Tue, 29 Nov 2022 19:57:52 GMT  
		Size: 112.3 MB (112285777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6ee551b9ad0ac601b43b4861741a5f33845d9a2fc5d873ec4671cc059c69e6`  
		Last Modified: Tue, 29 Nov 2022 19:57:38 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7161699fb9b87b4f9a547dc9e6df55e0b56182d80a62073fbc2064663f684c`  
		Last Modified: Tue, 29 Nov 2022 19:57:38 GMT  
		Size: 4.1 KB (4101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0aae5800814b272c0948b4230a6de556073556f384b0f5e2f16b6aa3dcbb57`  
		Last Modified: Tue, 29 Nov 2022 19:57:37 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f446193414d80df53beaf00fca5debb3bfeba160bbe40dcd8822f0d0d0e973ca`  
		Last Modified: Tue, 29 Nov 2022 19:57:37 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d949da2a92348229417dea7e08e8d0d9489dd7bbbb9214352d741b498c2efce`  
		Last Modified: Tue, 29 Nov 2022 19:57:38 GMT  
		Size: 8.1 MB (8137889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f20de6a9273cb4eeeb93996e6fa99810886d753246201faed28b1090a6c179e`  
		Last Modified: Tue, 29 Nov 2022 19:57:37 GMT  
		Size: 13.2 KB (13202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f26d33551c6ffad3353cab55f44325c9f1eb358f8bdbe4f8e44384c06fca96f`  
		Last Modified: Tue, 29 Nov 2022 19:57:36 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
