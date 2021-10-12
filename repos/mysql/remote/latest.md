## `mysql:latest`

```console
$ docker pull mysql@sha256:5d52dc010398db422949f079c76e98f6b62230e5b59c0bf7582409d2c85abacb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:882e55f40d61034a2bb8a1abab1353571ad2a33866f382350788eb34740528b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150587534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9da615fced53bc1bc11e3d7f20a37873362e1d5354354238f0b63c6d549f7f66`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:22:41 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 12 Oct 2021 16:22:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:22:48 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 16:22:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 16:22:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Oct 2021 16:23:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:23:15 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 12 Oct 2021 16:23:15 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 12 Oct 2021 16:23:16 GMT
ENV MYSQL_VERSION=8.0.26-1debian10
# Tue, 12 Oct 2021 16:23:16 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Oct 2021 16:23:31 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Oct 2021 16:23:32 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Oct 2021 16:23:32 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 12 Oct 2021 16:23:32 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 12 Oct 2021 16:23:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:23:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:23:34 GMT
EXPOSE 3306 33060
# Tue, 12 Oct 2021 16:23:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23cbf2ecc5d6ad68efaf326f8ff1c8b4adfab8faad61315440d21c396dd0160`  
		Last Modified: Tue, 12 Oct 2021 16:25:22 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cfc6c29c0af103c07adaa5e3ee70ffbd8de71ca7b9155079c9769f45fb9aa4`  
		Last Modified: Tue, 12 Oct 2021 16:25:22 GMT  
		Size: 4.2 MB (4179263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38609286cbe5e62cb8a5a9cb7ed553050e6fc1fa4c537b46c54b6d81a527a7b`  
		Last Modified: Tue, 12 Oct 2021 16:25:20 GMT  
		Size: 1.4 MB (1419434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8211d9e66cd658ab45002b3fa5f8558cd8c13d2f07ba492d7ea1520718d32cff`  
		Last Modified: Tue, 12 Oct 2021 16:25:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2313f9eeca4a60533540741b85137033831959ae5a9c4ea652fa4605c9a14bae`  
		Last Modified: Tue, 12 Oct 2021 16:25:23 GMT  
		Size: 13.4 MB (13448689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb487d00da0bfa9e36634d8c6ceae1e2116f2b56da6b272bec5233966f989e8`  
		Last Modified: Tue, 12 Oct 2021 16:25:19 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d2b117a9385bafc1761e043905b1e9a4b603a52a47b2e6f80fe92621530a95`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6cb474cd1c8a589d731f3aba876196cd5ad15fc04363d07e00998953d8bccc`  
		Last Modified: Tue, 12 Oct 2021 16:25:36 GMT  
		Size: 104.4 MB (104390152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896b3fd2ab079ed6501a2ddab191810f6e6a91a296a0600451bd5f15eb3be680`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532e67ebb3762ad33b4ffb25848be0166d216f456f7f91c4afff201419f24870`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 5.5 KB (5541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233c7958b33f5f424cd93ade1de9ab2c2e26fd7363a99d8b33d5d01ce57bd509`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
