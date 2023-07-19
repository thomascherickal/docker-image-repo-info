## `percona:psmdb-5.0`

```console
$ docker pull percona@sha256:fa0e444748db3ff83028a6078d2f54818d85f361a5aef109617e8c08a50b6ff9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0` - linux; amd64

```console
$ docker pull percona@sha256:ee7cfc8c66e10b8e254495fb9e40b77dc40fb4c19eb1ad3d757d45d3252bdd75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.1 MB (250128615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a009326b6d7a3604106da13a7acdcad6ad9f3868ab114f69f0ec14a4912b51d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:05 GMT
ADD file:8fc521f1b2e4f7b59337e4402431f69bfe062b1a367ee737d9b7c9c0babd9b7c in / 
# Tue, 04 Jul 2023 02:04:06 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:10:12 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 19 Jul 2023 20:56:40 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 19 Jul 2023 20:58:00 GMT
ENV PSMDB_VERSION=5.0.18-15
# Wed, 19 Jul 2023 20:58:01 GMT
ENV OS_VER=el8
# Wed, 19 Jul 2023 20:58:01 GMT
ENV FULL_PERCONA_VERSION=5.0.18-15.el8
# Wed, 19 Jul 2023 20:58:01 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 19 Jul 2023 20:58:01 GMT
ENV PSMDB_REPO=release
# Wed, 19 Jul 2023 20:58:58 GMT
RUN set -ex;     percona-release enable psmdb-50 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 19 Jul 2023 20:58:59 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Wed, 19 Jul 2023 20:58:59 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 19 Jul 2023 20:59:00 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 19 Jul 2023 20:59:00 GMT
ENV GOSU_VERSION=1.11
# Wed, 19 Jul 2023 20:59:02 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 19 Jul 2023 20:59:04 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 19 Jul 2023 20:59:04 GMT
VOLUME [/data/db]
# Wed, 19 Jul 2023 20:59:05 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 19 Jul 2023 20:59:05 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Wed, 19 Jul 2023 20:59:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Jul 2023 20:59:05 GMT
EXPOSE 27017
# Wed, 19 Jul 2023 20:59:05 GMT
USER 1001
# Wed, 19 Jul 2023 20:59:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c546ef01e0bbda802469231ee4605fdaf8b1e7053539dba8d510b9de02610eed`  
		Last Modified: Tue, 04 Jul 2023 02:05:13 GMT  
		Size: 88.9 MB (88868389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfeeb16bf8999edb45d62d837e2ffada6ed220395b6a998d1464045211c00cb`  
		Last Modified: Wed, 19 Jul 2023 21:02:46 GMT  
		Size: 3.8 MB (3780725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd845c49278956bd8137f2926049705289fc0ba2b25639dfc112c3fdd304231`  
		Last Modified: Wed, 19 Jul 2023 21:03:35 GMT  
		Size: 148.4 MB (148392930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eb2cb98ee02615351d2ede77bb7cffc1cfe2779a381f21cef187970ff01a71`  
		Last Modified: Wed, 19 Jul 2023 21:03:17 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4e4b962090116d45303fb6a3edf79030232d8375eedb8a77d357ceada8aa76`  
		Last Modified: Wed, 19 Jul 2023 21:03:17 GMT  
		Size: 4.1 KB (4101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0517123faf5fd64ff4e8bc47010f80fa09d990e118118b55b52a548cba70b5`  
		Last Modified: Wed, 19 Jul 2023 21:03:15 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bd601960d99ba75cef20bdf8809a0097e9de16d750d9522cbe7e648fb87293`  
		Last Modified: Wed, 19 Jul 2023 21:03:15 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef31239a775565f1864e2fa49b7ec537ff0879551d553400d81afa083e845550`  
		Last Modified: Wed, 19 Jul 2023 21:03:16 GMT  
		Size: 8.1 MB (8137901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3261247ac06e0c8c922f3ec3b9c79418a4c89cdfcbcdd1d19adeb8f88261ae48`  
		Last Modified: Wed, 19 Jul 2023 21:03:15 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b291da9a8c39bec59391364ce1f29d7566f87d7d2ac6e683dd45b1d9337ce8c`  
		Last Modified: Wed, 19 Jul 2023 21:03:15 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
