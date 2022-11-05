## `percona:psmdb-5.0.10`

```console
$ docker pull percona@sha256:b9ac3e98e50d13250dd8bbbd2a991a906b0e86233c88cfbb7a8c1c8ee1811ca3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0.10` - linux; amd64

```console
$ docker pull percona@sha256:5845910eb05be70509bf42e9c2460e0a40d80fb39f807a6074f2d1162fb4a621
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.1 MB (211082698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aacb46dce2c667b4d23417eb559c10ae4b1f871fad42588c1d14ff9d53552e45`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 04 Nov 2022 23:32:54 GMT
ADD file:2bc42b6875b914b1b6d99bf9e219400d534d6f6c5c0c529278df93ef1f2684c6 in / 
# Fri, 04 Nov 2022 23:32:54 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:27:35 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Nov 2022 02:29:06 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-50 release
# Sat, 05 Nov 2022 02:29:07 GMT
ENV PSMDB_VERSION=5.0.10-9
# Sat, 05 Nov 2022 02:29:07 GMT
ENV OS_VER=el8
# Sat, 05 Nov 2022 02:29:07 GMT
ENV FULL_PERCONA_VERSION=5.0.10-9.el8
# Sat, 05 Nov 2022 02:29:07 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 05 Nov 2022 02:29:45 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 05 Nov 2022 02:29:46 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Sat, 05 Nov 2022 02:29:46 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 05 Nov 2022 02:29:47 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 05 Nov 2022 02:29:47 GMT
ENV GOSU_VERSION=1.11
# Sat, 05 Nov 2022 02:29:51 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 05 Nov 2022 02:29:57 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 05 Nov 2022 02:29:57 GMT
VOLUME [/data/db]
# Sat, 05 Nov 2022 02:29:57 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 05 Nov 2022 02:29:57 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Sat, 05 Nov 2022 02:29:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Nov 2022 02:29:58 GMT
EXPOSE 27017
# Sat, 05 Nov 2022 02:29:58 GMT
USER 1001
# Sat, 05 Nov 2022 02:29:58 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f53ad0b8b1b9614b09bf69c21c965b04e683defa0796b21b55af5458264e49be`  
		Last Modified: Fri, 04 Nov 2022 23:34:33 GMT  
		Size: 85.9 MB (85945697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7460ea6db0ae37d93a9b2fa5d92c5c8d9155013bf3d69b016b8b3db9eb9843f0`  
		Last Modified: Sat, 05 Nov 2022 02:33:28 GMT  
		Size: 3.8 MB (3761208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50b0b75ee889f60c865676fe04bb65b0ad04ee559b3d7ac99ddb475f26fd2aa`  
		Last Modified: Sat, 05 Nov 2022 02:33:41 GMT  
		Size: 112.3 MB (112289743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f979fe094ee69402803627193bfd3df495a438b8be5c4be6a9b26dc2e5b30122`  
		Last Modified: Sat, 05 Nov 2022 02:33:27 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c98a76138b6d951e9b51dfad9252d922691e35169743ee133ffc68f35d514c6`  
		Last Modified: Sat, 05 Nov 2022 02:33:28 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e529d3922c6f0f0594d5b011ac3276a6059285473c1cf40dfcb84bc2ee73ab19`  
		Last Modified: Sat, 05 Nov 2022 02:33:25 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d279f979c028d207e0dcb89348abf5e1b318100875e1e17894e2dfe3149998da`  
		Last Modified: Sat, 05 Nov 2022 02:33:25 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a868ab07c3f35917f12cc1240ca90309c910ca3e3c52fa75f7cb2b7eafcba68b`  
		Last Modified: Sat, 05 Nov 2022 02:33:27 GMT  
		Size: 8.1 MB (8137887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951daa3e433c47d11571c20f7f7375708a1bc8b11b65ceacb4fca4ca9fc05593`  
		Last Modified: Sat, 05 Nov 2022 02:33:25 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da8202364a61539e6e79b4bb564dcbe6eb50516b7062e74b21bc85367c1c0aa`  
		Last Modified: Sat, 05 Nov 2022 02:33:25 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
