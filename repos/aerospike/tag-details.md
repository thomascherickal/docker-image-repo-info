<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:5.1.0.24`](#aerospike51024)
-	[`aerospike:5.2.0.16`](#aerospike52016)
-	[`aerospike:5.3.0.7`](#aerospike5307)
-	[`aerospike:5.4.0.2`](#aerospike5402)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:5.1.0.24`

```console
$ docker pull aerospike@sha256:8a572d1ab243ece5d26d3f19cd3a68c86255ecc2149e9625342a6634a82b4321
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.1.0.24` - linux; amd64

```console
$ docker pull aerospike@sha256:88bb33c4912188d333304e32c085ff5e4f48a436c88429c3e7558f5f9bb76451
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76362413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3af7f880912b7176e60736fc2e97843ba3374db03230022155d9103531e34e0f`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:21 GMT
ADD file:f47757e25d3861a5c0180542919c21264323d4dace1f5a6761fc2f38b53a9003 in / 
# Tue, 12 Jan 2021 00:35:21 GMT
CMD ["bash"]
# Mon, 25 Jan 2021 20:19:46 GMT
ENV AEROSPIKE_VERSION=5.1.0.24
# Mon, 25 Jan 2021 20:19:46 GMT
ENV AEROSPIKE_SHA256=8c10e2375679c017d836c8c5101fa424030d53cd95546e3c122d0be051e3f432
# Mon, 25 Jan 2021 20:20:10 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 25 Jan 2021 20:20:10 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Mon, 25 Jan 2021 20:20:10 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Mon, 25 Jan 2021 20:20:11 GMT
EXPOSE 3000 3001 3002 3003
# Mon, 25 Jan 2021 20:20:11 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Mon, 25 Jan 2021 20:20:11 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:8aff230071c97ddc86b6d29fbbb7a4caae7a0183a83f08aa5a06e69e26ce2c81`  
		Last Modified: Tue, 12 Jan 2021 00:43:25 GMT  
		Size: 22.5 MB (22528609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c1238fcd21c282d85f5f9362b91e34c05e4f9580549809cc224d28722d54ef`  
		Last Modified: Mon, 25 Jan 2021 20:22:06 GMT  
		Size: 53.8 MB (53831752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043071879c2a79f3c524dd152ed7cd983d622087925e33b0674802e8cf0ae861`  
		Last Modified: Mon, 25 Jan 2021 20:21:50 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:294f2b65a263bb340613ea34d8bf16c2f7972dadd4c14664d85d968dfa0abbeb`  
		Last Modified: Mon, 25 Jan 2021 20:21:50 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.2.0.16`

```console
$ docker pull aerospike@sha256:64f42e8f02697ea15b6e034a9dc4fb4666ad7b4d52f9b0c3591985821f31a132
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.2.0.16` - linux; amd64

```console
$ docker pull aerospike@sha256:a53ce6cbc02d5798163a422f794619d806fc3f9777ffdaec4bcdb1fc8f2df044
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76278841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d1c9e1f3697a04275c577b88dceec8f891117b95de45bfd6af0fa2a2bd1669f`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:21 GMT
ADD file:f47757e25d3861a5c0180542919c21264323d4dace1f5a6761fc2f38b53a9003 in / 
# Tue, 12 Jan 2021 00:35:21 GMT
CMD ["bash"]
# Mon, 25 Jan 2021 20:20:15 GMT
ENV AEROSPIKE_VERSION=5.2.0.16
# Mon, 25 Jan 2021 20:20:15 GMT
ENV AEROSPIKE_SHA256=2854058a722c21ee526bb478becbc0c0e0eb553eff325a8dc8e4fe0013e065ae
# Mon, 25 Jan 2021 20:20:38 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 25 Jan 2021 20:20:39 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Mon, 25 Jan 2021 20:20:39 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Mon, 25 Jan 2021 20:20:39 GMT
EXPOSE 3000 3001 3002 3003
# Mon, 25 Jan 2021 20:20:39 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Mon, 25 Jan 2021 20:20:39 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:8aff230071c97ddc86b6d29fbbb7a4caae7a0183a83f08aa5a06e69e26ce2c81`  
		Last Modified: Tue, 12 Jan 2021 00:43:25 GMT  
		Size: 22.5 MB (22528609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2110c895ebc8dc52c76e0f666f26374c74a1ee9911f3964cd08dff17ae396b`  
		Last Modified: Mon, 25 Jan 2021 20:22:19 GMT  
		Size: 53.7 MB (53748177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4b43e1ba7e1b3b526f84c7fd40521627e887da6c541c94a725ac1995096f03`  
		Last Modified: Mon, 25 Jan 2021 20:22:10 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b33addb7d5bcda188c600af291717a5e4d5a46564de73a1b44f9960edbeb685`  
		Last Modified: Mon, 25 Jan 2021 20:22:10 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.3.0.7`

```console
$ docker pull aerospike@sha256:52d0f3779a598f367a3aff1fc3d62c4e9e92726fd9e8391aaaa5867c70136685
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.3.0.7` - linux; amd64

```console
$ docker pull aerospike@sha256:9db71978a78e643d3a7186dc6484da40ed7f8e678ee31b7885eb3d05d7257e29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74707588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea6e4673ba895edaf2d9adf4e29435e7b331d68fd936aead007b0d692a14a997`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:21 GMT
ADD file:f47757e25d3861a5c0180542919c21264323d4dace1f5a6761fc2f38b53a9003 in / 
# Tue, 12 Jan 2021 00:35:21 GMT
CMD ["bash"]
# Mon, 25 Jan 2021 20:20:45 GMT
ENV AEROSPIKE_VERSION=5.3.0.7
# Mon, 25 Jan 2021 20:20:45 GMT
ENV AEROSPIKE_SHA256=60719c481ace4a6521afab686c19c728afbb4f90bf1daced5fbc43c7c6a9949d
# Mon, 25 Jan 2021 20:21:08 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 25 Jan 2021 20:21:09 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Mon, 25 Jan 2021 20:21:09 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Mon, 25 Jan 2021 20:21:09 GMT
EXPOSE 3000 3001 3002 3003
# Mon, 25 Jan 2021 20:21:09 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Mon, 25 Jan 2021 20:21:09 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:8aff230071c97ddc86b6d29fbbb7a4caae7a0183a83f08aa5a06e69e26ce2c81`  
		Last Modified: Tue, 12 Jan 2021 00:43:25 GMT  
		Size: 22.5 MB (22528609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16813d6513db1db9df6633bc342e188f1454a7a32a2435707d8003734dfb8777`  
		Last Modified: Mon, 25 Jan 2021 20:22:32 GMT  
		Size: 52.2 MB (52176927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a56f96b64625ae7e5e29208e7a20a154c663b5fc5403c6b4ddb406897aae650`  
		Last Modified: Mon, 25 Jan 2021 20:22:24 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514174fb3f8c05e77c23aab21577ebc378fecebb0c1a351ace5a1a33dc323f6f`  
		Last Modified: Mon, 25 Jan 2021 20:22:23 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.4.0.2`

```console
$ docker pull aerospike@sha256:3d0a36179a4ea9e094d81178f823a0004f9300e3e3a2689de479974e7f093282
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.4.0.2` - linux; amd64

```console
$ docker pull aerospike@sha256:e380b2dd6336569997e67529cf8f4f20345d8d11159aa7f05edba5111d3961a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74727848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afaa94543ff0a9da69fac4946010c2175285da30e9c5f08aba02363dc78dfe5a`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:21 GMT
ADD file:f47757e25d3861a5c0180542919c21264323d4dace1f5a6761fc2f38b53a9003 in / 
# Tue, 12 Jan 2021 00:35:21 GMT
CMD ["bash"]
# Mon, 25 Jan 2021 20:21:14 GMT
ENV AEROSPIKE_VERSION=5.4.0.2
# Mon, 25 Jan 2021 20:21:14 GMT
ENV AEROSPIKE_SHA256=f1fa3b73e5de572b1ff927b25ff43b5eef734a6f6854c34eb2fe01d886170e33
# Mon, 25 Jan 2021 20:21:37 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 25 Jan 2021 20:21:38 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Mon, 25 Jan 2021 20:21:38 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Mon, 25 Jan 2021 20:21:38 GMT
EXPOSE 3000 3001 3002 3003
# Mon, 25 Jan 2021 20:21:38 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Mon, 25 Jan 2021 20:21:39 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:8aff230071c97ddc86b6d29fbbb7a4caae7a0183a83f08aa5a06e69e26ce2c81`  
		Last Modified: Tue, 12 Jan 2021 00:43:25 GMT  
		Size: 22.5 MB (22528609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce9980d8f8f9d90196c6648ee5a42e22dc89f8b05792d6107a0a127d50c363c`  
		Last Modified: Mon, 25 Jan 2021 20:22:46 GMT  
		Size: 52.2 MB (52197187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaaad568b5e18c0eddd0a51d525d4bba7ef57cbc0decceaff76aa298ab353ec2`  
		Last Modified: Mon, 25 Jan 2021 20:22:37 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d860f6c3d9c8b0418028639ab766c3dd1a5e22089ace86110dcddd92c1d74d30`  
		Last Modified: Mon, 25 Jan 2021 20:22:36 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:3d0a36179a4ea9e094d81178f823a0004f9300e3e3a2689de479974e7f093282
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:e380b2dd6336569997e67529cf8f4f20345d8d11159aa7f05edba5111d3961a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74727848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afaa94543ff0a9da69fac4946010c2175285da30e9c5f08aba02363dc78dfe5a`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:21 GMT
ADD file:f47757e25d3861a5c0180542919c21264323d4dace1f5a6761fc2f38b53a9003 in / 
# Tue, 12 Jan 2021 00:35:21 GMT
CMD ["bash"]
# Mon, 25 Jan 2021 20:21:14 GMT
ENV AEROSPIKE_VERSION=5.4.0.2
# Mon, 25 Jan 2021 20:21:14 GMT
ENV AEROSPIKE_SHA256=f1fa3b73e5de572b1ff927b25ff43b5eef734a6f6854c34eb2fe01d886170e33
# Mon, 25 Jan 2021 20:21:37 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 25 Jan 2021 20:21:38 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Mon, 25 Jan 2021 20:21:38 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Mon, 25 Jan 2021 20:21:38 GMT
EXPOSE 3000 3001 3002 3003
# Mon, 25 Jan 2021 20:21:38 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Mon, 25 Jan 2021 20:21:39 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:8aff230071c97ddc86b6d29fbbb7a4caae7a0183a83f08aa5a06e69e26ce2c81`  
		Last Modified: Tue, 12 Jan 2021 00:43:25 GMT  
		Size: 22.5 MB (22528609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce9980d8f8f9d90196c6648ee5a42e22dc89f8b05792d6107a0a127d50c363c`  
		Last Modified: Mon, 25 Jan 2021 20:22:46 GMT  
		Size: 52.2 MB (52197187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaaad568b5e18c0eddd0a51d525d4bba7ef57cbc0decceaff76aa298ab353ec2`  
		Last Modified: Mon, 25 Jan 2021 20:22:37 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d860f6c3d9c8b0418028639ab766c3dd1a5e22089ace86110dcddd92c1d74d30`  
		Last Modified: Mon, 25 Jan 2021 20:22:36 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
