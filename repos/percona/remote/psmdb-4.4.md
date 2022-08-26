## `percona:psmdb-4.4`

```console
$ docker pull percona@sha256:81d71238f88e31fe0faea3591bfbc660d6442637bfae1acd21f4122cf27b9abf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4` - linux; amd64

```console
$ docker pull percona@sha256:3d15daf61cc757d2272eb1888f66151a43ef27ba09e8dd948783404c18ea9e37
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.6 MB (194580454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8be2ebf4c8edca15874f479b0748f60b9d8c1fe774904ff4ac8f46e65e0ab582`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 26 Aug 2022 21:25:47 GMT
ADD file:67ab7eee8368c5d1cd71a8cfac5ea227da5b36ae49291c75dadb87506b1f1195 in / 
# Fri, 26 Aug 2022 21:25:48 GMT
CMD ["/bin/bash"]
# Fri, 26 Aug 2022 21:58:56 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 26 Aug 2022 22:01:26 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Fri, 26 Aug 2022 22:01:26 GMT
ENV PSMDB_VERSION=4.4.15-15
# Fri, 26 Aug 2022 22:01:26 GMT
ENV OS_VER=el8
# Fri, 26 Aug 2022 22:01:26 GMT
ENV FULL_PERCONA_VERSION=4.4.15-15.el8
# Fri, 26 Aug 2022 22:01:26 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Fri, 26 Aug 2022 22:02:02 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Fri, 26 Aug 2022 22:02:03 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Fri, 26 Aug 2022 22:02:03 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Fri, 26 Aug 2022 22:02:04 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Fri, 26 Aug 2022 22:02:04 GMT
ENV GOSU_VERSION=1.11
# Fri, 26 Aug 2022 22:02:07 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Fri, 26 Aug 2022 22:02:09 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Fri, 26 Aug 2022 22:02:09 GMT
VOLUME [/data/db]
# Fri, 26 Aug 2022 22:02:10 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Fri, 26 Aug 2022 22:02:10 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Fri, 26 Aug 2022 22:02:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Aug 2022 22:02:11 GMT
EXPOSE 27017
# Fri, 26 Aug 2022 22:02:11 GMT
USER 1001
# Fri, 26 Aug 2022 22:02:11 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2c825b6c4689f5d76258b0f0f7f6a1e27cbbd03f813bf02abeca31d54bcc9fcf`  
		Last Modified: Fri, 26 Aug 2022 21:27:24 GMT  
		Size: 84.9 MB (84863365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fcaf839df9582cfce2983c8ba035e0c7a59c2d173e0ca37fdd50b0a05da93cd`  
		Last Modified: Fri, 26 Aug 2022 22:05:19 GMT  
		Size: 3.7 MB (3749684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6880eb5cee6f18fac6fae8662b391f0e0fc7e4e3df38402e38199a9d44a556b`  
		Last Modified: Fri, 26 Aug 2022 22:05:30 GMT  
		Size: 96.9 MB (96881362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebea0202932148d7dcff5f85ccc3c5fa5a5a41ccbe79ac4d5b48e4cb8498e028`  
		Last Modified: Fri, 26 Aug 2022 22:05:18 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5ff1d742cb088f156fc0c830f78854b0feacb133e4f0616daf484450ee6e86`  
		Last Modified: Fri, 26 Aug 2022 22:05:18 GMT  
		Size: 4.1 KB (4101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31835659eb270307bc703eb4ea9977be68d34a7d3321ca043d99ea54c27c0738`  
		Last Modified: Fri, 26 Aug 2022 22:05:16 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d27492c50fe3b36e50dfdbb1ffa2338be0939ff6cac83cb7891e5279a36e07`  
		Last Modified: Fri, 26 Aug 2022 22:05:16 GMT  
		Size: 914.5 KB (914544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6924ebf6ff01c6a368d48b50b59324f55903cf379e01587932b52dd9d6fe170`  
		Last Modified: Fri, 26 Aug 2022 22:05:17 GMT  
		Size: 8.1 MB (8137887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5efa303ce01026782485ae88691bc546c0b63dbd4e9f283a39454d56d1819650`  
		Last Modified: Fri, 26 Aug 2022 22:05:16 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1401925ea881d9a94073a1971661a63810da5ce8400d5e318b270166b87e3f66`  
		Last Modified: Fri, 26 Aug 2022 22:05:16 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
