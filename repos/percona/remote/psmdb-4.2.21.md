## `percona:psmdb-4.2.21`

```console
$ docker pull percona@sha256:6901f769fcdb2dddb9d5503392279ca66632240ab0c7f32d32ad00e91f9203e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.2.21` - linux; amd64

```console
$ docker pull percona@sha256:58ff120bad41d31dac8486ac302a80f620c10835992bca6535ce8f89dc027a02
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.4 MB (176361286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa2872eed817c747a98ebe3896f5f7bbb5b97217aa47dd793307016090adc59`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 04 Nov 2022 23:32:54 GMT
ADD file:2bc42b6875b914b1b6d99bf9e219400d534d6f6c5c0c529278df93ef1f2684c6 in / 
# Fri, 04 Nov 2022 23:32:54 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:27:35 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Sat, 05 Nov 2022 02:30:59 GMT
ENV PSMDB_VERSION=4.2.21-21
# Sat, 05 Nov 2022 02:31:00 GMT
ENV OS_VER=el8
# Sat, 05 Nov 2022 02:31:00 GMT
ENV FULL_PERCONA_VERSION=4.2.21-21.el8
# Sat, 05 Nov 2022 02:31:00 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Sat, 05 Nov 2022 02:31:02 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-42 release
# Sat, 05 Nov 2022 02:31:37 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         jq         procps-ng         oniguruma         tar         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-42/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Sat, 05 Nov 2022 02:31:38 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Sat, 05 Nov 2022 02:31:38 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Sat, 05 Nov 2022 02:31:39 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Sat, 05 Nov 2022 02:31:39 GMT
ENV GOSU_VERSION=1.11
# Sat, 05 Nov 2022 02:31:41 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Sat, 05 Nov 2022 02:31:43 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Sat, 05 Nov 2022 02:31:43 GMT
VOLUME [/data/db]
# Sat, 05 Nov 2022 02:31:43 GMT
COPY file:f695d42c4add7cde05638253f593b5a3f599ec240da8e578b8c6049c6e1672a9 in /entrypoint.sh 
# Sat, 05 Nov 2022 02:31:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Nov 2022 02:31:44 GMT
EXPOSE 27017
# Sat, 05 Nov 2022 02:31:44 GMT
USER 1001
# Sat, 05 Nov 2022 02:31:44 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f53ad0b8b1b9614b09bf69c21c965b04e683defa0796b21b55af5458264e49be`  
		Last Modified: Fri, 04 Nov 2022 23:34:33 GMT  
		Size: 85.9 MB (85945697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7bc0a2d84e4a0c583f5d600b5b1b7dd98b1f0fc3e63787698b7f1e46dcea508`  
		Last Modified: Sat, 05 Nov 2022 02:34:20 GMT  
		Size: 3.8 MB (3761208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf58c7082d2687ae48c3edcd95a28da7ad0ec32ccec3c9f85c5a45bcce5844d`  
		Last Modified: Sat, 05 Nov 2022 02:34:28 GMT  
		Size: 77.6 MB (77581542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90651c6f41a7262f2415a5d3acfec0d7a83e1cf9cafe9a1597e2e91699089ad`  
		Last Modified: Sat, 05 Nov 2022 02:34:19 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7689eb29eb7e693503e6601df0032ce2ec5d30a5070523f63014672dbdc51951`  
		Last Modified: Sat, 05 Nov 2022 02:34:17 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a8d09f93699969d2c546fdf2204205904e254b5ca51f5549ee4fca31f50f31`  
		Last Modified: Sat, 05 Nov 2022 02:34:17 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdeb3c74493942465aab670483c95721524ea5ff97249192f40b204c6cadbdab`  
		Last Modified: Sat, 05 Nov 2022 02:34:17 GMT  
		Size: 914.5 KB (914544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39380ebee04534753ec86a0a475caaa62837ebbe46b479f3e9db50307d86d4ae`  
		Last Modified: Sat, 05 Nov 2022 02:34:18 GMT  
		Size: 8.1 MB (8137890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1dbcbdaa607efd87beb5d618c2c00090a4af0186f60215a1ab8bbff85719d24`  
		Last Modified: Sat, 05 Nov 2022 02:34:17 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
