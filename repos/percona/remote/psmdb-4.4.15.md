## `percona:psmdb-4.4.15`

```console
$ docker pull percona@sha256:13d76c837fb66d595c97fea88242204d03c54ca06ecd0b8e842459984ee1233b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4.15` - linux; amd64

```console
$ docker pull percona@sha256:9ceb5dd646ef506f99b2e00940f7b008994e418a5c480fa3eb7d3d3acbd76d50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.7 MB (195702141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b901ec73bba2a8e08b1e47e4788adde6482b23d287b45295cee9bd1a05a5ceaa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 14 Sep 2022 21:20:18 GMT
ADD file:e80b88eaaaff4337df2e280f39f05fa55901ffe34cce7c0e05597362c0e60f1d in / 
# Wed, 14 Sep 2022 21:20:18 GMT
CMD ["/bin/bash"]
# Wed, 14 Sep 2022 21:47:59 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 14 Sep 2022 21:50:16 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Wed, 14 Sep 2022 21:50:16 GMT
ENV PSMDB_VERSION=4.4.15-15
# Wed, 14 Sep 2022 21:50:16 GMT
ENV OS_VER=el8
# Wed, 14 Sep 2022 21:50:16 GMT
ENV FULL_PERCONA_VERSION=4.4.15-15.el8
# Wed, 14 Sep 2022 21:50:16 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 14 Sep 2022 21:50:53 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 14 Sep 2022 21:50:54 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 14 Sep 2022 21:50:54 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 14 Sep 2022 21:50:55 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 14 Sep 2022 21:50:55 GMT
ENV GOSU_VERSION=1.11
# Wed, 14 Sep 2022 21:50:57 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 14 Sep 2022 21:50:59 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 14 Sep 2022 21:50:59 GMT
VOLUME [/data/db]
# Wed, 14 Sep 2022 21:51:00 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 14 Sep 2022 21:51:01 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Wed, 14 Sep 2022 21:51:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 21:51:01 GMT
EXPOSE 27017
# Wed, 14 Sep 2022 21:51:01 GMT
USER 1001
# Wed, 14 Sep 2022 21:51:01 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7cb069903b8a7a68536454971fb537ee41f021abcc75a62ee6b76efe61020d70`  
		Last Modified: Wed, 14 Sep 2022 21:21:09 GMT  
		Size: 86.0 MB (85955949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f043c35648c2077a89d09eed66971778b7ade8ebb3bf746136a35a779bc905`  
		Last Modified: Wed, 14 Sep 2022 21:54:11 GMT  
		Size: 3.8 MB (3765289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0845427e924cb66823ac6e66cce7a7cbae34a6c9e8ce952d66fd1ba716cfacd5`  
		Last Modified: Wed, 14 Sep 2022 21:54:22 GMT  
		Size: 96.9 MB (96894861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b735d6d368135f0f6b2ec3714298518b484b72676a8fd1b39a3e12e3fd1001`  
		Last Modified: Wed, 14 Sep 2022 21:54:10 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac9311211c55696f8213b09a17a91595451d4736dcd9009cdeb2d3c0434273b`  
		Last Modified: Wed, 14 Sep 2022 21:54:10 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22efe6a2d6350d0e05bfffd3d23fb29a0b15bcaf35bed5d0c5e984cca7ff340`  
		Last Modified: Wed, 14 Sep 2022 21:54:08 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5b4026df567a2425db077ce0839f4f243d6b2fe3d08ab7ae8cd24a7c10fa1a`  
		Last Modified: Wed, 14 Sep 2022 21:54:08 GMT  
		Size: 914.5 KB (914543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08246c55110e90e654eb451961952d630496ede58ee8ef3a10da4d89aefd866e`  
		Last Modified: Wed, 14 Sep 2022 21:54:09 GMT  
		Size: 8.1 MB (8137890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6be470bfb5c1d331a66319cdda0f4d5f3c05d4997c2c7caa380de10f902c83d`  
		Last Modified: Wed, 14 Sep 2022 21:54:08 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f0b57adcef5d5ab13f1cab8caff6c46ce3824bdb37bc39121cf58d98347c65`  
		Last Modified: Wed, 14 Sep 2022 21:54:08 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
