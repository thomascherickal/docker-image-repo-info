## `percona:psmdb-4.2.21`

```console
$ docker pull percona@sha256:0accc752c0ce87d49ca7a4374d04d7f00159eaaba1b2c0ee21ccff06960350c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2.21` - linux; amd64

```console
$ docker pull percona@sha256:79773818fc19435b6c757e64d6d70bca0f21508bc2660fd5a4ba88fed60e7823
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.9 MB (177891132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a501a615621063d102a00186387ee766d93a966dc8e2db64119f55c8893d48`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:14 GMT
ADD file:5a832f5300f589b7f2a820f29d0655906164c4946d5fcd467921017c28a26bee in / 
# Wed, 07 Dec 2022 01:51:15 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:14:45 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 07 Dec 2022 02:18:10 GMT
ENV PSMDB_VERSION=4.2.21-21
# Wed, 07 Dec 2022 02:18:10 GMT
ENV OS_VER=el8
# Wed, 07 Dec 2022 02:18:10 GMT
ENV FULL_PERCONA_VERSION=4.2.21-21.el8
# Wed, 07 Dec 2022 02:18:10 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 07 Dec 2022 02:18:13 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Wed, 07 Dec 2022 02:18:49 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 07 Dec 2022 02:18:50 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 07 Dec 2022 02:18:50 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 07 Dec 2022 02:18:51 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 07 Dec 2022 02:18:51 GMT
ENV GOSU_VERSION=1.11
# Wed, 07 Dec 2022 02:18:54 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 07 Dec 2022 02:18:56 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 07 Dec 2022 02:18:56 GMT
VOLUME [/data/db]
# Wed, 07 Dec 2022 02:18:56 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Wed, 07 Dec 2022 02:18:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 07 Dec 2022 02:18:56 GMT
EXPOSE 27017
# Wed, 07 Dec 2022 02:18:57 GMT
USER 1001
# Wed, 07 Dec 2022 02:18:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4c770e098606ecfd5b78f4d61fc5e11b92fdde43d07825e543f04fe64aaa62eb`  
		Last Modified: Wed, 07 Dec 2022 01:52:57 GMT  
		Size: 87.4 MB (87445275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c94cbf428f262d536cb3e18cdb875be40ca1339a68baf8ebcd393366d7ead19`  
		Last Modified: Wed, 07 Dec 2022 02:21:29 GMT  
		Size: 3.8 MB (3778983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccf1420c09b50e53c87094631d9243d1fdb5f4ed0023394b5f782bd7fbe98c1`  
		Last Modified: Wed, 07 Dec 2022 02:21:37 GMT  
		Size: 77.6 MB (77594033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1137a090de79c1c58f1e46e17eeec3e2d1e029c3d88566038fe44515d9b2d0a1`  
		Last Modified: Wed, 07 Dec 2022 02:21:28 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6293b37c6610f3b70b61523c95769870a1defbc5cba9aab7dffcb54cb69e3e5`  
		Last Modified: Wed, 07 Dec 2022 02:21:26 GMT  
		Size: 4.1 KB (4102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a497b9dead97c2c6f4d900fd49933d6a03374899197a10773c3a72373a45e`  
		Last Modified: Wed, 07 Dec 2022 02:21:26 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92c361b21ff8be57520fef56d108df3844c68b01af9acc62c74015b4827169c`  
		Last Modified: Wed, 07 Dec 2022 02:21:26 GMT  
		Size: 914.5 KB (914544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83636b00f756623363a7c3be4db3f339d3e178650e9af4a5d68fd4450dd9d87b`  
		Last Modified: Wed, 07 Dec 2022 02:21:27 GMT  
		Size: 8.1 MB (8137893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0eb02d528f2bdcdf1d6dca470c19a7b12355d0b336134aaf03b4c23d99b771c`  
		Last Modified: Wed, 07 Dec 2022 02:21:26 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
