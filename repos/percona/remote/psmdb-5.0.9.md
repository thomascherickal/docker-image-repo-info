## `percona:psmdb-5.0.9`

```console
$ docker pull percona@sha256:7d20db90afdbd04159e3ed6d9f46569c1283bf90a75127496b18f9cdad8ac881
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0.9` - linux; amd64

```console
$ docker pull percona@sha256:bfe774a328753ed3c1893fff5b493c629629dbe91d375a0fd6536deec0857f05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.8 MB (210809884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77106acc5ed508b9aa28e3d3a3cc8ac12b02bb1b42d07a5a33360f6e5baa11e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 30 Jun 2022 17:20:36 GMT
ADD file:fdf207441bdb80042fb0d3dfd9498e2bcff45ba92f9d44ab93e2596ed3bebe81 in / 
# Thu, 30 Jun 2022 17:20:37 GMT
CMD ["/bin/bash"]
# Thu, 30 Jun 2022 17:56:26 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jun 2022 17:57:44 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-50 release
# Thu, 30 Jun 2022 17:57:44 GMT
ENV PSMDB_VERSION=5.0.9-8
# Thu, 30 Jun 2022 17:57:44 GMT
ENV OS_VER=el8
# Thu, 30 Jun 2022 17:57:44 GMT
ENV FULL_PERCONA_VERSION=5.0.9-8.el8
# Thu, 30 Jun 2022 17:57:44 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 30 Jun 2022 17:58:22 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 30 Jun 2022 17:58:23 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 30 Jun 2022 17:58:23 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 30 Jun 2022 17:58:24 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 30 Jun 2022 17:58:24 GMT
ENV GOSU_VERSION=1.11
# Thu, 30 Jun 2022 17:58:27 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 30 Jun 2022 17:58:30 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 30 Jun 2022 17:58:30 GMT
VOLUME [/data/db]
# Thu, 30 Jun 2022 17:58:31 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Thu, 30 Jun 2022 17:58:31 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Thu, 30 Jun 2022 17:58:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Jun 2022 17:58:32 GMT
EXPOSE 27017
# Thu, 30 Jun 2022 17:58:32 GMT
USER 1001
# Thu, 30 Jun 2022 17:58:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c36ed75e1749dabbd82d16fdd8049d3367cb86423a42f58d554c3cb1cc6ddb05`  
		Last Modified: Thu, 30 Jun 2022 17:21:22 GMT  
		Size: 84.6 MB (84570755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0328b74870ae01f2d4a7bfc51e603de9e23250e16ef3f78f27c23959de26560`  
		Last Modified: Thu, 30 Jun 2022 18:02:19 GMT  
		Size: 3.7 MB (3740820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edd8eefb7cc952241795f01be7a6c0df8f412447fddb29f49eccd33dd4ee3c2`  
		Last Modified: Thu, 30 Jun 2022 18:02:32 GMT  
		Size: 113.4 MB (113412269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbffd95544f2d7582863c015aa2391ad8ad9d651a241d432e7cad259ceb645c`  
		Last Modified: Thu, 30 Jun 2022 18:02:17 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a04c011368a5bfd9ed084cc7b5a75aae4abc99080589b777d3317b0ed80629`  
		Last Modified: Thu, 30 Jun 2022 18:02:17 GMT  
		Size: 4.1 KB (4102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8e90110e831173c6ad52b0cb85cd25f368118cc1d60bbf20b19d489c80c086`  
		Last Modified: Thu, 30 Jun 2022 18:02:14 GMT  
		Size: 10.6 KB (10573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f98a861e57527156f3f80c3f6f0c409858023efeb573cf277825ed539da945`  
		Last Modified: Thu, 30 Jun 2022 18:02:14 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6846f6ceab83760f8600a22d08ba887e4ddbde7a878de1a81cc4c23fef8c6367`  
		Last Modified: Thu, 30 Jun 2022 18:02:16 GMT  
		Size: 8.1 MB (8137890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1820fd4fb4b9c6fed34f3cb93490d5c0c621cd6675aa65e0c62b8bf7a0cd2b21`  
		Last Modified: Thu, 30 Jun 2022 18:02:14 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3d35043063b12669591cb87856e03a1937fd73364d1f46a143aad8993e6e`  
		Last Modified: Thu, 30 Jun 2022 18:02:14 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
