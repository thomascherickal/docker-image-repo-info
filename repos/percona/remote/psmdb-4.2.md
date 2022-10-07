## `percona:psmdb-4.2`

```console
$ docker pull percona@sha256:ebb8722de6b6b5f01ec502047791767976100e2382d8a34cb106b5770c7b32e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2` - linux; amd64

```console
$ docker pull percona@sha256:1434aa049bf9b3736bcabed50cfda1fd3390f8f9d84b4e7b2f2088ec96423df0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.4 MB (176381370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4720b2b8b259e5b1f768327657aa130e7c606848bf544a1a72568efaf7b67a33`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 07 Oct 2022 20:31:30 GMT
ADD file:1a763d3c32483df4f458f63f05f916dadc3830f209f506ed7f01f2bbde698c0e in / 
# Fri, 07 Oct 2022 20:31:31 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 20:58:18 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 07 Oct 2022 21:01:31 GMT
ENV PSMDB_VERSION=4.2.21-21
# Fri, 07 Oct 2022 21:01:31 GMT
ENV OS_VER=el8
# Fri, 07 Oct 2022 21:01:31 GMT
ENV FULL_PERCONA_VERSION=4.2.21-21.el8
# Fri, 07 Oct 2022 21:01:31 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Fri, 07 Oct 2022 21:01:34 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Fri, 07 Oct 2022 21:02:09 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Fri, 07 Oct 2022 21:02:10 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Fri, 07 Oct 2022 21:02:10 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Fri, 07 Oct 2022 21:02:11 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Fri, 07 Oct 2022 21:02:11 GMT
ENV GOSU_VERSION=1.11
# Fri, 07 Oct 2022 21:02:15 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Fri, 07 Oct 2022 21:02:16 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Fri, 07 Oct 2022 21:02:16 GMT
VOLUME [/data/db]
# Fri, 07 Oct 2022 21:02:17 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Fri, 07 Oct 2022 21:02:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 21:02:17 GMT
EXPOSE 27017
# Fri, 07 Oct 2022 21:02:17 GMT
USER 1001
# Fri, 07 Oct 2022 21:02:17 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ac3ff104342371a096aefcc07640bfb6a35e22759a7dd43c53dcb9bc041669f7`  
		Last Modified: Fri, 07 Oct 2022 20:33:06 GMT  
		Size: 86.0 MB (85955384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf835dd74b507e7dbe10fb9476a231b4b7a17cf4bdb5805a377d88fd283ea2c2`  
		Last Modified: Fri, 07 Oct 2022 21:05:05 GMT  
		Size: 3.8 MB (3761844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42473d180aedd481f4bfc3d3b3beab40d78163de46eb889f4631cb6aa03e579e`  
		Last Modified: Fri, 07 Oct 2022 21:05:13 GMT  
		Size: 77.6 MB (77591292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab70ad2354d2d090847cb0351ab630e4ee9fccb6356349b2df0e0c824083e234`  
		Last Modified: Fri, 07 Oct 2022 21:05:04 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5707bd5f95ce18435ea3b5f695635418b905edf0cae869bda2d399cb8765b0f`  
		Last Modified: Fri, 07 Oct 2022 21:05:01 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3d5ff296813a1338a433680476de039c4961d4500ef9ce82687433ea8f9508`  
		Last Modified: Fri, 07 Oct 2022 21:05:01 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bd626eaa14927e336ed8acf913d464f48a85c2709138e585c5ad66e521269e`  
		Last Modified: Fri, 07 Oct 2022 21:05:01 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0abbf8bc6da2acd5700bcf3dc17829c39bdc7c21bafdb1d8b87b130053211e`  
		Last Modified: Fri, 07 Oct 2022 21:05:03 GMT  
		Size: 8.1 MB (8137894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e5a9b96ac407f922f1e63ee1deec5f226768905fab45d9901d8538c156e297`  
		Last Modified: Fri, 07 Oct 2022 21:05:01 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
