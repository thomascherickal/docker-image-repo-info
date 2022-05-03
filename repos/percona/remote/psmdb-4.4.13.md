## `percona:psmdb-4.4.13`

```console
$ docker pull percona@sha256:7c9596d6aa9960fe0c4d6a41a744f61e80bd3547cce4769a33d79703ce8eb5df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4.13` - linux; amd64

```console
$ docker pull percona@sha256:6f0ab7cc987b00110e5ba24c4eee15968d6ed5f95a4290676f39f48d6fab280d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.4 MB (198374681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6e0b7b096dd714f04ed1182163fe2834a6a522fdf0f4a0aebc9332daea30e1b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 02 May 2022 20:50:56 GMT
ADD file:84bf324680059e085907eb7d75c8cb37d4d01aff3cc8241463bbc7d042db93d9 in / 
# Mon, 02 May 2022 20:50:56 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 21:18:32 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 02 May 2022 21:20:50 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Mon, 02 May 2022 21:20:50 GMT
ENV PSMDB_VERSION=4.4.13-13
# Mon, 02 May 2022 21:20:50 GMT
ENV OS_VER=el8
# Mon, 02 May 2022 21:20:50 GMT
ENV FULL_PERCONA_VERSION=4.4.13-13.el8
# Mon, 02 May 2022 21:20:50 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 02 May 2022 21:21:29 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Mon, 02 May 2022 21:21:30 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 02 May 2022 21:21:30 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 02 May 2022 21:21:31 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 02 May 2022 21:21:31 GMT
ENV GOSU_VERSION=1.11
# Mon, 02 May 2022 21:21:34 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Mon, 02 May 2022 21:21:35 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 02 May 2022 21:21:35 GMT
VOLUME [/data/db]
# Mon, 02 May 2022 21:21:36 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Mon, 02 May 2022 21:21:36 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Mon, 02 May 2022 21:21:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 02 May 2022 21:21:36 GMT
EXPOSE 27017
# Mon, 02 May 2022 21:21:36 GMT
USER 1001
# Mon, 02 May 2022 21:21:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:42405d186b2e7939aa51dc1bcc0f4cf0ce1236f4d6e38f2fae9822c41e98078e`  
		Last Modified: Mon, 02 May 2022 20:51:41 GMT  
		Size: 87.5 MB (87479695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3145ec9ae99491a2a8164c77ae0f90568582ec8ec330b3e6e5f385852278a097`  
		Last Modified: Mon, 02 May 2022 21:24:51 GMT  
		Size: 3.8 MB (3759067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916edeeea10f0952d0f2201c1331a0b4d452111cd439a6c58801be5a97be72e0`  
		Last Modified: Mon, 02 May 2022 21:25:03 GMT  
		Size: 98.0 MB (98049873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650a2a1b061cb8bf0102271dddc9bef51ba12751825c2fcead1846c7039b4f0a`  
		Last Modified: Mon, 02 May 2022 21:24:50 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e9836447df2e53e1987ac2788f0968de7064cab4d240516566fa9d617d5c53`  
		Last Modified: Mon, 02 May 2022 21:24:50 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:313c1d3bf5dac68c4d078502c34ad0fe0c54047741161d118e22fb0bb7b5b897`  
		Last Modified: Mon, 02 May 2022 21:24:48 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87152d1ea220bdd242eaa1321727e8b690f2df69d8dba8abb139e0b467349afc`  
		Last Modified: Mon, 02 May 2022 21:24:48 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba67c4d344273f86eedb1e393a8a1348990c5547192a87c949ef79de5f214e3`  
		Last Modified: Mon, 02 May 2022 21:24:49 GMT  
		Size: 8.1 MB (8137889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40e497d8292dc451d2ec8b3756422067752bd8146615cf0032d4d468065cfa3`  
		Last Modified: Mon, 02 May 2022 21:24:48 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63a21a07c3e78e0fa32f514e596cc6184dca5698d4230f51fe4514074401eff`  
		Last Modified: Mon, 02 May 2022 21:24:48 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
