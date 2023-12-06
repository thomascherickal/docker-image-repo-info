## `percona:psmdb-4.4`

```console
$ docker pull percona@sha256:a00a7bde804e7f078e53d6b328f9e5f65c1362c159175f7ef965b031fd968448
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4` - linux; amd64

```console
$ docker pull percona@sha256:86ff9430f1ec2878d90b8d67886cb64ca4fd4540e3a8d18c23dfd1b263538195
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.2 MB (244185401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3c8ba56629db27a9c1de8ae7082bd037f4a07df8f6849c6818a28317299195c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 06 Dec 2023 19:23:06 GMT
ADD file:56e00fc237c2b28dde03c72a85001f865f02c455f532215409ee621993dcfe98 in / 
# Wed, 06 Dec 2023 19:23:07 GMT
CMD ["/bin/bash"]
# Wed, 06 Dec 2023 19:50:10 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 06 Dec 2023 19:51:54 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 06 Dec 2023 19:54:25 GMT
ENV PSMDB_VERSION=4.4.22-21
# Wed, 06 Dec 2023 19:54:25 GMT
ENV OS_VER=el8
# Wed, 06 Dec 2023 19:54:25 GMT
ENV FULL_PERCONA_VERSION=4.4.22-21.el8
# Wed, 06 Dec 2023 19:54:25 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 06 Dec 2023 19:54:25 GMT
ENV PSMDB_REPO=release
# Wed, 06 Dec 2023 19:55:20 GMT
RUN set -ex;     percona-release enable psmdb-44 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 06 Dec 2023 19:55:21 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Wed, 06 Dec 2023 19:55:21 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 06 Dec 2023 19:55:22 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 06 Dec 2023 19:55:22 GMT
ENV GOSU_VERSION=1.11
# Wed, 06 Dec 2023 19:55:25 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 06 Dec 2023 19:55:27 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 06 Dec 2023 19:55:27 GMT
VOLUME [/data/db]
# Wed, 06 Dec 2023 19:55:27 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 06 Dec 2023 19:55:28 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Wed, 06 Dec 2023 19:55:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:55:28 GMT
EXPOSE 27017
# Wed, 06 Dec 2023 19:55:28 GMT
USER 1001
# Wed, 06 Dec 2023 19:55:28 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6f1712686323e0a6cedaa7c814b922f2a093bf3a9181c622641857175f4d864e`  
		Last Modified: Wed, 06 Dec 2023 19:24:12 GMT  
		Size: 95.5 MB (95493114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41d34e3eb26fe19c2f4f87c1114cf5fc4c92ab0f5fd468e1ab48582f597883b`  
		Last Modified: Wed, 06 Dec 2023 19:57:54 GMT  
		Size: 3.8 MB (3800983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59975d30b3a55cffe0fddf34b2d9c87f68e9ed7895f90a77d2a2ae3090a3af97`  
		Last Modified: Wed, 06 Dec 2023 19:59:13 GMT  
		Size: 135.8 MB (135804747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f00d07425a2064c70097043d54110e35f3acd22b6fa2fb552a09b7216db87a9`  
		Last Modified: Wed, 06 Dec 2023 19:58:54 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c0a09896e486af184de3599ceeefc9c4945247509a4a8bab8db6a5667ac01f`  
		Last Modified: Wed, 06 Dec 2023 19:58:54 GMT  
		Size: 4.1 KB (4102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc661f430a27766a9c067b1f6da3e06514c3926e15d28655de3b5bfee35571f`  
		Last Modified: Wed, 06 Dec 2023 19:58:53 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91a29cd9695f48080f24fbf1e8114cef705507b39bb388dde547f54e390f1c3`  
		Last Modified: Wed, 06 Dec 2023 19:58:53 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31c9a1ad1d61450d86832eca41b4672fa5c32dfcf1bc17c767d343b672e5f14`  
		Last Modified: Wed, 06 Dec 2023 19:58:54 GMT  
		Size: 8.1 MB (8137889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e140b25e3bf4bca33996c0df307353a54438d196a93a99f3afb887238ad5142c`  
		Last Modified: Wed, 06 Dec 2023 19:58:52 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c94e25f62c8c98bfcb84e798ffd5b102654e31055307554b131e7fdc38ddc1f`  
		Last Modified: Wed, 06 Dec 2023 19:58:52 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
