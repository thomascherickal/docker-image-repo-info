## `percona:psmdb-4.2.21`

```console
$ docker pull percona@sha256:abea003d4fc8baf4411ee65ed6f715689f1aa1d6e099451835ede77e9da09e93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2.21` - linux; amd64

```console
$ docker pull percona@sha256:0805bcbda9b69803849eeed9368547d021a57f976e26b1982eb8637e95176cb4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.8 MB (178838412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3edd24c00b466de579db42a40d772ed82cc9377d0b3354900124427351c160dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 22 Mar 2023 23:55:09 GMT
ADD file:9545a60b93a26aad3efb7cb70c1d2099f15bf3adf38467dc56f286ff438b89b2 in / 
# Wed, 22 Mar 2023 23:55:10 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:20:39 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 23 Mar 2023 00:24:01 GMT
ENV PSMDB_VERSION=4.2.21-21
# Thu, 23 Mar 2023 00:24:01 GMT
ENV OS_VER=el8
# Thu, 23 Mar 2023 00:24:01 GMT
ENV FULL_PERCONA_VERSION=4.2.21-21.el8
# Thu, 23 Mar 2023 00:24:01 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 23 Mar 2023 00:24:03 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Thu, 23 Mar 2023 00:24:40 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 23 Mar 2023 00:24:41 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 23 Mar 2023 00:24:41 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 23 Mar 2023 00:24:41 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 23 Mar 2023 00:24:41 GMT
ENV GOSU_VERSION=1.11
# Thu, 23 Mar 2023 00:24:44 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 23 Mar 2023 00:24:46 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 23 Mar 2023 00:24:46 GMT
VOLUME [/data/db]
# Thu, 23 Mar 2023 00:24:46 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Thu, 23 Mar 2023 00:24:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 00:24:46 GMT
EXPOSE 27017
# Thu, 23 Mar 2023 00:24:46 GMT
USER 1001
# Thu, 23 Mar 2023 00:24:46 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5e8dcb5e56c183e88ba77bcc578f740c99b9e24522804c3588c46eda8f5cbdc1`  
		Last Modified: Wed, 22 Mar 2023 23:55:55 GMT  
		Size: 88.4 MB (88426082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ea930d881d0105fd786c12f58cbd36e45f8dfe6d1fb8f9e98cabc7b41b15be`  
		Last Modified: Thu, 23 Mar 2023 00:26:51 GMT  
		Size: 3.8 MB (3765188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2fad985ad30e1c3e73434194882babace5d845e8f1229a3fc7ca5e892e3f8`  
		Last Modified: Thu, 23 Mar 2023 00:26:59 GMT  
		Size: 77.6 MB (77574306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f104972c38c1a25d822a3d777ca05dd9b4c581b84dc564d21d12579f22efe0`  
		Last Modified: Thu, 23 Mar 2023 00:26:50 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75f4c1d2374ea1092ac9334bfbef4768343944d4f5e3253c87d01cb6f2ef956`  
		Last Modified: Thu, 23 Mar 2023 00:26:48 GMT  
		Size: 4.1 KB (4101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80537f1252452d55e7dfc6d01e7eae7b6a6f90c120f89ddb337479454617db41`  
		Last Modified: Thu, 23 Mar 2023 00:26:48 GMT  
		Size: 10.6 KB (10577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d27b533c6f4c3197917ebd9a2d39d2812047cf984d2523bdc6c9794fb6503bc`  
		Last Modified: Thu, 23 Mar 2023 00:26:49 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf3783536ec031b86885fefec5952557e7a83714fb2c40e943b5105a69ecb84`  
		Last Modified: Thu, 23 Mar 2023 00:26:50 GMT  
		Size: 8.1 MB (8137887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01efbc18b7040617b44f1b9707081241066539d148cb64ceae8ee25aa8d33940`  
		Last Modified: Thu, 23 Mar 2023 00:26:48 GMT  
		Size: 4.6 KB (4556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
