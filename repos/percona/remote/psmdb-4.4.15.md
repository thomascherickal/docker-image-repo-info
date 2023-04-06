## `percona:psmdb-4.4.15`

```console
$ docker pull percona@sha256:3421316d61e69e9a79c0916eadc52337b0e7bd6a24843acba697d7be1b923dd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4.15` - linux; amd64

```console
$ docker pull percona@sha256:fc70ab601dc64b7eb365ae5c40c6d763daa7aaffc54bc222f958017333e311dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.2 MB (198193154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91e3bfd645aec0b90e41d869a01999b124a8a6d88ef1730d7c3a43c7782147ba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 06 Apr 2023 18:20:21 GMT
ADD file:b8264f84035130ce589141b141f035b09d193dfca890914ecc0dc7ecd194e4b3 in / 
# Thu, 06 Apr 2023 18:20:22 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:39:05 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 06 Apr 2023 18:40:05 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Thu, 06 Apr 2023 18:40:05 GMT
ENV PSMDB_VERSION=4.4.15-15
# Thu, 06 Apr 2023 18:40:06 GMT
ENV OS_VER=el8
# Thu, 06 Apr 2023 18:40:06 GMT
ENV FULL_PERCONA_VERSION=4.4.15-15.el8
# Thu, 06 Apr 2023 18:40:06 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 06 Apr 2023 18:40:45 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 06 Apr 2023 18:40:46 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 06 Apr 2023 18:40:46 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 06 Apr 2023 18:40:47 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 06 Apr 2023 18:40:47 GMT
ENV GOSU_VERSION=1.11
# Thu, 06 Apr 2023 18:40:50 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 06 Apr 2023 18:40:52 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 06 Apr 2023 18:40:52 GMT
VOLUME [/data/db]
# Thu, 06 Apr 2023 18:40:52 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Thu, 06 Apr 2023 18:40:53 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Thu, 06 Apr 2023 18:40:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:40:53 GMT
EXPOSE 27017
# Thu, 06 Apr 2023 18:40:53 GMT
USER 1001
# Thu, 06 Apr 2023 18:40:53 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:06d6f22c2168ed40d437d9165a6c726f0bcaa2fd76ab943ed29f9ee4216e11fb`  
		Last Modified: Thu, 06 Apr 2023 18:21:04 GMT  
		Size: 88.4 MB (88436523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8db0af26248c5461314e11c0361877f3a1c939008b5393cb613e573d2b1fa7`  
		Last Modified: Thu, 06 Apr 2023 18:42:43 GMT  
		Size: 3.8 MB (3772609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a89a5c046ddf5108662a6ff9e6e1e9b9eec9f829df3c6efe7d29b14a692489a`  
		Last Modified: Thu, 06 Apr 2023 18:42:53 GMT  
		Size: 96.9 MB (96897986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242821e48dab7a454c77d464d139f6c459449ed3934c77d85a5ecd17cb8da157`  
		Last Modified: Thu, 06 Apr 2023 18:42:42 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f981cec8861b600006a68ddaf9ba0ebec728c3dcccaa14c21682a04b5382afa3`  
		Last Modified: Thu, 06 Apr 2023 18:42:41 GMT  
		Size: 4.1 KB (4098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3adb6f52f50dc79d7a1f33b5b932e4c61f7d42760f982c807ff8d28c73d2c1eb`  
		Last Modified: Thu, 06 Apr 2023 18:42:40 GMT  
		Size: 10.6 KB (10573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36013bfc6f441b483753227c9687461c3bd155796cebf099d92ae7ab289bd57e`  
		Last Modified: Thu, 06 Apr 2023 18:42:40 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4212cf5ff5299dfa77cff0c7c3ddbd9d27896dddc28952b01f471d2792590410`  
		Last Modified: Thu, 06 Apr 2023 18:42:41 GMT  
		Size: 8.1 MB (8137889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2d8aba5dfd7c5bd61bda1d97daaa4f7b15ab1f112e2db9ad5d5f573db7d513`  
		Last Modified: Thu, 06 Apr 2023 18:42:40 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2fd9593e0f008325204b69b6a05bcd2300636b8c40ca5c6fedf36f1613118c`  
		Last Modified: Thu, 06 Apr 2023 18:42:40 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
