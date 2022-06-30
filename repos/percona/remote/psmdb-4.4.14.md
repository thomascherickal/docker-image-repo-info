## `percona:psmdb-4.4.14`

```console
$ docker pull percona@sha256:c96e4cde30f8d1c73efd2faa28948f9326324726155131f70234cad3e13bae2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4.14` - linux; amd64

```console
$ docker pull percona@sha256:e6c05c67b067fdd315c669a3a4c5df8b591b92d22245f95abc25e8470964aac4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195488284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f779f1ad59c452bac39f0fd77684eabf4e18a0d4ebfb91590818e0ada46c2f1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 30 Jun 2022 17:20:36 GMT
ADD file:fdf207441bdb80042fb0d3dfd9498e2bcff45ba92f9d44ab93e2596ed3bebe81 in / 
# Thu, 30 Jun 2022 17:20:37 GMT
CMD ["/bin/bash"]
# Thu, 30 Jun 2022 17:56:26 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 30 Jun 2022 17:58:42 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Thu, 30 Jun 2022 17:58:42 GMT
ENV PSMDB_VERSION=4.4.14-14
# Thu, 30 Jun 2022 17:58:42 GMT
ENV OS_VER=el8
# Thu, 30 Jun 2022 17:58:42 GMT
ENV FULL_PERCONA_VERSION=4.4.14-14.el8
# Thu, 30 Jun 2022 17:58:42 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 30 Jun 2022 17:59:17 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 30 Jun 2022 17:59:18 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 30 Jun 2022 17:59:18 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 30 Jun 2022 17:59:19 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 30 Jun 2022 17:59:19 GMT
ENV GOSU_VERSION=1.11
# Thu, 30 Jun 2022 17:59:21 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 30 Jun 2022 17:59:23 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 30 Jun 2022 17:59:23 GMT
VOLUME [/data/db]
# Thu, 30 Jun 2022 17:59:24 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Thu, 30 Jun 2022 17:59:24 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Thu, 30 Jun 2022 17:59:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Jun 2022 17:59:24 GMT
EXPOSE 27017
# Thu, 30 Jun 2022 17:59:24 GMT
USER 1001
# Thu, 30 Jun 2022 17:59:24 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c36ed75e1749dabbd82d16fdd8049d3367cb86423a42f58d554c3cb1cc6ddb05`  
		Last Modified: Thu, 30 Jun 2022 17:21:22 GMT  
		Size: 84.6 MB (84570755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dedb6c3109b9f3e926802289629fe54724c261bd5f95bd02c6b5dd51c5730a`  
		Last Modified: Thu, 30 Jun 2022 18:02:47 GMT  
		Size: 3.7 MB (3740825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70717c77b1ea65be2fe809f106ff1cd65970485dd19bbb9c5f9c9073f92e338b`  
		Last Modified: Thu, 30 Jun 2022 18:02:59 GMT  
		Size: 98.1 MB (98090663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64993b40f4d4a346f6be993e22ac293a970ba2df762193497c06475fefe6c81`  
		Last Modified: Thu, 30 Jun 2022 18:02:46 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acb65a4e5a0dea0c4f8052f04c355028e4242b15376e8d1193de86ef953a063`  
		Last Modified: Thu, 30 Jun 2022 18:02:46 GMT  
		Size: 4.1 KB (4100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c845a2efe4b9c7b496599549f63bd319a9b20e813e6b8e33c235759d37b319`  
		Last Modified: Thu, 30 Jun 2022 18:02:44 GMT  
		Size: 10.6 KB (10574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93b83666d3f109574eac75979f01580e5cc5e3ae3d9c676a561d1396e81b989`  
		Last Modified: Thu, 30 Jun 2022 18:02:44 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176249d7bbc20c271842c33bc2f78f317b2719fb64ba2cd36ad28f514d015a16`  
		Last Modified: Thu, 30 Jun 2022 18:02:45 GMT  
		Size: 8.1 MB (8137889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885cd84be78373d461f8866ce5962e1f6d183565ce03e34cbe50bb95b4ab92c3`  
		Last Modified: Thu, 30 Jun 2022 18:02:43 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca789b51b1968a467ef7643540f66fba4b46ce42d518a3f9002aa27a8a87bf0`  
		Last Modified: Thu, 30 Jun 2022 18:02:44 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
