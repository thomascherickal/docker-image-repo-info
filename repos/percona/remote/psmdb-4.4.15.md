## `percona:psmdb-4.4.15`

```console
$ docker pull percona@sha256:e17051057081a92071971039a890a6926697ca58af5768ce1498dec980a9a843
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `percona:psmdb-4.4.15` - linux; amd64

```console
$ docker pull percona@sha256:3868ed6f348a9e66b4fabe3c5130aaff163fe21808347cab67aba8a36a9e12df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.2 MB (198160879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa67c82db307356605f3b1c91bc4bf59b830c69709fbef124e87ae6c22f385ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 22 Mar 2023 23:55:09 GMT
ADD file:9545a60b93a26aad3efb7cb70c1d2099f15bf3adf38467dc56f286ff438b89b2 in / 
# Wed, 22 Mar 2023 23:55:10 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:20:39 GMT
LABEL org.opencontainers.image.authors=info@percona.com
# Thu, 23 Mar 2023 00:23:06 GMT
RUN set -ex;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A 99DB70FAE1D7CE227FB6488205B555B38483C65D 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1;     gpg --batch --export --armor 430BDF5C56E7C94E848EE60C1C4CBDCDCD2EFD2A > ${GNUPGHOME}/RPM-GPG-KEY-Percona;     gpg --batch --export --armor 99DB70FAE1D7CE227FB6488205B555B38483C65D > ${GNUPGHOME}/RPM-GPG-KEY-centosofficial;     gpg --batch --export --armor 94E279EB8D8F25B21810ADF121EA45AB2F86D6A1 > ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     rpmkeys --import ${GNUPGHOME}/RPM-GPG-KEY-Percona ${GNUPGHOME}/RPM-GPG-KEY-centosofficial ${GNUPGHOME}/RPM-GPG-KEY-EPEL-8;     curl -Lf -o /tmp/percona-release.rpm https://repo.percona.com/yum/percona-release-latest.noarch.rpm;     rpmkeys --checksig /tmp/percona-release.rpm;     rpm -i /tmp/percona-release.rpm;     rm -rf "$GNUPGHOME" /tmp/percona-release.rpm;     rpm --import /etc/pki/rpm-gpg/PERCONA-PACKAGING-KEY;     percona-release enable psmdb-44 release
# Thu, 23 Mar 2023 00:23:06 GMT
ENV PSMDB_VERSION=4.4.15-15
# Thu, 23 Mar 2023 00:23:06 GMT
ENV OS_VER=el8
# Thu, 23 Mar 2023 00:23:06 GMT
ENV FULL_PERCONA_VERSION=4.4.15-15.el8
# Thu, 23 Mar 2023 00:23:06 GMT
ENV K8S_TOOLS_VERSION=0.5.0
# Thu, 23 Mar 2023 00:23:46 GMT
RUN set -ex;     dnf -y install         percona-server-mongodb-mongos-${FULL_PERCONA_VERSION}         percona-server-mongodb-shell-${FULL_PERCONA_VERSION}         procps-ng         jq         tar         oniguruma         policycoreutils;             curl -Lf -o /tmp/Percona-Server-MongoDB-server.rpm http://repo.percona.com/psmdb-44/yum/release/8/RPMS/x86_64/percona-server-mongodb-server-${FULL_PERCONA_VERSION}.x86_64.rpm;     rpmkeys --checksig /tmp/Percona-Server-MongoDB-server.rpm;     rpm -iv /tmp/Percona-Server-MongoDB-server.rpm --nodeps;     rm -rf /tmp/Percona-Server-MongoDB-server.rpm;     dnf clean all;     rm -rf /var/cache/dnf /var/cache/yum /data/db && mkdir -p /data/db;     chown -R 1001:0 /data/db
# Thu, 23 Mar 2023 00:23:46 GMT
RUN useradd -u 1001 -r -g 0 -s /sbin/nologin             -c "Default Application User" mongodb
# Thu, 23 Mar 2023 00:23:46 GMT
COPY file:b7c621ae843e72f20dd7ef20e8c42b89234688ceed5018592c3e5bfa61048aad in /licenses/LICENSE.Dockerfile 
# Thu, 23 Mar 2023 00:23:47 GMT
RUN cp /usr/share/doc/percona-server-mongodb-server/LICENSE-Community.txt /licenses/LICENSE.Percona-Server-for-MongoDB
# Thu, 23 Mar 2023 00:23:47 GMT
ENV GOSU_VERSION=1.11
# Thu, 23 Mar 2023 00:23:50 GMT
RUN set -eux;     curl -Lf -o /usr/bin/gosu https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64;     curl -Lf -o /usr/bin/gosu.asc https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-amd64.asc;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/bin/gosu.asc /usr/bin/gosu;     rm -rf "$GNUPGHOME" /usr/bin/gosu.asc;         chmod +x /usr/bin/gosu;     curl -f -o /licenses/LICENSE.gosu https://raw.githubusercontent.com/tianon/gosu/${GOSU_VERSION}/LICENSE
# Thu, 23 Mar 2023 00:23:52 GMT
RUN set -ex;     curl -fSL https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/k8s-mongodb-initiator -o /usr/local/bin/k8s-mongodb-initiator;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/mongodb-healthcheck -o /usr/local/bin/mongodb-healthcheck;     curl -fSL  https://github.com/percona/mongodb-orchestration-tools/releases/download/${K8S_TOOLS_VERSION}/SHA256SUMS -o /tmp/SHA256SUMS;     echo "$(grep 'k8s-mongodb-initiator' /tmp/SHA256SUMS | awk '{print $1}')" /usr/local/bin/k8s-mongodb-initiator | sha256sum -c -;     echo "$(grep 'mongodb-healthcheck' /tmp/SHA256SUMS   | awk '{print $1}')" /usr/local/bin/mongodb-healthcheck   | sha256sum -c -;     rm -f /tmp/SHA256SUMS;         chmod 0755 /usr/local/bin/k8s-mongodb-initiator /usr/local/bin/mongodb-healthcheck
# Thu, 23 Mar 2023 00:23:52 GMT
VOLUME [/data/db]
# Thu, 23 Mar 2023 00:23:52 GMT
RUN set -ex;     curl -fSL https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js -o /js-yaml.js;     echo "45dc3dd03dc07a06705a2c2989b8c7f709013f04bd5386e3279d4e447f07ebd7  /js-yaml.js" | sha256sum -c -
# Thu, 23 Mar 2023 00:23:53 GMT
COPY file:2e691e8e3c29008da8a3c85bbe67de1e1e3fbb73ae7ec22473431d5a771341bf in /entrypoint.sh 
# Thu, 23 Mar 2023 00:23:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Mar 2023 00:23:53 GMT
EXPOSE 27017
# Thu, 23 Mar 2023 00:23:53 GMT
USER 1001
# Thu, 23 Mar 2023 00:23:53 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5e8dcb5e56c183e88ba77bcc578f740c99b9e24522804c3588c46eda8f5cbdc1`  
		Last Modified: Wed, 22 Mar 2023 23:55:55 GMT  
		Size: 88.4 MB (88426082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f18a10877ccdcd3eeaab27671c328f482fe54787eda52e5f4898bf550887e79`  
		Last Modified: Thu, 23 Mar 2023 00:26:29 GMT  
		Size: 3.8 MB (3765192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32cd6303bb114a4ec82148dfc2518814b542207d2f41154f9217ab87f03f761`  
		Last Modified: Thu, 23 Mar 2023 00:26:39 GMT  
		Size: 96.9 MB (96883561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c402f806dc3fc0d25dbbbaf358aa0031891478795e4f64b346116a6410a6ff`  
		Last Modified: Thu, 23 Mar 2023 00:26:27 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd25ea4413f6664ab24fc2a43e9c10345e519e5248b3ad2e39ae07be45f15050`  
		Last Modified: Thu, 23 Mar 2023 00:26:27 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d936660b00f80fa76c2c0ef3b39bbc6401d9611d72c643bcedcc9e61d1d9b06e`  
		Last Modified: Thu, 23 Mar 2023 00:26:25 GMT  
		Size: 10.6 KB (10578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f5b85e0afc90039783fa43ba33ac7b59e795504ba70323a7a5940d4c84cd19`  
		Last Modified: Thu, 23 Mar 2023 00:26:26 GMT  
		Size: 914.5 KB (914546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5dfd42e283c56cc538538cc3bb124e0ff6504bd913a0ca273506356fbdcc493`  
		Last Modified: Thu, 23 Mar 2023 00:26:27 GMT  
		Size: 8.1 MB (8137888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27f631e9bc0b5ec8a705d1d7a7ed81e139aa9cca8d93a9f62d2c85161cc00c8`  
		Last Modified: Thu, 23 Mar 2023 00:26:25 GMT  
		Size: 13.2 KB (13204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed23b0ffca38ffab3c2e26fc0bc67853fc2cb702d2d9651fa1233311a85c2e3e`  
		Last Modified: Thu, 23 Mar 2023 00:26:26 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
