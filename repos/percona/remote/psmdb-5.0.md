## `percona:psmdb-5.0`

```console
$ docker pull percona@sha256:2f32976c61b7fc6c835c158ecc348a067519cb787fae53ca6d2a52d2bc224c4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0` - linux; amd64

```console
$ docker pull percona@sha256:78db8b25e689a9a79f6602e4e1c71d641ad5fe771e9810acab97086a16199b81
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.8 MB (256801715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7315001d080ce7f6e5ca15b3a971a058b2488807cc1544221dcf9038cd0ddbd`
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
# Wed, 06 Dec 2023 19:53:15 GMT
ENV PSMDB_VERSION=5.0.18-15
# Wed, 06 Dec 2023 19:53:15 GMT
ENV OS_VER=el8
# Wed, 06 Dec 2023 19:53:15 GMT
ENV FULL_PERCONA_VERSION=5.0.18-15.el8
# Wed, 06 Dec 2023 19:53:15 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 06 Dec 2023 19:53:15 GMT
ENV PSMDB_REPO=release
# Wed, 06 Dec 2023 19:54:12 GMT
RUN set -ex;     percona-release enable psmdb-50 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 06 Dec 2023 19:54:13 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Wed, 06 Dec 2023 19:54:13 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 06 Dec 2023 19:54:14 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 06 Dec 2023 19:54:14 GMT
ENV GOSU_VERSION=1.11
# Wed, 06 Dec 2023 19:54:17 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 06 Dec 2023 19:54:19 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 06 Dec 2023 19:54:19 GMT
VOLUME [/data/db]
# Wed, 06 Dec 2023 19:54:20 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 06 Dec 2023 19:54:20 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Wed, 06 Dec 2023 19:54:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:54:20 GMT
EXPOSE 27017
# Wed, 06 Dec 2023 19:54:20 GMT
USER 1001
# Wed, 06 Dec 2023 19:54:20 GMT
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
	-	`sha256:18fe13f7ba9bdc0203517b4efc96cfc90252be953fdbee803090ca6bd82dbbe7`  
		Last Modified: Wed, 06 Dec 2023 19:58:44 GMT  
		Size: 148.4 MB (148421056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b02af408c6aa2b6ccc89830d210d7c398381970dde508c091d8cbd1f6defa51`  
		Last Modified: Wed, 06 Dec 2023 19:58:25 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48405587532ae7e866500808386ddd08a3c6e6014e881d5c1447183408246042`  
		Last Modified: Wed, 06 Dec 2023 19:58:25 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b5cca5aaeed0a7d7e2187329f65631c4f972734e333ae8a555efde91866b8`  
		Last Modified: Wed, 06 Dec 2023 19:58:23 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32007141471b6fd716f948d64803876c48efed046d1e6347edf23c525104dadf`  
		Last Modified: Wed, 06 Dec 2023 19:58:24 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba5969d23ae4a090b0f1ac3030c8bb49293a5a28a3e1092660482db936262a2`  
		Last Modified: Wed, 06 Dec 2023 19:58:25 GMT  
		Size: 8.1 MB (8137889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b28a7785dd71dc0f112d033a488458d5e5498e4d4b9fb40439515bcc0d0a8`  
		Last Modified: Wed, 06 Dec 2023 19:58:23 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ed432dd9e4c160e2fe0aa7b31e636454207c5b440d84fe0d148c46a6d95354`  
		Last Modified: Wed, 06 Dec 2023 19:58:23 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
