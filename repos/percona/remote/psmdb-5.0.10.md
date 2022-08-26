## `percona:psmdb-5.0.10`

```console
$ docker pull percona@sha256:ccc26b68864e5272a973924bd15192282f3815a4d3ed78e53bc4e63cc72763bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0.10` - linux; amd64

```console
$ docker pull percona@sha256:b0d4cf85c9e1f843de038d7250ad5ed5f471eb8d180dea6533f9ece6156092f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.0 MB (209970579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8949b42bda95e6c448aecc0f5d0da10b6440b32cdd97fe571547814a1ef2d0e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 26 Aug 2022 21:25:47 GMT
ADD file:67ab7eee8368c5d1cd71a8cfac5ea227da5b36ae49291c75dadb87506b1f1195 in / 
# Fri, 26 Aug 2022 21:25:48 GMT
CMD ["/bin/bash"]
# Fri, 26 Aug 2022 21:58:56 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 26 Aug 2022 22:00:28 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-50 release
# Fri, 26 Aug 2022 22:00:28 GMT
ENV PSMDB_VERSION=5.0.10-9
# Fri, 26 Aug 2022 22:00:28 GMT
ENV OS_VER=el8
# Fri, 26 Aug 2022 22:00:28 GMT
ENV FULL_PERCONA_VERSION=5.0.10-9.el8
# Fri, 26 Aug 2022 22:00:28 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Fri, 26 Aug 2022 22:01:06 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Fri, 26 Aug 2022 22:01:07 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Fri, 26 Aug 2022 22:01:07 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Fri, 26 Aug 2022 22:01:08 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Fri, 26 Aug 2022 22:01:08 GMT
ENV GOSU_VERSION=1.11
# Fri, 26 Aug 2022 22:01:11 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Fri, 26 Aug 2022 22:01:14 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Fri, 26 Aug 2022 22:01:14 GMT
VOLUME [/data/db]
# Fri, 26 Aug 2022 22:01:15 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Fri, 26 Aug 2022 22:01:15 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Fri, 26 Aug 2022 22:01:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Aug 2022 22:01:15 GMT
EXPOSE 27017
# Fri, 26 Aug 2022 22:01:16 GMT
USER 1001
# Fri, 26 Aug 2022 22:01:16 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2c825b6c4689f5d76258b0f0f7f6a1e27cbbd03f813bf02abeca31d54bcc9fcf`  
		Last Modified: Fri, 26 Aug 2022 21:27:24 GMT  
		Size: 84.9 MB (84863365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17543915c07d169765712c9562d86ebae529490bc5bbbf17832a7c2bf5007ed6`  
		Last Modified: Fri, 26 Aug 2022 22:04:53 GMT  
		Size: 3.7 MB (3749745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c282d83b0491979c0054de5ab848b1ec8de65684d82744bd8cdc1446ee60e7ce`  
		Last Modified: Fri, 26 Aug 2022 22:05:06 GMT  
		Size: 112.3 MB (112271417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef83b08e7f6fd63e83243c3744f7b24bdc2167445a3c0c8723e10640097f9f2`  
		Last Modified: Fri, 26 Aug 2022 22:04:51 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e626940336ba90b5193968f91e129bef96b8fcf33fc383d66ade2f959f2928`  
		Last Modified: Fri, 26 Aug 2022 22:04:51 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3237780238939e48baeb5801e12baa68986becf3d1b8916f397eaff4a9cdf2d4`  
		Last Modified: Fri, 26 Aug 2022 22:04:49 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7b45f555098cd257541aaf781a1dfff5c72bde6f6915b45cb6a25a2e73250b`  
		Last Modified: Fri, 26 Aug 2022 22:04:50 GMT  
		Size: 914.5 KB (914546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2b7ca4fdf59f133e438685477a6d10ac7377de060086058103fda6b458bf3a`  
		Last Modified: Fri, 26 Aug 2022 22:04:51 GMT  
		Size: 8.1 MB (8137892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf00235df37c1594cd796692b4342569aba3a411e3a0040061ba7a20555512e1`  
		Last Modified: Fri, 26 Aug 2022 22:04:49 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45303d9b68c9f537718d07d3240c560756dbf80b499eb6f19dbcb5883246382d`  
		Last Modified: Fri, 26 Aug 2022 22:04:49 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
