## `percona:psmdb-5.0.10`

```console
$ docker pull percona@sha256:1d316680fb7855ab47ca9a46ab343bbc525388d46ece99006c2935b9ecc8b45c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0.10` - linux; amd64

```console
$ docker pull percona@sha256:76d7141e4a6443f664ce91344b1b481cc1dadd328b90a49ac63828612daac51f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.6 MB (213555187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026b1bf0f5a2d376fdfa279a22506c066e0dd603e8eab447bc9052b27654d737`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 22 Mar 2023 23:55:09 GMT
ADD file:9545a60b93a26aad3efb7cb70c1d2099f15bf3adf38467dc56f286ff438b89b2 in / 
# Wed, 22 Mar 2023 23:55:10 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:20:39 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 23 Mar 2023 00:22:08 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-50 release
# Thu, 23 Mar 2023 00:22:08 GMT
ENV PSMDB_VERSION=5.0.10-9
# Thu, 23 Mar 2023 00:22:08 GMT
ENV OS_VER=el8
# Thu, 23 Mar 2023 00:22:08 GMT
ENV FULL_PERCONA_VERSION=5.0.10-9.el8
# Thu, 23 Mar 2023 00:22:08 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 23 Mar 2023 00:22:49 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 23 Mar 2023 00:22:49 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 23 Mar 2023 00:22:50 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 23 Mar 2023 00:22:50 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 23 Mar 2023 00:22:50 GMT
ENV GOSU_VERSION=1.11
# Thu, 23 Mar 2023 00:22:53 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 23 Mar 2023 00:22:56 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 23 Mar 2023 00:22:56 GMT
VOLUME [/data/db]
# Thu, 23 Mar 2023 00:22:57 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Thu, 23 Mar 2023 00:22:57 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Thu, 23 Mar 2023 00:22:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 00:22:57 GMT
EXPOSE 27017
# Thu, 23 Mar 2023 00:22:57 GMT
USER 1001
# Thu, 23 Mar 2023 00:22:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5e8dcb5e56c183e88ba77bcc578f740c99b9e24522804c3588c46eda8f5cbdc1`  
		Last Modified: Wed, 22 Mar 2023 23:55:55 GMT  
		Size: 88.4 MB (88426082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de55515c3567e7c4be06940cb039e40975b8f499e3ce8854746eb200e218a5ec`  
		Last Modified: Thu, 23 Mar 2023 00:26:04 GMT  
		Size: 3.8 MB (3765181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdf86133bdfa1b151e66aee4ab1ef2dd43603f4e602955566fd9d48d75d87a3`  
		Last Modified: Thu, 23 Mar 2023 00:26:17 GMT  
		Size: 112.3 MB (112277880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094f9b806cdf6df94f9ad95117d54a5788d383d34b8018e4cc55e23efc6f2762`  
		Last Modified: Thu, 23 Mar 2023 00:26:03 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a796f682e1a0a1b7d6521ef3e352d1e857483042e45fc75e493b405b11733e7`  
		Last Modified: Thu, 23 Mar 2023 00:26:03 GMT  
		Size: 4.1 KB (4101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa08f5e6df6091bd409aee3523081bf6363c3d074fe5e15e7acc0d441320ccb`  
		Last Modified: Thu, 23 Mar 2023 00:26:01 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba849e975ad9a1117c249acd03fcf9966e502f6c0c8fddeb0ac939242e999fb`  
		Last Modified: Thu, 23 Mar 2023 00:26:01 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ce73ee0c013f5ce105b300ed6aa67ea8aa546ce4e3b1cd90864ba3f160c701`  
		Last Modified: Thu, 23 Mar 2023 00:26:02 GMT  
		Size: 8.1 MB (8137885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9da8fd93168f3a0e5e852a04398fc11c3b65066517c6cd7feb72ba91d73523`  
		Last Modified: Thu, 23 Mar 2023 00:26:01 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dac28d175c70acc8c420cd0397d2065fec0be30b62dbf6df3c118613924fcc0`  
		Last Modified: Thu, 23 Mar 2023 00:26:01 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
