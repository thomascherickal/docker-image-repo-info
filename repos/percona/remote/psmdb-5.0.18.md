## `percona:psmdb-5.0.18`

```console
$ docker pull percona@sha256:21e91704bb79201d420b7239ddc7fb2adbca47699ac06432334a345806d3907d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0.18` - linux; amd64

```console
$ docker pull percona@sha256:cb94f536ec060bb1e48e7be36993e202276dfbc8f4f56f716b8056a742316318
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.3 MB (249303679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d7c73c491abacfba41cf9f2f0b9cb9175bf28e395e79ce9bab5c812efff7746`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 12 Oct 2023 21:28:19 GMT
ADD file:08ccec25d0d1459d4c27b2b0354bb526203faac57f1570a94b91c0d83e7474db in / 
# Thu, 12 Oct 2023 21:28:20 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 22:22:31 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 12 Oct 2023 22:24:15 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Thu, 12 Oct 2023 22:25:36 GMT
ENV PSMDB_VERSION=5.0.18-15
# Thu, 12 Oct 2023 22:25:36 GMT
ENV OS_VER=el8
# Thu, 12 Oct 2023 22:25:36 GMT
ENV FULL_PERCONA_VERSION=5.0.18-15.el8
# Thu, 12 Oct 2023 22:25:36 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 12 Oct 2023 22:25:36 GMT
ENV PSMDB_REPO=release
# Thu, 12 Oct 2023 22:26:29 GMT
RUN set -ex;     percona-release enable psmdb-50 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 12 Oct 2023 22:26:30 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Thu, 12 Oct 2023 22:26:30 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 12 Oct 2023 22:26:30 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 12 Oct 2023 22:26:31 GMT
ENV GOSU_VERSION=1.11
# Thu, 12 Oct 2023 22:26:34 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 12 Oct 2023 22:26:36 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 12 Oct 2023 22:26:36 GMT
VOLUME [/data/db]
# Thu, 12 Oct 2023 22:26:37 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Thu, 12 Oct 2023 22:26:37 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Thu, 12 Oct 2023 22:26:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 22:26:37 GMT
EXPOSE 27017
# Thu, 12 Oct 2023 22:26:37 GMT
USER 1001
# Thu, 12 Oct 2023 22:26:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:eeccb7e6dc78cf3d674adcfebd1e8ff22148cf87ec3d731d3cd73eff435f6d9f`  
		Last Modified: Thu, 12 Oct 2023 21:29:47 GMT  
		Size: 88.0 MB (88009290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e26e8195de4845ab2bf941a400b26071c3b15161e70e9b0d422d9dc67a7576`  
		Last Modified: Thu, 12 Oct 2023 22:30:23 GMT  
		Size: 3.8 MB (3801638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c327b8cd512f5b9020676e3af67f5045854ea8235a07c35740da797c408da9`  
		Last Modified: Thu, 12 Oct 2023 22:31:13 GMT  
		Size: 148.4 MB (148406187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eedfc34453bdd2b473a155d7a3d37ed33637e01ecac8e13e99cc37ac4ef153`  
		Last Modified: Thu, 12 Oct 2023 22:30:55 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd5e7c7518d3a54f9697cf343960544baa6d84df4dec2375cd8981386b8f186`  
		Last Modified: Thu, 12 Oct 2023 22:30:55 GMT  
		Size: 4.1 KB (4100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581b1623ce48f2b68918c02f17a7d6c242935d8b7821f34c25198268607a1288`  
		Last Modified: Thu, 12 Oct 2023 22:30:53 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c826a1ef05dbab015ad4730c6e8480d0fac5932b22c91e47c5d90a86808c50b`  
		Last Modified: Thu, 12 Oct 2023 22:30:53 GMT  
		Size: 914.6 KB (914552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49935dbac4aae1d6f02dc6cc0aa26524f2b34c16474d9e4df7b2894650ec38f`  
		Last Modified: Thu, 12 Oct 2023 22:30:55 GMT  
		Size: 8.1 MB (8137894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fa57483cda53262e0979f9f57eeaa5fddd5ad76c3939fb02cf87027b5d3184`  
		Last Modified: Thu, 12 Oct 2023 22:30:53 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770967a3d8f02470084abdf2a3f0993a37dd4e958d7b25f6ea241b3ff82b70b8`  
		Last Modified: Thu, 12 Oct 2023 22:30:53 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
