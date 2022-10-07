## `percona:psmdb-4.4.15`

```console
$ docker pull percona@sha256:a594275279b34c04aa89d05d663baed519256eff0624ad489371f92c7c9ba369
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4.15` - linux; amd64

```console
$ docker pull percona@sha256:233bf79a44e3a2e03c113b5ea5b68df37b1b6aefe8287ab686eaef42315be562
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.7 MB (195703694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05295959ab98fe1ced7376971a7709eafa71a59660310253eeb890600c75177a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 07 Oct 2022 20:31:30 GMT
ADD file:1a763d3c32483df4f458f63f05f916dadc3830f209f506ed7f01f2bbde698c0e in / 
# Fri, 07 Oct 2022 20:31:31 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 20:58:18 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Fri, 07 Oct 2022 21:00:36 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Fri, 07 Oct 2022 21:00:36 GMT
ENV PSMDB_VERSION=4.4.15-15
# Fri, 07 Oct 2022 21:00:36 GMT
ENV OS_VER=el8
# Fri, 07 Oct 2022 21:00:36 GMT
ENV FULL_PERCONA_VERSION=4.4.15-15.el8
# Fri, 07 Oct 2022 21:00:36 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Fri, 07 Oct 2022 21:01:13 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Fri, 07 Oct 2022 21:01:14 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Fri, 07 Oct 2022 21:01:14 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Fri, 07 Oct 2022 21:01:15 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Fri, 07 Oct 2022 21:01:15 GMT
ENV GOSU_VERSION=1.11
# Fri, 07 Oct 2022 21:01:18 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Fri, 07 Oct 2022 21:01:20 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Fri, 07 Oct 2022 21:01:20 GMT
VOLUME [/data/db]
# Fri, 07 Oct 2022 21:01:20 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Fri, 07 Oct 2022 21:01:21 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Fri, 07 Oct 2022 21:01:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 21:01:21 GMT
EXPOSE 27017
# Fri, 07 Oct 2022 21:01:21 GMT
USER 1001
# Fri, 07 Oct 2022 21:01:21 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ac3ff104342371a096aefcc07640bfb6a35e22759a7dd43c53dcb9bc041669f7`  
		Last Modified: Fri, 07 Oct 2022 20:33:06 GMT  
		Size: 86.0 MB (85955384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76b224189b8021aa8294f67e83e6a255f75be8528a4b76c55439294415c135d`  
		Last Modified: Fri, 07 Oct 2022 21:04:39 GMT  
		Size: 3.8 MB (3761805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eaf59c3a2a07db5bab1924392e8f4aef116c69681024f3972e1fbcf97750564`  
		Last Modified: Fri, 07 Oct 2022 21:04:50 GMT  
		Size: 96.9 MB (96900455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987697625afe7621f210c53ab344ba1a96d33bee2b57cddc79c9c719493dda81`  
		Last Modified: Fri, 07 Oct 2022 21:04:38 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956b2bb541699d19e87771ebc0182c2b75ace428951d9e65fc6ddf3c742d0916`  
		Last Modified: Fri, 07 Oct 2022 21:04:37 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ca9787168420ea1a142ca61c7bdb476f442459f91db0efc9b3246c176a956d`  
		Last Modified: Fri, 07 Oct 2022 21:04:35 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ee0c12c82a69d564c919823fcd340b04a12ffef678ed48d31d0e3fcf220790`  
		Last Modified: Fri, 07 Oct 2022 21:04:35 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9573fe691e4e1010488d075d4bfe2040eb3b824e385b735d4d97c3dfda3ced9e`  
		Last Modified: Fri, 07 Oct 2022 21:04:36 GMT  
		Size: 8.1 MB (8137893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d20b664518504fdf25b1ec11084883894e1e6ea7ee2afd686db76b1c477bab`  
		Last Modified: Fri, 07 Oct 2022 21:04:35 GMT  
		Size: 13.2 KB (13202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf3c145c83d627ed6321b6aefa3ac25db3a00291d21b28d5232da3b24e4a1f8`  
		Last Modified: Fri, 07 Oct 2022 21:04:35 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
