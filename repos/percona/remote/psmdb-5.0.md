## `percona:psmdb-5.0`

```console
$ docker pull percona@sha256:748d8d12fa6387320a3bef8fa0d69b4c8543bbfc53a35ce9b12bb94e88d23245
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0` - linux; amd64

```console
$ docker pull percona@sha256:5700a9a81e952709e9c5135d44c47a5bca07db52fd7cabf86a0f6eb1d072137f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.1 MB (211134198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f325ded6bec4b46807c33b4400d7ead434a3b648d0a8d13c5c34f3f563017bca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Oct 2022 19:20:44 GMT
ADD file:13fd8e206cb28eeafe30eb7ce28aaa24652a47074e82b1229e25c3f07b525253 in / 
# Fri, 21 Oct 2022 19:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:38:52 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 21 Oct 2022 19:40:24 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-50 release
# Fri, 21 Oct 2022 19:40:24 GMT
ENV PSMDB_VERSION=5.0.10-9
# Fri, 21 Oct 2022 19:40:24 GMT
ENV OS_VER=el8
# Fri, 21 Oct 2022 19:40:24 GMT
ENV FULL_PERCONA_VERSION=5.0.10-9.el8
# Fri, 21 Oct 2022 19:40:25 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Fri, 21 Oct 2022 19:41:03 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Fri, 21 Oct 2022 19:41:04 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Fri, 21 Oct 2022 19:41:04 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Fri, 21 Oct 2022 19:41:05 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Fri, 21 Oct 2022 19:41:05 GMT
ENV GOSU_VERSION=1.11
# Fri, 21 Oct 2022 19:41:09 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Fri, 21 Oct 2022 19:41:13 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Fri, 21 Oct 2022 19:41:13 GMT
VOLUME [/data/db]
# Fri, 21 Oct 2022 19:41:14 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Fri, 21 Oct 2022 19:41:14 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Fri, 21 Oct 2022 19:41:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Oct 2022 19:41:14 GMT
EXPOSE 27017
# Fri, 21 Oct 2022 19:41:15 GMT
USER 1001
# Fri, 21 Oct 2022 19:41:15 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:1580782cb014754e166fa2c701113af0e745dba59fb5fc368a1b676059545818`  
		Last Modified: Fri, 21 Oct 2022 19:22:23 GMT  
		Size: 86.0 MB (85966825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f78c786fa9706363eb4e7f6a27c4652307707c729e3535ee1c4b27b92b8e427`  
		Last Modified: Fri, 21 Oct 2022 19:44:48 GMT  
		Size: 3.8 MB (3775637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861012396f6fc3f07977a029620e712cd35f33402b91aaffff35745523d6ac4`  
		Last Modified: Fri, 21 Oct 2022 19:45:02 GMT  
		Size: 112.3 MB (112305678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8436447e7ea9ec57e22da1ec63062e63a5791e5e18f2a5a8dc5fab516e1ba6`  
		Last Modified: Fri, 21 Oct 2022 19:44:47 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f72ab13de912c8a5151108381fa1638de2d78518ebd9fdf6954865067572a0`  
		Last Modified: Fri, 21 Oct 2022 19:44:47 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228ce1b8bc1f75fbebd57ab148c7d86354463f214ceb03cd11f3e18a68a74fa1`  
		Last Modified: Fri, 21 Oct 2022 19:44:45 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da07b6914eedbea8630fe71c5efbe60c2c933403339babe9b0f61338386ea9ac`  
		Last Modified: Fri, 21 Oct 2022 19:44:45 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da03e151f00b48649d5329bad6728ce7ca394eaf39f983178ad62952e3119cb`  
		Last Modified: Fri, 21 Oct 2022 19:44:46 GMT  
		Size: 8.1 MB (8137893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359b0a6f2df577075e93958372a2c7e1a0ca3896445d4582b5f836c6934a54ff`  
		Last Modified: Fri, 21 Oct 2022 19:44:45 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fa4367c24ac8e0738a3d04bc1791f1312ced7df37c238a5c1de80caf784e66`  
		Last Modified: Fri, 21 Oct 2022 19:44:45 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
