## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:034ffbf8ae7ad434f2548ebea516f18bb90d1a2086c4dc46afc078aa36d0b883
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:7f897cb6b9295583111f438bc1478680964a60124bfd188d5548e4203e914af1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.1 MB (179090845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ac5ceb5aefe07f949907dd96aa7999a2c7559bd1f17f2bc2406ff5ad259f716`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 02 May 2022 20:50:56 GMT
ADD file:84bf324680059e085907eb7d75c8cb37d4d01aff3cc8241463bbc7d042db93d9 in / 
# Mon, 02 May 2022 20:50:56 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 21:18:32 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Mon, 02 May 2022 21:21:44 GMT
ENV PSMDB_VERSION=4.2.19-19
# Mon, 02 May 2022 21:21:44 GMT
ENV OS_VER=el8
# Mon, 02 May 2022 21:21:44 GMT
ENV FULL_PERCONA_VERSION=4.2.19-19.el8
# Mon, 02 May 2022 21:21:44 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Mon, 02 May 2022 21:21:48 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Mon, 02 May 2022 21:22:25 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Mon, 02 May 2022 21:22:26 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Mon, 02 May 2022 21:22:26 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Mon, 02 May 2022 21:22:27 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Mon, 02 May 2022 21:22:27 GMT
ENV GOSU_VERSION=1.11
# Mon, 02 May 2022 21:22:29 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Mon, 02 May 2022 21:22:30 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Mon, 02 May 2022 21:22:31 GMT
VOLUME [/data/db]
# Mon, 02 May 2022 21:22:31 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Mon, 02 May 2022 21:22:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 02 May 2022 21:22:31 GMT
EXPOSE 27017
# Mon, 02 May 2022 21:22:31 GMT
USER 1001
# Mon, 02 May 2022 21:22:31 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:42405d186b2e7939aa51dc1bcc0f4cf0ce1236f4d6e38f2fae9822c41e98078e`  
		Last Modified: Mon, 02 May 2022 20:51:41 GMT  
		Size: 87.5 MB (87479695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd49c577213c11123046b0380c305c6c7a9cab85caf353a056a347984b3faa4`  
		Last Modified: Mon, 02 May 2022 21:25:16 GMT  
		Size: 3.8 MB (3759058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5231d662c97215e98176c1ce7c7407689bbfca9490b8be3badfb9f3a67a3a0b4`  
		Last Modified: Mon, 02 May 2022 21:25:25 GMT  
		Size: 78.8 MB (78779255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62abed6eb2971fad54f561d241bd7f9e69c90f9fd7eb28baacc08322d8af7cf`  
		Last Modified: Mon, 02 May 2022 21:25:15 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d9518e408e8b785fdd9109b00494d6e33c5468be7019738db278a9d1fc81b3`  
		Last Modified: Mon, 02 May 2022 21:25:13 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22c5e78cde6bb561a0015264f2b0657ca126907521157c40c0e5c94fe775d75`  
		Last Modified: Mon, 02 May 2022 21:25:13 GMT  
		Size: 10.6 KB (10579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e339b2e1a89059feb72f204d1a3241efc4dddf7a7ce3187418ce6d106904ddb4`  
		Last Modified: Mon, 02 May 2022 21:25:13 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a24970d5cb8962187ec1b751b52e620528f5a99d0a062aedff25e46857638e4`  
		Last Modified: Mon, 02 May 2022 21:25:15 GMT  
		Size: 8.1 MB (8137885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e05f3cd7f5baf2512f9971d7ed377dd2a017154100c8c140580e6af5fe8111`  
		Last Modified: Mon, 02 May 2022 21:25:13 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
