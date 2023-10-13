## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:046240f998945a97a1040270368c85d3c346585a4a3db3bea10a09cd85a1d397
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:b69af201cc93ee74a8d4db55ca1085b9631b684f6084821450bef2538952513c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.2 MB (218155920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a5dd4cdce73eb12ee8ed1e3621c777e481a65133a58243bc5f630c53a77f50`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 12 Oct 2023 21:28:19 GMT
ADD file:08ccec25d0d1459d4c27b2b0354bb526203faac57f1570a94b91c0d83e7474db in / 
# Thu, 12 Oct 2023 21:28:20 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 22:22:31 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 12 Oct 2023 22:27:56 GMT
ENV PSMDB_VERSION=4.2.24-24
# Thu, 12 Oct 2023 22:27:56 GMT
ENV OS_VER=el8
# Thu, 12 Oct 2023 22:27:56 GMT
ENV FULL_PERCONA_VERSION=4.2.24-24.el8
# Thu, 12 Oct 2023 22:27:56 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 12 Oct 2023 22:27:56 GMT
ENV PSMDB_REPO=release
# Thu, 12 Oct 2023 22:27:59 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Thu, 12 Oct 2023 22:28:49 GMT
RUN set -ex;     percona-release enable psmdb-42 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 12 Oct 2023 22:28:50 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Thu, 12 Oct 2023 22:28:50 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 12 Oct 2023 22:28:51 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 12 Oct 2023 22:28:51 GMT
ENV GOSU_VERSION=1.11
# Thu, 12 Oct 2023 22:28:54 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 12 Oct 2023 22:28:56 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -;     rm -f /tmp/SHA256SUMS;     chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 12 Oct 2023 22:28:56 GMT
VOLUME [/data/db]
# Thu, 12 Oct 2023 22:28:56 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Thu, 12 Oct 2023 22:28:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 22:28:56 GMT
EXPOSE 27017
# Thu, 12 Oct 2023 22:28:56 GMT
USER 1001
# Thu, 12 Oct 2023 22:28:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:eeccb7e6dc78cf3d674adcfebd1e8ff22148cf87ec3d731d3cd73eff435f6d9f`  
		Last Modified: Thu, 12 Oct 2023 21:29:47 GMT  
		Size: 88.0 MB (88009290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b54343162aaf252f2fb34f1c635beb41340675e445ed568f03f800e39c2e10`  
		Last Modified: Thu, 12 Oct 2023 22:31:56 GMT  
		Size: 3.8 MB (3801653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027f1c3584050db3239d82c147ef56d549933ed792a0e630c82653e4e46c849e`  
		Last Modified: Thu, 12 Oct 2023 22:32:10 GMT  
		Size: 117.3 MB (117258062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc8a0ad608767d4a6829804d61cb112fb0fccb2622e1723f43e3605e5d7b7de`  
		Last Modified: Thu, 12 Oct 2023 22:31:55 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a90f8295fc7eea857355d20ecb51e90d42eb03aaf21e6b51100cd7e3e8cd18`  
		Last Modified: Thu, 12 Oct 2023 22:31:53 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7bb311d1389d5121e43c8dcb586c592061834792167bf2469486f7dbd5334e`  
		Last Modified: Thu, 12 Oct 2023 22:31:53 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23445bccc1013c076fcdcb245f494c0017a3e2380ce5e3486d301a701af96622`  
		Last Modified: Thu, 12 Oct 2023 22:31:53 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca5276b8805adf6a0a283caa56c0b725264e7a4495c1071e8094f9f3d3d80da`  
		Last Modified: Thu, 12 Oct 2023 22:31:54 GMT  
		Size: 8.2 MB (8151448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766c211d0c4f0f48824415527227606545ff740ec421146799ce457a47918480`  
		Last Modified: Thu, 12 Oct 2023 22:31:53 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
