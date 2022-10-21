## `percona:psmdb-4.4`

```console
$ docker pull percona@sha256:8ff89ce362d19b967260a62fd28c0d7be4673b4f0aa76d37fcb3be78bd75887c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4` - linux; amd64

```console
$ docker pull percona@sha256:a38a16157a5a88df602f477b811b6208125cee707f45f692a85115e9b687ef91
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.7 MB (195742821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98498213c11c6d3e2700be848ac729b64379ba8d082ef73aa68a39024e40d7a5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Oct 2022 19:20:44 GMT
ADD file:13fd8e206cb28eeafe30eb7ce28aaa24652a47074e82b1229e25c3f07b525253 in / 
# Fri, 21 Oct 2022 19:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:38:52 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 21 Oct 2022 19:41:22 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Fri, 21 Oct 2022 19:41:22 GMT
ENV PSMDB_VERSION=4.4.15-15
# Fri, 21 Oct 2022 19:41:22 GMT
ENV OS_VER=el8
# Fri, 21 Oct 2022 19:41:22 GMT
ENV FULL_PERCONA_VERSION=4.4.15-15.el8
# Fri, 21 Oct 2022 19:41:22 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Fri, 21 Oct 2022 19:42:00 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Fri, 21 Oct 2022 19:42:01 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Fri, 21 Oct 2022 19:42:01 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Fri, 21 Oct 2022 19:42:01 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Fri, 21 Oct 2022 19:42:02 GMT
ENV GOSU_VERSION=1.11
# Fri, 21 Oct 2022 19:42:05 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Fri, 21 Oct 2022 19:42:07 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Fri, 21 Oct 2022 19:42:07 GMT
VOLUME [/data/db]
# Fri, 21 Oct 2022 19:42:08 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Fri, 21 Oct 2022 19:42:08 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Fri, 21 Oct 2022 19:42:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Oct 2022 19:42:09 GMT
EXPOSE 27017
# Fri, 21 Oct 2022 19:42:09 GMT
USER 1001
# Fri, 21 Oct 2022 19:42:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:1580782cb014754e166fa2c701113af0e745dba59fb5fc368a1b676059545818`  
		Last Modified: Fri, 21 Oct 2022 19:22:23 GMT  
		Size: 86.0 MB (85966825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d2cd6ac6b824f3a288f3040709236fa4a3a691eea278f5b819a38ed09afd30`  
		Last Modified: Fri, 21 Oct 2022 19:45:17 GMT  
		Size: 3.8 MB (3775671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8825f4ae61b9ef09d82fc04be1b2fb0e34a109b9a3d3e05511827d7b4461b74c`  
		Last Modified: Fri, 21 Oct 2022 19:45:29 GMT  
		Size: 96.9 MB (96914275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfd1efb843d93a0e49b886382db997f604a2b2ea522e60dbc45ed09c2094f3d`  
		Last Modified: Fri, 21 Oct 2022 19:45:16 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc336c525724c9911a92c054514eaf34b825dbe81f4931ffb9e3d8ce45b93bbd`  
		Last Modified: Fri, 21 Oct 2022 19:45:15 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c331cdf3f458302c8d4f9e6488dda178435961f6ec2f6241e3970b95475933`  
		Last Modified: Fri, 21 Oct 2022 19:45:13 GMT  
		Size: 10.6 KB (10577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a374740eac365e1c6b250cab3e89b43019955c03349efb51e395efdbeced06ed`  
		Last Modified: Fri, 21 Oct 2022 19:45:14 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3fb49539abf289b38ff65924784b9fc40c520fd78f31ced863399246fb8033`  
		Last Modified: Fri, 21 Oct 2022 19:45:15 GMT  
		Size: 8.1 MB (8137891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56b50fba9c332b29cd18a7aa30647555cd30471b59aeaede52ac74649233e6c`  
		Last Modified: Fri, 21 Oct 2022 19:45:13 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5ef330110e072f9460afd664f3d5a8ded3d39567d414dca5974a4149fc1125`  
		Last Modified: Fri, 21 Oct 2022 19:45:13 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
