## `percona:psmdb-5.0.10`

```console
$ docker pull percona@sha256:52e164d164433abb4781fb6180cc72291da3ac1534cc4ec34555a35d70df0727
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0.10` - linux; amd64

```console
$ docker pull percona@sha256:2053844fecd7c310bb87e2e67c0a8d47f132aec34b61cf6f52ca73fd8670b284
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.6 MB (212570254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23cd8a3277036e6b2aa8ff7a983b2c214c22ed820da411c12c76f2d0140aee37`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 16 Nov 2022 07:52:18 GMT
ADD file:95e25b6cc4a22c4ecb537bc949b3636ae408264d293c1c32a3ad180e54f80ae9 in / 
# Wed, 16 Nov 2022 07:52:19 GMT
CMD ["/bin/bash"]
# Wed, 16 Nov 2022 08:52:25 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 16 Nov 2022 08:53:57 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-50 release
# Wed, 16 Nov 2022 08:53:57 GMT
ENV PSMDB_VERSION=5.0.10-9
# Wed, 16 Nov 2022 08:53:57 GMT
ENV OS_VER=el8
# Wed, 16 Nov 2022 08:53:58 GMT
ENV FULL_PERCONA_VERSION=5.0.10-9.el8
# Wed, 16 Nov 2022 08:53:58 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 16 Nov 2022 08:54:37 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 16 Nov 2022 08:54:38 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 16 Nov 2022 08:54:38 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 16 Nov 2022 08:54:39 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 16 Nov 2022 08:54:39 GMT
ENV GOSU_VERSION=1.11
# Wed, 16 Nov 2022 08:54:42 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 16 Nov 2022 08:54:47 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 16 Nov 2022 08:54:47 GMT
VOLUME [/data/db]
# Wed, 16 Nov 2022 08:54:48 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 16 Nov 2022 08:54:48 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Wed, 16 Nov 2022 08:54:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 08:54:48 GMT
EXPOSE 27017
# Wed, 16 Nov 2022 08:54:48 GMT
USER 1001
# Wed, 16 Nov 2022 08:54:48 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:df958f680f30541ef9f464f2f49bd4366e5904477b5ca521a78a4c68db2aa858`  
		Last Modified: Wed, 16 Nov 2022 07:53:09 GMT  
		Size: 87.4 MB (87435022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf47d0b5cf4757c65d217d3dcdf80ebd0d38fde95cfd96ad2010e4361760b45`  
		Last Modified: Wed, 16 Nov 2022 08:58:50 GMT  
		Size: 3.8 MB (3767739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81553f098b3a897cba710391c24e88855b075febeff652aeb83198b680d0c02`  
		Last Modified: Wed, 16 Nov 2022 08:59:03 GMT  
		Size: 112.3 MB (112281443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3a7611c698006e90846ed98b0fb1fe68d3ffdd52a03e20a51a2a78780bb652`  
		Last Modified: Wed, 16 Nov 2022 08:58:49 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb5ba7e991778e95f1e67c6a0298929ced5fbe264c40d181614962f128c8e08`  
		Last Modified: Wed, 16 Nov 2022 08:58:49 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe182fc99eb09155646db918d386255f22dc6ffe42957fc86d64b24e68a5483c`  
		Last Modified: Wed, 16 Nov 2022 08:58:47 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a52f74a44e9ec2f7670decff7e1ac78a504c8aa4b6af3c2b1ba7812f0f8e3c`  
		Last Modified: Wed, 16 Nov 2022 08:58:47 GMT  
		Size: 914.6 KB (914552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf59188eb8fef60a9deb5533547e9660abda052ad0ae8e1980efcdbb695ad23`  
		Last Modified: Wed, 16 Nov 2022 08:58:48 GMT  
		Size: 8.1 MB (8137887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5560ecaf01e950e59184593b8484fccd92842d9ff95df9f4e6bb96bc52caeeb5`  
		Last Modified: Wed, 16 Nov 2022 08:58:47 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c404fd7d6e48b82622d10c64371578699bfa53ea16ede10c3c031391c8341be`  
		Last Modified: Wed, 16 Nov 2022 08:58:46 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
