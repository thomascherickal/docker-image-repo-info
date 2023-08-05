## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:834ef5c7b8e6fef0ea9cd0b0ccb2dda695918297b42c0d5e81f8ccaad7b3e10f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:496b74852365c466f12578e70370988dea33801c613ab6c75cde93b41a9a75d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.1 MB (219057763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfbe111938d4a1343f641676a7e50c2f8b4867184f87f8b10b54dc3d28f8c47b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 05 Aug 2023 02:18:45 GMT
ADD file:231422907b7712864f26e05c23accdd356e75fc74ecc490907153265e423d543 in / 
# Sat, 05 Aug 2023 02:18:46 GMT
CMD ["/bin/bash"]
# Sat, 05 Aug 2023 02:37:13 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Aug 2023 02:41:58 GMT
ENV PSMDB_VERSION=4.2.24-24
# Sat, 05 Aug 2023 02:41:58 GMT
ENV OS_VER=el8
# Sat, 05 Aug 2023 02:41:58 GMT
ENV FULL_PERCONA_VERSION=4.2.24-24.el8
# Sat, 05 Aug 2023 02:41:58 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 05 Aug 2023 02:41:58 GMT
ENV PSMDB_REPO=release
# Sat, 05 Aug 2023 02:42:01 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 05 Aug 2023 02:42:47 GMT
RUN set -ex;     percona-release enable psmdb-42 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 05 Aug 2023 02:42:48 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 05 Aug 2023 02:42:48 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 05 Aug 2023 02:42:49 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 05 Aug 2023 02:42:49 GMT
ENV GOSU_VERSION=1.11
# Sat, 05 Aug 2023 02:42:51 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 05 Aug 2023 02:42:53 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -;     rm -f /tmp/SHA256SUMS;     chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 05 Aug 2023 02:42:53 GMT
VOLUME [/data/db]
# Sat, 05 Aug 2023 02:42:53 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Sat, 05 Aug 2023 02:42:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Aug 2023 02:42:54 GMT
EXPOSE 27017
# Sat, 05 Aug 2023 02:42:54 GMT
USER 1001
# Sat, 05 Aug 2023 02:42:54 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d55ddda9334e792e9c0ab817c79e3057c261ab6000bf8ff25221f4ae844aa0fb`  
		Last Modified: Sat, 05 Aug 2023 02:20:20 GMT  
		Size: 88.9 MB (88921738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fe55b577f35b2e3214ee0c80e3f125b04361c7d422e7b11f2f6dc89d054698`  
		Last Modified: Sat, 05 Aug 2023 02:46:32 GMT  
		Size: 3.8 MB (3790421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d9c907441dd2fb44ee227e9753545c0e3a866f19d1671ff795788b5ddae9f9`  
		Last Modified: Sat, 05 Aug 2023 02:46:45 GMT  
		Size: 117.3 MB (117258681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10196e7d599fb38dfdb161d198de299fef4d4cec325ac2a90d5e46b82ece49f`  
		Last Modified: Sat, 05 Aug 2023 02:46:31 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f6d3f27ad1fbda0840cb7ca477037b6c08f275a8b36c8eebfa7892e9df773a`  
		Last Modified: Sat, 05 Aug 2023 02:46:29 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81ed758e7227d1f3d895ddef89608f240c22b11b01b15211eab0ca019bb46ef`  
		Last Modified: Sat, 05 Aug 2023 02:46:29 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6255dcc1a76890d649287ed30da091761e6c26d84ffc1752a418b4f2c62d4d2a`  
		Last Modified: Sat, 05 Aug 2023 02:46:29 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f15f8563fd5840d1a3eee6822ef042c41a093295cf0b2ca7cf0fb4f69012078`  
		Last Modified: Sat, 05 Aug 2023 02:46:30 GMT  
		Size: 8.2 MB (8151460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6162883bee527ee5da4cf6176e0fad4baf25fb2eeafe32028814241ac258e0e6`  
		Last Modified: Sat, 05 Aug 2023 02:46:29 GMT  
		Size: 4.6 KB (4555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
