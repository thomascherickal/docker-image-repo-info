## `percona:psmdb-6.0.6`

```console
$ docker pull percona@sha256:948161caf1185872446f5c12aec045e7ee97ca6dea8f1360a2edd0861ef26645
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-6.0.6` - linux; amd64

```console
$ docker pull percona@sha256:fe2f29cf57c86ae7333c52dd4b5cb023081688d68b738e587f9db6e2e17c8314
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.7 MB (272721827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c7111d989c1fb2c6d50663a0603a59f1b45112667ca8e558bb06033e9c1361`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 12 Oct 2023 21:28:19 GMT
ADD file:08ccec25d0d1459d4c27b2b0354bb526203faac57f1570a94b91c0d83e7474db in / 
# Thu, 12 Oct 2023 21:28:20 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 22:22:31 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 12 Oct 2023 22:24:15 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY
# Thu, 12 Oct 2023 22:24:15 GMT
ENV PSMDB_VERSION=6.0.6-5
# Thu, 12 Oct 2023 22:24:15 GMT
ENV OS_VER=el8
# Thu, 12 Oct 2023 22:24:15 GMT
ENV FULL_PERCONA_VERSION=6.0.6-5.el8
# Thu, 12 Oct 2023 22:24:15 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 12 Oct 2023 22:24:15 GMT
ENV PSMDB_REPO=release
# Thu, 12 Oct 2023 22:25:10 GMT
RUN set -ex;     percona-release enable psmdb-60 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         percona-mongodb-mongosh         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-60/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 12 Oct 2023 22:25:11 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Thu, 12 Oct 2023 22:25:11 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 12 Oct 2023 22:25:12 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 12 Oct 2023 22:25:12 GMT
ENV GOSU_VERSION=1.11
# Thu, 12 Oct 2023 22:25:16 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 12 Oct 2023 22:25:19 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 12 Oct 2023 22:25:19 GMT
VOLUME [/data/db]
# Thu, 12 Oct 2023 22:25:20 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Thu, 12 Oct 2023 22:25:20 GMT
COPY file:7ab35f422fd362616b84e1dc71329cc9be05b7f834182c48bf98ceb92ee28956 in /entrypoint.sh 
# Thu, 12 Oct 2023 22:25:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 22:25:20 GMT
EXPOSE 27017
# Thu, 12 Oct 2023 22:25:20 GMT
USER 1001
# Thu, 12 Oct 2023 22:25:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:eeccb7e6dc78cf3d674adcfebd1e8ff22148cf87ec3d731d3cd73eff435f6d9f`  
		Last Modified: Thu, 12 Oct 2023 21:29:47 GMT  
		Size: 88.0 MB (88009290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e26e8195de4845ab2bf941a400b26071c3b15161e70e9b0d422d9dc67a7576`  
		Last Modified: Thu, 12 Oct 2023 22:30:23 GMT  
		Size: 3.8 MB (3801638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186f27567efcfcd014f47c7bce0dfe9019281ef774c2f345372187b21e366dba`  
		Last Modified: Thu, 12 Oct 2023 22:30:43 GMT  
		Size: 171.8 MB (171824336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89bfc5a9ceb3a8c474dbc4e878ae0b7dda97ca7382a833abf557b8b8bd5d84b3`  
		Last Modified: Thu, 12 Oct 2023 22:30:22 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcafd63a11d76bd28bd8c13909acdf1eb28f33b11244eee99cb738cd9e64665`  
		Last Modified: Thu, 12 Oct 2023 22:30:21 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdcec744f978cf7250f9625788fa7cd9e9478c0a2293a58aa29bd377dedc8c6`  
		Last Modified: Thu, 12 Oct 2023 22:30:19 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9700e39f6eb52339c5da7e1e37351369feaa9cebf80342fc212a3c52059dd37`  
		Last Modified: Thu, 12 Oct 2023 22:30:19 GMT  
		Size: 914.5 KB (914549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a177ac6ccbf63410cf801ed435563058338401e5ed4cf68c5a3f6f9e56ef671`  
		Last Modified: Thu, 12 Oct 2023 22:30:21 GMT  
		Size: 8.1 MB (8137887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d73f92033014a62c7161f572f119d558f249acf7469be1e5dfa94a4a0add45`  
		Last Modified: Thu, 12 Oct 2023 22:30:19 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db60b613ddce37d088004b73a1153b72ec134406ff66de243bcdbf04aa1e9e6`  
		Last Modified: Thu, 12 Oct 2023 22:30:19 GMT  
		Size: 4.6 KB (4566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
