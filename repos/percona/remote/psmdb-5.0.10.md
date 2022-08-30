## `percona:psmdb-5.0.10`

```console
$ docker pull percona@sha256:eb7bf3f1a0798286bf54c5584d211144db4adb18506235c566d0c981332c4ffa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0.10` - linux; amd64

```console
$ docker pull percona@sha256:e88c88c1b38c7a34d36bf6196113227a6aea7f70476ab3d11840142ab3474017
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.0 MB (209974097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fce8435d10c7d5722cf88f0a5dd166aad3d026add59a80d0549d7d7511a8dad1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 30 Aug 2022 21:20:24 GMT
ADD file:89b329a9c0e7f31e805663a6efe50c116e65ed0b9ebe1afa97f66b3c29c95980 in / 
# Tue, 30 Aug 2022 21:20:25 GMT
CMD ["/bin/bash"]
# Tue, 30 Aug 2022 21:39:47 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Tue, 30 Aug 2022 21:41:19 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-50 release
# Tue, 30 Aug 2022 21:41:19 GMT
ENV PSMDB_VERSION=5.0.10-9
# Tue, 30 Aug 2022 21:41:20 GMT
ENV OS_VER=el8
# Tue, 30 Aug 2022 21:41:20 GMT
ENV FULL_PERCONA_VERSION=5.0.10-9.el8
# Tue, 30 Aug 2022 21:41:20 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Tue, 30 Aug 2022 21:41:57 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Tue, 30 Aug 2022 21:41:59 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Tue, 30 Aug 2022 21:41:59 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Tue, 30 Aug 2022 21:41:59 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Tue, 30 Aug 2022 21:41:59 GMT
ENV GOSU_VERSION=1.11
# Tue, 30 Aug 2022 21:42:03 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Tue, 30 Aug 2022 21:42:06 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Tue, 30 Aug 2022 21:42:06 GMT
VOLUME [/data/db]
# Tue, 30 Aug 2022 21:42:07 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Tue, 30 Aug 2022 21:42:07 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Tue, 30 Aug 2022 21:42:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Aug 2022 21:42:08 GMT
EXPOSE 27017
# Tue, 30 Aug 2022 21:42:08 GMT
USER 1001
# Tue, 30 Aug 2022 21:42:08 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7266c81ed91338580bd46dbd5ea0787661dc5b416c63ed01711df0b108c861a4`  
		Last Modified: Tue, 30 Aug 2022 21:21:17 GMT  
		Size: 84.9 MB (84864369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc697a4940ec3e43b7b0199f19d9c4d4cc2898cfa4ccb1bdbb74a3c35166196`  
		Last Modified: Tue, 30 Aug 2022 21:45:47 GMT  
		Size: 3.8 MB (3750915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d175039e7054377a8cf4ec1fd6526e0be6c1aacb7e06523a346929de86f94884`  
		Last Modified: Tue, 30 Aug 2022 21:46:00 GMT  
		Size: 112.3 MB (112272763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e39d52b28dbdc571d639553116d8710b88ee3e7cca89bae5ed47de59d8f6f92`  
		Last Modified: Tue, 30 Aug 2022 21:45:46 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1dc571ead012dfbf95943a98c782995da31865d57b6c5f6b63cc846aed4002`  
		Last Modified: Tue, 30 Aug 2022 21:45:45 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ec6ca2dccd50827132dac5eacb24d8f66bbfca3904b0bdf874ffd77a20ca77`  
		Last Modified: Tue, 30 Aug 2022 21:45:43 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b0d8a77660f05793cf1548c8c83aba4d8d995fa0342b85a6bc11ea8435bc342`  
		Last Modified: Tue, 30 Aug 2022 21:45:44 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4be4f14da9b8165f5961b96e17c5bac8b4033550999f936da758631e9a27c8`  
		Last Modified: Tue, 30 Aug 2022 21:45:45 GMT  
		Size: 8.1 MB (8137885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2993933d27f1ea413ea309fd4bed4856f21e061079459fa29daf9109a905716`  
		Last Modified: Tue, 30 Aug 2022 21:45:43 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fd5ca339b734470f10b30e63169bdab5cd6e89837e09ca481ec174cecc998f`  
		Last Modified: Tue, 30 Aug 2022 21:45:43 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
