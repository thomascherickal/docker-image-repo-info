## `mysql:debian`

```console
$ docker pull mysql@sha256:e0a793ddd093df31139fc695ed889fdd3ec910c76ddf3186683efe2d67a2ba96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:ac248facf748e93a1022552d4f15311ef8bd8be7ba841305a1b404ed59196de6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.5 MB (177548446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b748431f76159ff04ec985c63bf42dae5206be3aee4e1d244182b297299354`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:31:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 21 Dec 2022 11:31:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:31:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 21 Dec 2022 11:32:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 21 Dec 2022 11:32:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 21 Dec 2022 11:32:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:32:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 21 Dec 2022 11:32:10 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 21 Dec 2022 11:32:11 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Wed, 21 Dec 2022 11:32:11 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 21 Dec 2022 11:32:26 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 21 Dec 2022 11:32:27 GMT
VOLUME [/var/lib/mysql]
# Wed, 21 Dec 2022 11:32:27 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 21 Dec 2022 11:32:27 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 21 Dec 2022 11:32:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Dec 2022 11:32:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 11:32:28 GMT
EXPOSE 3306 33060
# Wed, 21 Dec 2022 11:32:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c71b14b90321c4c925c97bde825eb21b3c97f7f6b9f73ad028c29bf93347ee2`  
		Last Modified: Wed, 21 Dec 2022 11:33:54 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b20239cd5b3eb4255955404db9ddf231a20a91b74c52e8ae82513e70d75e84a`  
		Last Modified: Wed, 21 Dec 2022 11:33:55 GMT  
		Size: 4.4 MB (4414844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a92a8be7b81fc7d582c733edcb95ffe26bd8ff252e05167b70b896561c550a`  
		Last Modified: Wed, 21 Dec 2022 11:33:53 GMT  
		Size: 1.4 MB (1418501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed87af8210d03be6cf68e7ddc53ca53f0b7cb5d2526d8b350a6499f0b09d7b7f`  
		Last Modified: Wed, 21 Dec 2022 11:33:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89326f0fbca735cd9db355568c579a062d4e4f1a151dee777fca6739679c8559`  
		Last Modified: Wed, 21 Dec 2022 11:33:55 GMT  
		Size: 12.7 MB (12662005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d532ea748ea86b00b0defbd158232a20f45862f4693dd6967e7ed4f379c57f`  
		Last Modified: Wed, 21 Dec 2022 11:33:52 GMT  
		Size: 2.5 KB (2545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e4e09af7ec7aa3580ada1847200f65da4879d557475f2f356c43d6f2200669`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d62f3c764f6b95a24939111413263a1dd1e0ffcf895cb6757b4aff64a412340`  
		Last Modified: Wed, 21 Dec 2022 11:34:10 GMT  
		Size: 127.6 MB (127645114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edad28c75e273ba1d4fade07eba864f0ad81767b605529a4918c6d6aa8b4a2ba`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2005ac0b2c3804a85b1ef7cfc06d078e2ecce524d07697c9f58f811367b26e`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff97e27ba8e3f53c701cbd1841c5e91dfe25863598c0d09302e83871f2b344e`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
