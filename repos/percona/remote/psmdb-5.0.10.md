## `percona:psmdb-5.0.10`

```console
$ docker pull percona@sha256:8c5ae9348b411d57bfc12767f3207ae535d19449ce1b63b0d4289bac146380f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0.10` - linux; amd64

```console
$ docker pull percona@sha256:9e972a4f768e1f767b6d9fa8a3e1354c0cea2f517fc274b8658b0c094daba742
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.1 MB (211098679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44e66061f6aa2b7a75c8bf682345a44a1a519265486a171c789d191e3aabcc8a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 07 Oct 2022 20:31:30 GMT
ADD file:1a763d3c32483df4f458f63f05f916dadc3830f209f506ed7f01f2bbde698c0e in / 
# Fri, 07 Oct 2022 20:31:31 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 20:58:18 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 07 Oct 2022 20:59:38 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-50 release
# Fri, 07 Oct 2022 20:59:38 GMT
ENV PSMDB_VERSION=5.0.10-9
# Fri, 07 Oct 2022 20:59:38 GMT
ENV OS_VER=el8
# Fri, 07 Oct 2022 20:59:39 GMT
ENV FULL_PERCONA_VERSION=5.0.10-9.el8
# Fri, 07 Oct 2022 20:59:39 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Fri, 07 Oct 2022 21:00:17 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Fri, 07 Oct 2022 21:00:18 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Fri, 07 Oct 2022 21:00:18 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Fri, 07 Oct 2022 21:00:19 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Fri, 07 Oct 2022 21:00:19 GMT
ENV GOSU_VERSION=1.11
# Fri, 07 Oct 2022 21:00:23 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Fri, 07 Oct 2022 21:00:25 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Fri, 07 Oct 2022 21:00:25 GMT
VOLUME [/data/db]
# Fri, 07 Oct 2022 21:00:26 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Fri, 07 Oct 2022 21:00:26 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Fri, 07 Oct 2022 21:00:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 21:00:27 GMT
EXPOSE 27017
# Fri, 07 Oct 2022 21:00:27 GMT
USER 1001
# Fri, 07 Oct 2022 21:00:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ac3ff104342371a096aefcc07640bfb6a35e22759a7dd43c53dcb9bc041669f7`  
		Last Modified: Fri, 07 Oct 2022 20:33:06 GMT  
		Size: 86.0 MB (85955384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fca43748708484a8a4bacba4823966981ac88d8a8a9f9456a0afd729d36b96`  
		Last Modified: Fri, 07 Oct 2022 21:04:11 GMT  
		Size: 3.8 MB (3761843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa0a91baf8f63afaff5082b02315a538fed32e890285346e06449e9290d5ee9`  
		Last Modified: Fri, 07 Oct 2022 21:04:24 GMT  
		Size: 112.3 MB (112295404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b13561f7fbf3716eb10829afcb0d10419319d53a4f5219f6f3e98af68b83e4`  
		Last Modified: Fri, 07 Oct 2022 21:04:09 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649c1e5476be1057bb9692e52875629454e5cca1e93c2449aebb6f4013cad3d9`  
		Last Modified: Fri, 07 Oct 2022 21:04:09 GMT  
		Size: 4.1 KB (4102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6341f84e472edc9c8d99fac3d461a7b2a8c757b592da183efe91985c5bac44`  
		Last Modified: Fri, 07 Oct 2022 21:04:07 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63db911aadf3106dd135e61297ba5e48dd58d30bb5bba102102c6d9461b0d8e9`  
		Last Modified: Fri, 07 Oct 2022 21:04:07 GMT  
		Size: 914.6 KB (914551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66de5a28a66a6892c1ebabd3e35a2bbbc859564e63f3350591471162ba70d495`  
		Last Modified: Fri, 07 Oct 2022 21:04:08 GMT  
		Size: 8.1 MB (8137890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3ddd8e0e9d69b4d5b93da172dfeeed3a5035f049dbad8e9367962a90636e1b`  
		Last Modified: Fri, 07 Oct 2022 21:04:07 GMT  
		Size: 13.2 KB (13202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cb3cdf16a814e3426ad65bb7277a45fff2c3b4d3034975e72e26f0b49c2122`  
		Last Modified: Fri, 07 Oct 2022 21:04:07 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
