## `percona:psmdb-4.2.24`

```console
$ docker pull percona@sha256:23abd672819951926cc88313b72ffb55e38216b9a33a8f28d4535acab28dee82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2.24` - linux; amd64

```console
$ docker pull percona@sha256:7945b80af0a2c7469457dad587627d88457dc09605580a3660c8b9f636424500
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.0 MB (219041553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0a7612184008c7ab6b31a6a43b6fe944ad67fc1e0bc16e15f9c376232ea60fb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:24:25 GMT
ENV PSMDB_VERSION=4.2.24-24
# Sat, 16 Sep 2023 03:24:25 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:24:25 GMT
ENV FULL_PERCONA_VERSION=4.2.24-24.el8
# Sat, 16 Sep 2023 03:24:25 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 16 Sep 2023 03:24:25 GMT
ENV PSMDB_REPO=release
# Sat, 16 Sep 2023 03:24:28 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 16 Sep 2023 03:25:16 GMT
RUN set -ex;     percona-release enable psmdb-42 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 16 Sep 2023 03:25:17 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 16 Sep 2023 03:25:17 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 16 Sep 2023 03:25:18 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 16 Sep 2023 03:25:18 GMT
ENV GOSU_VERSION=1.11
# Sat, 16 Sep 2023 03:25:21 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 16 Sep 2023 03:25:23 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -;     rm -f /tmp/SHA256SUMS;     chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 16 Sep 2023 03:25:23 GMT
VOLUME [/data/db]
# Sat, 16 Sep 2023 03:25:23 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Sat, 16 Sep 2023 03:25:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Sep 2023 03:25:23 GMT
EXPOSE 27017
# Sat, 16 Sep 2023 03:25:23 GMT
USER 1001
# Sat, 16 Sep 2023 03:25:24 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164f7a68b7030bc124d9cf34d07c76d54ec1e79572e31be3295e182a2e21c6d8`  
		Last Modified: Sat, 16 Sep 2023 03:29:36 GMT  
		Size: 3.8 MB (3787089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa491dd6268e0b275a5a4fcf806e2dc7223b0e14fd3acc0934b505750da44f01`  
		Last Modified: Sat, 16 Sep 2023 03:29:49 GMT  
		Size: 117.2 MB (117248300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e22a62adb6db81041318c87098dbeacedd0f94a5e386156a837ee8b447869d2`  
		Last Modified: Sat, 16 Sep 2023 03:29:34 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee62e609fee604f1c59eacedc4931822640150fe98cc28cb3fac909d072b0c5`  
		Last Modified: Sat, 16 Sep 2023 03:29:32 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14fdbc03b279777b2c0b114065624c47425321bc690f66299718abd1411c62fb`  
		Last Modified: Sat, 16 Sep 2023 03:29:32 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc65965ba646c52e9491c7f1596407af88f353a61f5f24c817915c18fcde045`  
		Last Modified: Sat, 16 Sep 2023 03:29:34 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f40cca8a55dad9ae9da7a03390bf5f4237ab2e2c6865f3c960f626819021c7f`  
		Last Modified: Sat, 16 Sep 2023 03:29:34 GMT  
		Size: 8.2 MB (8151461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5966d0fa83dea102b0f55fd20f6b988f830c5ea4837ca6697106dcb76144cef`  
		Last Modified: Sat, 16 Sep 2023 03:29:33 GMT  
		Size: 4.6 KB (4556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
