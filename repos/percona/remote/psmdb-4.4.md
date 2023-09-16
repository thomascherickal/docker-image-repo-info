## `percona:psmdb-4.4`

```console
$ docker pull percona@sha256:c1d21c2f4497ec62f77a284d5fee49e7c03bc0ecd598a1306a04ba45342889e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4` - linux; amd64

```console
$ docker pull percona@sha256:1bcf9ad1246413083ef89c2982e1c9dd4dd25bb88dfc3862b339032ce6fef012
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.6 MB (237567526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffd830a53b347b0eb40ecc8828a564514d3e27b9fa150eb185ceb72293a8ed4d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:20:57 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 16 Sep 2023 03:23:14 GMT
ENV PSMDB_VERSION=4.4.22-21
# Sat, 16 Sep 2023 03:23:15 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:23:15 GMT
ENV FULL_PERCONA_VERSION=4.4.22-21.el8
# Sat, 16 Sep 2023 03:23:15 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 16 Sep 2023 03:23:15 GMT
ENV PSMDB_REPO=release
# Sat, 16 Sep 2023 03:24:06 GMT
RUN set -ex;     percona-release enable psmdb-44 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 16 Sep 2023 03:24:07 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 16 Sep 2023 03:24:07 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 16 Sep 2023 03:24:08 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 16 Sep 2023 03:24:08 GMT
ENV GOSU_VERSION=1.11
# Sat, 16 Sep 2023 03:24:10 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 16 Sep 2023 03:24:12 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 16 Sep 2023 03:24:12 GMT
VOLUME [/data/db]
# Sat, 16 Sep 2023 03:24:13 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 16 Sep 2023 03:24:13 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Sat, 16 Sep 2023 03:24:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Sep 2023 03:24:13 GMT
EXPOSE 27017
# Sat, 16 Sep 2023 03:24:13 GMT
USER 1001
# Sat, 16 Sep 2023 03:24:13 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05e3d36be41c8199349fc1fbf86a3bbc59e02a85af0a54a344e3be2526541d3`  
		Last Modified: Sat, 16 Sep 2023 03:28:02 GMT  
		Size: 3.8 MB (3787089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e54ff162db57c7d144feb0389c3530d109205efec0388e9e9603987a4114e5`  
		Last Modified: Sat, 16 Sep 2023 03:29:21 GMT  
		Size: 135.8 MB (135774644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786e05d09e9a80aa0579350a6bcdce8f577cdf3346f2ef91300445da278c14ab`  
		Last Modified: Sat, 16 Sep 2023 03:29:02 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b344a316644c660de39209499f7b9b81630b9cdc57adf3e12e30191ca84d1614`  
		Last Modified: Sat, 16 Sep 2023 03:29:02 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646ac6209edb2c87239c2a843c162afe141cd5f92e79117dd9257b7141701b66`  
		Last Modified: Sat, 16 Sep 2023 03:29:01 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4959b31cd07fffcd1df50e0f737c260fd31a486286ac1309d19eb451cd378c1c`  
		Last Modified: Sat, 16 Sep 2023 03:29:02 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dc0fb6c1ded9be533e4ecc8efff05c51a811b1cc845068bc350fd47505f3e3`  
		Last Modified: Sat, 16 Sep 2023 03:29:02 GMT  
		Size: 8.1 MB (8137885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d95bedb436b5533dbcf9477eec10a8baccb941e82c4eba3e6dbadf8c7a580a`  
		Last Modified: Sat, 16 Sep 2023 03:29:00 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0cf6fa3ad13b2d92feb6417ab0e0beb7c49e436b46f6c1067b78731705ae12`  
		Last Modified: Sat, 16 Sep 2023 03:29:01 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
