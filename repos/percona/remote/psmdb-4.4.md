## `percona:psmdb-4.4`

```console
$ docker pull percona@sha256:c1180a15d228f2adda4443465e4507be325f8cb387edc9168465ed63cab9149d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4` - linux; amd64

```console
$ docker pull percona@sha256:752c1dd7c40be7816f1e5ef4cdedcddbf3dc4db2cec66546d5ec098d68501651
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.2 MB (197201880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a2bf96b68ad48be4a9149fb611b4259a87b5d63b3483bf84161bbc4b679f55f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 29 Nov 2022 19:20:47 GMT
ADD file:0b5cd2f93e1c6f939d535c707f7dda5d950091382d18cdd7cf32ded784e057fc in / 
# Tue, 29 Nov 2022 19:20:48 GMT
CMD ["/bin/bash"]
# Tue, 29 Nov 2022 19:51:48 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 29 Nov 2022 19:54:18 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Tue, 29 Nov 2022 19:54:18 GMT
ENV PSMDB_VERSION=4.4.15-15
# Tue, 29 Nov 2022 19:54:18 GMT
ENV OS_VER=el8
# Tue, 29 Nov 2022 19:54:18 GMT
ENV FULL_PERCONA_VERSION=4.4.15-15.el8
# Tue, 29 Nov 2022 19:54:18 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 29 Nov 2022 19:54:56 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Tue, 29 Nov 2022 19:54:58 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 29 Nov 2022 19:54:58 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 29 Nov 2022 19:54:58 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 29 Nov 2022 19:54:58 GMT
ENV GOSU_VERSION=1.11
# Tue, 29 Nov 2022 19:55:01 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Tue, 29 Nov 2022 19:55:03 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 29 Nov 2022 19:55:03 GMT
VOLUME [/data/db]
# Tue, 29 Nov 2022 19:55:04 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Tue, 29 Nov 2022 19:55:04 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Tue, 29 Nov 2022 19:55:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Nov 2022 19:55:04 GMT
EXPOSE 27017
# Tue, 29 Nov 2022 19:55:04 GMT
USER 1001
# Tue, 29 Nov 2022 19:55:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d0409ace7ea3bb98342dc30153bf50a92eeb0872d0474ef4fb0eabf9aba2390c`  
		Last Modified: Tue, 29 Nov 2022 19:22:26 GMT  
		Size: 87.4 MB (87437780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb55ea0c7bd7c1b28ee16d11092250a21444f3fea1bf4f88d6f85e01ab3128c2`  
		Last Modified: Tue, 29 Nov 2022 19:58:05 GMT  
		Size: 3.8 MB (3774962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a387feda11536d2ee20b36474411002024aeba962a48b2bdb5060cc8dfc770`  
		Last Modified: Tue, 29 Nov 2022 19:58:15 GMT  
		Size: 96.9 MB (96903092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad4f929508bdcde6ec54d2e3c571cb91f2e4943bcaa896754ddf401cea08079`  
		Last Modified: Tue, 29 Nov 2022 19:58:03 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8afb649ac9a0c74e6bbf062a4510d1d53edd9d04195875386de677054d167de`  
		Last Modified: Tue, 29 Nov 2022 19:58:03 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6704095e58127c3f5444c7a5c504e1daa4403f21ec844349d6bb550f0ee4121c`  
		Last Modified: Tue, 29 Nov 2022 19:58:01 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5818e4a1529561167914c3f4605da482330c75c368fa3e1a0c9739a4b669efff`  
		Last Modified: Tue, 29 Nov 2022 19:58:02 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3ff081c44491f1d8646a22a66299ce918336a597293c0bf31ebc7415903662`  
		Last Modified: Tue, 29 Nov 2022 19:58:03 GMT  
		Size: 8.1 MB (8137886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8be54a2f826ee65d8a5a1949b7e82b2e174ac0d0d6c3c934e58d652ba4e28b`  
		Last Modified: Tue, 29 Nov 2022 19:58:02 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a764b7a8fac12f0caf09be4df6bf90c9b1286c86db802aae55afede8bad801c3`  
		Last Modified: Tue, 29 Nov 2022 19:58:01 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
