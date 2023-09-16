## `percona:psmdb-6.0`

```console
$ docker pull percona@sha256:ded7b39fba731d32a7ab789b698ebbaac684344ad492c186ca079eba6581621d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-6.0` - linux; amd64

```console
$ docker pull percona@sha256:41d8d8b0d3181637b5dd493b660980570f32df6d254e202eb16d3793823a4cbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.6 MB (273606863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1beee0ffb717a17048ce1f17eedc2ec80d713f43b3ee9c39dbe9c6d5d5e94f31`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:43 GMT
ADD file:b086fe56323a44d446277e97c9f63e00d66130dd7fbdae2f3b730542be66287d in / 
# Sat, 16 Sep 2023 02:40:44 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 03:19:28 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 16 Sep 2023 03:20:57 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Sat, 16 Sep 2023 03:20:57 GMT
ENV PSMDB_VERSION=6.0.6-5
# Sat, 16 Sep 2023 03:20:57 GMT
ENV OS_VER=el8
# Sat, 16 Sep 2023 03:20:57 GMT
ENV FULL_PERCONA_VERSION=6.0.6-5.el8
# Sat, 16 Sep 2023 03:20:57 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 16 Sep 2023 03:20:57 GMT
ENV PSMDB_REPO=release
# Sat, 16 Sep 2023 03:21:53 GMT
RUN set -ex;     percona-release enable psmdb-60 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         percona-mongodb-mongosh         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-60/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 16 Sep 2023 03:21:54 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Sat, 16 Sep 2023 03:21:54 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 16 Sep 2023 03:21:55 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 16 Sep 2023 03:21:55 GMT
ENV GOSU_VERSION=1.11
# Sat, 16 Sep 2023 03:21:58 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 16 Sep 2023 03:22:00 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 16 Sep 2023 03:22:00 GMT
VOLUME [/data/db]
# Sat, 16 Sep 2023 03:22:01 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Sat, 16 Sep 2023 03:22:01 GMT
COPY file:7ab35f422fd362616b84e1dc71329cc9be05b7f834182c48bf98ceb92ee28956 in /entrypoint.sh 
# Sat, 16 Sep 2023 03:22:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Sep 2023 03:22:01 GMT
EXPOSE 27017
# Sat, 16 Sep 2023 03:22:01 GMT
USER 1001
# Sat, 16 Sep 2023 03:22:01 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a593ca9036ed77a51fca10362e5bf79d470b50f344e2db99a940ae4406c7a06d`  
		Last Modified: Sat, 16 Sep 2023 02:42:14 GMT  
		Size: 88.9 MB (88919239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05e3d36be41c8199349fc1fbf86a3bbc59e02a85af0a54a344e3be2526541d3`  
		Last Modified: Sat, 16 Sep 2023 03:28:02 GMT  
		Size: 3.8 MB (3787089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6797beff72ae7d4fb4042b0fbfa43229b899e9e2d03fe23f2c33c158ef4e3009`  
		Last Modified: Sat, 16 Sep 2023 03:28:20 GMT  
		Size: 171.8 MB (171813971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8207b8bc10dbfe3dac16324aeaba242a3cf036c263bac1407a56cce0fd3cea7`  
		Last Modified: Sat, 16 Sep 2023 03:27:58 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd461e079adf112c435382b24f3769a4e88bd43d411a092d5a5ff0b17d711426`  
		Last Modified: Sat, 16 Sep 2023 03:27:59 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606fca07bd5ba781da4820182065ffbe912bb07ec46f198af2d05b54142b6322`  
		Last Modified: Sat, 16 Sep 2023 03:27:56 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ed15729968bb75f0f6c602164192d3cfa61d331a1fb772c6dddec8e9dd7e0d`  
		Last Modified: Sat, 16 Sep 2023 03:27:58 GMT  
		Size: 914.5 KB (914546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d8477fb148d790ed4faad835bad6bdfc63f96f71abdcda7233fec85a4dc8ec`  
		Last Modified: Sat, 16 Sep 2023 03:27:58 GMT  
		Size: 8.1 MB (8137889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42a2ba3f90f7b01d71c4346365d6fc4ab229d0d1e131ffc45f47290d79d14d8`  
		Last Modified: Sat, 16 Sep 2023 03:27:56 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4c139e1d69ec80bed495fe387d648484d98948fbb6117458956fa55df3c2e9`  
		Last Modified: Sat, 16 Sep 2023 03:27:56 GMT  
		Size: 4.6 KB (4566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
