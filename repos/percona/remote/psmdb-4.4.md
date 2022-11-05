## `percona:psmdb-4.4`

```console
$ docker pull percona@sha256:139a548e19b149fbde85759fb89a99ea238b1dd3cbb412f8ca9ab6a013a918ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4` - linux; amd64

```console
$ docker pull percona@sha256:d446a4d46c8acd8b5f9ec035c1a6f2c71ca3f4b804662d5cd99cc076dd7087a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.7 MB (195698221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed6a2d8286baa204bd3dbe5e5474076907eee9c26c768c72d2c874b0358cff99`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 04 Nov 2022 23:32:54 GMT
ADD file:2bc42b6875b914b1b6d99bf9e219400d534d6f6c5c0c529278df93ef1f2684c6 in / 
# Fri, 04 Nov 2022 23:32:54 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:27:35 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Nov 2022 02:30:04 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Sat, 05 Nov 2022 02:30:04 GMT
ENV PSMDB_VERSION=4.4.15-15
# Sat, 05 Nov 2022 02:30:04 GMT
ENV OS_VER=el8
# Sat, 05 Nov 2022 02:30:05 GMT
ENV FULL_PERCONA_VERSION=4.4.15-15.el8
# Sat, 05 Nov 2022 02:30:05 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 05 Nov 2022 02:30:42 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 05 Nov 2022 02:30:43 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Sat, 05 Nov 2022 02:30:43 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 05 Nov 2022 02:30:43 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 05 Nov 2022 02:30:44 GMT
ENV GOSU_VERSION=1.11
# Sat, 05 Nov 2022 02:30:46 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 05 Nov 2022 02:30:48 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 05 Nov 2022 02:30:48 GMT
VOLUME [/data/db]
# Sat, 05 Nov 2022 02:30:49 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 05 Nov 2022 02:30:49 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Sat, 05 Nov 2022 02:30:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Nov 2022 02:30:49 GMT
EXPOSE 27017
# Sat, 05 Nov 2022 02:30:50 GMT
USER 1001
# Sat, 05 Nov 2022 02:30:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f53ad0b8b1b9614b09bf69c21c965b04e683defa0796b21b55af5458264e49be`  
		Last Modified: Fri, 04 Nov 2022 23:34:33 GMT  
		Size: 85.9 MB (85945697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3129c96b468588cb92f79a500d2099d80c0ee1a10a84c92d791a4e7b7eca2755`  
		Last Modified: Sat, 05 Nov 2022 02:33:55 GMT  
		Size: 3.8 MB (3761244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed89f68d5301cd7962a59daae70a17ec149994556634de50d6ccadfcec8d5d5`  
		Last Modified: Sat, 05 Nov 2022 02:34:06 GMT  
		Size: 96.9 MB (96905227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a53eb0de7d7b0160a8ed12cb952916e8cda821d5b5e12383117a03e8f5c1f81`  
		Last Modified: Sat, 05 Nov 2022 02:33:54 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac4d7d4e1e7eeaa572e5575656955ac8f9995d8d1f61e406ca238effccf19d1`  
		Last Modified: Sat, 05 Nov 2022 02:33:54 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bcc329aeee3439d408c2b9f3121f8acd04c1de6ca0b254cb1dc0812ce8d233`  
		Last Modified: Sat, 05 Nov 2022 02:33:52 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b11df068275642ec5c63c615a37e1731966e7880c1d6185693dcce51d29efd7`  
		Last Modified: Sat, 05 Nov 2022 02:33:52 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8cf8a38f5ecd6aa7fcea239ce218b58eee8663d834d586e300cc8fb756db78`  
		Last Modified: Sat, 05 Nov 2022 02:33:53 GMT  
		Size: 8.1 MB (8137891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a6e547e89fe1281d1b42e4a1b7a9ed8e83a0d50e74f95591635e7f211fb496`  
		Last Modified: Sat, 05 Nov 2022 02:33:52 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1046c87a5e56e86e76fca221c7d30b0e4acd70ebdfefdec6cf7234a37af984`  
		Last Modified: Sat, 05 Nov 2022 02:33:52 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
