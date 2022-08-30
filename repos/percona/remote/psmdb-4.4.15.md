## `percona:psmdb-4.4.15`

```console
$ docker pull percona@sha256:ab1702a75dd3296215919b69ebc79ca792a95aae768c7bfb201d40b2a4a924cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4.15` - linux; amd64

```console
$ docker pull percona@sha256:a96e99d22f968bad67134da5a2ffbf59490b8930a369e8d3ee2d7f65c4a1cacb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.6 MB (194585600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2724e0ecf0b83f93bee926a74acdaf57a545ecced1e0c032a100fd4adecdb57b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 30 Aug 2022 21:20:24 GMT
ADD file:89b329a9c0e7f31e805663a6efe50c116e65ed0b9ebe1afa97f66b3c29c95980 in / 
# Tue, 30 Aug 2022 21:20:25 GMT
CMD ["/bin/bash"]
# Tue, 30 Aug 2022 21:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 30 Aug 2022 21:42:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Tue, 30 Aug 2022 21:42:17 GMT
ENV PSMDB_VERSION=4.4.15-15
# Tue, 30 Aug 2022 21:42:17 GMT
ENV OS_VER=el8
# Tue, 30 Aug 2022 21:42:17 GMT
ENV FULL_PERCONA_VERSION=4.4.15-15.el8
# Tue, 30 Aug 2022 21:42:17 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 30 Aug 2022 21:42:54 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Tue, 30 Aug 2022 21:42:55 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 30 Aug 2022 21:42:55 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 30 Aug 2022 21:42:56 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 30 Aug 2022 21:42:56 GMT
ENV GOSU_VERSION=1.11
# Tue, 30 Aug 2022 21:42:59 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Tue, 30 Aug 2022 21:43:00 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 30 Aug 2022 21:43:00 GMT
VOLUME [/data/db]
# Tue, 30 Aug 2022 21:43:01 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Tue, 30 Aug 2022 21:43:01 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Tue, 30 Aug 2022 21:43:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Aug 2022 21:43:01 GMT
EXPOSE 27017
# Tue, 30 Aug 2022 21:43:01 GMT
USER 1001
# Tue, 30 Aug 2022 21:43:01 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7266c81ed91338580bd46dbd5ea0787661dc5b416c63ed01711df0b108c861a4`  
		Last Modified: Tue, 30 Aug 2022 21:21:17 GMT  
		Size: 84.9 MB (84864369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae32e7a063e1c35a712d07229fc598c416bc7c14b42469c8db81be53f8876a1`  
		Last Modified: Tue, 30 Aug 2022 21:46:13 GMT  
		Size: 3.8 MB (3750912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a097d8b39eb7396c0cc31bdce72c794d20951d7f6331b0a459c979ea157c3012`  
		Last Modified: Tue, 30 Aug 2022 21:46:25 GMT  
		Size: 96.9 MB (96884273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ef794a3f69efef896c2c2db880f7e92f81c15cd14e1c340c72aa1407bd958c`  
		Last Modified: Tue, 30 Aug 2022 21:46:12 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb8c953a7e2852eddab0d591e418ea915e1eb8babcb1102ec73bae979618860`  
		Last Modified: Tue, 30 Aug 2022 21:46:12 GMT  
		Size: 4.1 KB (4102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ca64c7acd2fe75e90c1c29607f93a8900a08e12e5b570ad3b0ded553063bd2`  
		Last Modified: Tue, 30 Aug 2022 21:46:10 GMT  
		Size: 10.6 KB (10577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f0da28828bc325e480c0439fd7b8d673d748594f9f1dea606d188b76b973dd`  
		Last Modified: Tue, 30 Aug 2022 21:46:10 GMT  
		Size: 914.5 KB (914544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b83feccc572abdf8c2777dc6488c24c3a3db50ada02481fe27f585c223030b8`  
		Last Modified: Tue, 30 Aug 2022 21:46:12 GMT  
		Size: 8.1 MB (8137895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9347196cf2bc83fa2ef658a8f582b58379f2e6fec1def8a74531da2849561a1`  
		Last Modified: Tue, 30 Aug 2022 21:46:10 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fbe1c5faf6ff1d54cf058b99c54f5eecb04fb14a244558eb33f79b5b6064b7`  
		Last Modified: Tue, 30 Aug 2022 21:46:10 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
