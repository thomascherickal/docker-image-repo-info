## `percona:psmdb-5.0`

```console
$ docker pull percona@sha256:db5f495a21742cc4de93ffc645d98d7e76104f4629a2c0c0e8c5e950b408a7ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0` - linux; amd64

```console
$ docker pull percona@sha256:92c65b7586ec38b37058bd06dc4bc10b2c5cd1dd776a86776e5360e79aa84fd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.1 MB (211101313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46fb39b74753d8a32faf3efd18c2da7372fb9a6f42b6941fa9e2c170490e3745`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 14 Sep 2022 21:20:18 GMT
ADD file:e80b88eaaaff4337df2e280f39f05fa55901ffe34cce7c0e05597362c0e60f1d in / 
# Wed, 14 Sep 2022 21:20:18 GMT
CMD ["/bin/bash"]
# Wed, 14 Sep 2022 21:47:59 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 14 Sep 2022 21:49:18 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-50 release
# Wed, 14 Sep 2022 21:49:18 GMT
ENV PSMDB_VERSION=5.0.10-9
# Wed, 14 Sep 2022 21:49:18 GMT
ENV OS_VER=el8
# Wed, 14 Sep 2022 21:49:18 GMT
ENV FULL_PERCONA_VERSION=5.0.10-9.el8
# Wed, 14 Sep 2022 21:49:18 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 14 Sep 2022 21:49:56 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 14 Sep 2022 21:49:57 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 14 Sep 2022 21:49:57 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 14 Sep 2022 21:49:58 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 14 Sep 2022 21:49:58 GMT
ENV GOSU_VERSION=1.11
# Wed, 14 Sep 2022 21:50:01 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 14 Sep 2022 21:50:04 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 14 Sep 2022 21:50:04 GMT
VOLUME [/data/db]
# Wed, 14 Sep 2022 21:50:05 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 14 Sep 2022 21:50:05 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Wed, 14 Sep 2022 21:50:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 21:50:06 GMT
EXPOSE 27017
# Wed, 14 Sep 2022 21:50:06 GMT
USER 1001
# Wed, 14 Sep 2022 21:50:06 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7cb069903b8a7a68536454971fb537ee41f021abcc75a62ee6b76efe61020d70`  
		Last Modified: Wed, 14 Sep 2022 21:21:09 GMT  
		Size: 86.0 MB (85955949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db6b39e6c560b5312bb7d537cb504abccf6bc7046fcc7a86138eeea96e9a2bd`  
		Last Modified: Wed, 14 Sep 2022 21:53:44 GMT  
		Size: 3.8 MB (3765283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdf7cbe0d2b9746efb59beaf726fc0a67bd65e3535c19cf0fc86cfe6bb78601`  
		Last Modified: Wed, 14 Sep 2022 21:53:58 GMT  
		Size: 112.3 MB (112294040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cccef336d2a0d1e4ff9e1990f325a02c49e03c185c2522ca94027b4011731e4`  
		Last Modified: Wed, 14 Sep 2022 21:53:43 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f252158d5d00a911b6af7d52d191fe912ceb7a19ff17ec0210afda9114d78f`  
		Last Modified: Wed, 14 Sep 2022 21:53:43 GMT  
		Size: 4.1 KB (4102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258ed0c6e7a1a48dd2076793492d9332e1313cc9398c6aaeb37cb74310d82869`  
		Last Modified: Wed, 14 Sep 2022 21:53:41 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66a86e14da8bd3bf1b18ea0a76847dc3acac1a1af0296f4b388a3fb80c00f31`  
		Last Modified: Wed, 14 Sep 2022 21:53:41 GMT  
		Size: 914.5 KB (914547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f17a8416e5a47095601d0fa67a93eaa35dea3ab93fce0c39d0e1c5ae6a71d5`  
		Last Modified: Wed, 14 Sep 2022 21:53:42 GMT  
		Size: 8.1 MB (8137886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f2abb424b71936d34970f6411b268383e0c2e377c04cc0bb60a04632017485`  
		Last Modified: Wed, 14 Sep 2022 21:53:41 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81de9d47e9deb34b4fbff515b24164c1e3c89d2f26bb667c409a6d6147f05b0b`  
		Last Modified: Wed, 14 Sep 2022 21:53:41 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
