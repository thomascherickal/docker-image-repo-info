## `percona:psmdb-5.0.7`

```console
$ docker pull percona@sha256:d857f6a2b0e98e87baa2337f2998452b733fb27a8d5fc23b5c05bc67b64d0e25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0.7` - linux; amd64

```console
$ docker pull percona@sha256:1e4481f64a4ed7c2699cf2d535cb2328a076a211c0577525dda562e5afa9ca46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.6 MB (213612481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b856fefd961d72ad3b435475b6c8afda0a5a42878ca4b74f2d0a5ce7ed028612`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 02 May 2022 20:50:56 GMT
ADD file:84bf324680059e085907eb7d75c8cb37d4d01aff3cc8241463bbc7d042db93d9 in / 
# Mon, 02 May 2022 20:50:56 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 21:18:32 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 02 May 2022 21:19:52 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-50 release
# Mon, 02 May 2022 21:19:52 GMT
ENV PSMDB_VERSION=5.0.7-6
# Mon, 02 May 2022 21:19:52 GMT
ENV OS_VER=el8
# Mon, 02 May 2022 21:19:52 GMT
ENV FULL_PERCONA_VERSION=5.0.7-6.el8
# Mon, 02 May 2022 21:19:53 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 02 May 2022 21:20:35 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Mon, 02 May 2022 21:20:36 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 02 May 2022 21:20:36 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 02 May 2022 21:20:37 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 02 May 2022 21:20:37 GMT
ENV GOSU_VERSION=1.11
# Mon, 02 May 2022 21:20:40 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Mon, 02 May 2022 21:20:42 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 02 May 2022 21:20:42 GMT
VOLUME [/data/db]
# Mon, 02 May 2022 21:20:43 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Mon, 02 May 2022 21:20:43 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Mon, 02 May 2022 21:20:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 02 May 2022 21:20:44 GMT
EXPOSE 27017
# Mon, 02 May 2022 21:20:44 GMT
USER 1001
# Mon, 02 May 2022 21:20:44 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:42405d186b2e7939aa51dc1bcc0f4cf0ce1236f4d6e38f2fae9822c41e98078e`  
		Last Modified: Mon, 02 May 2022 20:51:41 GMT  
		Size: 87.5 MB (87479695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acac54c59b32792a2363b5cd85242c5762c2455e2f4e7a2dda2983e394c9c79`  
		Last Modified: Mon, 02 May 2022 21:24:24 GMT  
		Size: 3.8 MB (3759061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eadf6a242304b49c981926be9abeb17885af1de7983427ee038bf6e0c61dbad`  
		Last Modified: Mon, 02 May 2022 21:24:37 GMT  
		Size: 113.3 MB (113287686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83a9c6ca618822510897c2c9a7aa898d2aba08fb74ea1df29e08bff81880418`  
		Last Modified: Mon, 02 May 2022 21:24:23 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546f158b30c68c56f6659796ee4e6d1356f20991d5e8084b32639c69d180fc65`  
		Last Modified: Mon, 02 May 2022 21:24:23 GMT  
		Size: 4.1 KB (4102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daec0796dc4c718644ecb968a9f9e8820c4f489debf5d974af13ba2b83b11ba6`  
		Last Modified: Mon, 02 May 2022 21:24:20 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3990bd67ac0026a701614cdecee2532704581e1cc7bd1d15aab3115c8e0c5b4`  
		Last Modified: Mon, 02 May 2022 21:24:21 GMT  
		Size: 914.5 KB (914545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291f609b0cfbd44db44a6b3b806fd38c3f811d2a6c8f66e5562a929612e2813d`  
		Last Modified: Mon, 02 May 2022 21:24:22 GMT  
		Size: 8.1 MB (8137886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007cfa62a2b44640d240187fcf717475579585440a0a68fbc4c98b953a813663`  
		Last Modified: Mon, 02 May 2022 21:24:20 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2981bd0bef186e0a6674fca4130d87a88cf074880d6b52afab1a6696da718ff`  
		Last Modified: Mon, 02 May 2022 21:24:21 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
