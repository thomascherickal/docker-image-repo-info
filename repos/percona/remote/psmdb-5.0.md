## `percona:psmdb-5.0`

```console
$ docker pull percona@sha256:9360ebb9c827e357a61db248f42fe4143989b3fd1c3c001dac159b810bd84cf9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0` - linux; amd64

```console
$ docker pull percona@sha256:2b85952163ebff4d3eb06bfda810718a0859ab3b7c9341771b05e507e1d32d5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.8 MB (210788529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc7a670114ed5c3cc2bae959d5f363f6d8bd117d29dace0e76786455ac4b8e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 14 Jun 2022 18:23:16 GMT
ADD file:f0e6a328565074e88f761104e323c9f82d10f3a6835f494f792b9550d6c0780c in / 
# Tue, 14 Jun 2022 18:23:17 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 18:54:39 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 14 Jun 2022 18:56:11 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-50 release
# Tue, 21 Jun 2022 23:58:38 GMT
ENV PSMDB_VERSION=5.0.9-8
# Tue, 21 Jun 2022 23:58:38 GMT
ENV OS_VER=el8
# Tue, 21 Jun 2022 23:58:38 GMT
ENV FULL_PERCONA_VERSION=5.0.9-8.el8
# Tue, 21 Jun 2022 23:58:38 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 21 Jun 2022 23:59:15 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Tue, 21 Jun 2022 23:59:16 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 21 Jun 2022 23:59:16 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 21 Jun 2022 23:59:17 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 21 Jun 2022 23:59:17 GMT
ENV GOSU_VERSION=1.11
# Tue, 21 Jun 2022 23:59:21 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Tue, 21 Jun 2022 23:59:24 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 21 Jun 2022 23:59:24 GMT
VOLUME [/data/db]
# Tue, 21 Jun 2022 23:59:25 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Tue, 21 Jun 2022 23:59:25 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Tue, 21 Jun 2022 23:59:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Jun 2022 23:59:25 GMT
EXPOSE 27017
# Tue, 21 Jun 2022 23:59:25 GMT
USER 1001
# Tue, 21 Jun 2022 23:59:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f658974cd1e22c258b47ec713e6cfe60d8f00ec42264206a49a37bf7193cb96e`  
		Last Modified: Tue, 14 Jun 2022 18:24:03 GMT  
		Size: 84.6 MB (84562622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48518af5f057cf51636bd9c9c6ece0ac01ee2af5ac4e654759222730eb51144`  
		Last Modified: Tue, 14 Jun 2022 19:00:46 GMT  
		Size: 3.7 MB (3738879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2599c9165a850b974498a5214dcd1c944ffbf47c804c2b0603287b8660b5f3f8`  
		Last Modified: Wed, 22 Jun 2022 00:01:37 GMT  
		Size: 113.4 MB (113400974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a9f70a4d03e5e14a534e3e7fd6aea434c84e8cf1f848017b57f9563a82bfa3`  
		Last Modified: Wed, 22 Jun 2022 00:01:22 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae7449c07cabb93ebb4b1adddbc9d01956959cd96c7c3ceceb470c663e81457`  
		Last Modified: Wed, 22 Jun 2022 00:01:22 GMT  
		Size: 4.1 KB (4102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8acf269ce7291599f73e37c453a44459ad47d990151d55f676cfd130ecadf9d1`  
		Last Modified: Wed, 22 Jun 2022 00:01:20 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c4b87ca5025c089555bde0f17dc08ab1c756d9c8ab17e98104be38907e866e`  
		Last Modified: Wed, 22 Jun 2022 00:01:20 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655f5c40ed84a05d81d6906feb26e30ab16aee1a2c5be20b87a4d690be92e109`  
		Last Modified: Wed, 22 Jun 2022 00:01:21 GMT  
		Size: 8.1 MB (8137894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695e8ba2a36ff677a0a0a79a4a8e75fa8e77efd41402bd4553f34099f0a7104d`  
		Last Modified: Wed, 22 Jun 2022 00:01:20 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6478ec97cf738d84674a90629b106d108b6ce6ba1d7605942059640a18baff2`  
		Last Modified: Wed, 22 Jun 2022 00:01:20 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
