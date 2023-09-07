## `spiped:latest`

```console
$ docker pull spiped@sha256:1cd9812c97a4759a662ef28ba171b7ed9405e4c4de37b3f9540d185359ffba2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `spiped:latest` - linux; amd64

```console
$ docker pull spiped@sha256:698668efa921def0868a98b18970565ee8dc2670c052d302622d3034268b8d04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38182047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d45b970fdfa1b7672ee2b095ab2f42483add98c0d4845377543f8694a365194d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 07 Sep 2023 00:20:51 GMT
ADD file:3a8cd4de7f163d93718670f4db1de49045f5e04af3a8aa27d81c0f14647db707 in / 
# Thu, 07 Sep 2023 00:20:51 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 15:02:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 07 Sep 2023 15:02:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 15:02:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 07 Sep 2023 15:02:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 15:02:38 GMT
VOLUME [/spiped]
# Thu, 07 Sep 2023 15:02:38 GMT
WORKDIR /spiped
# Thu, 07 Sep 2023 15:02:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 07 Sep 2023 15:02:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Sep 2023 15:02:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:360eba32fa65016e0d558c6af176db31a202e9a6071666f9b629cb8ba6ccedf0`  
		Last Modified: Thu, 07 Sep 2023 00:25:22 GMT  
		Size: 29.1 MB (29124494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:632819797c06687ca493c9a47e46eb757cebf1b86b510ab440e9af68fa94c822`  
		Last Modified: Thu, 07 Sep 2023 15:02:54 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f52e3efebae3582c96b28638d287a009e8cb04d500cd2807eebe5ed62ffb625`  
		Last Modified: Thu, 07 Sep 2023 15:02:55 GMT  
		Size: 2.6 MB (2586438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45599c713b4eb697ee988c71036177fc8ba49608225b0085002d8327d3d8d556`  
		Last Modified: Thu, 07 Sep 2023 15:02:55 GMT  
		Size: 6.5 MB (6469513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05af6ba82265aa60d68c8f4b108c6ea95e69f1206d127179debe9216e9c5a7`  
		Last Modified: Thu, 07 Sep 2023 15:02:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441712062da0b9e6514b1c7ecc53cfd96d8449fe9d8a43fdbc86b8936b804b58`  
		Last Modified: Thu, 07 Sep 2023 15:02:54 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a9ff597f329ef38c50b6136504b6252dbe227c3d19d617f1887ee9bc27e4712a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34305759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d39348a27db2d4d5e45ffa409ae752062ffbfeb87dc65228fb0ffdf1adb7b4f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 07 Sep 2023 00:48:30 GMT
ADD file:e7b77e5797ddb7e058507462fd5f5aad6864ba08ebc4a6c2743dae81ed0f445d in / 
# Thu, 07 Sep 2023 00:48:31 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 12:16:05 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 07 Sep 2023 12:16:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 12:16:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 07 Sep 2023 12:16:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 12:16:32 GMT
VOLUME [/spiped]
# Thu, 07 Sep 2023 12:16:32 GMT
WORKDIR /spiped
# Thu, 07 Sep 2023 12:16:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 07 Sep 2023 12:16:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Sep 2023 12:16:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d971e043cc5e8068fe39c736806d279b128c720a08d2e0d41002dcf027787939`  
		Last Modified: Thu, 07 Sep 2023 00:51:35 GMT  
		Size: 27.0 MB (26983530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4a06c4bbc621ca81c1f8385f4b57bf57b465885bd171cebbf783918fa445f2`  
		Last Modified: Thu, 07 Sep 2023 12:16:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68ffb63c06c0a0bac5f5aa92055b5160625a576852a64fed97826577a17876b`  
		Last Modified: Thu, 07 Sep 2023 12:16:45 GMT  
		Size: 2.2 MB (2184068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c2b7cefa68fa7eaa0d8b23b57aad0ccedc6f00ff8906bbe3f739373784ecc8`  
		Last Modified: Thu, 07 Sep 2023 12:16:45 GMT  
		Size: 5.1 MB (5136568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ab23eb4ed83442d0a1a64f4305012f8b924a585b3d4d6db25f2904beaa5c35`  
		Last Modified: Thu, 07 Sep 2023 12:16:44 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cab120623d4374f81ca44188d1583e9e9304a192517b0f5c3d4a4f0c12d914`  
		Last Modified: Thu, 07 Sep 2023 12:16:44 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5e8f0c26a16c4df76b2dc3fc6e710f79f928bc84e4ba1738ffb16a38d097769f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31728545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce26cf5793431ba1477cc81a099f7b8fec63f842df5a4d2ef708cfba02b37b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:12 GMT
ADD file:45cc27bd11f601d2fef5d7494a1a6253287e6d22e108e39c0884761c7533cd9c in / 
# Wed, 16 Aug 2023 00:17:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:25:29 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 05:25:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:25:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 05:25:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 05:25:51 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 05:25:51 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 05:25:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 05:25:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 05:25:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a44aa9565b062e4216f7b39ce6c67dcc5376e10f76caec55bd3acd1cc8b76b75`  
		Last Modified: Wed, 16 Aug 2023 00:21:27 GMT  
		Size: 24.8 MB (24805419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9c11d18979b89d7fa32eabe7f88a8cd64e01b4b8fa271fc334fb7d2b699b2`  
		Last Modified: Wed, 16 Aug 2023 05:26:05 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b903a5c832d6f2fe4b495269a61fdf5cb49b36db7bea0569860fa6d84d00e`  
		Last Modified: Wed, 16 Aug 2023 05:26:06 GMT  
		Size: 2.0 MB (2043310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2f485e2da8130574c637c09ae0956f61e314214b2723b60575c9716e0f89ec`  
		Last Modified: Wed, 16 Aug 2023 05:26:06 GMT  
		Size: 4.9 MB (4878216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ff0fe969b7330d3d7bb0cf4092f32ed845104416d60805fd202948a8404909`  
		Last Modified: Wed, 16 Aug 2023 05:26:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25331bf9ce347281c7ed517293d861fd29f7d86535538cc031c9e9f3cfccbd97`  
		Last Modified: Wed, 16 Aug 2023 05:26:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:084095b02a15abf96f7ca4d2429ce16218cf7883ff3191ae1707ff2bc064f378
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37067386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ae6874e340894f444a9fc3b554ed2bc2d103d722d35e4a3b77137973d46ad89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:39 GMT
ADD file:fb5c8f411c4a1e06c25ac32455221938386907d0b4782fc228ca67de63a7e9de in / 
# Thu, 07 Sep 2023 00:39:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:02 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 07 Sep 2023 01:39:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:39:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 07 Sep 2023 01:39:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:39:23 GMT
VOLUME [/spiped]
# Thu, 07 Sep 2023 01:39:23 GMT
WORKDIR /spiped
# Thu, 07 Sep 2023 01:39:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:39:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Sep 2023 01:39:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:155eab17d86c47443adc8cebe7fc62c847c03db8cfb1ca53aa6276564fff23ef`  
		Last Modified: Thu, 07 Sep 2023 00:43:02 GMT  
		Size: 29.2 MB (29157149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea87234f31097cb9ca8da4ce312ae1144ca4335fce0dd6083d63786f18c14dd4`  
		Last Modified: Thu, 07 Sep 2023 01:39:33 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6766bc9b7d5b3ce10f74ca32998c01c7d7965e44b76daeb635e198a2cba19415`  
		Last Modified: Thu, 07 Sep 2023 01:39:34 GMT  
		Size: 2.4 MB (2429873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55ecc6bc88386b589732b162b70beec26c7c095c46b0f34a778ef2edf7fe4ea`  
		Last Modified: Thu, 07 Sep 2023 01:39:34 GMT  
		Size: 5.5 MB (5478764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ec2278e5e88b74cf0740bab686b2682c2948d2c5ac0ed2e041e9a829b9dc37`  
		Last Modified: Thu, 07 Sep 2023 01:39:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c37605157e6ea730333fb409b33b0cbbe75429cd00ff371aa12c84b4eb869a6`  
		Last Modified: Thu, 07 Sep 2023 01:39:33 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:c1269ae34205a7105e15e21afb748acf092303d42802e691703c620acdfe126e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38667169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e9dccc0b103ac44995ceb2445bec61936130bb9cfa4d0b782e16ad93ff12327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:01 GMT
ADD file:ffdb2f26091492ac2e82793b461bb70da9ce1d68d219ec0db182b4510e82586b in / 
# Tue, 15 Aug 2023 23:39:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 20:40:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Aug 2023 20:40:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 20:40:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Aug 2023 20:41:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 20:41:03 GMT
VOLUME [/spiped]
# Wed, 16 Aug 2023 20:41:03 GMT
WORKDIR /spiped
# Wed, 16 Aug 2023 20:41:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Aug 2023 20:41:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 20:41:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a12cc43de7614ac71c57865601eb4cedd27ce910b66c5091e07781b8547d5b0b`  
		Last Modified: Tue, 15 Aug 2023 23:43:26 GMT  
		Size: 30.1 MB (30141823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03457c876b07f1c91adaf8fb6937472beeda4a93329a4ea034beddb49371b3a0`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24a2251fa8712a87ba72cf1b7210863ff8ffb1714aea584978ffb9257568d78`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 2.6 MB (2583561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea65716bab4c92cfb7167bcec8537472d71948f927537f09b9ba7430fe8177ec`  
		Last Modified: Wed, 16 Aug 2023 20:41:23 GMT  
		Size: 5.9 MB (5940186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e7fe253882086312121ecd6331d5e7ccda72ef6ff2245bff10b4760a2211b6`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe62b93bfa24ccf2d27d2385608f70dcaed03bb85755b5e0d5b8967c58417b0`  
		Last Modified: Wed, 16 Aug 2023 20:41:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:78a90b24784fa980d784a5948e995a6ce8523ccd1d9b5d66c179e05ff6b055ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36756444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:757e8085aa8fc8338a5f230334c1f05a433c19ffdcf7358b738756ade7ed945c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 07 Sep 2023 01:09:11 GMT
ADD file:263719948aa8496c0852aa2ef6c6660c25ce35618af5b1c5bc35c901d853bcf8 in / 
# Thu, 07 Sep 2023 01:09:17 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 14:59:19 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 07 Sep 2023 14:59:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 14:59:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 07 Sep 2023 15:01:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 15:01:26 GMT
VOLUME [/spiped]
# Thu, 07 Sep 2023 15:01:29 GMT
WORKDIR /spiped
# Thu, 07 Sep 2023 15:01:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 07 Sep 2023 15:01:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Sep 2023 15:01:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6519d39af9071c1099bd2a01d04c824d095fb31f439e10814371707227802ae`  
		Last Modified: Thu, 07 Sep 2023 01:20:14 GMT  
		Size: 29.1 MB (29121387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aefb9a6905bf168eeced8e83a91e7068b7fb4755b8e7857c50c3dcd173b85e5`  
		Last Modified: Thu, 07 Sep 2023 15:01:48 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205c01df5896968bbf6e6317ad4f7d3ea3cad21bce8da9f3d43d160e62304a06`  
		Last Modified: Thu, 07 Sep 2023 15:01:50 GMT  
		Size: 1.8 MB (1831686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6736bbe590ef520568c5c56fd7e96b0513fe8d2efd0e874b5e734cf04939d285`  
		Last Modified: Thu, 07 Sep 2023 15:01:53 GMT  
		Size: 5.8 MB (5801853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71816f5552a92da3f78474b698659b9026050c3b8c048f4d754fffe26169f6a`  
		Last Modified: Thu, 07 Sep 2023 15:01:48 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d57f9d6402fe11212989b0272189df10b78ed901c1dd2605d1c31c0d18e3c6`  
		Last Modified: Thu, 07 Sep 2023 15:01:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:3d6c0965915fcc87fc69cf417f42a674b4b7b6b7caa0c1b31377967a476d86d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42306129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38286d79d5b86c0e20b179f07d455a8eab6b835da41a9eda080a126f32058243`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:33 GMT
ADD file:9578bf6d6b33f2ba960ab9309642d1c9dcc131d7b9e6f818b8cc4b843fe3aec8 in / 
# Wed, 16 Aug 2023 01:09:35 GMT
CMD ["bash"]
# Thu, 17 Aug 2023 08:36:31 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 17 Aug 2023 08:36:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 08:36:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 17 Aug 2023 08:37:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 17 Aug 2023 08:37:32 GMT
VOLUME [/spiped]
# Thu, 17 Aug 2023 08:37:32 GMT
WORKDIR /spiped
# Thu, 17 Aug 2023 08:37:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Aug 2023 08:37:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Aug 2023 08:37:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0500920b409f06d69819525676ebf090702285435050f7b1f973c8c7b034ea7c`  
		Last Modified: Wed, 16 Aug 2023 01:15:59 GMT  
		Size: 33.1 MB (33119300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec54fbbe846acd5f1832bae50bceb47f640988246e9474bc1a66fb8d7cb7064`  
		Last Modified: Thu, 17 Aug 2023 08:37:55 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a896f95d60612d17c91fcd7d1e82e830ab2342412bf4a1b76707b8d36ceff79`  
		Last Modified: Thu, 17 Aug 2023 08:37:56 GMT  
		Size: 2.8 MB (2764970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f12bc3101f2ee2eaf19000e077384f0e11af69bfeaa63e660a3936ccb9608f0`  
		Last Modified: Thu, 17 Aug 2023 08:37:57 GMT  
		Size: 6.4 MB (6420255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22854dcf0be02af986e8adf2ce1b2f5566daf0bbdbe2acb1120c0f54870cb663`  
		Last Modified: Thu, 17 Aug 2023 08:37:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecde07d9483e4d8fe792f3eda26f0afb1ed8ea84e3872dc435e3d9245afbc35`  
		Last Modified: Thu, 17 Aug 2023 08:37:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:dbfbfe94e6cd2381da42c76f56b6bcbf60ba1f4034a52102f0b2386813f7b643
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35132516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8368d5020290da560fd277a9096efb1926a3d8a2ee6ce916acaac713a4ea158`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 07 Sep 2023 00:43:39 GMT
ADD file:2a617cce71dc34ce7b62d4b1da4b45cca574c219300ba2be25396630f80bb9cd in / 
# Thu, 07 Sep 2023 00:43:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:59:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 07 Sep 2023 09:59:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 09:59:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 07 Sep 2023 09:59:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 09:59:28 GMT
VOLUME [/spiped]
# Thu, 07 Sep 2023 09:59:28 GMT
WORKDIR /spiped
# Thu, 07 Sep 2023 09:59:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 07 Sep 2023 09:59:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Sep 2023 09:59:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:68043338ec5d8515f0dcc40f82eb11d30dd8539a1d30984e4b157df8779f6d53`  
		Last Modified: Thu, 07 Sep 2023 00:49:40 GMT  
		Size: 27.5 MB (27489648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04b7b00a3a06d014d022c971cb4c21d708fee1686f9b03b1a73788fa09f348a`  
		Last Modified: Thu, 07 Sep 2023 09:59:48 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff354ccea337ca10f1c9f0a48e8ef8b083beb0fb0da5a8812fa7839650d355b`  
		Last Modified: Thu, 07 Sep 2023 09:59:49 GMT  
		Size: 2.3 MB (2257949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfa6faa50dd4967dd1dbbc41de27a7f36d4e2ba74598c770a411ad46c8d0643`  
		Last Modified: Thu, 07 Sep 2023 09:59:49 GMT  
		Size: 5.4 MB (5383324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8faefcfc9499909296c23ba7fe0e88c23173a8c49278045486233e8726658e48`  
		Last Modified: Thu, 07 Sep 2023 09:59:48 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e712c4ad1bec8aa9728604552d09b49710a513ab8ca534b29dfc52ae6436f1d`  
		Last Modified: Thu, 07 Sep 2023 09:59:48 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
