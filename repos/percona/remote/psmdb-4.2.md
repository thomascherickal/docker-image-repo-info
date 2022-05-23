## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:50fca1c90dbf992c0a29f3a466e1813bbcf1437bdad0a12b073ba08f1db6a476
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:b1d12b6d190c1a2010434ca91b9a8ad5c690c0bb6211f5d2e369424354429dda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.2 MB (176201654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a45f56f4345d2f4b8b63a433935fe7b362e4089ce501f0fe3524745ed910949`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 17 May 2022 22:41:30 GMT
ADD file:eafd9e49bc2d45c1c5bf5571be43743e0500886224b81c0a07dc7c3d1702d7bb in / 
# Tue, 17 May 2022 22:41:30 GMT
CMD ["/bin/bash"]
# Tue, 17 May 2022 23:13:01 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 23 May 2022 18:32:20 GMT
ENV PSMDB_VERSION=4.2.20-20
# Mon, 23 May 2022 18:32:20 GMT
ENV OS_VER=el8
# Mon, 23 May 2022 18:32:20 GMT
ENV FULL_PERCONA_VERSION=4.2.20-20.el8
# Mon, 23 May 2022 18:32:20 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 23 May 2022 18:32:25 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Mon, 23 May 2022 18:33:03 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Mon, 23 May 2022 18:33:04 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 23 May 2022 18:33:05 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 23 May 2022 18:33:05 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 23 May 2022 18:33:05 GMT
ENV GOSU_VERSION=1.11
# Mon, 23 May 2022 18:33:08 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Mon, 23 May 2022 18:33:13 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 23 May 2022 18:33:13 GMT
VOLUME [/data/db]
# Mon, 23 May 2022 18:33:13 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Mon, 23 May 2022 18:33:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 23 May 2022 18:33:13 GMT
EXPOSE 27017
# Mon, 23 May 2022 18:33:13 GMT
USER 1001
# Mon, 23 May 2022 18:33:13 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:25cd53f41add30fe2e87a488316e4bcfbecf123077c0f9f29be5cd359cbafd32`  
		Last Modified: Tue, 17 May 2022 22:42:23 GMT  
		Size: 84.6 MB (84569034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ea8e92ed69fac46022a5cb24af3a31799a470381d801572588d4487742e386`  
		Last Modified: Mon, 23 May 2022 18:34:10 GMT  
		Size: 3.7 MB (3745453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b90a9ceae0b002b3fb6fc03ed1920c89b97dddbad8c220e73ed356ae3f87b523`  
		Last Modified: Mon, 23 May 2022 18:34:20 GMT  
		Size: 78.8 MB (78814324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cebdba97569cd97b6ceec6df5f884a00edd2bdc34cedaebcd9c9e4bcbd8ff1d`  
		Last Modified: Mon, 23 May 2022 18:34:09 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf3775f954cc37c045457aed4c28a96095e80515f3894390493394baf6959ae`  
		Last Modified: Mon, 23 May 2022 18:34:07 GMT  
		Size: 4.1 KB (4101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09ea6b300c2f67a1c9e26765535991c34c78661de948d7595b67cd92f4a4179`  
		Last Modified: Mon, 23 May 2022 18:34:07 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49005da2e61049b295f0da0ce9a57d4aa4be21bcf0bb82aff295e6869e9d4750`  
		Last Modified: Mon, 23 May 2022 18:34:07 GMT  
		Size: 914.5 KB (914544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009760ac9ed8e0afc6b0e0925890fdd6a304bd29c584e0fd321681ac7ceb5a51`  
		Last Modified: Mon, 23 May 2022 18:34:08 GMT  
		Size: 8.1 MB (8137894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc9aa1998ff631e5c981522b9137e5509ef3a71aa1810ea5ba2298c039c6abd`  
		Last Modified: Mon, 23 May 2022 18:34:07 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
