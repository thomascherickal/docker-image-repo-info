## `rethinkdb:bookworm-slim`

```console
$ docker pull rethinkdb@sha256:b22e56633e2fa39d3892f1a6fc8a8d0d424416ebe9c7edfbfccfb7e75e720bb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rethinkdb:bookworm-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:0ee83237c6a2c9c0f4b38d1ca48652beac9d38846cb9450844ab6ac861c14be8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49111500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30debf8a5123f891a1122ae9865a2aab58a5357838e290553460f748e8bc4405`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 19 Dec 2023 01:20:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 04:12:36 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:12:38 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 19 Dec 2023 04:12:38 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Tue, 19 Dec 2023 04:12:43 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:12:43 GMT
VOLUME [/data]
# Tue, 19 Dec 2023 04:12:43 GMT
WORKDIR /data
# Tue, 19 Dec 2023 04:12:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 19 Dec 2023 04:12:43 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64eb3a2188b6b353cf28d7fb4e5e43ec807c20b2686a9e78df0836be465514c9`  
		Last Modified: Tue, 19 Dec 2023 04:12:55 GMT  
		Size: 9.8 MB (9785456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52d50deec548879cd07aa62d94afe73286730ded405c969d8240df161f9b9d9`  
		Last Modified: Tue, 19 Dec 2023 04:12:53 GMT  
		Size: 2.7 KB (2687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e71ceec2269c34d9e2a3431e4cada3a2bc7c7dc1564be81e96aa6c180c55b`  
		Last Modified: Tue, 19 Dec 2023 04:12:55 GMT  
		Size: 10.2 MB (10197267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2a0fa25342b49e391e3c87e16665bc1b807dd204aa2963bff4a8ea6c3425ae`  
		Last Modified: Tue, 19 Dec 2023 04:12:53 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:bookworm-slim` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:f85dc716c4972b9bb61c97e490a8817cdb88dd0925843f1ef2072670ef9d76a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48336901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff85603eb84c64c3a5c88879e1dabf7bc242dd559bd141686ccf911d820a56`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:58:39 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:58:41 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:54:44 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:54:49 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:54:49 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:54:49 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:54:49 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:54:49 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c9135c3915c6365fef3780e67e564c24edf19b0c1218bf60d1cde501e1f427`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9586130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e301a7defddc5c4579d99f4805faa531b084dc7af58b8f4547f3d3bfff51b3b`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
		Size: 2.7 KB (2688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf605ac1f12920a5d09f4e42786654bf4916f67c9bcd2b9c4493c78a7e91979`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9568679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ceb8a7a135f8c51d5cdc2503be85c4e1bd5657b7f5bf85a771ef0e00aff88f3`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
