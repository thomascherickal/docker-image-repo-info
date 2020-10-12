<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:5.0.0.13`](#aerospike50013)
-	[`aerospike:5.1.0.10`](#aerospike51010)
-	[`aerospike:5.2.0.2`](#aerospike5202)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:5.0.0.13`

```console
$ docker pull aerospike@sha256:087446dbeffbde8aac28ea290d5ceb43fb34834681678518c34b132b8dc5e88a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.0.0.13` - linux; amd64

```console
$ docker pull aerospike@sha256:9e5e70738bc1e1aab20e6e24aedbb8db72023f64e28eafbc0d7ff98c5255eca6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58576241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82dcd1bf28dde8a203c8e95fda791c4a64351b980536334d96427a81cae18a3f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:37 GMT
ADD file:83fbd2352bbac612c7a954e19abd295607cea4482c556c225308e0241b58e2bf in / 
# Thu, 10 Sep 2020 00:30:37 GMT
CMD ["bash"]
# Mon, 12 Oct 2020 22:19:40 GMT
ENV AEROSPIKE_VERSION=5.0.0.13
# Mon, 12 Oct 2020 22:19:40 GMT
ENV AEROSPIKE_SHA256=17850647ecb0b1e92714acbb8ae4e77034d292c6d891251a2bfaac3fe48bd03f
# Mon, 12 Oct 2020 22:19:58 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 12 Oct 2020 22:19:58 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Mon, 12 Oct 2020 22:19:58 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Mon, 12 Oct 2020 22:19:58 GMT
EXPOSE 3000 3001 3002 3003
# Mon, 12 Oct 2020 22:19:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Oct 2020 22:19:59 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:abb454610128b028301ee40af387d31111a1e699e4ea424fd53186ff77067402`  
		Last Modified: Thu, 10 Sep 2020 00:37:40 GMT  
		Size: 22.5 MB (22522274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd46e5777d9a4dcfb08a14edd0fe4ed9f485e476783e06836842efa34a47b5`  
		Last Modified: Mon, 12 Oct 2020 22:21:05 GMT  
		Size: 36.1 MB (36051914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea013b5ac9884c98fab069dd8aa93c16491bf9edef286bc8df6da738649fddb`  
		Last Modified: Mon, 12 Oct 2020 22:20:58 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1ad6fda7d29015a952083d204a0716da1761ea8618328a24f36a6b0498aa36`  
		Last Modified: Mon, 12 Oct 2020 22:20:58 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.1.0.10`

```console
$ docker pull aerospike@sha256:5e2a78eb58777dd2008935fee144fb2c8a966db93369602201d585bfdd65938f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.1.0.10` - linux; amd64

```console
$ docker pull aerospike@sha256:784b93fd8dc475126da7f6674d37e141792c0a725c2b40c38fb6dac679ffb342
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66025073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96b8cbff746b0b5b5182a6642c0b2fbd899a085d24b3ed50cb111c04c85009dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:37 GMT
ADD file:83fbd2352bbac612c7a954e19abd295607cea4482c556c225308e0241b58e2bf in / 
# Thu, 10 Sep 2020 00:30:37 GMT
CMD ["bash"]
# Mon, 12 Oct 2020 22:20:05 GMT
ENV AEROSPIKE_VERSION=5.1.0.10
# Mon, 12 Oct 2020 22:20:05 GMT
ENV AEROSPIKE_SHA256=6e2bf927a092725385fbdb70ec90bc0b6431c5e0d3aa8bcc8c7f57c7ddf09cac
# Mon, 12 Oct 2020 22:20:23 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 12 Oct 2020 22:20:23 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Mon, 12 Oct 2020 22:20:23 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Mon, 12 Oct 2020 22:20:23 GMT
EXPOSE 3000 3001 3002 3003
# Mon, 12 Oct 2020 22:20:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Oct 2020 22:20:24 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:abb454610128b028301ee40af387d31111a1e699e4ea424fd53186ff77067402`  
		Last Modified: Thu, 10 Sep 2020 00:37:40 GMT  
		Size: 22.5 MB (22522274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76205bb5996a90856f54dbe69e357e1badbf47f3882752892a1bd424f956b016`  
		Last Modified: Mon, 12 Oct 2020 22:21:15 GMT  
		Size: 43.5 MB (43500747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3358e804f99f5f41c30e5fee81cae9ef4096f775b7e6b075eb5f8663a5c5e252`  
		Last Modified: Mon, 12 Oct 2020 22:21:09 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6564b2e3324688256ab43930c1d6e13674b4cb3721b9912ca10c601e578bc7a7`  
		Last Modified: Mon, 12 Oct 2020 22:21:08 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.2.0.2`

```console
$ docker pull aerospike@sha256:1a49b9be06cad6f6697c5b85213f472c3fd861e1bb3f7b8590ce63f5cc6ee3c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.2.0.2` - linux; amd64

```console
$ docker pull aerospike@sha256:7c128ef363d571e0ce87995b1976919e82ecfa99aee79bc552ae428fabf7263f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65942736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e73ffe21fd483cb346eda54db898c693f8b6aa8c7682eb93cc486d93f268585`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:37 GMT
ADD file:83fbd2352bbac612c7a954e19abd295607cea4482c556c225308e0241b58e2bf in / 
# Thu, 10 Sep 2020 00:30:37 GMT
CMD ["bash"]
# Mon, 12 Oct 2020 22:20:31 GMT
ENV AEROSPIKE_VERSION=5.2.0.2
# Mon, 12 Oct 2020 22:20:31 GMT
ENV AEROSPIKE_SHA256=a60799791567b845d20aeaf73adf96ed2285d08145b3c5cac6746cc4e1f1f0d5
# Mon, 12 Oct 2020 22:20:48 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 12 Oct 2020 22:20:48 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Mon, 12 Oct 2020 22:20:49 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Mon, 12 Oct 2020 22:20:49 GMT
EXPOSE 3000 3001 3002 3003
# Mon, 12 Oct 2020 22:20:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Oct 2020 22:20:49 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:abb454610128b028301ee40af387d31111a1e699e4ea424fd53186ff77067402`  
		Last Modified: Thu, 10 Sep 2020 00:37:40 GMT  
		Size: 22.5 MB (22522274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebf44dc2eafa63b194b5fd385f0eab57742501c25734d94c8bfade2b582b7f9`  
		Last Modified: Mon, 12 Oct 2020 22:21:27 GMT  
		Size: 43.4 MB (43418408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b5373c93f52309e7458a527d4ce1d98b91214d1df5982e3e61a2541f7f3678`  
		Last Modified: Mon, 12 Oct 2020 22:21:20 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93eb3fe7f39a630629cb932430d66b74231aa66eb8b9b618fb027847b07f3c89`  
		Last Modified: Mon, 12 Oct 2020 22:21:20 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:1a49b9be06cad6f6697c5b85213f472c3fd861e1bb3f7b8590ce63f5cc6ee3c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:7c128ef363d571e0ce87995b1976919e82ecfa99aee79bc552ae428fabf7263f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65942736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e73ffe21fd483cb346eda54db898c693f8b6aa8c7682eb93cc486d93f268585`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:37 GMT
ADD file:83fbd2352bbac612c7a954e19abd295607cea4482c556c225308e0241b58e2bf in / 
# Thu, 10 Sep 2020 00:30:37 GMT
CMD ["bash"]
# Mon, 12 Oct 2020 22:20:31 GMT
ENV AEROSPIKE_VERSION=5.2.0.2
# Mon, 12 Oct 2020 22:20:31 GMT
ENV AEROSPIKE_SHA256=a60799791567b845d20aeaf73adf96ed2285d08145b3c5cac6746cc4e1f1f0d5
# Mon, 12 Oct 2020 22:20:48 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 12 Oct 2020 22:20:48 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Mon, 12 Oct 2020 22:20:49 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Mon, 12 Oct 2020 22:20:49 GMT
EXPOSE 3000 3001 3002 3003
# Mon, 12 Oct 2020 22:20:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Oct 2020 22:20:49 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:abb454610128b028301ee40af387d31111a1e699e4ea424fd53186ff77067402`  
		Last Modified: Thu, 10 Sep 2020 00:37:40 GMT  
		Size: 22.5 MB (22522274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebf44dc2eafa63b194b5fd385f0eab57742501c25734d94c8bfade2b582b7f9`  
		Last Modified: Mon, 12 Oct 2020 22:21:27 GMT  
		Size: 43.4 MB (43418408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b5373c93f52309e7458a527d4ce1d98b91214d1df5982e3e61a2541f7f3678`  
		Last Modified: Mon, 12 Oct 2020 22:21:20 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93eb3fe7f39a630629cb932430d66b74231aa66eb8b9b618fb027847b07f3c89`  
		Last Modified: Mon, 12 Oct 2020 22:21:20 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
