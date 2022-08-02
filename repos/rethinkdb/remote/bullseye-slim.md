## `rethinkdb:bullseye-slim`

```console
$ docker pull rethinkdb@sha256:61607ebe23e1b89e899cdb5b69d88a5b5e1240e165be76e076ceae025917f312
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `rethinkdb:bullseye-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:8d3a6848c23c5eb7c5936de3fc75d84dc904154f6c6532a0804c7dea97009841
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47933695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b535431c6e2086300d242bc661bae4597bbdd9f5075d47caa85529137c057bad`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:46:46 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:46:48 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 02 Aug 2022 12:46:48 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 02 Aug 2022 12:46:53 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:46:53 GMT
VOLUME [/data]
# Tue, 02 Aug 2022 12:46:53 GMT
WORKDIR /data
# Tue, 02 Aug 2022 12:46:53 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 02 Aug 2022 12:46:53 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9658d3e40358a32fad96ece20eee7ef0d804284e37a80faa8d8be5d49689ad7f`  
		Last Modified: Tue, 02 Aug 2022 12:47:12 GMT  
		Size: 6.3 MB (6328381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048aa934dab21974b3e48fa7de51c9b3a78444726d74c879be2119c97990ebd6`  
		Last Modified: Tue, 02 Aug 2022 12:47:11 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3716e23539870975f4f809e8e7030d9f53a77986645d2748c4223d6b0c0b9002`  
		Last Modified: Tue, 02 Aug 2022 12:47:12 GMT  
		Size: 10.2 MB (10235741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f612adae7822d56cff91ff5ea875f1d7a4e635ab592ef16fed6208691f8dd5fb`  
		Last Modified: Tue, 02 Aug 2022 12:47:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:9b54389d666294397edc192a3ff29333beb120c9e715bccbfab726125fec3c54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45737482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f4a8aedefb7f3f026acefecd5f0849afa951e44ca2526bca61833a1fbab2e43`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 15:01:56 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 15:01:58 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 02 Aug 2022 15:01:58 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 02 Aug 2022 15:02:04 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 15:02:04 GMT
VOLUME [/data]
# Tue, 02 Aug 2022 15:02:05 GMT
WORKDIR /data
# Tue, 02 Aug 2022 15:02:06 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 02 Aug 2022 15:02:07 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0034a0db5e4c6b47f0c5d70c7159f86c720383d300c1148c9705e348a84f48`  
		Last Modified: Tue, 02 Aug 2022 15:02:34 GMT  
		Size: 6.3 MB (6308283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3ee9fe72ba45e9c1e96482f3c119c5cc1659b1aa286feabc4fd1c17c5ddf9b`  
		Last Modified: Tue, 02 Aug 2022 15:02:33 GMT  
		Size: 2.7 KB (2669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164d57dc8c08adce1f0e3e92b627d5dc6a0b0ba6a8780548615e2547d309335c`  
		Last Modified: Tue, 02 Aug 2022 15:02:35 GMT  
		Size: 9.4 MB (9372135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3669076f37e6e35af6a2eafac0ffeddeb15aad7c9ef007488b6cebd72d885d1`  
		Last Modified: Tue, 02 Aug 2022 15:02:33 GMT  
		Size: 91.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:bullseye-slim` - linux; s390x

```console
$ docker pull rethinkdb@sha256:40e237281ee93fee08a956576e0bc0a0119bfe0057ed79726b58804229d0c213
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45419310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fcbbb88a70cac8bc2a678c7c328755208c1f97dd27c326db1694d388764f0f7`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 10:55:02 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 10:55:04 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 02 Aug 2022 10:55:04 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 02 Aug 2022 10:55:09 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 10:55:10 GMT
VOLUME [/data]
# Tue, 02 Aug 2022 10:55:10 GMT
WORKDIR /data
# Tue, 02 Aug 2022 10:55:10 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 02 Aug 2022 10:55:10 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fe87117e4568bfb6add8dd26572b21afd5c396e49590d988b6eeaee85209e7`  
		Last Modified: Tue, 02 Aug 2022 10:55:39 GMT  
		Size: 6.2 MB (6203854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48dcc841a94ada0274732111adc797208e2b26799304e564e96cfe9d93a22165`  
		Last Modified: Tue, 02 Aug 2022 10:55:38 GMT  
		Size: 2.7 KB (2687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71783e804788ed52350649312270c194bc364ca483f0e786efd704615e184a68`  
		Last Modified: Tue, 02 Aug 2022 10:55:40 GMT  
		Size: 9.6 MB (9572383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d483a35165a8fe3b67822a81ac6ebc1c4f71229c351a1f26d309b4c3014b08`  
		Last Modified: Tue, 02 Aug 2022 10:55:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
