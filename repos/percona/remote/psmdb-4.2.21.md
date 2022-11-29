## `percona:psmdb-4.2.21`

```console
$ docker pull percona@sha256:106c3e0f0e0b1afc20fab332a2c98b1107157b5eba4acca5ee0ec0898ff4c082
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2.21` - linux; amd64

```console
$ docker pull percona@sha256:7f9097207c08359d6efa9086e07e54aead4deb41f0ab8d6036425920edea05a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.9 MB (177876450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3bf1f55b6a0bdbb638589d3ddf611e9e497bef44f5412c602349a5f524ffbec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 29 Nov 2022 19:20:47 GMT
ADD file:0b5cd2f93e1c6f939d535c707f7dda5d950091382d18cdd7cf32ded784e057fc in / 
# Tue, 29 Nov 2022 19:20:48 GMT
CMD ["/bin/bash"]
# Tue, 29 Nov 2022 19:51:48 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 29 Nov 2022 19:55:13 GMT
ENV PSMDB_VERSION=4.2.21-21
# Tue, 29 Nov 2022 19:55:13 GMT
ENV OS_VER=el8
# Tue, 29 Nov 2022 19:55:13 GMT
ENV FULL_PERCONA_VERSION=4.2.21-21.el8
# Tue, 29 Nov 2022 19:55:13 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 29 Nov 2022 19:55:16 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Tue, 29 Nov 2022 19:55:52 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Tue, 29 Nov 2022 19:55:53 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 29 Nov 2022 19:55:53 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 29 Nov 2022 19:55:54 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 29 Nov 2022 19:55:54 GMT
ENV GOSU_VERSION=1.11
# Tue, 29 Nov 2022 19:55:56 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Tue, 29 Nov 2022 19:55:58 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 29 Nov 2022 19:55:58 GMT
VOLUME [/data/db]
# Tue, 29 Nov 2022 19:55:59 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Tue, 29 Nov 2022 19:55:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Nov 2022 19:55:59 GMT
EXPOSE 27017
# Tue, 29 Nov 2022 19:55:59 GMT
USER 1001
# Tue, 29 Nov 2022 19:55:59 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d0409ace7ea3bb98342dc30153bf50a92eeb0872d0474ef4fb0eabf9aba2390c`  
		Last Modified: Tue, 29 Nov 2022 19:22:26 GMT  
		Size: 87.4 MB (87437780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c13285f5f745eeaef3d1bf7c36645cf05e058c435d5fe060249ebe89ba470f`  
		Last Modified: Tue, 29 Nov 2022 19:58:27 GMT  
		Size: 3.8 MB (3774967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50007faae02582cfcfb915823a6c699e313c72820d99ef8f2b3744352e776051`  
		Last Modified: Tue, 29 Nov 2022 19:58:36 GMT  
		Size: 77.6 MB (77590864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9fc0364fdcc60b97dfe89c33bc903cef9c6ac364709fb0249b1402ffadc6fa`  
		Last Modified: Tue, 29 Nov 2022 19:58:26 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50953315a6bb067b3da0ef508a8f8f8d9a995902b50d3e973675582d278ec69e`  
		Last Modified: Tue, 29 Nov 2022 19:58:24 GMT  
		Size: 4.1 KB (4102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0d962d8622c0658cf907832087eb1c9dfff564c862a30cd6a61cb3d3974488`  
		Last Modified: Tue, 29 Nov 2022 19:58:24 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab2fe183ca7d30f63f2da21c56e37e3595c025fbf2a1fa5a946c362b4cc10eb`  
		Last Modified: Tue, 29 Nov 2022 19:58:25 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745316443509a31b863dbfd0d285c1cec7d104ae554ba85728f46befd377b3f8`  
		Last Modified: Tue, 29 Nov 2022 19:58:26 GMT  
		Size: 8.1 MB (8137889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a36f903cb9f1665b753b2747b147d548455a9f1c6ef6b914f3c736c95fe465`  
		Last Modified: Tue, 29 Nov 2022 19:58:24 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
