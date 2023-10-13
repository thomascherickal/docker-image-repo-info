## `percona:psmdb-4.4`

```console
$ docker pull percona@sha256:e5df9ad41e4565022c65398a01170307436b2b491e195dd8d7c11057964deefe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4` - linux; amd64

```console
$ docker pull percona@sha256:9001e5404b09afec88ead2f3ce629ea792001d7661c49197accb6c155ef62e3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.7 MB (236706048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8100ca0ec1cc42d4260eec28a543dafa00ff97f5629091db435d63ccd544ed1`
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
# Thu, 12 Oct 2023 22:26:46 GMT
ENV PSMDB_VERSION=4.4.22-21
# Thu, 12 Oct 2023 22:26:46 GMT
ENV OS_VER=el8
# Thu, 12 Oct 2023 22:26:46 GMT
ENV FULL_PERCONA_VERSION=4.4.22-21.el8
# Thu, 12 Oct 2023 22:26:46 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 12 Oct 2023 22:26:46 GMT
ENV PSMDB_REPO=release
# Thu, 12 Oct 2023 22:27:37 GMT
RUN set -ex;     percona-release enable psmdb-44 ${PSMDB_REPO};     dnf config-manager --enable ol8_u4_security_validation;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         percona-server-mongodb-tools-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         cyrus-sasl-gssapi         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/${PSMDB_REPO}/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 12 Oct 2023 22:27:38 GMT
RUN useradd -u 1001 -r -g 0 -m -s /sbin/nologin             -c "Default Application User" mongodb;     chmod g+rwx /var/log/mongo;     chown :0 /var/log/mongo
# Thu, 12 Oct 2023 22:27:38 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 12 Oct 2023 22:27:39 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 12 Oct 2023 22:27:39 GMT
ENV GOSU_VERSION=1.11
# Thu, 12 Oct 2023 22:27:42 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 12 Oct 2023 22:27:44 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 12 Oct 2023 22:27:44 GMT
VOLUME [/data/db]
# Thu, 12 Oct 2023 22:27:45 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Thu, 12 Oct 2023 22:27:45 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Thu, 12 Oct 2023 22:27:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 22:27:45 GMT
EXPOSE 27017
# Thu, 12 Oct 2023 22:27:46 GMT
USER 1001
# Thu, 12 Oct 2023 22:27:46 GMT
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
	-	`sha256:148a7ae2dd4f8983eb723ede1c169a988b0eec3006f4ca964286f8433f3eae8d`  
		Last Modified: Thu, 12 Oct 2023 22:31:43 GMT  
		Size: 135.8 MB (135808558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d67a46e8ed49eff10768c6fc48ea4d03e9da4dbbdc5ceb037de760de4e45dfe`  
		Last Modified: Thu, 12 Oct 2023 22:31:26 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba014ac89564cdc99d5b392f1bfd512e95a5bfaba916c6dccd1a431d66df9c7`  
		Last Modified: Thu, 12 Oct 2023 22:31:25 GMT  
		Size: 4.1 KB (4104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b381e9a672a1dfc74fbe92ae620b2be8e5f3ed479e54117e59cba500120fce`  
		Last Modified: Thu, 12 Oct 2023 22:31:26 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce2e9c77cf08c5a8ac08845c6ae68eb864db13181bbc4ad8ada4e40ce96fdb4`  
		Last Modified: Thu, 12 Oct 2023 22:31:24 GMT  
		Size: 914.6 KB (914552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6795d08f80a7b2686c413458095dc6cad8fe7d59a74599f5f1e5a294078e481`  
		Last Modified: Thu, 12 Oct 2023 22:31:25 GMT  
		Size: 8.1 MB (8137890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161a2393a71514fbdeebfa07681565cf70f18cd7a404becd5ba2f6ff76bac36a`  
		Last Modified: Thu, 12 Oct 2023 22:31:23 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a03b65f6994e586e0e7856c553747be6cdb443d612c8944760babdcc356af41`  
		Last Modified: Thu, 12 Oct 2023 22:31:23 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
