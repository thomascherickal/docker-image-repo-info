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
$ docker pull spiped@sha256:3f7aee6424d8e855ebe6dddca85bc4e87b619aff2edd89bcbb74f516a64e1b24
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
$ docker pull spiped@sha256:699a597305fe7100c7693c271debbb205f614e3d0121cc56df4d15176f2c61cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4610169607c66b15865617305efd55c796fb1bb4d0b782c7dd7f3ec01f12f9a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 03:09:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 23 Jul 2021 03:09:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 03:09:33 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 23 Jul 2021 03:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 23 Jul 2021 03:10:30 GMT
VOLUME [/spiped]
# Fri, 23 Jul 2021 03:10:30 GMT
WORKDIR /spiped
# Fri, 23 Jul 2021 03:10:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 23 Jul 2021 03:10:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Jul 2021 03:10:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de916f7b97e5eb43a8edd2b6ee1ad63498619b50eb4cbfb017d71b95ff289caf`  
		Last Modified: Fri, 23 Jul 2021 03:11:38 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d4af5c0777c03753720afc23f1dd0b7cacab3c99d8954a8c8f57db7f2af33e`  
		Last Modified: Fri, 23 Jul 2021 03:11:38 GMT  
		Size: 1.8 MB (1759505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855cd38fb8bc28302f7e48641a16bb36c4f04eb022bb47f30151f3c2033f05de`  
		Last Modified: Fri, 23 Jul 2021 03:11:42 GMT  
		Size: 5.3 MB (5285901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796be87dfcfd639be2c0b1c65cd816cb684ab2b8422083c24745817fceaa49a2`  
		Last Modified: Fri, 23 Jul 2021 03:11:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e33f6a15f0addd124b890009c782cbe3a9181bd787565d37bc87cea0ef09bf`  
		Last Modified: Fri, 23 Jul 2021 03:11:38 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:20370abf15be60a98880c1b7557f40a4c2755aed4b2a27119d7979b785bc795d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39525135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f3494d6eae461220831621f3c69c3cf3f83c4a86ea58aa8cbad0b72fde83bbd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 02:13:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 23 Jul 2021 02:13:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:13:47 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 23 Jul 2021 02:17:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 23 Jul 2021 02:17:15 GMT
VOLUME [/spiped]
# Fri, 23 Jul 2021 02:17:20 GMT
WORKDIR /spiped
# Fri, 23 Jul 2021 02:17:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 23 Jul 2021 02:17:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Jul 2021 02:17:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79e2a440de83ae3592492eb9dd671bc9d11ced769aa02ea4af21ec4ec9361bc`  
		Last Modified: Fri, 23 Jul 2021 02:20:16 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cea156edf57e948965a4a5fc44b087c2535d880466c6b805fd0895a3d52d873`  
		Last Modified: Fri, 23 Jul 2021 02:20:17 GMT  
		Size: 2.2 MB (2225179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7301bf2714c9f1f9d2a9e50d20641ce37bafa4aeef3a74d6754e00cf00df33a`  
		Last Modified: Fri, 23 Jul 2021 02:20:18 GMT  
		Size: 6.7 MB (6744030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f949d63c4f754b5ad6ec1ff0f6a9f8bd05f76157aa184ad4296d6a03d04967df`  
		Last Modified: Fri, 23 Jul 2021 02:20:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10f2ba44cd479a0906c8865a991c102b39311bcd0ad5c461a282e6a40643f01`  
		Last Modified: Fri, 23 Jul 2021 02:20:16 GMT  
		Size: 343.0 B  
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
$ docker pull spiped@sha256:e7dbba32f20064755cf05c473ae6e9b44a3eea8a6cd5e81fdc51e22bc6028fd4
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
$ docker pull spiped@sha256:81959987e9809ba3bedbd6901a88e9fe28f2b16377bc8d3e43604661d48c2d15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3034576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d417cc665c58c81ae417555e8357d1f37bf78df7aaf23da4dcc13659df5a95a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:25:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 22:25:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 22:25:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 22:26:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 22:26:12 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 22:26:13 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 22:26:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 22:26:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 22:26:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9c880241f8602d0cc47e4fabf713180b354b6d9819786e78aaf3a9665b7767`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008bccb485a15a7ccb6581c8d02974f14fd68b58810d648f7295647a532772b0`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 7.3 KB (7279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7741dee13e8d6c91732585334d7cef9f489ff0ba3dda16074f7cf05e58ed528a`  
		Last Modified: Fri, 06 Aug 2021 22:26:33 GMT  
		Size: 212.6 KB (212550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0337b646a0031aa1e94edce7b03cdab87816253a6850b30bf5fcfe39128e09`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc226b22f034d312b242c20826de8afa099040078d13d904d45dfeb771850e6`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:5106236450e3abdcba7735635894ff0393e5f0ce938d3fab894ece612e116c92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2837884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07cdb6952199964783a11e1091cc96fa94684fd9e645edcea0376c4fef959217`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 23:52:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 23:52:52 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 23:52:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 23:53:27 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 23:53:27 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 23:53:28 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 23:53:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 23:53:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 23:53:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2adf0d4d8cc8b9e29d8414cae24c000412da47df5cb21a2a05ddf2e10dce570`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33562af158cbe4a36f2391938531bae4126685733de295b7ed766183da4b65ef`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 7.3 KB (7298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23d92f94fd24201f1627f9cdbd4e09c0eced2bcbb6ebf6edd1cd206d43e2989`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 202.5 KB (202496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e821b43798aa5a90978114728243266a0f589a4f572c8034852cb0d17ce7c803`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ba2a665cda34f66fc655e2d76ea1f17e791687438e3675a6ca88c09fa438d`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:4b39dd207a36df0ab651368a23dd5f7fb85cb40c73169a18ed6a650c9e1e9fc5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2634162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a80c87f5ffe5257a7577c370989dbed14396b7ee0a5768d7e330b488935c5205`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:50:46 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 19:50:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 19:50:52 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 19:51:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 19:51:30 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 19:51:31 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 19:51:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 19:51:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:51:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d7a90d848ed25f9597b7555466d565e3c10725a9f17b4863bb5543b964fbef`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56efc9f5e430a2d91ff87e40f30089c0015233688200b25c6c645b9c75917480`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7705d09d2948f05566c3ad4b7184193f719c33fb432e05f9e9d134e1850c51f2`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 195.8 KB (195768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576177e1db2fc775ca441543afa32e5f65ec818813bbb783b5cfea5edcb0da7d`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd82adbb730f7bc7d4c11d373678c8f08c809f2f46e9cd79ae1f11169ec1f8b`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:11f573b8237bb1841a7175c9c9b77f7b8c680623ab91182c3b15186ce6d0a684
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2924266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11d2305d4144c6a7caf39b8b6ca94a94d25dce28a8b4d51cbf4904172d0d3d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:20:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 07 Aug 2021 01:20:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 07 Aug 2021 01:20:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 07 Aug 2021 01:20:46 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 07 Aug 2021 01:20:47 GMT
VOLUME [/spiped]
# Sat, 07 Aug 2021 01:20:47 GMT
WORKDIR /spiped
# Sat, 07 Aug 2021 01:20:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 07 Aug 2021 01:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 01:20:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0faf3295f84c6343ed4bedec1bceca8f73e65a202fab2dde2578d5032f0264`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909cb3a09ec0e0c7512a5e0803fb90d9fa40a1331ebd44ac5923e377ef619c88`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 7.3 KB (7293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da73e2091b0f5e799ac0526b25f8ee65662172dccf092bfcebac9a4f451801e2`  
		Last Modified: Sat, 07 Aug 2021 01:21:19 GMT  
		Size: 204.6 KB (204623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d3f2992d2b842a28dfa27d50163a579400dcff25c9326252f55415706303af`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac232dfb34c3889ce2beb5d4442d4a3b927e0ece42f3ab8a81de9779d579cba`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:f99c513faad87e225c2e474c95f7ceace240bcfdc0f161e74943db703f489f36
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3054380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:355bc30b5b850a5b153236ee5157aa164f2754488c4565a7142fb520abe22f4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:38:26 GMT
ADD file:bafaec4a54d6cef99b5f3660d074a3d2251e4d4bd09df9ea65f33e9bffb7d88d in / 
# Fri, 06 Aug 2021 17:38:26 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 17:57:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 17:57:45 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 17:57:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 17:58:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 17:58:08 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 17:58:08 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 17:58:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 17:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 17:58:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:935703e1179e32e201e4a36d5664d58299dc8e7bcac197b70c295c0a59216db1`  
		Last Modified: Fri, 06 Aug 2021 17:39:15 GMT  
		Size: 2.8 MB (2821910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9f8235dc8f7a2cb2e106af5945d974007f182ef18717b1358dc418b51672e7`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c8e66016715cac7eea56fb6278759a154b998e9cc867cfd9e699f45749f938`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 7.3 KB (7288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b143265a7e8e4e62818a693cb546d0cdbedb96dac486cdfaa3326b27c5669`  
		Last Modified: Fri, 06 Aug 2021 17:58:43 GMT  
		Size: 223.4 KB (223442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac32f75f64f9f329d462d69b46dad0bde0e7c7356333e99089593e3e0359d85`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3d678fb9c378cbc3489d13a25fa17ca3d91d2319e6ffef53f6f84101025d21`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:fb4e68d177bc77f575c1a12ed21a941cb1ac2e423be4e1231ec7f327802e88a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3041425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8692281a7b48476e4611c785ef1f090697d8d28d64eca5cd85eabdf3842f44aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 18:28:28 GMT
ADD file:40f3b617d7ff269d92f0ffcf8aad561b5f2c0626ef519a7f584f1ba0182b3188 in / 
# Fri, 06 Aug 2021 18:28:35 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:30:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 07 Aug 2021 01:31:04 GMT
RUN apk add --no-cache libssl1.1
# Sat, 07 Aug 2021 01:31:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 07 Aug 2021 01:31:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 07 Aug 2021 01:31:47 GMT
VOLUME [/spiped]
# Sat, 07 Aug 2021 01:31:54 GMT
WORKDIR /spiped
# Sat, 07 Aug 2021 01:31:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 07 Aug 2021 01:32:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 01:32:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0ff902055236f70c4694c806877243e1dd52c513825a2a3ecc7eba8f5202acc8`  
		Last Modified: Fri, 06 Aug 2021 18:29:33 GMT  
		Size: 2.8 MB (2811152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e1daa083c0d4e8922acb4a3735a2446ec516ebedf8992b97d0d8ac09474f9e`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ab775043317669024edb01d89328f75341409396938066bd82d18bcfa0f1b6`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f9821113c32743f01e0620003d0630b6021c4148138f74add3efc51d82916a`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 221.2 KB (221239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2760cfc3e6b029ffb984aafe5b489eac1b215d0fe413a43cd00255dac46393`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b6d8de58c0e97f9000849b6c5be64af02ae4149134d50dedcb8e40e121b5e2`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 340.0 B  
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
$ docker pull spiped@sha256:3f7aee6424d8e855ebe6dddca85bc4e87b619aff2edd89bcbb74f516a64e1b24
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
$ docker pull spiped@sha256:699a597305fe7100c7693c271debbb205f614e3d0121cc56df4d15176f2c61cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4610169607c66b15865617305efd55c796fb1bb4d0b782c7dd7f3ec01f12f9a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 03:09:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 23 Jul 2021 03:09:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 03:09:33 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 23 Jul 2021 03:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 23 Jul 2021 03:10:30 GMT
VOLUME [/spiped]
# Fri, 23 Jul 2021 03:10:30 GMT
WORKDIR /spiped
# Fri, 23 Jul 2021 03:10:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 23 Jul 2021 03:10:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Jul 2021 03:10:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de916f7b97e5eb43a8edd2b6ee1ad63498619b50eb4cbfb017d71b95ff289caf`  
		Last Modified: Fri, 23 Jul 2021 03:11:38 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d4af5c0777c03753720afc23f1dd0b7cacab3c99d8954a8c8f57db7f2af33e`  
		Last Modified: Fri, 23 Jul 2021 03:11:38 GMT  
		Size: 1.8 MB (1759505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855cd38fb8bc28302f7e48641a16bb36c4f04eb022bb47f30151f3c2033f05de`  
		Last Modified: Fri, 23 Jul 2021 03:11:42 GMT  
		Size: 5.3 MB (5285901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796be87dfcfd639be2c0b1c65cd816cb684ab2b8422083c24745817fceaa49a2`  
		Last Modified: Fri, 23 Jul 2021 03:11:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e33f6a15f0addd124b890009c782cbe3a9181bd787565d37bc87cea0ef09bf`  
		Last Modified: Fri, 23 Jul 2021 03:11:38 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:20370abf15be60a98880c1b7557f40a4c2755aed4b2a27119d7979b785bc795d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39525135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f3494d6eae461220831621f3c69c3cf3f83c4a86ea58aa8cbad0b72fde83bbd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 02:13:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 23 Jul 2021 02:13:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:13:47 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 23 Jul 2021 02:17:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 23 Jul 2021 02:17:15 GMT
VOLUME [/spiped]
# Fri, 23 Jul 2021 02:17:20 GMT
WORKDIR /spiped
# Fri, 23 Jul 2021 02:17:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 23 Jul 2021 02:17:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Jul 2021 02:17:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79e2a440de83ae3592492eb9dd671bc9d11ced769aa02ea4af21ec4ec9361bc`  
		Last Modified: Fri, 23 Jul 2021 02:20:16 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cea156edf57e948965a4a5fc44b087c2535d880466c6b805fd0895a3d52d873`  
		Last Modified: Fri, 23 Jul 2021 02:20:17 GMT  
		Size: 2.2 MB (2225179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7301bf2714c9f1f9d2a9e50d20641ce37bafa4aeef3a74d6754e00cf00df33a`  
		Last Modified: Fri, 23 Jul 2021 02:20:18 GMT  
		Size: 6.7 MB (6744030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f949d63c4f754b5ad6ec1ff0f6a9f8bd05f76157aa184ad4296d6a03d04967df`  
		Last Modified: Fri, 23 Jul 2021 02:20:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10f2ba44cd479a0906c8865a991c102b39311bcd0ad5c461a282e6a40643f01`  
		Last Modified: Fri, 23 Jul 2021 02:20:16 GMT  
		Size: 343.0 B  
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
$ docker pull spiped@sha256:e7dbba32f20064755cf05c473ae6e9b44a3eea8a6cd5e81fdc51e22bc6028fd4
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
$ docker pull spiped@sha256:81959987e9809ba3bedbd6901a88e9fe28f2b16377bc8d3e43604661d48c2d15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3034576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d417cc665c58c81ae417555e8357d1f37bf78df7aaf23da4dcc13659df5a95a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:25:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 22:25:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 22:25:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 22:26:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 22:26:12 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 22:26:13 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 22:26:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 22:26:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 22:26:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9c880241f8602d0cc47e4fabf713180b354b6d9819786e78aaf3a9665b7767`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008bccb485a15a7ccb6581c8d02974f14fd68b58810d648f7295647a532772b0`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 7.3 KB (7279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7741dee13e8d6c91732585334d7cef9f489ff0ba3dda16074f7cf05e58ed528a`  
		Last Modified: Fri, 06 Aug 2021 22:26:33 GMT  
		Size: 212.6 KB (212550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0337b646a0031aa1e94edce7b03cdab87816253a6850b30bf5fcfe39128e09`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc226b22f034d312b242c20826de8afa099040078d13d904d45dfeb771850e6`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:5106236450e3abdcba7735635894ff0393e5f0ce938d3fab894ece612e116c92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2837884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07cdb6952199964783a11e1091cc96fa94684fd9e645edcea0376c4fef959217`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 23:52:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 23:52:52 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 23:52:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 23:53:27 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 23:53:27 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 23:53:28 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 23:53:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 23:53:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 23:53:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2adf0d4d8cc8b9e29d8414cae24c000412da47df5cb21a2a05ddf2e10dce570`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33562af158cbe4a36f2391938531bae4126685733de295b7ed766183da4b65ef`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 7.3 KB (7298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23d92f94fd24201f1627f9cdbd4e09c0eced2bcbb6ebf6edd1cd206d43e2989`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 202.5 KB (202496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e821b43798aa5a90978114728243266a0f589a4f572c8034852cb0d17ce7c803`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ba2a665cda34f66fc655e2d76ea1f17e791687438e3675a6ca88c09fa438d`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:4b39dd207a36df0ab651368a23dd5f7fb85cb40c73169a18ed6a650c9e1e9fc5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2634162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a80c87f5ffe5257a7577c370989dbed14396b7ee0a5768d7e330b488935c5205`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:50:46 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 19:50:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 19:50:52 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 19:51:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 19:51:30 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 19:51:31 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 19:51:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 19:51:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:51:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d7a90d848ed25f9597b7555466d565e3c10725a9f17b4863bb5543b964fbef`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56efc9f5e430a2d91ff87e40f30089c0015233688200b25c6c645b9c75917480`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7705d09d2948f05566c3ad4b7184193f719c33fb432e05f9e9d134e1850c51f2`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 195.8 KB (195768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576177e1db2fc775ca441543afa32e5f65ec818813bbb783b5cfea5edcb0da7d`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd82adbb730f7bc7d4c11d373678c8f08c809f2f46e9cd79ae1f11169ec1f8b`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:11f573b8237bb1841a7175c9c9b77f7b8c680623ab91182c3b15186ce6d0a684
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2924266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11d2305d4144c6a7caf39b8b6ca94a94d25dce28a8b4d51cbf4904172d0d3d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:20:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 07 Aug 2021 01:20:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 07 Aug 2021 01:20:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 07 Aug 2021 01:20:46 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 07 Aug 2021 01:20:47 GMT
VOLUME [/spiped]
# Sat, 07 Aug 2021 01:20:47 GMT
WORKDIR /spiped
# Sat, 07 Aug 2021 01:20:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 07 Aug 2021 01:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 01:20:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0faf3295f84c6343ed4bedec1bceca8f73e65a202fab2dde2578d5032f0264`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909cb3a09ec0e0c7512a5e0803fb90d9fa40a1331ebd44ac5923e377ef619c88`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 7.3 KB (7293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da73e2091b0f5e799ac0526b25f8ee65662172dccf092bfcebac9a4f451801e2`  
		Last Modified: Sat, 07 Aug 2021 01:21:19 GMT  
		Size: 204.6 KB (204623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d3f2992d2b842a28dfa27d50163a579400dcff25c9326252f55415706303af`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac232dfb34c3889ce2beb5d4442d4a3b927e0ece42f3ab8a81de9779d579cba`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:f99c513faad87e225c2e474c95f7ceace240bcfdc0f161e74943db703f489f36
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3054380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:355bc30b5b850a5b153236ee5157aa164f2754488c4565a7142fb520abe22f4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:38:26 GMT
ADD file:bafaec4a54d6cef99b5f3660d074a3d2251e4d4bd09df9ea65f33e9bffb7d88d in / 
# Fri, 06 Aug 2021 17:38:26 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 17:57:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 17:57:45 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 17:57:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 17:58:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 17:58:08 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 17:58:08 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 17:58:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 17:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 17:58:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:935703e1179e32e201e4a36d5664d58299dc8e7bcac197b70c295c0a59216db1`  
		Last Modified: Fri, 06 Aug 2021 17:39:15 GMT  
		Size: 2.8 MB (2821910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9f8235dc8f7a2cb2e106af5945d974007f182ef18717b1358dc418b51672e7`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c8e66016715cac7eea56fb6278759a154b998e9cc867cfd9e699f45749f938`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 7.3 KB (7288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b143265a7e8e4e62818a693cb546d0cdbedb96dac486cdfaa3326b27c5669`  
		Last Modified: Fri, 06 Aug 2021 17:58:43 GMT  
		Size: 223.4 KB (223442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac32f75f64f9f329d462d69b46dad0bde0e7c7356333e99089593e3e0359d85`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3d678fb9c378cbc3489d13a25fa17ca3d91d2319e6ffef53f6f84101025d21`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:fb4e68d177bc77f575c1a12ed21a941cb1ac2e423be4e1231ec7f327802e88a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3041425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8692281a7b48476e4611c785ef1f090697d8d28d64eca5cd85eabdf3842f44aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 18:28:28 GMT
ADD file:40f3b617d7ff269d92f0ffcf8aad561b5f2c0626ef519a7f584f1ba0182b3188 in / 
# Fri, 06 Aug 2021 18:28:35 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:30:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 07 Aug 2021 01:31:04 GMT
RUN apk add --no-cache libssl1.1
# Sat, 07 Aug 2021 01:31:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 07 Aug 2021 01:31:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 07 Aug 2021 01:31:47 GMT
VOLUME [/spiped]
# Sat, 07 Aug 2021 01:31:54 GMT
WORKDIR /spiped
# Sat, 07 Aug 2021 01:31:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 07 Aug 2021 01:32:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 01:32:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0ff902055236f70c4694c806877243e1dd52c513825a2a3ecc7eba8f5202acc8`  
		Last Modified: Fri, 06 Aug 2021 18:29:33 GMT  
		Size: 2.8 MB (2811152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e1daa083c0d4e8922acb4a3735a2446ec516ebedf8992b97d0d8ac09474f9e`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ab775043317669024edb01d89328f75341409396938066bd82d18bcfa0f1b6`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f9821113c32743f01e0620003d0630b6021c4148138f74add3efc51d82916a`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 221.2 KB (221239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2760cfc3e6b029ffb984aafe5b489eac1b215d0fe413a43cd00255dac46393`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b6d8de58c0e97f9000849b6c5be64af02ae4149134d50dedcb8e40e121b5e2`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 340.0 B  
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
$ docker pull spiped@sha256:3f7aee6424d8e855ebe6dddca85bc4e87b619aff2edd89bcbb74f516a64e1b24
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
$ docker pull spiped@sha256:699a597305fe7100c7693c271debbb205f614e3d0121cc56df4d15176f2c61cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4610169607c66b15865617305efd55c796fb1bb4d0b782c7dd7f3ec01f12f9a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 03:09:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 23 Jul 2021 03:09:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 03:09:33 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 23 Jul 2021 03:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 23 Jul 2021 03:10:30 GMT
VOLUME [/spiped]
# Fri, 23 Jul 2021 03:10:30 GMT
WORKDIR /spiped
# Fri, 23 Jul 2021 03:10:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 23 Jul 2021 03:10:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Jul 2021 03:10:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de916f7b97e5eb43a8edd2b6ee1ad63498619b50eb4cbfb017d71b95ff289caf`  
		Last Modified: Fri, 23 Jul 2021 03:11:38 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d4af5c0777c03753720afc23f1dd0b7cacab3c99d8954a8c8f57db7f2af33e`  
		Last Modified: Fri, 23 Jul 2021 03:11:38 GMT  
		Size: 1.8 MB (1759505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855cd38fb8bc28302f7e48641a16bb36c4f04eb022bb47f30151f3c2033f05de`  
		Last Modified: Fri, 23 Jul 2021 03:11:42 GMT  
		Size: 5.3 MB (5285901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796be87dfcfd639be2c0b1c65cd816cb684ab2b8422083c24745817fceaa49a2`  
		Last Modified: Fri, 23 Jul 2021 03:11:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e33f6a15f0addd124b890009c782cbe3a9181bd787565d37bc87cea0ef09bf`  
		Last Modified: Fri, 23 Jul 2021 03:11:38 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:20370abf15be60a98880c1b7557f40a4c2755aed4b2a27119d7979b785bc795d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39525135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f3494d6eae461220831621f3c69c3cf3f83c4a86ea58aa8cbad0b72fde83bbd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 02:13:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 23 Jul 2021 02:13:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:13:47 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 23 Jul 2021 02:17:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 23 Jul 2021 02:17:15 GMT
VOLUME [/spiped]
# Fri, 23 Jul 2021 02:17:20 GMT
WORKDIR /spiped
# Fri, 23 Jul 2021 02:17:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 23 Jul 2021 02:17:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Jul 2021 02:17:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79e2a440de83ae3592492eb9dd671bc9d11ced769aa02ea4af21ec4ec9361bc`  
		Last Modified: Fri, 23 Jul 2021 02:20:16 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cea156edf57e948965a4a5fc44b087c2535d880466c6b805fd0895a3d52d873`  
		Last Modified: Fri, 23 Jul 2021 02:20:17 GMT  
		Size: 2.2 MB (2225179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7301bf2714c9f1f9d2a9e50d20641ce37bafa4aeef3a74d6754e00cf00df33a`  
		Last Modified: Fri, 23 Jul 2021 02:20:18 GMT  
		Size: 6.7 MB (6744030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f949d63c4f754b5ad6ec1ff0f6a9f8bd05f76157aa184ad4296d6a03d04967df`  
		Last Modified: Fri, 23 Jul 2021 02:20:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10f2ba44cd479a0906c8865a991c102b39311bcd0ad5c461a282e6a40643f01`  
		Last Modified: Fri, 23 Jul 2021 02:20:16 GMT  
		Size: 343.0 B  
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
$ docker pull spiped@sha256:e7dbba32f20064755cf05c473ae6e9b44a3eea8a6cd5e81fdc51e22bc6028fd4
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
$ docker pull spiped@sha256:81959987e9809ba3bedbd6901a88e9fe28f2b16377bc8d3e43604661d48c2d15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3034576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d417cc665c58c81ae417555e8357d1f37bf78df7aaf23da4dcc13659df5a95a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:25:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 22:25:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 22:25:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 22:26:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 22:26:12 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 22:26:13 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 22:26:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 22:26:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 22:26:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9c880241f8602d0cc47e4fabf713180b354b6d9819786e78aaf3a9665b7767`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008bccb485a15a7ccb6581c8d02974f14fd68b58810d648f7295647a532772b0`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 7.3 KB (7279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7741dee13e8d6c91732585334d7cef9f489ff0ba3dda16074f7cf05e58ed528a`  
		Last Modified: Fri, 06 Aug 2021 22:26:33 GMT  
		Size: 212.6 KB (212550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0337b646a0031aa1e94edce7b03cdab87816253a6850b30bf5fcfe39128e09`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc226b22f034d312b242c20826de8afa099040078d13d904d45dfeb771850e6`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:5106236450e3abdcba7735635894ff0393e5f0ce938d3fab894ece612e116c92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2837884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07cdb6952199964783a11e1091cc96fa94684fd9e645edcea0376c4fef959217`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 23:52:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 23:52:52 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 23:52:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 23:53:27 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 23:53:27 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 23:53:28 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 23:53:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 23:53:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 23:53:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2adf0d4d8cc8b9e29d8414cae24c000412da47df5cb21a2a05ddf2e10dce570`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33562af158cbe4a36f2391938531bae4126685733de295b7ed766183da4b65ef`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 7.3 KB (7298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23d92f94fd24201f1627f9cdbd4e09c0eced2bcbb6ebf6edd1cd206d43e2989`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 202.5 KB (202496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e821b43798aa5a90978114728243266a0f589a4f572c8034852cb0d17ce7c803`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ba2a665cda34f66fc655e2d76ea1f17e791687438e3675a6ca88c09fa438d`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:4b39dd207a36df0ab651368a23dd5f7fb85cb40c73169a18ed6a650c9e1e9fc5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2634162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a80c87f5ffe5257a7577c370989dbed14396b7ee0a5768d7e330b488935c5205`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:50:46 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 19:50:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 19:50:52 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 19:51:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 19:51:30 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 19:51:31 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 19:51:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 19:51:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:51:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d7a90d848ed25f9597b7555466d565e3c10725a9f17b4863bb5543b964fbef`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56efc9f5e430a2d91ff87e40f30089c0015233688200b25c6c645b9c75917480`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7705d09d2948f05566c3ad4b7184193f719c33fb432e05f9e9d134e1850c51f2`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 195.8 KB (195768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576177e1db2fc775ca441543afa32e5f65ec818813bbb783b5cfea5edcb0da7d`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd82adbb730f7bc7d4c11d373678c8f08c809f2f46e9cd79ae1f11169ec1f8b`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:11f573b8237bb1841a7175c9c9b77f7b8c680623ab91182c3b15186ce6d0a684
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2924266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11d2305d4144c6a7caf39b8b6ca94a94d25dce28a8b4d51cbf4904172d0d3d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:20:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 07 Aug 2021 01:20:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 07 Aug 2021 01:20:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 07 Aug 2021 01:20:46 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 07 Aug 2021 01:20:47 GMT
VOLUME [/spiped]
# Sat, 07 Aug 2021 01:20:47 GMT
WORKDIR /spiped
# Sat, 07 Aug 2021 01:20:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 07 Aug 2021 01:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 01:20:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0faf3295f84c6343ed4bedec1bceca8f73e65a202fab2dde2578d5032f0264`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909cb3a09ec0e0c7512a5e0803fb90d9fa40a1331ebd44ac5923e377ef619c88`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 7.3 KB (7293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da73e2091b0f5e799ac0526b25f8ee65662172dccf092bfcebac9a4f451801e2`  
		Last Modified: Sat, 07 Aug 2021 01:21:19 GMT  
		Size: 204.6 KB (204623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d3f2992d2b842a28dfa27d50163a579400dcff25c9326252f55415706303af`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac232dfb34c3889ce2beb5d4442d4a3b927e0ece42f3ab8a81de9779d579cba`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:f99c513faad87e225c2e474c95f7ceace240bcfdc0f161e74943db703f489f36
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3054380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:355bc30b5b850a5b153236ee5157aa164f2754488c4565a7142fb520abe22f4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:38:26 GMT
ADD file:bafaec4a54d6cef99b5f3660d074a3d2251e4d4bd09df9ea65f33e9bffb7d88d in / 
# Fri, 06 Aug 2021 17:38:26 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 17:57:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 17:57:45 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 17:57:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 17:58:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 17:58:08 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 17:58:08 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 17:58:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 17:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 17:58:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:935703e1179e32e201e4a36d5664d58299dc8e7bcac197b70c295c0a59216db1`  
		Last Modified: Fri, 06 Aug 2021 17:39:15 GMT  
		Size: 2.8 MB (2821910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9f8235dc8f7a2cb2e106af5945d974007f182ef18717b1358dc418b51672e7`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c8e66016715cac7eea56fb6278759a154b998e9cc867cfd9e699f45749f938`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 7.3 KB (7288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b143265a7e8e4e62818a693cb546d0cdbedb96dac486cdfaa3326b27c5669`  
		Last Modified: Fri, 06 Aug 2021 17:58:43 GMT  
		Size: 223.4 KB (223442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac32f75f64f9f329d462d69b46dad0bde0e7c7356333e99089593e3e0359d85`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3d678fb9c378cbc3489d13a25fa17ca3d91d2319e6ffef53f6f84101025d21`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:fb4e68d177bc77f575c1a12ed21a941cb1ac2e423be4e1231ec7f327802e88a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3041425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8692281a7b48476e4611c785ef1f090697d8d28d64eca5cd85eabdf3842f44aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 18:28:28 GMT
ADD file:40f3b617d7ff269d92f0ffcf8aad561b5f2c0626ef519a7f584f1ba0182b3188 in / 
# Fri, 06 Aug 2021 18:28:35 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:30:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 07 Aug 2021 01:31:04 GMT
RUN apk add --no-cache libssl1.1
# Sat, 07 Aug 2021 01:31:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 07 Aug 2021 01:31:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 07 Aug 2021 01:31:47 GMT
VOLUME [/spiped]
# Sat, 07 Aug 2021 01:31:54 GMT
WORKDIR /spiped
# Sat, 07 Aug 2021 01:31:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 07 Aug 2021 01:32:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 01:32:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0ff902055236f70c4694c806877243e1dd52c513825a2a3ecc7eba8f5202acc8`  
		Last Modified: Fri, 06 Aug 2021 18:29:33 GMT  
		Size: 2.8 MB (2811152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e1daa083c0d4e8922acb4a3735a2446ec516ebedf8992b97d0d8ac09474f9e`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ab775043317669024edb01d89328f75341409396938066bd82d18bcfa0f1b6`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f9821113c32743f01e0620003d0630b6021c4148138f74add3efc51d82916a`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 221.2 KB (221239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2760cfc3e6b029ffb984aafe5b489eac1b215d0fe413a43cd00255dac46393`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b6d8de58c0e97f9000849b6c5be64af02ae4149134d50dedcb8e40e121b5e2`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 340.0 B  
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
$ docker pull spiped@sha256:e7dbba32f20064755cf05c473ae6e9b44a3eea8a6cd5e81fdc51e22bc6028fd4
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
$ docker pull spiped@sha256:81959987e9809ba3bedbd6901a88e9fe28f2b16377bc8d3e43604661d48c2d15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3034576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d417cc665c58c81ae417555e8357d1f37bf78df7aaf23da4dcc13659df5a95a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:25:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 22:25:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 22:25:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 22:26:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 22:26:12 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 22:26:13 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 22:26:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 22:26:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 22:26:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9c880241f8602d0cc47e4fabf713180b354b6d9819786e78aaf3a9665b7767`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008bccb485a15a7ccb6581c8d02974f14fd68b58810d648f7295647a532772b0`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 7.3 KB (7279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7741dee13e8d6c91732585334d7cef9f489ff0ba3dda16074f7cf05e58ed528a`  
		Last Modified: Fri, 06 Aug 2021 22:26:33 GMT  
		Size: 212.6 KB (212550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0337b646a0031aa1e94edce7b03cdab87816253a6850b30bf5fcfe39128e09`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc226b22f034d312b242c20826de8afa099040078d13d904d45dfeb771850e6`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:5106236450e3abdcba7735635894ff0393e5f0ce938d3fab894ece612e116c92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2837884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07cdb6952199964783a11e1091cc96fa94684fd9e645edcea0376c4fef959217`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 23:52:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 23:52:52 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 23:52:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 23:53:27 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 23:53:27 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 23:53:28 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 23:53:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 23:53:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 23:53:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2adf0d4d8cc8b9e29d8414cae24c000412da47df5cb21a2a05ddf2e10dce570`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33562af158cbe4a36f2391938531bae4126685733de295b7ed766183da4b65ef`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 7.3 KB (7298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23d92f94fd24201f1627f9cdbd4e09c0eced2bcbb6ebf6edd1cd206d43e2989`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 202.5 KB (202496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e821b43798aa5a90978114728243266a0f589a4f572c8034852cb0d17ce7c803`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ba2a665cda34f66fc655e2d76ea1f17e791687438e3675a6ca88c09fa438d`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:4b39dd207a36df0ab651368a23dd5f7fb85cb40c73169a18ed6a650c9e1e9fc5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2634162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a80c87f5ffe5257a7577c370989dbed14396b7ee0a5768d7e330b488935c5205`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:50:46 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 19:50:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 19:50:52 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 19:51:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 19:51:30 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 19:51:31 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 19:51:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 19:51:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:51:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d7a90d848ed25f9597b7555466d565e3c10725a9f17b4863bb5543b964fbef`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56efc9f5e430a2d91ff87e40f30089c0015233688200b25c6c645b9c75917480`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7705d09d2948f05566c3ad4b7184193f719c33fb432e05f9e9d134e1850c51f2`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 195.8 KB (195768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576177e1db2fc775ca441543afa32e5f65ec818813bbb783b5cfea5edcb0da7d`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd82adbb730f7bc7d4c11d373678c8f08c809f2f46e9cd79ae1f11169ec1f8b`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:11f573b8237bb1841a7175c9c9b77f7b8c680623ab91182c3b15186ce6d0a684
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2924266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11d2305d4144c6a7caf39b8b6ca94a94d25dce28a8b4d51cbf4904172d0d3d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:20:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 07 Aug 2021 01:20:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 07 Aug 2021 01:20:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 07 Aug 2021 01:20:46 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 07 Aug 2021 01:20:47 GMT
VOLUME [/spiped]
# Sat, 07 Aug 2021 01:20:47 GMT
WORKDIR /spiped
# Sat, 07 Aug 2021 01:20:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 07 Aug 2021 01:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 01:20:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0faf3295f84c6343ed4bedec1bceca8f73e65a202fab2dde2578d5032f0264`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909cb3a09ec0e0c7512a5e0803fb90d9fa40a1331ebd44ac5923e377ef619c88`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 7.3 KB (7293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da73e2091b0f5e799ac0526b25f8ee65662172dccf092bfcebac9a4f451801e2`  
		Last Modified: Sat, 07 Aug 2021 01:21:19 GMT  
		Size: 204.6 KB (204623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d3f2992d2b842a28dfa27d50163a579400dcff25c9326252f55415706303af`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac232dfb34c3889ce2beb5d4442d4a3b927e0ece42f3ab8a81de9779d579cba`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:f99c513faad87e225c2e474c95f7ceace240bcfdc0f161e74943db703f489f36
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3054380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:355bc30b5b850a5b153236ee5157aa164f2754488c4565a7142fb520abe22f4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:38:26 GMT
ADD file:bafaec4a54d6cef99b5f3660d074a3d2251e4d4bd09df9ea65f33e9bffb7d88d in / 
# Fri, 06 Aug 2021 17:38:26 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 17:57:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 17:57:45 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 17:57:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 17:58:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 17:58:08 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 17:58:08 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 17:58:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 17:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 17:58:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:935703e1179e32e201e4a36d5664d58299dc8e7bcac197b70c295c0a59216db1`  
		Last Modified: Fri, 06 Aug 2021 17:39:15 GMT  
		Size: 2.8 MB (2821910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9f8235dc8f7a2cb2e106af5945d974007f182ef18717b1358dc418b51672e7`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c8e66016715cac7eea56fb6278759a154b998e9cc867cfd9e699f45749f938`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 7.3 KB (7288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b143265a7e8e4e62818a693cb546d0cdbedb96dac486cdfaa3326b27c5669`  
		Last Modified: Fri, 06 Aug 2021 17:58:43 GMT  
		Size: 223.4 KB (223442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac32f75f64f9f329d462d69b46dad0bde0e7c7356333e99089593e3e0359d85`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3d678fb9c378cbc3489d13a25fa17ca3d91d2319e6ffef53f6f84101025d21`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:fb4e68d177bc77f575c1a12ed21a941cb1ac2e423be4e1231ec7f327802e88a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3041425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8692281a7b48476e4611c785ef1f090697d8d28d64eca5cd85eabdf3842f44aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 18:28:28 GMT
ADD file:40f3b617d7ff269d92f0ffcf8aad561b5f2c0626ef519a7f584f1ba0182b3188 in / 
# Fri, 06 Aug 2021 18:28:35 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:30:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 07 Aug 2021 01:31:04 GMT
RUN apk add --no-cache libssl1.1
# Sat, 07 Aug 2021 01:31:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 07 Aug 2021 01:31:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 07 Aug 2021 01:31:47 GMT
VOLUME [/spiped]
# Sat, 07 Aug 2021 01:31:54 GMT
WORKDIR /spiped
# Sat, 07 Aug 2021 01:31:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 07 Aug 2021 01:32:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 01:32:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0ff902055236f70c4694c806877243e1dd52c513825a2a3ecc7eba8f5202acc8`  
		Last Modified: Fri, 06 Aug 2021 18:29:33 GMT  
		Size: 2.8 MB (2811152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e1daa083c0d4e8922acb4a3735a2446ec516ebedf8992b97d0d8ac09474f9e`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ab775043317669024edb01d89328f75341409396938066bd82d18bcfa0f1b6`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f9821113c32743f01e0620003d0630b6021c4148138f74add3efc51d82916a`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 221.2 KB (221239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2760cfc3e6b029ffb984aafe5b489eac1b215d0fe413a43cd00255dac46393`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b6d8de58c0e97f9000849b6c5be64af02ae4149134d50dedcb8e40e121b5e2`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 340.0 B  
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
$ docker pull spiped@sha256:3f7aee6424d8e855ebe6dddca85bc4e87b619aff2edd89bcbb74f516a64e1b24
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
$ docker pull spiped@sha256:699a597305fe7100c7693c271debbb205f614e3d0121cc56df4d15176f2c61cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4610169607c66b15865617305efd55c796fb1bb4d0b782c7dd7f3ec01f12f9a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 03:09:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 23 Jul 2021 03:09:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 03:09:33 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 23 Jul 2021 03:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 23 Jul 2021 03:10:30 GMT
VOLUME [/spiped]
# Fri, 23 Jul 2021 03:10:30 GMT
WORKDIR /spiped
# Fri, 23 Jul 2021 03:10:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 23 Jul 2021 03:10:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Jul 2021 03:10:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de916f7b97e5eb43a8edd2b6ee1ad63498619b50eb4cbfb017d71b95ff289caf`  
		Last Modified: Fri, 23 Jul 2021 03:11:38 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d4af5c0777c03753720afc23f1dd0b7cacab3c99d8954a8c8f57db7f2af33e`  
		Last Modified: Fri, 23 Jul 2021 03:11:38 GMT  
		Size: 1.8 MB (1759505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855cd38fb8bc28302f7e48641a16bb36c4f04eb022bb47f30151f3c2033f05de`  
		Last Modified: Fri, 23 Jul 2021 03:11:42 GMT  
		Size: 5.3 MB (5285901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796be87dfcfd639be2c0b1c65cd816cb684ab2b8422083c24745817fceaa49a2`  
		Last Modified: Fri, 23 Jul 2021 03:11:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e33f6a15f0addd124b890009c782cbe3a9181bd787565d37bc87cea0ef09bf`  
		Last Modified: Fri, 23 Jul 2021 03:11:38 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:20370abf15be60a98880c1b7557f40a4c2755aed4b2a27119d7979b785bc795d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39525135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f3494d6eae461220831621f3c69c3cf3f83c4a86ea58aa8cbad0b72fde83bbd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 02:13:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 23 Jul 2021 02:13:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:13:47 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 23 Jul 2021 02:17:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 23 Jul 2021 02:17:15 GMT
VOLUME [/spiped]
# Fri, 23 Jul 2021 02:17:20 GMT
WORKDIR /spiped
# Fri, 23 Jul 2021 02:17:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 23 Jul 2021 02:17:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Jul 2021 02:17:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79e2a440de83ae3592492eb9dd671bc9d11ced769aa02ea4af21ec4ec9361bc`  
		Last Modified: Fri, 23 Jul 2021 02:20:16 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cea156edf57e948965a4a5fc44b087c2535d880466c6b805fd0895a3d52d873`  
		Last Modified: Fri, 23 Jul 2021 02:20:17 GMT  
		Size: 2.2 MB (2225179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7301bf2714c9f1f9d2a9e50d20641ce37bafa4aeef3a74d6754e00cf00df33a`  
		Last Modified: Fri, 23 Jul 2021 02:20:18 GMT  
		Size: 6.7 MB (6744030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f949d63c4f754b5ad6ec1ff0f6a9f8bd05f76157aa184ad4296d6a03d04967df`  
		Last Modified: Fri, 23 Jul 2021 02:20:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10f2ba44cd479a0906c8865a991c102b39311bcd0ad5c461a282e6a40643f01`  
		Last Modified: Fri, 23 Jul 2021 02:20:16 GMT  
		Size: 343.0 B  
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
