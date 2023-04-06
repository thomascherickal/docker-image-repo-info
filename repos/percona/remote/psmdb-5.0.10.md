## `percona:psmdb-5.0.10`

```console
$ docker pull percona@sha256:695a4f97cbb3282440178f833352e556f2e55ecbe0eb2cceb905d9cef436e4d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-5.0.10` - linux; amd64

```console
$ docker pull percona@sha256:e6347fae9e670a89d2ab3e0f01c06a176483635e97228731d645f86842101ad1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.6 MB (213586333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17da9766dce0bcf7eb2cca4b33fd09d882fba3387813673ed4c654c2fb5641ba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 06 Apr 2023 18:20:21 GMT
ADD file:b8264f84035130ce589141b141f035b09d193dfca890914ecc0dc7ecd194e4b3 in / 
# Thu, 06 Apr 2023 18:20:22 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:39:05 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 06 Apr 2023 18:39:09 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-50 release
# Thu, 06 Apr 2023 18:39:09 GMT
ENV PSMDB_VERSION=5.0.10-9
# Thu, 06 Apr 2023 18:39:09 GMT
ENV OS_VER=el8
# Thu, 06 Apr 2023 18:39:09 GMT
ENV FULL_PERCONA_VERSION=5.0.10-9.el8
# Thu, 06 Apr 2023 18:39:09 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 06 Apr 2023 18:39:50 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-50/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 06 Apr 2023 18:39:51 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 06 Apr 2023 18:39:51 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 06 Apr 2023 18:39:52 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 06 Apr 2023 18:39:52 GMT
ENV GOSU_VERSION=1.11
# Thu, 06 Apr 2023 18:39:55 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 06 Apr 2023 18:39:57 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 06 Apr 2023 18:39:57 GMT
VOLUME [/data/db]
# Thu, 06 Apr 2023 18:39:58 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Thu, 06 Apr 2023 18:39:58 GMT
COPY file:e6e9d8018241e8459aecdafe395233cbfaee0351829ed9f41c721972a859a6d6 in /entrypoint.sh 
# Thu, 06 Apr 2023 18:39:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:39:58 GMT
EXPOSE 27017
# Thu, 06 Apr 2023 18:39:59 GMT
USER 1001
# Thu, 06 Apr 2023 18:39:59 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:06d6f22c2168ed40d437d9165a6c726f0bcaa2fd76ab943ed29f9ee4216e11fb`  
		Last Modified: Thu, 06 Apr 2023 18:21:04 GMT  
		Size: 88.4 MB (88436523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e128868022fb47efb81283548ee695af7a92321f508e35e00b7f604158be47`  
		Last Modified: Thu, 06 Apr 2023 18:42:19 GMT  
		Size: 3.8 MB (3772643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b8e6dcb763589bcabd10c1ac9dba95aa31fc83e2785fc2427207019220f0a5`  
		Last Modified: Thu, 06 Apr 2023 18:42:31 GMT  
		Size: 112.3 MB (112291129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7682eb7ee08486dd0c05f37e7e2c69fc1984978ef21b06510e62c9601f7bba25`  
		Last Modified: Thu, 06 Apr 2023 18:42:18 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ec8c7c193fc96db2b577c2ac223c71e0250051a3dfe5f4b218efc8ccc9f72c`  
		Last Modified: Thu, 06 Apr 2023 18:42:18 GMT  
		Size: 4.1 KB (4102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9139ab758ae9ddc9b48858f6ea1a3315e08de87992a83f4ce044011c5a39c9ec`  
		Last Modified: Thu, 06 Apr 2023 18:42:16 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e291cca98175e60bac13c3965306bff1143c6344c176339ab25dd691abcece67`  
		Last Modified: Thu, 06 Apr 2023 18:42:16 GMT  
		Size: 914.5 KB (914544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec2b8d78664928758a920166131a87efdd3b1560926ffe56073b1b80a7bcf2e`  
		Last Modified: Thu, 06 Apr 2023 18:42:18 GMT  
		Size: 8.1 MB (8137886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953bd79f278dca3dd15cd57c55117b087875236853bbb743eec3fe844fc4b89a`  
		Last Modified: Thu, 06 Apr 2023 18:42:16 GMT  
		Size: 13.2 KB (13205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b74a7d67355f18f11a53e73ef6f0afee43fa47dbe44dc7669884a200b9e0102`  
		Last Modified: Thu, 06 Apr 2023 18:42:16 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
