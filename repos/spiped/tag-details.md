<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `spiped`

-	[`spiped:1`](#spiped1)
-	[`spiped:1-alpine`](#spiped1-alpine)
-	[`spiped:1.6`](#spiped16)
-	[`spiped:1.6-alpine`](#spiped16-alpine)
-	[`spiped:1.6.1`](#spiped161)
-	[`spiped:1.6.1-alpine`](#spiped161-alpine)
-	[`spiped:alpine`](#spipedalpine)
-	[`spiped:latest`](#spipedlatest)

## `spiped:1`

```console
$ docker pull spiped@sha256:9e61faf7766c81d1b2bc92b19060fbb472e131154e6cf997e1fcf9900ae34480
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

### `spiped:1` - linux; amd64

```console
$ docker pull spiped@sha256:b956b0767d9f807a72c03707fe982b145fad5c08520cb20e311ca7e0818d48cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36313927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6cb81ebb115101411214569dc66a92f6ec17458f63d2812c746f6d646e830e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 18:36:22 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 18:36:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 18:36:29 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 18:37:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 18:37:13 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 18:37:14 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 18:37:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 18:37:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 18:37:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fcdf017f7218b1a75d3fecaf7ec1ed0b82e9d4a2cbf0a3aa748904aa91d5e9`  
		Last Modified: Thu, 22 Jul 2021 18:37:42 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c276e87105455c7cb1d515eff3df184ecdd8d5521db6f69468e61ccf0a3ff31`  
		Last Modified: Thu, 22 Jul 2021 18:37:42 GMT  
		Size: 2.1 MB (2128530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584f9bacb5873a6304fc5b45beb1ee4bb0934a09b2a5b886326e26970c0759ee`  
		Last Modified: Thu, 22 Jul 2021 18:37:46 GMT  
		Size: 7.0 MB (7037393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fd07bb166f5100f180eae6c104818d3fb5c07a685780089267afb2c788050f`  
		Last Modified: Thu, 22 Jul 2021 18:37:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9b27eeedf14c9964238ee10c7883ca4c207714d8b2bba7d79d77d8b3a1b240`  
		Last Modified: Thu, 22 Jul 2021 18:37:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:bf3cfe9903cc41ba0683a7cb0a80a8b685ad944460db431c12f66693f1652917
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32200786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c8136d93f716d701747570bfaf290654c3a70f98c1ee463327ab1881cfe3334`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:50:06 GMT
ADD file:885454a996e63d5eb93f1f365a3be77a441f368d7f5a77a7fd1636edf5d0b8cd in / 
# Thu, 22 Jul 2021 00:50:07 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 15:19:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 15:19:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 15:19:31 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 15:20:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 15:20:31 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 15:20:31 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 15:20:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 15:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 15:20:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2b96a0a1ddfe4fab89025b13e583392414251af73361434f28af076c3db77100`  
		Last Modified: Thu, 22 Jul 2021 01:02:11 GMT  
		Size: 24.9 MB (24879093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf71053fc8a635e22437d2e5f42546178aae83512d063e9cf8f448d96bf735c`  
		Last Modified: Thu, 22 Jul 2021 15:21:13 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fda2dec2a04768a237686201e0c2109d4405df968028c4eabc9e3ece91db53e`  
		Last Modified: Thu, 22 Jul 2021 15:21:14 GMT  
		Size: 1.8 MB (1839352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f2a9767797338b3b65675c1484be98470f735697b7e1a13beff9f70e3aa937`  
		Last Modified: Thu, 22 Jul 2021 15:21:18 GMT  
		Size: 5.5 MB (5480142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f5dbc08870311239eda68a9dac3a09339346f5ee9fc589c7d36a7c62233bcb`  
		Last Modified: Thu, 22 Jul 2021 15:21:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619df22f1e652b1ffd841285f8fa97c3271a8d90ca24a50898bc592f2d26dddf`  
		Last Modified: Thu, 22 Jul 2021 15:21:13 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:c8fcd50e24a2fac4210299a2ee03f0d8d0de3a6e51ba6f61a56c263f16a82fd4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5275d81bc421af6ac42959ab8c655ffe4f05b57d6f87325b371cbe74019778`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Thu, 24 Jun 2021 07:24:26 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 24 Jun 2021 07:24:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 07:24:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 24 Jun 2021 07:25:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 24 Jun 2021 07:25:32 GMT
VOLUME [/spiped]
# Thu, 24 Jun 2021 07:25:33 GMT
WORKDIR /spiped
# Thu, 24 Jun 2021 07:25:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 24 Jun 2021 07:25:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 07:25:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae14b3189ef30e120910a62a83035bb35be5ad21d868baa15635cd4093e57b28`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fbbe41540f8564924d1bbf33810a5cca942d52258a07a9a0a9fa47d3e2ee4d`  
		Last Modified: Thu, 24 Jun 2021 07:26:44 GMT  
		Size: 1.8 MB (1759528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6efa0bc06b8244fc2b99086aaab3707ad97a5c1562d486c49f2643704d4c14f`  
		Last Modified: Thu, 24 Jun 2021 07:26:47 GMT  
		Size: 5.3 MB (5285807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf51d89722279aa5fe979daa99ecca041af3e85c0ecb284c9eef346e12a8525`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ce586c187940aa96e929532b8802dd2d2590ae0629d8d6ff5683defad7d791`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:65f4bd8a8f82126f671cba7e50a4e29ae5be674ccd4e8b54fc903f0122529d1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33830174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bffda7f2326039982bc71ccb3ed7a23ab83f9cb3a0edb8f6b57bec2f05c33640`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:40:14 GMT
ADD file:074ffc2065bab83c9a5c596576656b04d271dd78406aadad160b68e38f38269f in / 
# Thu, 22 Jul 2021 00:40:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 13:06:06 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 13:06:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:06:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 13:06:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 13:06:31 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 13:06:31 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 13:06:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 13:06:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 13:06:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:513c6babab2b9079da61a69300c0e26d1037ca98910376098e9ae87baeb112c0`  
		Last Modified: Thu, 22 Jul 2021 00:45:53 GMT  
		Size: 25.9 MB (25914794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1411af469d8f92bb97698e5703d8f7ad244f1cd857675e0a75d70ee944f14245`  
		Last Modified: Thu, 22 Jul 2021 13:07:02 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3243c8e98ff7d2e88e83ff04990f61634881d1cce8810e0828c3efa28b6c2bca`  
		Last Modified: Thu, 22 Jul 2021 13:07:03 GMT  
		Size: 2.0 MB (2007837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5177afdd0c15ac2fff990100a9693273628249825d2816fe38b1af0635d6e8`  
		Last Modified: Thu, 22 Jul 2021 13:07:04 GMT  
		Size: 5.9 MB (5905334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb096a33b8faa1635a48c84a411ee598af2de78005eb2bf4193c98abd1acf710`  
		Last Modified: Thu, 22 Jul 2021 13:07:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26f77edbf391edf857b771c93043e37da21fe182146025e17e1e84b9b901b5a`  
		Last Modified: Thu, 22 Jul 2021 13:07:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:416f3217a461a18ce8841b0e919b4597c3c7cfbbb8e15cb6aed1034aeb76a530
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41565749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75e57c6d1f54be87f02edae84315b3167268ec573dc93c7fa200082f3d11d06b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:50 GMT
ADD file:cb657a3d01f25bf815677ce223e8802d054f11aeb95f85b160982277916637bd in / 
# Thu, 22 Jul 2021 00:39:51 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:46:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 04:46:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:46:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 04:47:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 04:47:05 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 04:47:05 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 04:47:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 04:47:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 04:47:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fa9d06db5f4195bd51665a89e08e2e7db25636ac28ab162fe876ae0a53093fe5`  
		Last Modified: Thu, 22 Jul 2021 00:46:36 GMT  
		Size: 27.8 MB (27797459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d98317cc5a7bbb137cb721cd14964996fcc1cd226e74c42f1d3e9a6f1c21d26`  
		Last Modified: Thu, 22 Jul 2021 04:47:52 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6c852cdd837170bfd8e188d0ee0a9ed2d53645c00502b910e4f5740ac7f274`  
		Last Modified: Thu, 22 Jul 2021 04:47:53 GMT  
		Size: 2.1 MB (2132624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a49b79994d5ac64b456769f7c7746db459fb1750ae0bdfd1e57c5722d5442a`  
		Last Modified: Thu, 22 Jul 2021 04:47:56 GMT  
		Size: 11.6 MB (11633464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00df8cfac155a64078f92787eb8dae0d3f1a6cc9773c91a6f396a5b9c74bebc`  
		Last Modified: Thu, 22 Jul 2021 04:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f4e2ee058c53ad3e4e974fec117bedb80d84ebc68e960b4dfbd7a5a2627a6b`  
		Last Modified: Thu, 22 Jul 2021 04:47:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:ae9a43f44545fa4f8fbc9216f110bea9275772fb3a34302a054a67578b0e92aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33944082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7851e8a264abf459df1961aa3498a0bd3367a58c9efbf8fea901e773c256a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 06:24:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 06:24:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 06:24:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 06:25:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 06:25:34 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 06:25:35 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 06:25:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 06:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 06:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a23924c8bf3350b569f20c725a3858bdc00af64d69c0e78716993be2cb12af`  
		Last Modified: Thu, 22 Jul 2021 06:26:01 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9b33f3cd0917d540b7337cbbbbbc3230c86c7025c904328033c96c8cda9acb`  
		Last Modified: Thu, 22 Jul 2021 06:26:02 GMT  
		Size: 1.7 MB (1712436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fac5ae579dc8b67efab3cb1b2eba289fce2cd42d3bb110f7f3586e620cd22b`  
		Last Modified: Thu, 22 Jul 2021 06:26:07 GMT  
		Size: 6.4 MB (6416700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906932f9ba8b6e63d86125ee0773e094992a32cbefaaa53ef2f248a493fe1b57`  
		Last Modified: Thu, 22 Jul 2021 06:26:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c08f426acceaf16dcdab867559e0cc19c40516df69d43f2eb413d38f6f4d70`  
		Last Modified: Thu, 22 Jul 2021 06:26:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:57915ff2469ccc919bfb944e9bb1b2296a969b92f48cefedea889844de387440
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39525102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db2498759c4271881a8f7943dea35cfb72b5a49109ebcba5683fadfef3f7ef2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 09 Jul 2021 15:58:12 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Fri, 09 Jul 2021 15:58:14 GMT
CMD ["bash"]
# Sat, 10 Jul 2021 18:27:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Jul 2021 18:28:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 18:28:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Jul 2021 18:31:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Jul 2021 18:31:37 GMT
VOLUME [/spiped]
# Sat, 10 Jul 2021 18:31:47 GMT
WORKDIR /spiped
# Sat, 10 Jul 2021 18:31:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Jul 2021 18:31:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Jul 2021 18:32:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f764f35401eb3acc21df9952db2a5406b3f74fb2e579f644235267047cabe99`  
		Last Modified: Sat, 10 Jul 2021 18:34:09 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068bdd38effbf7875a984997014fff888c478fe938893c543d68e4b840f23b9c`  
		Last Modified: Sat, 10 Jul 2021 18:34:10 GMT  
		Size: 2.2 MB (2225215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbf2f9b9473984973301b1c0ee9c16a48c9a9ab25f87853ddc2032a5e658213`  
		Last Modified: Sat, 10 Jul 2021 18:34:11 GMT  
		Size: 6.7 MB (6744035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26eaba43bac44e8558c21156253c7946c0fe34ec5ae51c5195fdbc66e9afdf3`  
		Last Modified: Sat, 10 Jul 2021 18:34:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4233853c46d89e1b399edf2a5c9ef3b7ea3fdfcac7f613cda66e2494a13b4043`  
		Last Modified: Sat, 10 Jul 2021 18:34:09 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:bc2dfc336f6be99f61ec31eb236fe7d40b1d65a144ed2a2daa58b5631b76ffc6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33528844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef8ad7ad1f3aa5aeb9fa6b8c6bf05ab5ba1d7afc75b8e526d18b21f9bbe232b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:50:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 14:50:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:50:47 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 14:51:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 14:51:49 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 14:51:50 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 14:51:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 14:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 14:51:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddea14b5f0a990ced2cda7fd38b283db7cf2fbc39c095bcb65f07619e005a1fd`  
		Last Modified: Thu, 22 Jul 2021 14:53:08 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92318915694ecdd948d31dd3f08fff61a56c18a58f81d5fa7e674725024b12cd`  
		Last Modified: Thu, 22 Jul 2021 14:53:08 GMT  
		Size: 1.8 MB (1822006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f3a050896b6bda47286d667435dd2e707b1eba373bb686f2361940f5e901f7`  
		Last Modified: Thu, 22 Jul 2021 14:53:09 GMT  
		Size: 5.9 MB (5943867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c128e97627da3cae6da006801c37701839cfe0bb5005ade0b2c5bf572d96bd3`  
		Last Modified: Thu, 22 Jul 2021 14:53:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacd404e715c681b31d67211acb85f8d321a1cb864e5157130b9e7ed515d370a`  
		Last Modified: Thu, 22 Jul 2021 14:53:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:1054032dfae72f0807214d0751246c6675a4527de4b0af06446b9ed3281c5ff9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:77bb7048879f502a0be6947d6ded556dedd56bfbd65846f202ddbae6c0220f84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecec5286e75ac64570dd86ae159bec30df6ff4bb0ecc79f42dd8a5c7126be6eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:41:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:41:21 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:41:21 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:03:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:03:03 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:03:03 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:03:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:03:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc49c1d100974d70cd457c65f0e781af958b9d07a56e03267424f0d11990712`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f3e43d8c62d03bca76a106e58c3099bd76fb7fbad003082a81a3670c07ba69`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 7.3 KB (7282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdfa185ef47533e780a1502b6ecf0f1486cc0955b4930432fdfdc77813e9d50`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 212.6 KB (212559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241cc499201ce5b553c5be7e1b77bfddb66137711a90180f2e25689109405751`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179d6882fdc5e95f3b1481ffb5d149c0fda3dc71d8fa51eba15edc3be50dc54c`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:b758b42acbf998e5a39dc12204e0be903d69a2af37753e5d2133b5df87b06523
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2835923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae8ff3806515f364a387402ad57b51af1f948f849240b2e704a6de2c048ada9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Tue, 22 Jun 2021 00:21:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 22 Jun 2021 00:21:09 GMT
RUN apk add --no-cache libssl1.1
# Tue, 22 Jun 2021 00:21:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:38:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:38:07 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:38:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:38:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:38:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:38:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9e2daf3ec825cb3613604aa1365dbe414dc4e91784135871c1b1dfc68db23d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6101fbc0ffdf60230b896427f198bc223946522d7d1f77e2275181837980568d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 7.3 KB (7308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296999154521c5c6c6c67a405f842cacada3793a86c889ce922a114bae5354a6`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 202.5 KB (202495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22c40bed8d80ea82bb949a3747badad3421eb16ea2e2440962324c9d79ab00b`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd55faef8cc92525b1be13e1e39b9ee16e5caaf2df3e0db276ed2683a509da9`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:57f8db33a0eec466bfc76dd17cee895a03a3789dbd31bd89ef2e8dc7da3455e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2632718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:676e5f41ec430a6e87108a46dd408d068f0e501170755f72925c7a760ed458ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 07:25:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 24 Jun 2021 07:25:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 24 Jun 2021 07:25:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:17:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:17:30 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:17:30 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:17:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:17:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:17:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c429d40f3f855015d365208d1b968cd8f34de9ccedd71360b7f05eab24ddd1`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4522338918253627f69a56835ddb741f10f29e2de17157de4ca03a12561d3e05`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58f4ce029c4b37ef76a46da093755b9e24c2d0765592fd00547e013edf3479c`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 195.8 KB (195767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10cb1e83ae0b13c5adcff700076e63bf3322c49067170f59c7ec0c9d6f0698f`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e1913bac6b271f9c4b484fad7338dcbc98a4526b6e48bf1f6a8ccb3fa3b9a`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:40541478eb401d67036d56bbd4cfd5933f148ce155f8e3292a4d083fbb62ba19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2923277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02b54f6f7a1b548ed3db2fc33cafcbb8ef9b27d6ae45811deeb5ecf484a3d75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:50 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:54:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:54:08 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:54:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:54:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:54:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:54:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a6e447f49f6576247dd515ff88f610088fde09c8c378492a19009d6f6fd3b`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05549f8a714910bf1ba795919183eda4ed8c6c1dacd25e27d16f60e584efd239`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b70a09132ff271f43729154235e305beed323f6f44bb8f91d3f71be66c9f58`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 204.6 KB (204616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf3cdb40c67131120870a15e3902a71c8b1db82a03999be16d35d7d6ae59309`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb17f3d198dd5104ea91d70276d05d71182af08cf309adc75a3b64bd770c1699`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:041a4401f89326839b354e7fb7aeb38b07f545fab3de4c84dc0c8f9cebefacca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f94b397232ecc82d13aa208dbbe6e5a315e7a44a1d284fc0089f766e22aea2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:32 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:33 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:55:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:55:36 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:55:37 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:55:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:55:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:55:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8a1adc7e61a91c39fcba896b070192f506dd419fc77a733ce377c563448785`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982f88ff86958b26737edc45adbf2bf850db25cdc970e348723b0d305f5f6db2`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24fe46b36c0cdba759eaf8ea030281f67337289db167fb4d8d3b7da3e191680`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 223.4 KB (223438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eb79119bc0cf80b5d4a32e3035a171c2c43177ce8bd6cf5f6ad53da848ae22`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1027751b1d208d42e1c73a3526f36a885067bd323348563fb1186928a536a01a`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9d383336851f89b74885b174acf82891ef2bf8c945a6373dec31ca6676fd1107
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2fd56c4b0659f3c04e8bff71019d31b85529f0f9a53b88c69fb81d0bfe3351c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:03:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:03:27 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:03:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 07:04:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 07:04:28 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 07:04:35 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 07:04:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 07:04:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:04:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602add23d4a6d2eadfe98b28abe912c5fcac90dbe9c2a51a54f428ad33d692ee`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451504af2e04d8b41445eedc1f1f9c76a59c85eb2be170be0d8aa078d0aa93e9`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 7.1 KB (7065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd1d09b1e4f40662048b2b792797406a48e2cb33e7e0c06a3b60ff7f189ee3e`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 221.0 KB (220986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38387eb6968cbda04a7e8b097378ba4eba871862d73839fa97fc66d70f606c32`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b42ba1d6389eba3e53edf2210a840a60b804cc8e51a81a4f42bcc86848d85a`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:6ec14094d3594e86c89a330bd9ac7db9109578591c71a7fc895ef583f56a0ebc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8e10c73436dfd94b9788c63d5d89c26217f62795e62170bfee7bb5fddea096c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:06:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 14 Apr 2021 20:06:27 GMT
RUN apk add --no-cache libssl1.1
# Wed, 14 Apr 2021 20:06:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 14 Apr 2021 20:06:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 14 Apr 2021 20:06:37 GMT
VOLUME [/spiped]
# Wed, 14 Apr 2021 20:06:37 GMT
WORKDIR /spiped
# Wed, 14 Apr 2021 20:06:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:06:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:06:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64390452532879e125a5bb8a9120ef0206a6ffed9b7b45143408593823449b69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe161c1af56f1ac1b902a43d31cc07ce45e66ce5deaae0c37c972f8d4d505530`  
		Last Modified: Wed, 14 Apr 2021 20:06:59 GMT  
		Size: 7.1 KB (7054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62195a09ae764bb27e5a0afa4b95616824bbb859a891aaf48c9f5979d1482176`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 205.0 KB (205043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c57dc974a3fd6357043b304379826936777167d99e198e01a3341c951c15b9`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113c0808aca0ef9883bd02b957ed90398dbfabff1dcf1d5e822af51ba8e53d69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:9e61faf7766c81d1b2bc92b19060fbb472e131154e6cf997e1fcf9900ae34480
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

### `spiped:1.6` - linux; amd64

```console
$ docker pull spiped@sha256:b956b0767d9f807a72c03707fe982b145fad5c08520cb20e311ca7e0818d48cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36313927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6cb81ebb115101411214569dc66a92f6ec17458f63d2812c746f6d646e830e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 18:36:22 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 18:36:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 18:36:29 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 18:37:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 18:37:13 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 18:37:14 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 18:37:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 18:37:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 18:37:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fcdf017f7218b1a75d3fecaf7ec1ed0b82e9d4a2cbf0a3aa748904aa91d5e9`  
		Last Modified: Thu, 22 Jul 2021 18:37:42 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c276e87105455c7cb1d515eff3df184ecdd8d5521db6f69468e61ccf0a3ff31`  
		Last Modified: Thu, 22 Jul 2021 18:37:42 GMT  
		Size: 2.1 MB (2128530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584f9bacb5873a6304fc5b45beb1ee4bb0934a09b2a5b886326e26970c0759ee`  
		Last Modified: Thu, 22 Jul 2021 18:37:46 GMT  
		Size: 7.0 MB (7037393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fd07bb166f5100f180eae6c104818d3fb5c07a685780089267afb2c788050f`  
		Last Modified: Thu, 22 Jul 2021 18:37:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9b27eeedf14c9964238ee10c7883ca4c207714d8b2bba7d79d77d8b3a1b240`  
		Last Modified: Thu, 22 Jul 2021 18:37:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:bf3cfe9903cc41ba0683a7cb0a80a8b685ad944460db431c12f66693f1652917
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32200786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c8136d93f716d701747570bfaf290654c3a70f98c1ee463327ab1881cfe3334`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:50:06 GMT
ADD file:885454a996e63d5eb93f1f365a3be77a441f368d7f5a77a7fd1636edf5d0b8cd in / 
# Thu, 22 Jul 2021 00:50:07 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 15:19:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 15:19:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 15:19:31 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 15:20:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 15:20:31 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 15:20:31 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 15:20:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 15:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 15:20:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2b96a0a1ddfe4fab89025b13e583392414251af73361434f28af076c3db77100`  
		Last Modified: Thu, 22 Jul 2021 01:02:11 GMT  
		Size: 24.9 MB (24879093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf71053fc8a635e22437d2e5f42546178aae83512d063e9cf8f448d96bf735c`  
		Last Modified: Thu, 22 Jul 2021 15:21:13 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fda2dec2a04768a237686201e0c2109d4405df968028c4eabc9e3ece91db53e`  
		Last Modified: Thu, 22 Jul 2021 15:21:14 GMT  
		Size: 1.8 MB (1839352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f2a9767797338b3b65675c1484be98470f735697b7e1a13beff9f70e3aa937`  
		Last Modified: Thu, 22 Jul 2021 15:21:18 GMT  
		Size: 5.5 MB (5480142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f5dbc08870311239eda68a9dac3a09339346f5ee9fc589c7d36a7c62233bcb`  
		Last Modified: Thu, 22 Jul 2021 15:21:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619df22f1e652b1ffd841285f8fa97c3271a8d90ca24a50898bc592f2d26dddf`  
		Last Modified: Thu, 22 Jul 2021 15:21:13 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:c8fcd50e24a2fac4210299a2ee03f0d8d0de3a6e51ba6f61a56c263f16a82fd4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5275d81bc421af6ac42959ab8c655ffe4f05b57d6f87325b371cbe74019778`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Thu, 24 Jun 2021 07:24:26 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 24 Jun 2021 07:24:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 07:24:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 24 Jun 2021 07:25:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 24 Jun 2021 07:25:32 GMT
VOLUME [/spiped]
# Thu, 24 Jun 2021 07:25:33 GMT
WORKDIR /spiped
# Thu, 24 Jun 2021 07:25:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 24 Jun 2021 07:25:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 07:25:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae14b3189ef30e120910a62a83035bb35be5ad21d868baa15635cd4093e57b28`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fbbe41540f8564924d1bbf33810a5cca942d52258a07a9a0a9fa47d3e2ee4d`  
		Last Modified: Thu, 24 Jun 2021 07:26:44 GMT  
		Size: 1.8 MB (1759528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6efa0bc06b8244fc2b99086aaab3707ad97a5c1562d486c49f2643704d4c14f`  
		Last Modified: Thu, 24 Jun 2021 07:26:47 GMT  
		Size: 5.3 MB (5285807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf51d89722279aa5fe979daa99ecca041af3e85c0ecb284c9eef346e12a8525`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ce586c187940aa96e929532b8802dd2d2590ae0629d8d6ff5683defad7d791`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:65f4bd8a8f82126f671cba7e50a4e29ae5be674ccd4e8b54fc903f0122529d1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33830174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bffda7f2326039982bc71ccb3ed7a23ab83f9cb3a0edb8f6b57bec2f05c33640`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:40:14 GMT
ADD file:074ffc2065bab83c9a5c596576656b04d271dd78406aadad160b68e38f38269f in / 
# Thu, 22 Jul 2021 00:40:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 13:06:06 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 13:06:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:06:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 13:06:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 13:06:31 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 13:06:31 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 13:06:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 13:06:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 13:06:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:513c6babab2b9079da61a69300c0e26d1037ca98910376098e9ae87baeb112c0`  
		Last Modified: Thu, 22 Jul 2021 00:45:53 GMT  
		Size: 25.9 MB (25914794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1411af469d8f92bb97698e5703d8f7ad244f1cd857675e0a75d70ee944f14245`  
		Last Modified: Thu, 22 Jul 2021 13:07:02 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3243c8e98ff7d2e88e83ff04990f61634881d1cce8810e0828c3efa28b6c2bca`  
		Last Modified: Thu, 22 Jul 2021 13:07:03 GMT  
		Size: 2.0 MB (2007837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5177afdd0c15ac2fff990100a9693273628249825d2816fe38b1af0635d6e8`  
		Last Modified: Thu, 22 Jul 2021 13:07:04 GMT  
		Size: 5.9 MB (5905334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb096a33b8faa1635a48c84a411ee598af2de78005eb2bf4193c98abd1acf710`  
		Last Modified: Thu, 22 Jul 2021 13:07:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26f77edbf391edf857b771c93043e37da21fe182146025e17e1e84b9b901b5a`  
		Last Modified: Thu, 22 Jul 2021 13:07:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:416f3217a461a18ce8841b0e919b4597c3c7cfbbb8e15cb6aed1034aeb76a530
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41565749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75e57c6d1f54be87f02edae84315b3167268ec573dc93c7fa200082f3d11d06b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:50 GMT
ADD file:cb657a3d01f25bf815677ce223e8802d054f11aeb95f85b160982277916637bd in / 
# Thu, 22 Jul 2021 00:39:51 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:46:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 04:46:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:46:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 04:47:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 04:47:05 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 04:47:05 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 04:47:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 04:47:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 04:47:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fa9d06db5f4195bd51665a89e08e2e7db25636ac28ab162fe876ae0a53093fe5`  
		Last Modified: Thu, 22 Jul 2021 00:46:36 GMT  
		Size: 27.8 MB (27797459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d98317cc5a7bbb137cb721cd14964996fcc1cd226e74c42f1d3e9a6f1c21d26`  
		Last Modified: Thu, 22 Jul 2021 04:47:52 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6c852cdd837170bfd8e188d0ee0a9ed2d53645c00502b910e4f5740ac7f274`  
		Last Modified: Thu, 22 Jul 2021 04:47:53 GMT  
		Size: 2.1 MB (2132624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a49b79994d5ac64b456769f7c7746db459fb1750ae0bdfd1e57c5722d5442a`  
		Last Modified: Thu, 22 Jul 2021 04:47:56 GMT  
		Size: 11.6 MB (11633464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00df8cfac155a64078f92787eb8dae0d3f1a6cc9773c91a6f396a5b9c74bebc`  
		Last Modified: Thu, 22 Jul 2021 04:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f4e2ee058c53ad3e4e974fec117bedb80d84ebc68e960b4dfbd7a5a2627a6b`  
		Last Modified: Thu, 22 Jul 2021 04:47:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:ae9a43f44545fa4f8fbc9216f110bea9275772fb3a34302a054a67578b0e92aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33944082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7851e8a264abf459df1961aa3498a0bd3367a58c9efbf8fea901e773c256a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 06:24:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 06:24:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 06:24:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 06:25:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 06:25:34 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 06:25:35 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 06:25:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 06:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 06:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a23924c8bf3350b569f20c725a3858bdc00af64d69c0e78716993be2cb12af`  
		Last Modified: Thu, 22 Jul 2021 06:26:01 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9b33f3cd0917d540b7337cbbbbbc3230c86c7025c904328033c96c8cda9acb`  
		Last Modified: Thu, 22 Jul 2021 06:26:02 GMT  
		Size: 1.7 MB (1712436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fac5ae579dc8b67efab3cb1b2eba289fce2cd42d3bb110f7f3586e620cd22b`  
		Last Modified: Thu, 22 Jul 2021 06:26:07 GMT  
		Size: 6.4 MB (6416700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906932f9ba8b6e63d86125ee0773e094992a32cbefaaa53ef2f248a493fe1b57`  
		Last Modified: Thu, 22 Jul 2021 06:26:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c08f426acceaf16dcdab867559e0cc19c40516df69d43f2eb413d38f6f4d70`  
		Last Modified: Thu, 22 Jul 2021 06:26:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:57915ff2469ccc919bfb944e9bb1b2296a969b92f48cefedea889844de387440
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39525102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db2498759c4271881a8f7943dea35cfb72b5a49109ebcba5683fadfef3f7ef2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 09 Jul 2021 15:58:12 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Fri, 09 Jul 2021 15:58:14 GMT
CMD ["bash"]
# Sat, 10 Jul 2021 18:27:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Jul 2021 18:28:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 18:28:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Jul 2021 18:31:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Jul 2021 18:31:37 GMT
VOLUME [/spiped]
# Sat, 10 Jul 2021 18:31:47 GMT
WORKDIR /spiped
# Sat, 10 Jul 2021 18:31:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Jul 2021 18:31:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Jul 2021 18:32:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f764f35401eb3acc21df9952db2a5406b3f74fb2e579f644235267047cabe99`  
		Last Modified: Sat, 10 Jul 2021 18:34:09 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068bdd38effbf7875a984997014fff888c478fe938893c543d68e4b840f23b9c`  
		Last Modified: Sat, 10 Jul 2021 18:34:10 GMT  
		Size: 2.2 MB (2225215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbf2f9b9473984973301b1c0ee9c16a48c9a9ab25f87853ddc2032a5e658213`  
		Last Modified: Sat, 10 Jul 2021 18:34:11 GMT  
		Size: 6.7 MB (6744035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26eaba43bac44e8558c21156253c7946c0fe34ec5ae51c5195fdbc66e9afdf3`  
		Last Modified: Sat, 10 Jul 2021 18:34:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4233853c46d89e1b399edf2a5c9ef3b7ea3fdfcac7f613cda66e2494a13b4043`  
		Last Modified: Sat, 10 Jul 2021 18:34:09 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:bc2dfc336f6be99f61ec31eb236fe7d40b1d65a144ed2a2daa58b5631b76ffc6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33528844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef8ad7ad1f3aa5aeb9fa6b8c6bf05ab5ba1d7afc75b8e526d18b21f9bbe232b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:50:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 14:50:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:50:47 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 14:51:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 14:51:49 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 14:51:50 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 14:51:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 14:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 14:51:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddea14b5f0a990ced2cda7fd38b283db7cf2fbc39c095bcb65f07619e005a1fd`  
		Last Modified: Thu, 22 Jul 2021 14:53:08 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92318915694ecdd948d31dd3f08fff61a56c18a58f81d5fa7e674725024b12cd`  
		Last Modified: Thu, 22 Jul 2021 14:53:08 GMT  
		Size: 1.8 MB (1822006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f3a050896b6bda47286d667435dd2e707b1eba373bb686f2361940f5e901f7`  
		Last Modified: Thu, 22 Jul 2021 14:53:09 GMT  
		Size: 5.9 MB (5943867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c128e97627da3cae6da006801c37701839cfe0bb5005ade0b2c5bf572d96bd3`  
		Last Modified: Thu, 22 Jul 2021 14:53:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacd404e715c681b31d67211acb85f8d321a1cb864e5157130b9e7ed515d370a`  
		Last Modified: Thu, 22 Jul 2021 14:53:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:1054032dfae72f0807214d0751246c6675a4527de4b0af06446b9ed3281c5ff9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:77bb7048879f502a0be6947d6ded556dedd56bfbd65846f202ddbae6c0220f84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecec5286e75ac64570dd86ae159bec30df6ff4bb0ecc79f42dd8a5c7126be6eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:41:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:41:21 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:41:21 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:03:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:03:03 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:03:03 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:03:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:03:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc49c1d100974d70cd457c65f0e781af958b9d07a56e03267424f0d11990712`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f3e43d8c62d03bca76a106e58c3099bd76fb7fbad003082a81a3670c07ba69`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 7.3 KB (7282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdfa185ef47533e780a1502b6ecf0f1486cc0955b4930432fdfdc77813e9d50`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 212.6 KB (212559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241cc499201ce5b553c5be7e1b77bfddb66137711a90180f2e25689109405751`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179d6882fdc5e95f3b1481ffb5d149c0fda3dc71d8fa51eba15edc3be50dc54c`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:b758b42acbf998e5a39dc12204e0be903d69a2af37753e5d2133b5df87b06523
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2835923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae8ff3806515f364a387402ad57b51af1f948f849240b2e704a6de2c048ada9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Tue, 22 Jun 2021 00:21:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 22 Jun 2021 00:21:09 GMT
RUN apk add --no-cache libssl1.1
# Tue, 22 Jun 2021 00:21:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:38:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:38:07 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:38:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:38:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:38:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:38:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9e2daf3ec825cb3613604aa1365dbe414dc4e91784135871c1b1dfc68db23d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6101fbc0ffdf60230b896427f198bc223946522d7d1f77e2275181837980568d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 7.3 KB (7308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296999154521c5c6c6c67a405f842cacada3793a86c889ce922a114bae5354a6`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 202.5 KB (202495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22c40bed8d80ea82bb949a3747badad3421eb16ea2e2440962324c9d79ab00b`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd55faef8cc92525b1be13e1e39b9ee16e5caaf2df3e0db276ed2683a509da9`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:57f8db33a0eec466bfc76dd17cee895a03a3789dbd31bd89ef2e8dc7da3455e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2632718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:676e5f41ec430a6e87108a46dd408d068f0e501170755f72925c7a760ed458ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 07:25:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 24 Jun 2021 07:25:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 24 Jun 2021 07:25:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:17:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:17:30 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:17:30 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:17:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:17:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:17:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c429d40f3f855015d365208d1b968cd8f34de9ccedd71360b7f05eab24ddd1`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4522338918253627f69a56835ddb741f10f29e2de17157de4ca03a12561d3e05`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58f4ce029c4b37ef76a46da093755b9e24c2d0765592fd00547e013edf3479c`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 195.8 KB (195767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10cb1e83ae0b13c5adcff700076e63bf3322c49067170f59c7ec0c9d6f0698f`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e1913bac6b271f9c4b484fad7338dcbc98a4526b6e48bf1f6a8ccb3fa3b9a`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:40541478eb401d67036d56bbd4cfd5933f148ce155f8e3292a4d083fbb62ba19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2923277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02b54f6f7a1b548ed3db2fc33cafcbb8ef9b27d6ae45811deeb5ecf484a3d75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:50 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:54:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:54:08 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:54:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:54:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:54:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:54:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a6e447f49f6576247dd515ff88f610088fde09c8c378492a19009d6f6fd3b`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05549f8a714910bf1ba795919183eda4ed8c6c1dacd25e27d16f60e584efd239`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b70a09132ff271f43729154235e305beed323f6f44bb8f91d3f71be66c9f58`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 204.6 KB (204616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf3cdb40c67131120870a15e3902a71c8b1db82a03999be16d35d7d6ae59309`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb17f3d198dd5104ea91d70276d05d71182af08cf309adc75a3b64bd770c1699`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:041a4401f89326839b354e7fb7aeb38b07f545fab3de4c84dc0c8f9cebefacca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f94b397232ecc82d13aa208dbbe6e5a315e7a44a1d284fc0089f766e22aea2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:32 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:33 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:55:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:55:36 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:55:37 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:55:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:55:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:55:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8a1adc7e61a91c39fcba896b070192f506dd419fc77a733ce377c563448785`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982f88ff86958b26737edc45adbf2bf850db25cdc970e348723b0d305f5f6db2`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24fe46b36c0cdba759eaf8ea030281f67337289db167fb4d8d3b7da3e191680`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 223.4 KB (223438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eb79119bc0cf80b5d4a32e3035a171c2c43177ce8bd6cf5f6ad53da848ae22`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1027751b1d208d42e1c73a3526f36a885067bd323348563fb1186928a536a01a`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9d383336851f89b74885b174acf82891ef2bf8c945a6373dec31ca6676fd1107
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2fd56c4b0659f3c04e8bff71019d31b85529f0f9a53b88c69fb81d0bfe3351c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:03:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:03:27 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:03:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 07:04:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 07:04:28 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 07:04:35 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 07:04:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 07:04:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:04:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602add23d4a6d2eadfe98b28abe912c5fcac90dbe9c2a51a54f428ad33d692ee`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451504af2e04d8b41445eedc1f1f9c76a59c85eb2be170be0d8aa078d0aa93e9`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 7.1 KB (7065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd1d09b1e4f40662048b2b792797406a48e2cb33e7e0c06a3b60ff7f189ee3e`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 221.0 KB (220986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38387eb6968cbda04a7e8b097378ba4eba871862d73839fa97fc66d70f606c32`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b42ba1d6389eba3e53edf2210a840a60b804cc8e51a81a4f42bcc86848d85a`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:6ec14094d3594e86c89a330bd9ac7db9109578591c71a7fc895ef583f56a0ebc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8e10c73436dfd94b9788c63d5d89c26217f62795e62170bfee7bb5fddea096c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:06:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 14 Apr 2021 20:06:27 GMT
RUN apk add --no-cache libssl1.1
# Wed, 14 Apr 2021 20:06:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 14 Apr 2021 20:06:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 14 Apr 2021 20:06:37 GMT
VOLUME [/spiped]
# Wed, 14 Apr 2021 20:06:37 GMT
WORKDIR /spiped
# Wed, 14 Apr 2021 20:06:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:06:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:06:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64390452532879e125a5bb8a9120ef0206a6ffed9b7b45143408593823449b69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe161c1af56f1ac1b902a43d31cc07ce45e66ce5deaae0c37c972f8d4d505530`  
		Last Modified: Wed, 14 Apr 2021 20:06:59 GMT  
		Size: 7.1 KB (7054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62195a09ae764bb27e5a0afa4b95616824bbb859a891aaf48c9f5979d1482176`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 205.0 KB (205043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c57dc974a3fd6357043b304379826936777167d99e198e01a3341c951c15b9`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113c0808aca0ef9883bd02b957ed90398dbfabff1dcf1d5e822af51ba8e53d69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:9e61faf7766c81d1b2bc92b19060fbb472e131154e6cf997e1fcf9900ae34480
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

### `spiped:1.6.1` - linux; amd64

```console
$ docker pull spiped@sha256:b956b0767d9f807a72c03707fe982b145fad5c08520cb20e311ca7e0818d48cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36313927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6cb81ebb115101411214569dc66a92f6ec17458f63d2812c746f6d646e830e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 18:36:22 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 18:36:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 18:36:29 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 18:37:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 18:37:13 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 18:37:14 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 18:37:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 18:37:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 18:37:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fcdf017f7218b1a75d3fecaf7ec1ed0b82e9d4a2cbf0a3aa748904aa91d5e9`  
		Last Modified: Thu, 22 Jul 2021 18:37:42 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c276e87105455c7cb1d515eff3df184ecdd8d5521db6f69468e61ccf0a3ff31`  
		Last Modified: Thu, 22 Jul 2021 18:37:42 GMT  
		Size: 2.1 MB (2128530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584f9bacb5873a6304fc5b45beb1ee4bb0934a09b2a5b886326e26970c0759ee`  
		Last Modified: Thu, 22 Jul 2021 18:37:46 GMT  
		Size: 7.0 MB (7037393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fd07bb166f5100f180eae6c104818d3fb5c07a685780089267afb2c788050f`  
		Last Modified: Thu, 22 Jul 2021 18:37:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9b27eeedf14c9964238ee10c7883ca4c207714d8b2bba7d79d77d8b3a1b240`  
		Last Modified: Thu, 22 Jul 2021 18:37:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:bf3cfe9903cc41ba0683a7cb0a80a8b685ad944460db431c12f66693f1652917
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32200786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c8136d93f716d701747570bfaf290654c3a70f98c1ee463327ab1881cfe3334`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:50:06 GMT
ADD file:885454a996e63d5eb93f1f365a3be77a441f368d7f5a77a7fd1636edf5d0b8cd in / 
# Thu, 22 Jul 2021 00:50:07 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 15:19:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 15:19:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 15:19:31 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 15:20:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 15:20:31 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 15:20:31 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 15:20:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 15:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 15:20:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2b96a0a1ddfe4fab89025b13e583392414251af73361434f28af076c3db77100`  
		Last Modified: Thu, 22 Jul 2021 01:02:11 GMT  
		Size: 24.9 MB (24879093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf71053fc8a635e22437d2e5f42546178aae83512d063e9cf8f448d96bf735c`  
		Last Modified: Thu, 22 Jul 2021 15:21:13 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fda2dec2a04768a237686201e0c2109d4405df968028c4eabc9e3ece91db53e`  
		Last Modified: Thu, 22 Jul 2021 15:21:14 GMT  
		Size: 1.8 MB (1839352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f2a9767797338b3b65675c1484be98470f735697b7e1a13beff9f70e3aa937`  
		Last Modified: Thu, 22 Jul 2021 15:21:18 GMT  
		Size: 5.5 MB (5480142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f5dbc08870311239eda68a9dac3a09339346f5ee9fc589c7d36a7c62233bcb`  
		Last Modified: Thu, 22 Jul 2021 15:21:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619df22f1e652b1ffd841285f8fa97c3271a8d90ca24a50898bc592f2d26dddf`  
		Last Modified: Thu, 22 Jul 2021 15:21:13 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:c8fcd50e24a2fac4210299a2ee03f0d8d0de3a6e51ba6f61a56c263f16a82fd4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5275d81bc421af6ac42959ab8c655ffe4f05b57d6f87325b371cbe74019778`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Thu, 24 Jun 2021 07:24:26 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 24 Jun 2021 07:24:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 07:24:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 24 Jun 2021 07:25:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 24 Jun 2021 07:25:32 GMT
VOLUME [/spiped]
# Thu, 24 Jun 2021 07:25:33 GMT
WORKDIR /spiped
# Thu, 24 Jun 2021 07:25:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 24 Jun 2021 07:25:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 07:25:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae14b3189ef30e120910a62a83035bb35be5ad21d868baa15635cd4093e57b28`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fbbe41540f8564924d1bbf33810a5cca942d52258a07a9a0a9fa47d3e2ee4d`  
		Last Modified: Thu, 24 Jun 2021 07:26:44 GMT  
		Size: 1.8 MB (1759528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6efa0bc06b8244fc2b99086aaab3707ad97a5c1562d486c49f2643704d4c14f`  
		Last Modified: Thu, 24 Jun 2021 07:26:47 GMT  
		Size: 5.3 MB (5285807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf51d89722279aa5fe979daa99ecca041af3e85c0ecb284c9eef346e12a8525`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ce586c187940aa96e929532b8802dd2d2590ae0629d8d6ff5683defad7d791`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:65f4bd8a8f82126f671cba7e50a4e29ae5be674ccd4e8b54fc903f0122529d1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33830174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bffda7f2326039982bc71ccb3ed7a23ab83f9cb3a0edb8f6b57bec2f05c33640`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:40:14 GMT
ADD file:074ffc2065bab83c9a5c596576656b04d271dd78406aadad160b68e38f38269f in / 
# Thu, 22 Jul 2021 00:40:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 13:06:06 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 13:06:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:06:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 13:06:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 13:06:31 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 13:06:31 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 13:06:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 13:06:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 13:06:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:513c6babab2b9079da61a69300c0e26d1037ca98910376098e9ae87baeb112c0`  
		Last Modified: Thu, 22 Jul 2021 00:45:53 GMT  
		Size: 25.9 MB (25914794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1411af469d8f92bb97698e5703d8f7ad244f1cd857675e0a75d70ee944f14245`  
		Last Modified: Thu, 22 Jul 2021 13:07:02 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3243c8e98ff7d2e88e83ff04990f61634881d1cce8810e0828c3efa28b6c2bca`  
		Last Modified: Thu, 22 Jul 2021 13:07:03 GMT  
		Size: 2.0 MB (2007837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5177afdd0c15ac2fff990100a9693273628249825d2816fe38b1af0635d6e8`  
		Last Modified: Thu, 22 Jul 2021 13:07:04 GMT  
		Size: 5.9 MB (5905334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb096a33b8faa1635a48c84a411ee598af2de78005eb2bf4193c98abd1acf710`  
		Last Modified: Thu, 22 Jul 2021 13:07:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26f77edbf391edf857b771c93043e37da21fe182146025e17e1e84b9b901b5a`  
		Last Modified: Thu, 22 Jul 2021 13:07:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:416f3217a461a18ce8841b0e919b4597c3c7cfbbb8e15cb6aed1034aeb76a530
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41565749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75e57c6d1f54be87f02edae84315b3167268ec573dc93c7fa200082f3d11d06b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:50 GMT
ADD file:cb657a3d01f25bf815677ce223e8802d054f11aeb95f85b160982277916637bd in / 
# Thu, 22 Jul 2021 00:39:51 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:46:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 04:46:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:46:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 04:47:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 04:47:05 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 04:47:05 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 04:47:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 04:47:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 04:47:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fa9d06db5f4195bd51665a89e08e2e7db25636ac28ab162fe876ae0a53093fe5`  
		Last Modified: Thu, 22 Jul 2021 00:46:36 GMT  
		Size: 27.8 MB (27797459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d98317cc5a7bbb137cb721cd14964996fcc1cd226e74c42f1d3e9a6f1c21d26`  
		Last Modified: Thu, 22 Jul 2021 04:47:52 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6c852cdd837170bfd8e188d0ee0a9ed2d53645c00502b910e4f5740ac7f274`  
		Last Modified: Thu, 22 Jul 2021 04:47:53 GMT  
		Size: 2.1 MB (2132624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a49b79994d5ac64b456769f7c7746db459fb1750ae0bdfd1e57c5722d5442a`  
		Last Modified: Thu, 22 Jul 2021 04:47:56 GMT  
		Size: 11.6 MB (11633464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00df8cfac155a64078f92787eb8dae0d3f1a6cc9773c91a6f396a5b9c74bebc`  
		Last Modified: Thu, 22 Jul 2021 04:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f4e2ee058c53ad3e4e974fec117bedb80d84ebc68e960b4dfbd7a5a2627a6b`  
		Last Modified: Thu, 22 Jul 2021 04:47:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:ae9a43f44545fa4f8fbc9216f110bea9275772fb3a34302a054a67578b0e92aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33944082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7851e8a264abf459df1961aa3498a0bd3367a58c9efbf8fea901e773c256a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 06:24:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 06:24:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 06:24:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 06:25:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 06:25:34 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 06:25:35 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 06:25:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 06:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 06:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a23924c8bf3350b569f20c725a3858bdc00af64d69c0e78716993be2cb12af`  
		Last Modified: Thu, 22 Jul 2021 06:26:01 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9b33f3cd0917d540b7337cbbbbbc3230c86c7025c904328033c96c8cda9acb`  
		Last Modified: Thu, 22 Jul 2021 06:26:02 GMT  
		Size: 1.7 MB (1712436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fac5ae579dc8b67efab3cb1b2eba289fce2cd42d3bb110f7f3586e620cd22b`  
		Last Modified: Thu, 22 Jul 2021 06:26:07 GMT  
		Size: 6.4 MB (6416700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906932f9ba8b6e63d86125ee0773e094992a32cbefaaa53ef2f248a493fe1b57`  
		Last Modified: Thu, 22 Jul 2021 06:26:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c08f426acceaf16dcdab867559e0cc19c40516df69d43f2eb413d38f6f4d70`  
		Last Modified: Thu, 22 Jul 2021 06:26:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:57915ff2469ccc919bfb944e9bb1b2296a969b92f48cefedea889844de387440
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39525102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db2498759c4271881a8f7943dea35cfb72b5a49109ebcba5683fadfef3f7ef2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 09 Jul 2021 15:58:12 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Fri, 09 Jul 2021 15:58:14 GMT
CMD ["bash"]
# Sat, 10 Jul 2021 18:27:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Jul 2021 18:28:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 18:28:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Jul 2021 18:31:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Jul 2021 18:31:37 GMT
VOLUME [/spiped]
# Sat, 10 Jul 2021 18:31:47 GMT
WORKDIR /spiped
# Sat, 10 Jul 2021 18:31:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Jul 2021 18:31:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Jul 2021 18:32:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f764f35401eb3acc21df9952db2a5406b3f74fb2e579f644235267047cabe99`  
		Last Modified: Sat, 10 Jul 2021 18:34:09 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068bdd38effbf7875a984997014fff888c478fe938893c543d68e4b840f23b9c`  
		Last Modified: Sat, 10 Jul 2021 18:34:10 GMT  
		Size: 2.2 MB (2225215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbf2f9b9473984973301b1c0ee9c16a48c9a9ab25f87853ddc2032a5e658213`  
		Last Modified: Sat, 10 Jul 2021 18:34:11 GMT  
		Size: 6.7 MB (6744035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26eaba43bac44e8558c21156253c7946c0fe34ec5ae51c5195fdbc66e9afdf3`  
		Last Modified: Sat, 10 Jul 2021 18:34:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4233853c46d89e1b399edf2a5c9ef3b7ea3fdfcac7f613cda66e2494a13b4043`  
		Last Modified: Sat, 10 Jul 2021 18:34:09 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:bc2dfc336f6be99f61ec31eb236fe7d40b1d65a144ed2a2daa58b5631b76ffc6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33528844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef8ad7ad1f3aa5aeb9fa6b8c6bf05ab5ba1d7afc75b8e526d18b21f9bbe232b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:50:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 14:50:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:50:47 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 14:51:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 14:51:49 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 14:51:50 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 14:51:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 14:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 14:51:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddea14b5f0a990ced2cda7fd38b283db7cf2fbc39c095bcb65f07619e005a1fd`  
		Last Modified: Thu, 22 Jul 2021 14:53:08 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92318915694ecdd948d31dd3f08fff61a56c18a58f81d5fa7e674725024b12cd`  
		Last Modified: Thu, 22 Jul 2021 14:53:08 GMT  
		Size: 1.8 MB (1822006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f3a050896b6bda47286d667435dd2e707b1eba373bb686f2361940f5e901f7`  
		Last Modified: Thu, 22 Jul 2021 14:53:09 GMT  
		Size: 5.9 MB (5943867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c128e97627da3cae6da006801c37701839cfe0bb5005ade0b2c5bf572d96bd3`  
		Last Modified: Thu, 22 Jul 2021 14:53:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacd404e715c681b31d67211acb85f8d321a1cb864e5157130b9e7ed515d370a`  
		Last Modified: Thu, 22 Jul 2021 14:53:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:1054032dfae72f0807214d0751246c6675a4527de4b0af06446b9ed3281c5ff9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6.1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:77bb7048879f502a0be6947d6ded556dedd56bfbd65846f202ddbae6c0220f84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecec5286e75ac64570dd86ae159bec30df6ff4bb0ecc79f42dd8a5c7126be6eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:41:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:41:21 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:41:21 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:03:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:03:03 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:03:03 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:03:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:03:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc49c1d100974d70cd457c65f0e781af958b9d07a56e03267424f0d11990712`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f3e43d8c62d03bca76a106e58c3099bd76fb7fbad003082a81a3670c07ba69`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 7.3 KB (7282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdfa185ef47533e780a1502b6ecf0f1486cc0955b4930432fdfdc77813e9d50`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 212.6 KB (212559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241cc499201ce5b553c5be7e1b77bfddb66137711a90180f2e25689109405751`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179d6882fdc5e95f3b1481ffb5d149c0fda3dc71d8fa51eba15edc3be50dc54c`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:b758b42acbf998e5a39dc12204e0be903d69a2af37753e5d2133b5df87b06523
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2835923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae8ff3806515f364a387402ad57b51af1f948f849240b2e704a6de2c048ada9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Tue, 22 Jun 2021 00:21:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 22 Jun 2021 00:21:09 GMT
RUN apk add --no-cache libssl1.1
# Tue, 22 Jun 2021 00:21:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:38:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:38:07 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:38:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:38:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:38:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:38:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9e2daf3ec825cb3613604aa1365dbe414dc4e91784135871c1b1dfc68db23d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6101fbc0ffdf60230b896427f198bc223946522d7d1f77e2275181837980568d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 7.3 KB (7308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296999154521c5c6c6c67a405f842cacada3793a86c889ce922a114bae5354a6`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 202.5 KB (202495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22c40bed8d80ea82bb949a3747badad3421eb16ea2e2440962324c9d79ab00b`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd55faef8cc92525b1be13e1e39b9ee16e5caaf2df3e0db276ed2683a509da9`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:57f8db33a0eec466bfc76dd17cee895a03a3789dbd31bd89ef2e8dc7da3455e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2632718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:676e5f41ec430a6e87108a46dd408d068f0e501170755f72925c7a760ed458ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 07:25:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 24 Jun 2021 07:25:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 24 Jun 2021 07:25:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:17:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:17:30 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:17:30 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:17:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:17:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:17:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c429d40f3f855015d365208d1b968cd8f34de9ccedd71360b7f05eab24ddd1`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4522338918253627f69a56835ddb741f10f29e2de17157de4ca03a12561d3e05`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58f4ce029c4b37ef76a46da093755b9e24c2d0765592fd00547e013edf3479c`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 195.8 KB (195767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10cb1e83ae0b13c5adcff700076e63bf3322c49067170f59c7ec0c9d6f0698f`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e1913bac6b271f9c4b484fad7338dcbc98a4526b6e48bf1f6a8ccb3fa3b9a`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:40541478eb401d67036d56bbd4cfd5933f148ce155f8e3292a4d083fbb62ba19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2923277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02b54f6f7a1b548ed3db2fc33cafcbb8ef9b27d6ae45811deeb5ecf484a3d75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:50 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:54:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:54:08 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:54:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:54:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:54:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:54:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a6e447f49f6576247dd515ff88f610088fde09c8c378492a19009d6f6fd3b`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05549f8a714910bf1ba795919183eda4ed8c6c1dacd25e27d16f60e584efd239`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b70a09132ff271f43729154235e305beed323f6f44bb8f91d3f71be66c9f58`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 204.6 KB (204616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf3cdb40c67131120870a15e3902a71c8b1db82a03999be16d35d7d6ae59309`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb17f3d198dd5104ea91d70276d05d71182af08cf309adc75a3b64bd770c1699`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:041a4401f89326839b354e7fb7aeb38b07f545fab3de4c84dc0c8f9cebefacca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f94b397232ecc82d13aa208dbbe6e5a315e7a44a1d284fc0089f766e22aea2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:32 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:33 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:55:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:55:36 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:55:37 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:55:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:55:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:55:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8a1adc7e61a91c39fcba896b070192f506dd419fc77a733ce377c563448785`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982f88ff86958b26737edc45adbf2bf850db25cdc970e348723b0d305f5f6db2`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24fe46b36c0cdba759eaf8ea030281f67337289db167fb4d8d3b7da3e191680`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 223.4 KB (223438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eb79119bc0cf80b5d4a32e3035a171c2c43177ce8bd6cf5f6ad53da848ae22`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1027751b1d208d42e1c73a3526f36a885067bd323348563fb1186928a536a01a`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9d383336851f89b74885b174acf82891ef2bf8c945a6373dec31ca6676fd1107
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2fd56c4b0659f3c04e8bff71019d31b85529f0f9a53b88c69fb81d0bfe3351c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:03:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:03:27 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:03:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 07:04:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 07:04:28 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 07:04:35 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 07:04:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 07:04:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:04:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602add23d4a6d2eadfe98b28abe912c5fcac90dbe9c2a51a54f428ad33d692ee`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451504af2e04d8b41445eedc1f1f9c76a59c85eb2be170be0d8aa078d0aa93e9`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 7.1 KB (7065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd1d09b1e4f40662048b2b792797406a48e2cb33e7e0c06a3b60ff7f189ee3e`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 221.0 KB (220986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38387eb6968cbda04a7e8b097378ba4eba871862d73839fa97fc66d70f606c32`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b42ba1d6389eba3e53edf2210a840a60b804cc8e51a81a4f42bcc86848d85a`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:6ec14094d3594e86c89a330bd9ac7db9109578591c71a7fc895ef583f56a0ebc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8e10c73436dfd94b9788c63d5d89c26217f62795e62170bfee7bb5fddea096c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:06:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 14 Apr 2021 20:06:27 GMT
RUN apk add --no-cache libssl1.1
# Wed, 14 Apr 2021 20:06:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 14 Apr 2021 20:06:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 14 Apr 2021 20:06:37 GMT
VOLUME [/spiped]
# Wed, 14 Apr 2021 20:06:37 GMT
WORKDIR /spiped
# Wed, 14 Apr 2021 20:06:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:06:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:06:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64390452532879e125a5bb8a9120ef0206a6ffed9b7b45143408593823449b69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe161c1af56f1ac1b902a43d31cc07ce45e66ce5deaae0c37c972f8d4d505530`  
		Last Modified: Wed, 14 Apr 2021 20:06:59 GMT  
		Size: 7.1 KB (7054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62195a09ae764bb27e5a0afa4b95616824bbb859a891aaf48c9f5979d1482176`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 205.0 KB (205043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c57dc974a3fd6357043b304379826936777167d99e198e01a3341c951c15b9`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113c0808aca0ef9883bd02b957ed90398dbfabff1dcf1d5e822af51ba8e53d69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:1054032dfae72f0807214d0751246c6675a4527de4b0af06446b9ed3281c5ff9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:alpine` - linux; amd64

```console
$ docker pull spiped@sha256:77bb7048879f502a0be6947d6ded556dedd56bfbd65846f202ddbae6c0220f84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecec5286e75ac64570dd86ae159bec30df6ff4bb0ecc79f42dd8a5c7126be6eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:41:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:41:21 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:41:21 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:03:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:03:03 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:03:03 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:03:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:03:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc49c1d100974d70cd457c65f0e781af958b9d07a56e03267424f0d11990712`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f3e43d8c62d03bca76a106e58c3099bd76fb7fbad003082a81a3670c07ba69`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 7.3 KB (7282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdfa185ef47533e780a1502b6ecf0f1486cc0955b4930432fdfdc77813e9d50`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 212.6 KB (212559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241cc499201ce5b553c5be7e1b77bfddb66137711a90180f2e25689109405751`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179d6882fdc5e95f3b1481ffb5d149c0fda3dc71d8fa51eba15edc3be50dc54c`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:b758b42acbf998e5a39dc12204e0be903d69a2af37753e5d2133b5df87b06523
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2835923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae8ff3806515f364a387402ad57b51af1f948f849240b2e704a6de2c048ada9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Tue, 22 Jun 2021 00:21:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 22 Jun 2021 00:21:09 GMT
RUN apk add --no-cache libssl1.1
# Tue, 22 Jun 2021 00:21:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:38:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:38:07 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:38:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:38:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:38:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:38:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9e2daf3ec825cb3613604aa1365dbe414dc4e91784135871c1b1dfc68db23d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6101fbc0ffdf60230b896427f198bc223946522d7d1f77e2275181837980568d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 7.3 KB (7308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296999154521c5c6c6c67a405f842cacada3793a86c889ce922a114bae5354a6`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 202.5 KB (202495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22c40bed8d80ea82bb949a3747badad3421eb16ea2e2440962324c9d79ab00b`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd55faef8cc92525b1be13e1e39b9ee16e5caaf2df3e0db276ed2683a509da9`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:57f8db33a0eec466bfc76dd17cee895a03a3789dbd31bd89ef2e8dc7da3455e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2632718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:676e5f41ec430a6e87108a46dd408d068f0e501170755f72925c7a760ed458ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 07:25:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 24 Jun 2021 07:25:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 24 Jun 2021 07:25:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:17:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:17:30 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:17:30 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:17:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:17:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:17:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c429d40f3f855015d365208d1b968cd8f34de9ccedd71360b7f05eab24ddd1`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4522338918253627f69a56835ddb741f10f29e2de17157de4ca03a12561d3e05`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58f4ce029c4b37ef76a46da093755b9e24c2d0765592fd00547e013edf3479c`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 195.8 KB (195767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10cb1e83ae0b13c5adcff700076e63bf3322c49067170f59c7ec0c9d6f0698f`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e1913bac6b271f9c4b484fad7338dcbc98a4526b6e48bf1f6a8ccb3fa3b9a`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:40541478eb401d67036d56bbd4cfd5933f148ce155f8e3292a4d083fbb62ba19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2923277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02b54f6f7a1b548ed3db2fc33cafcbb8ef9b27d6ae45811deeb5ecf484a3d75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:50 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:54:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:54:08 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:54:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:54:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:54:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:54:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a6e447f49f6576247dd515ff88f610088fde09c8c378492a19009d6f6fd3b`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05549f8a714910bf1ba795919183eda4ed8c6c1dacd25e27d16f60e584efd239`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b70a09132ff271f43729154235e305beed323f6f44bb8f91d3f71be66c9f58`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 204.6 KB (204616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf3cdb40c67131120870a15e3902a71c8b1db82a03999be16d35d7d6ae59309`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb17f3d198dd5104ea91d70276d05d71182af08cf309adc75a3b64bd770c1699`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:041a4401f89326839b354e7fb7aeb38b07f545fab3de4c84dc0c8f9cebefacca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f94b397232ecc82d13aa208dbbe6e5a315e7a44a1d284fc0089f766e22aea2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:32 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:33 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:55:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:55:36 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:55:37 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:55:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:55:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:55:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8a1adc7e61a91c39fcba896b070192f506dd419fc77a733ce377c563448785`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982f88ff86958b26737edc45adbf2bf850db25cdc970e348723b0d305f5f6db2`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24fe46b36c0cdba759eaf8ea030281f67337289db167fb4d8d3b7da3e191680`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 223.4 KB (223438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eb79119bc0cf80b5d4a32e3035a171c2c43177ce8bd6cf5f6ad53da848ae22`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1027751b1d208d42e1c73a3526f36a885067bd323348563fb1186928a536a01a`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9d383336851f89b74885b174acf82891ef2bf8c945a6373dec31ca6676fd1107
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2fd56c4b0659f3c04e8bff71019d31b85529f0f9a53b88c69fb81d0bfe3351c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:03:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:03:27 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:03:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 07:04:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 07:04:28 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 07:04:35 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 07:04:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 07:04:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:04:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602add23d4a6d2eadfe98b28abe912c5fcac90dbe9c2a51a54f428ad33d692ee`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451504af2e04d8b41445eedc1f1f9c76a59c85eb2be170be0d8aa078d0aa93e9`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 7.1 KB (7065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd1d09b1e4f40662048b2b792797406a48e2cb33e7e0c06a3b60ff7f189ee3e`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 221.0 KB (220986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38387eb6968cbda04a7e8b097378ba4eba871862d73839fa97fc66d70f606c32`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b42ba1d6389eba3e53edf2210a840a60b804cc8e51a81a4f42bcc86848d85a`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:6ec14094d3594e86c89a330bd9ac7db9109578591c71a7fc895ef583f56a0ebc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8e10c73436dfd94b9788c63d5d89c26217f62795e62170bfee7bb5fddea096c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:06:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 14 Apr 2021 20:06:27 GMT
RUN apk add --no-cache libssl1.1
# Wed, 14 Apr 2021 20:06:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 14 Apr 2021 20:06:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 14 Apr 2021 20:06:37 GMT
VOLUME [/spiped]
# Wed, 14 Apr 2021 20:06:37 GMT
WORKDIR /spiped
# Wed, 14 Apr 2021 20:06:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:06:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:06:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64390452532879e125a5bb8a9120ef0206a6ffed9b7b45143408593823449b69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe161c1af56f1ac1b902a43d31cc07ce45e66ce5deaae0c37c972f8d4d505530`  
		Last Modified: Wed, 14 Apr 2021 20:06:59 GMT  
		Size: 7.1 KB (7054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62195a09ae764bb27e5a0afa4b95616824bbb859a891aaf48c9f5979d1482176`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 205.0 KB (205043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c57dc974a3fd6357043b304379826936777167d99e198e01a3341c951c15b9`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113c0808aca0ef9883bd02b957ed90398dbfabff1dcf1d5e822af51ba8e53d69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:9e61faf7766c81d1b2bc92b19060fbb472e131154e6cf997e1fcf9900ae34480
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
$ docker pull spiped@sha256:b956b0767d9f807a72c03707fe982b145fad5c08520cb20e311ca7e0818d48cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36313927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6cb81ebb115101411214569dc66a92f6ec17458f63d2812c746f6d646e830e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 18:36:22 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 18:36:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 18:36:29 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 18:37:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 18:37:13 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 18:37:14 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 18:37:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 18:37:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 18:37:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fcdf017f7218b1a75d3fecaf7ec1ed0b82e9d4a2cbf0a3aa748904aa91d5e9`  
		Last Modified: Thu, 22 Jul 2021 18:37:42 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c276e87105455c7cb1d515eff3df184ecdd8d5521db6f69468e61ccf0a3ff31`  
		Last Modified: Thu, 22 Jul 2021 18:37:42 GMT  
		Size: 2.1 MB (2128530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584f9bacb5873a6304fc5b45beb1ee4bb0934a09b2a5b886326e26970c0759ee`  
		Last Modified: Thu, 22 Jul 2021 18:37:46 GMT  
		Size: 7.0 MB (7037393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fd07bb166f5100f180eae6c104818d3fb5c07a685780089267afb2c788050f`  
		Last Modified: Thu, 22 Jul 2021 18:37:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9b27eeedf14c9964238ee10c7883ca4c207714d8b2bba7d79d77d8b3a1b240`  
		Last Modified: Thu, 22 Jul 2021 18:37:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:bf3cfe9903cc41ba0683a7cb0a80a8b685ad944460db431c12f66693f1652917
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32200786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c8136d93f716d701747570bfaf290654c3a70f98c1ee463327ab1881cfe3334`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:50:06 GMT
ADD file:885454a996e63d5eb93f1f365a3be77a441f368d7f5a77a7fd1636edf5d0b8cd in / 
# Thu, 22 Jul 2021 00:50:07 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 15:19:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 15:19:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 15:19:31 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 15:20:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 15:20:31 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 15:20:31 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 15:20:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 15:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 15:20:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2b96a0a1ddfe4fab89025b13e583392414251af73361434f28af076c3db77100`  
		Last Modified: Thu, 22 Jul 2021 01:02:11 GMT  
		Size: 24.9 MB (24879093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf71053fc8a635e22437d2e5f42546178aae83512d063e9cf8f448d96bf735c`  
		Last Modified: Thu, 22 Jul 2021 15:21:13 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fda2dec2a04768a237686201e0c2109d4405df968028c4eabc9e3ece91db53e`  
		Last Modified: Thu, 22 Jul 2021 15:21:14 GMT  
		Size: 1.8 MB (1839352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f2a9767797338b3b65675c1484be98470f735697b7e1a13beff9f70e3aa937`  
		Last Modified: Thu, 22 Jul 2021 15:21:18 GMT  
		Size: 5.5 MB (5480142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f5dbc08870311239eda68a9dac3a09339346f5ee9fc589c7d36a7c62233bcb`  
		Last Modified: Thu, 22 Jul 2021 15:21:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619df22f1e652b1ffd841285f8fa97c3271a8d90ca24a50898bc592f2d26dddf`  
		Last Modified: Thu, 22 Jul 2021 15:21:13 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:c8fcd50e24a2fac4210299a2ee03f0d8d0de3a6e51ba6f61a56c263f16a82fd4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5275d81bc421af6ac42959ab8c655ffe4f05b57d6f87325b371cbe74019778`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Thu, 24 Jun 2021 07:24:26 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 24 Jun 2021 07:24:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 07:24:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 24 Jun 2021 07:25:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 24 Jun 2021 07:25:32 GMT
VOLUME [/spiped]
# Thu, 24 Jun 2021 07:25:33 GMT
WORKDIR /spiped
# Thu, 24 Jun 2021 07:25:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 24 Jun 2021 07:25:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 07:25:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae14b3189ef30e120910a62a83035bb35be5ad21d868baa15635cd4093e57b28`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fbbe41540f8564924d1bbf33810a5cca942d52258a07a9a0a9fa47d3e2ee4d`  
		Last Modified: Thu, 24 Jun 2021 07:26:44 GMT  
		Size: 1.8 MB (1759528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6efa0bc06b8244fc2b99086aaab3707ad97a5c1562d486c49f2643704d4c14f`  
		Last Modified: Thu, 24 Jun 2021 07:26:47 GMT  
		Size: 5.3 MB (5285807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf51d89722279aa5fe979daa99ecca041af3e85c0ecb284c9eef346e12a8525`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ce586c187940aa96e929532b8802dd2d2590ae0629d8d6ff5683defad7d791`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:65f4bd8a8f82126f671cba7e50a4e29ae5be674ccd4e8b54fc903f0122529d1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33830174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bffda7f2326039982bc71ccb3ed7a23ab83f9cb3a0edb8f6b57bec2f05c33640`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:40:14 GMT
ADD file:074ffc2065bab83c9a5c596576656b04d271dd78406aadad160b68e38f38269f in / 
# Thu, 22 Jul 2021 00:40:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 13:06:06 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 13:06:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:06:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 13:06:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 13:06:31 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 13:06:31 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 13:06:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 13:06:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 13:06:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:513c6babab2b9079da61a69300c0e26d1037ca98910376098e9ae87baeb112c0`  
		Last Modified: Thu, 22 Jul 2021 00:45:53 GMT  
		Size: 25.9 MB (25914794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1411af469d8f92bb97698e5703d8f7ad244f1cd857675e0a75d70ee944f14245`  
		Last Modified: Thu, 22 Jul 2021 13:07:02 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3243c8e98ff7d2e88e83ff04990f61634881d1cce8810e0828c3efa28b6c2bca`  
		Last Modified: Thu, 22 Jul 2021 13:07:03 GMT  
		Size: 2.0 MB (2007837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5177afdd0c15ac2fff990100a9693273628249825d2816fe38b1af0635d6e8`  
		Last Modified: Thu, 22 Jul 2021 13:07:04 GMT  
		Size: 5.9 MB (5905334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb096a33b8faa1635a48c84a411ee598af2de78005eb2bf4193c98abd1acf710`  
		Last Modified: Thu, 22 Jul 2021 13:07:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26f77edbf391edf857b771c93043e37da21fe182146025e17e1e84b9b901b5a`  
		Last Modified: Thu, 22 Jul 2021 13:07:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:416f3217a461a18ce8841b0e919b4597c3c7cfbbb8e15cb6aed1034aeb76a530
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41565749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75e57c6d1f54be87f02edae84315b3167268ec573dc93c7fa200082f3d11d06b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:50 GMT
ADD file:cb657a3d01f25bf815677ce223e8802d054f11aeb95f85b160982277916637bd in / 
# Thu, 22 Jul 2021 00:39:51 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:46:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 04:46:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:46:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 04:47:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 04:47:05 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 04:47:05 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 04:47:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 04:47:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 04:47:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fa9d06db5f4195bd51665a89e08e2e7db25636ac28ab162fe876ae0a53093fe5`  
		Last Modified: Thu, 22 Jul 2021 00:46:36 GMT  
		Size: 27.8 MB (27797459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d98317cc5a7bbb137cb721cd14964996fcc1cd226e74c42f1d3e9a6f1c21d26`  
		Last Modified: Thu, 22 Jul 2021 04:47:52 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6c852cdd837170bfd8e188d0ee0a9ed2d53645c00502b910e4f5740ac7f274`  
		Last Modified: Thu, 22 Jul 2021 04:47:53 GMT  
		Size: 2.1 MB (2132624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a49b79994d5ac64b456769f7c7746db459fb1750ae0bdfd1e57c5722d5442a`  
		Last Modified: Thu, 22 Jul 2021 04:47:56 GMT  
		Size: 11.6 MB (11633464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00df8cfac155a64078f92787eb8dae0d3f1a6cc9773c91a6f396a5b9c74bebc`  
		Last Modified: Thu, 22 Jul 2021 04:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f4e2ee058c53ad3e4e974fec117bedb80d84ebc68e960b4dfbd7a5a2627a6b`  
		Last Modified: Thu, 22 Jul 2021 04:47:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:ae9a43f44545fa4f8fbc9216f110bea9275772fb3a34302a054a67578b0e92aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33944082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7851e8a264abf459df1961aa3498a0bd3367a58c9efbf8fea901e773c256a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 06:24:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 06:24:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 06:24:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 06:25:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 06:25:34 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 06:25:35 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 06:25:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 06:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 06:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a23924c8bf3350b569f20c725a3858bdc00af64d69c0e78716993be2cb12af`  
		Last Modified: Thu, 22 Jul 2021 06:26:01 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9b33f3cd0917d540b7337cbbbbbc3230c86c7025c904328033c96c8cda9acb`  
		Last Modified: Thu, 22 Jul 2021 06:26:02 GMT  
		Size: 1.7 MB (1712436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fac5ae579dc8b67efab3cb1b2eba289fce2cd42d3bb110f7f3586e620cd22b`  
		Last Modified: Thu, 22 Jul 2021 06:26:07 GMT  
		Size: 6.4 MB (6416700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906932f9ba8b6e63d86125ee0773e094992a32cbefaaa53ef2f248a493fe1b57`  
		Last Modified: Thu, 22 Jul 2021 06:26:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c08f426acceaf16dcdab867559e0cc19c40516df69d43f2eb413d38f6f4d70`  
		Last Modified: Thu, 22 Jul 2021 06:26:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:57915ff2469ccc919bfb944e9bb1b2296a969b92f48cefedea889844de387440
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39525102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db2498759c4271881a8f7943dea35cfb72b5a49109ebcba5683fadfef3f7ef2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 09 Jul 2021 15:58:12 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Fri, 09 Jul 2021 15:58:14 GMT
CMD ["bash"]
# Sat, 10 Jul 2021 18:27:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Jul 2021 18:28:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 18:28:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Jul 2021 18:31:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Jul 2021 18:31:37 GMT
VOLUME [/spiped]
# Sat, 10 Jul 2021 18:31:47 GMT
WORKDIR /spiped
# Sat, 10 Jul 2021 18:31:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Jul 2021 18:31:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Jul 2021 18:32:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f764f35401eb3acc21df9952db2a5406b3f74fb2e579f644235267047cabe99`  
		Last Modified: Sat, 10 Jul 2021 18:34:09 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068bdd38effbf7875a984997014fff888c478fe938893c543d68e4b840f23b9c`  
		Last Modified: Sat, 10 Jul 2021 18:34:10 GMT  
		Size: 2.2 MB (2225215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbf2f9b9473984973301b1c0ee9c16a48c9a9ab25f87853ddc2032a5e658213`  
		Last Modified: Sat, 10 Jul 2021 18:34:11 GMT  
		Size: 6.7 MB (6744035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26eaba43bac44e8558c21156253c7946c0fe34ec5ae51c5195fdbc66e9afdf3`  
		Last Modified: Sat, 10 Jul 2021 18:34:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4233853c46d89e1b399edf2a5c9ef3b7ea3fdfcac7f613cda66e2494a13b4043`  
		Last Modified: Sat, 10 Jul 2021 18:34:09 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:bc2dfc336f6be99f61ec31eb236fe7d40b1d65a144ed2a2daa58b5631b76ffc6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33528844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef8ad7ad1f3aa5aeb9fa6b8c6bf05ab5ba1d7afc75b8e526d18b21f9bbe232b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:50:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 22 Jul 2021 14:50:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:50:47 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Jul 2021 14:51:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 14:51:49 GMT
VOLUME [/spiped]
# Thu, 22 Jul 2021 14:51:50 GMT
WORKDIR /spiped
# Thu, 22 Jul 2021 14:51:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Jul 2021 14:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 14:51:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddea14b5f0a990ced2cda7fd38b283db7cf2fbc39c095bcb65f07619e005a1fd`  
		Last Modified: Thu, 22 Jul 2021 14:53:08 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92318915694ecdd948d31dd3f08fff61a56c18a58f81d5fa7e674725024b12cd`  
		Last Modified: Thu, 22 Jul 2021 14:53:08 GMT  
		Size: 1.8 MB (1822006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f3a050896b6bda47286d667435dd2e707b1eba373bb686f2361940f5e901f7`  
		Last Modified: Thu, 22 Jul 2021 14:53:09 GMT  
		Size: 5.9 MB (5943867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c128e97627da3cae6da006801c37701839cfe0bb5005ade0b2c5bf572d96bd3`  
		Last Modified: Thu, 22 Jul 2021 14:53:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacd404e715c681b31d67211acb85f8d321a1cb864e5157130b9e7ed515d370a`  
		Last Modified: Thu, 22 Jul 2021 14:53:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
