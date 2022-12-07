## `percona:psmdb-5.0`

```console
$ docker pull percona@sha256:7576db4bd23e01102de22b6ba426a90541ca7c79620dfe3de175de00ce251bdc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0` - linux; amd64

```console
$ docker pull percona@sha256:68280e1b247ffe97198d5d10b354fd7b0843c5f547c914a1e6d65e78e4b9e754
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.6 MB (212601772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f04db5082859f3e521ce70b857ff376a89b4a0b6ef50f02fb20e171bb8cc060`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:14 GMT
ADD file:5a832f5300f589b7f2a820f29d0655906164c4946d5fcd467921017c28a26bee in / 
# Wed, 07 Dec 2022 01:51:15 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:14:45 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Wed, 07 Dec 2022 02:16:17 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-50 release
# Wed, 07 Dec 2022 02:16:17 GMT
ENV PSMDB_VERSION=5.0.10-9
# Wed, 07 Dec 2022 02:16:17 GMT
ENV OS_VER=el8
# Wed, 07 Dec 2022 02:16:17 GMT
ENV FULL_PERCONA_VERSION=5.0.10-9.el8
# Wed, 07 Dec 2022 02:16:17 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Wed, 07 Dec 2022 02:16:57 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Wed, 07 Dec 2022 02:16:58 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Wed, 07 Dec 2022 02:16:58 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Wed, 07 Dec 2022 02:16:59 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Wed, 07 Dec 2022 02:16:59 GMT
ENV GOSU_VERSION=1.11
# Wed, 07 Dec 2022 02:17:02 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Wed, 07 Dec 2022 02:17:06 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Wed, 07 Dec 2022 02:17:06 GMT
VOLUME [/data/db]
# Wed, 07 Dec 2022 02:17:07 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Wed, 07 Dec 2022 02:17:07 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Wed, 07 Dec 2022 02:17:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 07 Dec 2022 02:17:07 GMT
EXPOSE 27017
# Wed, 07 Dec 2022 02:17:07 GMT
USER 1001
# Wed, 07 Dec 2022 02:17:08 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4c770e098606ecfd5b78f4d61fc5e11b92fdde43d07825e543f04fe64aaa62eb`  
		Last Modified: Wed, 07 Dec 2022 01:52:57 GMT  
		Size: 87.4 MB (87445275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8051926408244e724951d0b33b920a941411550f4105512dda599fe710da528d`  
		Last Modified: Wed, 07 Dec 2022 02:20:42 GMT  
		Size: 3.8 MB (3778983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b65bb466bbb578529499934618fcb23cc45f61d6f0fff1f45a49c4e17770fc`  
		Last Modified: Wed, 07 Dec 2022 02:20:55 GMT  
		Size: 112.3 MB (112291464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89dbf1bdf93e11509de3e5afc2746945e325f9cf87e3212818e2708f5a66853`  
		Last Modified: Wed, 07 Dec 2022 02:20:40 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aeafec2bbfe462002283fdfece5054bf2371217b8eede492f44dfbea64325fb`  
		Last Modified: Wed, 07 Dec 2022 02:20:41 GMT  
		Size: 4.1 KB (4102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e2d2d93c952d1a1b263b3f196e1ba11bedfea8afb79d561ac180820b2a1c4e`  
		Last Modified: Wed, 07 Dec 2022 02:20:38 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9568dd20f1f24edef12ec590a8f424cb427f2be68138a6bbeccf331b4a2af661`  
		Last Modified: Wed, 07 Dec 2022 02:20:39 GMT  
		Size: 914.5 KB (914550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac398cc0293a7c989072083fe65c5d01b688e4681587067fb192704b6d5c8055`  
		Last Modified: Wed, 07 Dec 2022 02:20:40 GMT  
		Size: 8.1 MB (8137889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c252b7635b3ed543baca8686298c4b410690e0a1bc1eded4ea8e7b92535dfe`  
		Last Modified: Wed, 07 Dec 2022 02:20:38 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10f681e62b162f41ddd0db82c285b10b531369a9eb843f0a54d54d355b626f6`  
		Last Modified: Wed, 07 Dec 2022 02:20:39 GMT  
		Size: 4.6 KB (4560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
