## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:ed531b8d63ef9150075c1fa07e52c1f33ddd412452c6561ceac0a5b424b83817
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:3fc9daf0c47e95398396afd5f28f5a01c874220d906d336557fa07f16387ab85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.7 MB (225667958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:544ee2b3e1f8f88152f4c84948e82133946087b852c249a24aaa4c479009bb19`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 06 Dec 2023 19:23:06 GMT
ADD file:56e00fc237c2b28dde03c72a85001f865f02c455f532215409ee621993dcfe98 in / 
# Wed, 06 Dec 2023 19:23:07 GMT
CMD ["/bin/bash"]
# Wed, 06 Dec 2023 19:50:10 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 06 Dec 2023 19:55:34 GMT
ENV PSMDB_VERSION=4.2.24-24
# Wed, 06 Dec 2023 19:55:35 GMT
ENV OS_VER=el8
# Wed, 06 Dec 2023 19:55:35 GMT
ENV FULL_PERCONA_VERSION=4.2.24-24.el8
# Wed, 06 Dec 2023 19:55:35 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 06 Dec 2023 19:55:35 GMT
ENV PSMDB_REPO=release
# Wed, 06 Dec 2023 19:55:38 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 06 Dec 2023 19:56:31 GMT
RUN set -ex;     percona-release enable psmdb-42 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 06 Dec 2023 19:56:33 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Wed, 06 Dec 2023 19:56:33 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 06 Dec 2023 19:56:33 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 06 Dec 2023 19:56:33 GMT
ENV GOSU_VERSION=1.11
# Wed, 06 Dec 2023 19:56:36 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 06 Dec 2023 19:56:38 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -;     rm -f /tmp/SHA256SUMS;     chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 06 Dec 2023 19:56:38 GMT
VOLUME [/data/db]
# Wed, 06 Dec 2023 19:56:38 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Wed, 06 Dec 2023 19:56:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:56:38 GMT
EXPOSE 27017
# Wed, 06 Dec 2023 19:56:39 GMT
USER 1001
# Wed, 06 Dec 2023 19:56:39 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6f1712686323e0a6cedaa7c814b922f2a093bf3a9181c622641857175f4d864e`  
		Last Modified: Wed, 06 Dec 2023 19:24:12 GMT  
		Size: 95.5 MB (95493114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49641185a14c67a9fbb0fbf5dabf264097dcd04766d7590cef74ad5ae8621cbe`  
		Last Modified: Wed, 06 Dec 2023 19:59:25 GMT  
		Size: 3.8 MB (3800972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e90f3c02df60e0f519eee8ebc0fd09ed3b51de401d9f3b3293a07cb923d18a`  
		Last Modified: Wed, 06 Dec 2023 19:59:39 GMT  
		Size: 117.3 MB (117286955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8235f411770c9fcb9d0763d85aaaa4c52728de09e553433db77486f758e4fdaa`  
		Last Modified: Wed, 06 Dec 2023 19:59:24 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be89eece74947dda28b446cfe5d628a953794f36935ea2725ee96a73cb49c303`  
		Last Modified: Wed, 06 Dec 2023 19:59:22 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d62ca86e50ffccb801d1ded957986a4fbc3bff5d8ef084170167551bad95401`  
		Last Modified: Wed, 06 Dec 2023 19:59:22 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7162d3958af8238a6fb573d5c5fa6fd9cf89a3fff7df7c7ee21ebc98925f350d`  
		Last Modified: Wed, 06 Dec 2023 19:59:23 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00de37405f2a0f4b5a924597beb9252aa38b3521a69c806a76986f6893139d67`  
		Last Modified: Wed, 06 Dec 2023 19:59:24 GMT  
		Size: 8.2 MB (8151453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf8f95e2a0db02962b0e30b758d006397113216c8e5c5a436e6f77664b0f39d`  
		Last Modified: Wed, 06 Dec 2023 19:59:22 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
