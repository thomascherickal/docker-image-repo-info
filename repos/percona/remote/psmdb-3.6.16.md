## `percona:psmdb-3.6.16`

```console
$ docker pull percona@sha256:3b45ebe07a6e764f96b0cff8c2568a55512a68ae3d46cdc7e284d890aedf5c1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `percona:psmdb-3.6.16` - linux; amd64

```console
$ docker pull percona@sha256:f840867a97e0a8f6c239faae8f9ee505f81eac4ce023e9b777a9b351deff60b4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.2 MB (156237561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c13f4a85937ed8fc5d1cf8ca167808ebf58987b27f278ec366517892eda1b05`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Wed, 29 Jan 2020 19:37:33 GMT
LABEL org.label-schema.schema-version=1.0
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.name=Percona Server for MongoDB
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.vendor=Percona
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.label-schema.license=SSPLv1
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.opencontainers.image.title=Percona Server for MongoDB
# Wed, 29 Jan 2020 19:37:34 GMT
LABEL org.opencontainers.image.vendor=Percona
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.description=Percona Server for MongoDB is our free and open-source drop-in replacement for MongoDB Community Edition. It offers all the features and benefits of MongoDB Community Edition, plus additional enterprise-grade functionality.
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.license=SSPLv1
# Wed, 29 Jan 2020 19:37:35 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 29 Jan 2020 19:38:27 GMT
ENV PSMDB_VERSION=3.6.16-3.6
# Wed, 29 Jan 2020 19:38:27 GMT
LABEL org.label-schema.schema-version=3.6.16-3.6
# Wed, 29 Jan 2020 19:38:27 GMT
LABEL org.opencontainers.image.version=3.6.16-3.6
# Wed, 29 Jan 2020 19:38:31 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5;     gpg --batch --keyserver pool.sks-keyservers.net --recv-keys 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5;         gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 6341AB2753D78A78A7C27BB124C6A8A7F4A80EB5 > ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7;     gpg --batch --export --armor 91E97D7C4A5E96F17F3E888F6A2FAEA2352C64E5 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-CentOS-7 ${GNUPGHOME}/RPM-GPG-KEY-EPEL-7;         curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Wed, 29 Jan 2020 19:38:31 GMT
ENV OS_VER=el7
# Wed, 29 Jan 2020 19:38:31 GMT
ENV FULL_PERCONA_VERSION=3.6.16-3.6.el7
# Wed, 29 Jan 2020 19:38:32 GMT
ENV K8S_TOOLS_VERSION=0.4.2
# Wed, 29 Jan 2020 19:38:37 GMT
RUN set -ex;     curl -Lf -o /tmp/jq.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/j/jq-1.6-1.el7.x86_64.rpm;     curl -Lf -o /tmp/oniguruma.rpm https://download.fedoraproject.org/pub/epel/7/x86_64/Packages/o/oniguruma-5.9.5-3.el7.x86_64.rpm;     rpmkeys --checksig /tmp/jq.rpm /tmp/oniguruma.rpm;         rpm -i /tmp/jq.rpm /tmp/oniguruma.rpm;     rm -rf /tmp/jq.rpm /tmp/oniguruma.rpm
# Wed, 29 Jan 2020 19:39:33 GMT
RUN set -ex;     sed -i '/nodocs/d' /etc/yum.conf || :;     yum install -y         yum-utils         shadow-utils         curl         procps-ng         Percona-Server-MongoDB-36-shell-${FULL_PERCONA_VERSION}         Percona-Server-MongoDB-36-mongos-${FULL_PERCONA_VERSION};         repoquery -a --location             policycoreutils                 | xargs curl -Lf -o /tmp/policycoreutils.rpm;         repoquery -a --location             Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}                 | xargs curl -Lf -o /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         rpm -iv /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm --nodeps;                 rm -rf /tmp/policycoreutils.rpm /tmp/Percona-Server-MongoDB-36-server-${FULL_PERCONA_VERSION}.rpm;         yum clean all;         rm -rf /var/cache/yum /data/db && mkdir -p /data/db;         chown -R 1001:0 /data/db
# Wed, 29 Jan 2020 19:39:34 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 29 Jan 2020 19:39:34 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 29 Jan 2020 19:39:35 GMT
RUN cp /usr/share/doc/Percona-Server-MongoDB-36-server-$(echo ${FULL_PERCONA_VERSION} | cut -d - -f 1)/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 29 Jan 2020 19:39:38 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 29 Jan 2020 19:39:38 GMT
VOLUME [/data/db]
# Wed, 29 Jan 2020 19:39:38 GMT
COPY file:85995e73e1e4d284ba65fabe65ed1e96fcb9c00ac0d328edb8b0b48749d784e1 in /entrypoint.sh 
# Wed, 29 Jan 2020 19:39:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jan 2020 19:39:39 GMT
EXPOSE 27017
# Wed, 29 Jan 2020 19:39:39 GMT
USER 1001
# Wed, 29 Jan 2020 19:39:39 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fbe7d180ed89de6f48845a8efec93f14b170ee9de1c4843fe0a55e6c22947c`  
		Last Modified: Wed, 29 Jan 2020 19:40:34 GMT  
		Size: 6.4 MB (6373087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03f2b091cecd7b21c74ef437e20f83829ed002f85676ac67ad5cde9db056e17`  
		Last Modified: Wed, 29 Jan 2020 19:40:34 GMT  
		Size: 6.7 MB (6701948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f885049d322d8f846ce683718c61bcbeedbb1d7efb3520f8be6dbe3fb4fe74`  
		Last Modified: Wed, 29 Jan 2020 19:40:45 GMT  
		Size: 59.8 MB (59796187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0d5065db278bfcd88761044e018119b4188aa3c9b581ccab40a454f423ebff`  
		Last Modified: Wed, 29 Jan 2020 19:40:29 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd4b8352524372d9e80ed51147ba64189619c7b93334d73daf3207e6b626543`  
		Last Modified: Wed, 29 Jan 2020 19:40:29 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f364e83bd306717868204518f83ac9930f43778a9048fe6def86bb41c4532b41`  
		Last Modified: Wed, 29 Jan 2020 19:40:29 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c090b71c27de9ac8659f24929c6ef467459fbfcb5547024c5cf15d8749c4dd`  
		Last Modified: Wed, 29 Jan 2020 19:40:33 GMT  
		Size: 7.6 MB (7565360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809ab9a5e9e8bd1cc9a33fd286587c272d68e5667ce1764c301cd55d6e91caa1`  
		Last Modified: Wed, 29 Jan 2020 19:40:29 GMT  
		Size: 4.0 KB (4017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
