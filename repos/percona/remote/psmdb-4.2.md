## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:c189de1f81ff002f84faddfa9d687667697e6245a2c316d51284e8b245c3fa15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:1d4d61f0c313f263dbb78363a71666fd7548c3e329e7f8d90d5382e1e55472e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.4 MB (176384449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03251e55ce5ae9a12e87734d423cc1132cae48ab8db0c851afc83c09f3877e1f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 14 Sep 2022 21:20:18 GMT
ADD file:e80b88eaaaff4337df2e280f39f05fa55901ffe34cce7c0e05597362c0e60f1d in / 
# Wed, 14 Sep 2022 21:20:18 GMT
CMD ["/bin/bash"]
# Wed, 14 Sep 2022 21:47:59 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 14 Sep 2022 21:51:11 GMT
ENV PSMDB_VERSION=4.2.21-21
# Wed, 14 Sep 2022 21:51:11 GMT
ENV OS_VER=el8
# Wed, 14 Sep 2022 21:51:12 GMT
ENV FULL_PERCONA_VERSION=4.2.21-21.el8
# Wed, 14 Sep 2022 21:51:12 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 14 Sep 2022 21:51:14 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Wed, 14 Sep 2022 21:51:48 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 14 Sep 2022 21:51:49 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 14 Sep 2022 21:51:49 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 14 Sep 2022 21:51:50 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 14 Sep 2022 21:51:50 GMT
ENV GOSU_VERSION=1.11
# Wed, 14 Sep 2022 21:51:53 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 14 Sep 2022 21:51:54 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 14 Sep 2022 21:51:54 GMT
VOLUME [/data/db]
# Wed, 14 Sep 2022 21:51:54 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Wed, 14 Sep 2022 21:51:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 21:51:54 GMT
EXPOSE 27017
# Wed, 14 Sep 2022 21:51:55 GMT
USER 1001
# Wed, 14 Sep 2022 21:51:55 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7cb069903b8a7a68536454971fb537ee41f021abcc75a62ee6b76efe61020d70`  
		Last Modified: Wed, 14 Sep 2022 21:21:09 GMT  
		Size: 86.0 MB (85955949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c7dc5c2feca360a2a466b0ce29c7d5685e8a17bc670f64e25b760a4201c218`  
		Last Modified: Wed, 14 Sep 2022 21:54:35 GMT  
		Size: 3.8 MB (3765231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a01434c4fbcc98c6b250148c4d46bfc1df7f11240e103a79cedc4797725604e`  
		Last Modified: Wed, 14 Sep 2022 21:54:44 GMT  
		Size: 77.6 MB (77590423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25229fb4c428189cf1e4c46bcbe3b1b202779caa170181d3d6a18828df84c63c`  
		Last Modified: Wed, 14 Sep 2022 21:54:34 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da59cf106fe1f3cee534f341b57a32776df0f96f53c8751792318be5299ba5ef`  
		Last Modified: Wed, 14 Sep 2022 21:54:32 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ba644c76b4a0ff230a1633c6b853a86ff962a8601555696e2915e8122b34a6`  
		Last Modified: Wed, 14 Sep 2022 21:54:33 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23aae6c56595a6eef240af473091507d7cdc2ef69d3560eb6d6bb1c79d8f71e9`  
		Last Modified: Wed, 14 Sep 2022 21:54:33 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99f32c77242e82b17d9280a4016003e4238ee76d54cdb4468cbba705470c9c1`  
		Last Modified: Wed, 14 Sep 2022 21:54:34 GMT  
		Size: 8.1 MB (8137893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df59721c3f24273cf85185d30b21b1b756d1b5f87b56fd972a55867940c43ec0`  
		Last Modified: Wed, 14 Sep 2022 21:54:32 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
