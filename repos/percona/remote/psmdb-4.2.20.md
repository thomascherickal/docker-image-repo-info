## `percona:psmdb-4.2.20`

```console
$ docker pull percona@sha256:670d748fc4bce72fc74d36898ec97a02db025ec257d1332b0116869673d86764
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2.20` - linux; amd64

```console
$ docker pull percona@sha256:e6f57c3b80fe1ec4a3d5cb5a0a29584265ee863ad191ccf7f0777befc551428d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.2 MB (176205525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:319703129f0a1650e76be4b5089fa2e59f4b354481fad8b5f2337a1e76f69121`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 30 Jun 2022 17:20:36 GMT
ADD file:fdf207441bdb80042fb0d3dfd9498e2bcff45ba92f9d44ab93e2596ed3bebe81 in / 
# Thu, 30 Jun 2022 17:20:37 GMT
CMD ["/bin/bash"]
# Thu, 30 Jun 2022 17:56:26 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jun 2022 17:59:27 GMT
ENV PSMDB_VERSION=4.2.20-20
# Thu, 30 Jun 2022 17:59:27 GMT
ENV OS_VER=el8
# Thu, 30 Jun 2022 17:59:27 GMT
ENV FULL_PERCONA_VERSION=4.2.20-20.el8
# Thu, 30 Jun 2022 17:59:28 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 30 Jun 2022 17:59:30 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Thu, 30 Jun 2022 18:00:03 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 30 Jun 2022 18:00:04 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 30 Jun 2022 18:00:04 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 30 Jun 2022 18:00:05 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 30 Jun 2022 18:00:05 GMT
ENV GOSU_VERSION=1.11
# Thu, 30 Jun 2022 18:00:08 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 30 Jun 2022 18:00:09 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 30 Jun 2022 18:00:09 GMT
VOLUME [/data/db]
# Thu, 30 Jun 2022 18:00:10 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Thu, 30 Jun 2022 18:00:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Jun 2022 18:00:10 GMT
EXPOSE 27017
# Thu, 30 Jun 2022 18:00:10 GMT
USER 1001
# Thu, 30 Jun 2022 18:00:10 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c36ed75e1749dabbd82d16fdd8049d3367cb86423a42f58d554c3cb1cc6ddb05`  
		Last Modified: Thu, 30 Jun 2022 17:21:22 GMT  
		Size: 84.6 MB (84570755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d86cb8ac2f80b90e070d201012a3e21196c3f6fc2980066084fb5bcc3a294c7`  
		Last Modified: Thu, 30 Jun 2022 18:03:16 GMT  
		Size: 3.7 MB (3740839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1cb8fe1d8ebf7f1bf35dbd2c54c3873d12ece8df64066819b47d7c1c4d0978e`  
		Last Modified: Thu, 30 Jun 2022 18:03:25 GMT  
		Size: 78.8 MB (78821099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aca56aa6c3315e12c6365cf0aaf3490adcd6d4a5eb71e83a90b7070d82c3d38`  
		Last Modified: Thu, 30 Jun 2022 18:03:15 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119ec71561ba5213c6170148e290a2281755e517776b9bc7a8d740cfca851d0`  
		Last Modified: Thu, 30 Jun 2022 18:03:12 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7aa3f7026f286181833ce09f5e118b8f63b017ef1b32fa9e3efe1bb1fd22a38`  
		Last Modified: Thu, 30 Jun 2022 18:03:12 GMT  
		Size: 10.6 KB (10575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cbe2040a807e93d5c1ada8817a24fcd8ee2ec6a8d87115133c0eb46b6ed93d`  
		Last Modified: Thu, 30 Jun 2022 18:03:13 GMT  
		Size: 914.5 KB (914545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd38aa4369f94286d823f79c7da2e1e28af32ddb4379fb8e9cad96121a28904`  
		Last Modified: Thu, 30 Jun 2022 18:03:14 GMT  
		Size: 8.1 MB (8137887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1aaa93f1723b27404abb3bfdc3b71acf6b8189afc9e19de7d8e5ebd405f0ae`  
		Last Modified: Thu, 30 Jun 2022 18:03:12 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
