## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:38e88d1ef0a02a5e5732b5cfac77c2389425f97b210fcf77854c688b133c1fa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:a57a243901a5ba8dae61122cc71617c110a5a021960c29295d611e613b3bd1de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.9 MB (178865518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90f10fdc7bef57baf9a79d1a5936bd73f245b0def0f8aba944afe6af1ea09bb5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 06 Apr 2023 18:20:21 GMT
ADD file:b8264f84035130ce589141b141f035b09d193dfca890914ecc0dc7ecd194e4b3 in / 
# Thu, 06 Apr 2023 18:20:22 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:39:05 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 06 Apr 2023 18:41:01 GMT
ENV PSMDB_VERSION=4.2.21-21
# Thu, 06 Apr 2023 18:41:01 GMT
ENV OS_VER=el8
# Thu, 06 Apr 2023 18:41:01 GMT
ENV FULL_PERCONA_VERSION=4.2.21-21.el8
# Thu, 06 Apr 2023 18:41:01 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 06 Apr 2023 18:41:04 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Thu, 06 Apr 2023 18:41:40 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 06 Apr 2023 18:41:41 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 06 Apr 2023 18:41:41 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 06 Apr 2023 18:41:42 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 06 Apr 2023 18:41:42 GMT
ENV GOSU_VERSION=1.11
# Thu, 06 Apr 2023 18:41:44 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 06 Apr 2023 18:41:46 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 06 Apr 2023 18:41:46 GMT
VOLUME [/data/db]
# Thu, 06 Apr 2023 18:41:46 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Thu, 06 Apr 2023 18:41:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:41:46 GMT
EXPOSE 27017
# Thu, 06 Apr 2023 18:41:46 GMT
USER 1001
# Thu, 06 Apr 2023 18:41:46 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:06d6f22c2168ed40d437d9165a6c726f0bcaa2fd76ab943ed29f9ee4216e11fb`  
		Last Modified: Thu, 06 Apr 2023 18:21:04 GMT  
		Size: 88.4 MB (88436523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6624a916da2e8bd118cb267a7d56d24be04a6829ceaf95bb23f9e3e4f90e0853`  
		Last Modified: Thu, 06 Apr 2023 18:43:06 GMT  
		Size: 3.8 MB (3772637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5174e7a14293159fdf37ca7ff98095f443836cd3185e963d6c3d12fae821974a`  
		Last Modified: Thu, 06 Apr 2023 18:43:13 GMT  
		Size: 77.6 MB (77583518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe8ad93f5e84be02750e730349cf9c74caa2c1612605216348c5102929c4bdc`  
		Last Modified: Thu, 06 Apr 2023 18:43:04 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982cdb1fa8d08ef47c75894be430b7bd253ff61d824890f1dd39219a8ca32c48`  
		Last Modified: Thu, 06 Apr 2023 18:43:02 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2c5e9f88ba77b3d6c752aed7d5bfc5067cb3bf2c728b38398b672caf567550`  
		Last Modified: Thu, 06 Apr 2023 18:43:02 GMT  
		Size: 10.6 KB (10577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617f4f5f3a9c1dc47221023e6fc79b94342fecb838a394dc883f8d64ecfa39b3`  
		Last Modified: Thu, 06 Apr 2023 18:43:03 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a3af41d36a487339ff22be586340962046b180a3035a8a77ee48640d7a5bf5`  
		Last Modified: Thu, 06 Apr 2023 18:43:04 GMT  
		Size: 8.1 MB (8137887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1f35b4f24f4f9e2d88e9386450e749c7efb64e4e62aa154da22ff6aba1d935`  
		Last Modified: Thu, 06 Apr 2023 18:43:02 GMT  
		Size: 4.6 KB (4556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
