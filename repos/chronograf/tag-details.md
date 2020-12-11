<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `chronograf`

-	[`chronograf:1.6`](#chronograf16)
-	[`chronograf:1.6.2`](#chronograf162)
-	[`chronograf:1.6.2-alpine`](#chronograf162-alpine)
-	[`chronograf:1.6-alpine`](#chronograf16-alpine)
-	[`chronograf:1.7`](#chronograf17)
-	[`chronograf:1.7.17`](#chronograf1717)
-	[`chronograf:1.7.17-alpine`](#chronograf1717-alpine)
-	[`chronograf:1.7-alpine`](#chronograf17-alpine)
-	[`chronograf:1.8`](#chronograf18)
-	[`chronograf:1.8.8`](#chronograf188)
-	[`chronograf:1.8.8-alpine`](#chronograf188-alpine)
-	[`chronograf:1.8-alpine`](#chronograf18-alpine)
-	[`chronograf:alpine`](#chronografalpine)
-	[`chronograf:latest`](#chronograflatest)

## `chronograf:1.6`

```console
$ docker pull chronograf@sha256:f677cba47202c2be3c32f5d6275d6780e1a58fddd87637b0b1679845ce282bc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6` - linux; amd64

```console
$ docker pull chronograf@sha256:0c63a160dbccba212dc543e64158fab9a77b0a01f49a4c0bc0b0a00c7fef480d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49337463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2c9efc36b1b97e5bcacf38531931278106d9b34ce92f1e32f47c696760fa00c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:58 GMT
ADD file:f03e68a10b84e2342cfffbb8cdec1117c7f5e5d0dd004072e84efb62cfdf157c in / 
# Fri, 11 Dec 2020 02:08:58 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:51:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 02:51:29 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 11 Dec 2020 02:51:36 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 02:51:36 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 02:51:37 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 02:51:37 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 02:51:37 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 02:51:37 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 02:51:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 02:51:38 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e50c3c9ef5a201a24959788dcbc7ebf88d95c63e132a4d7396ce541127afd88e`  
		Last Modified: Fri, 11 Dec 2020 02:15:43 GMT  
		Size: 22.5 MB (22527860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121258f8a02a8e6785249c0e846752cef626dea7d69f721857d361346ce8c23d`  
		Last Modified: Fri, 11 Dec 2020 02:53:44 GMT  
		Size: 6.7 MB (6742130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382b5064a70659c8e793aeef613f2ea731cec998c7d9e4c707637c41a89c8fed`  
		Last Modified: Fri, 11 Dec 2020 02:53:47 GMT  
		Size: 20.0 MB (20043066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd0c76f546b92774dcb8835644ff2d7f0abe491f6fc6ac7162fbe76df76932c`  
		Last Modified: Fri, 11 Dec 2020 02:53:42 GMT  
		Size: 12.3 KB (12254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c0fceceb07b83e3ea939b7487539c31ecdcc20033330062996d01d58661ffa`  
		Last Modified: Fri, 11 Dec 2020 02:53:42 GMT  
		Size: 11.9 KB (11913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb2842f1e22040f350588f35db11e621a61c60246e008670652a12ea509fd43`  
		Last Modified: Fri, 11 Dec 2020 02:53:42 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:25d8e09268de99ca40364c857fed099eaf43de4055875e547fd5f3080abde562
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43918658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e318ffd9531bf0ba8f3001ff576506b7c8769ad19481a0c86c99a71711e2f8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:28:33 GMT
ADD file:a5ae44ff42f691e7afa1f743d1f05f6fd72d9c1737ae20b97977f9de76811260 in / 
# Fri, 11 Dec 2020 02:28:34 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 20:43:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 20:43:39 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 11 Dec 2020 20:43:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 20:43:54 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 20:43:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 20:43:55 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 20:43:56 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 20:43:57 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 20:43:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 20:43:58 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:3844aeda5f39338d766015a56d78b18d6d4d4b95b0e6b41f8d37105ee5b91a80`  
		Last Modified: Fri, 11 Dec 2020 02:37:12 GMT  
		Size: 19.3 MB (19313560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01f6f4ab74e3df5409e7c7b9fbf06f93ee005364bdfce72d9264eea24777ba9`  
		Last Modified: Fri, 11 Dec 2020 20:45:43 GMT  
		Size: 5.8 MB (5764540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218ada51ead5103b9eaeb308f58019e82eea9f1cef35677e443fd8ab78ce0a2b`  
		Last Modified: Fri, 11 Dec 2020 20:45:48 GMT  
		Size: 18.8 MB (18816147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3e03b88a119443fb24a1ebb8b3896df803101a9fa9ac46372bd0cc5a7e09a9`  
		Last Modified: Fri, 11 Dec 2020 20:45:42 GMT  
		Size: 12.3 KB (12256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69595d255f5bdff1636a1e39b5de4edb0bb8cae16b65539982c85d6f14d3f0b4`  
		Last Modified: Fri, 11 Dec 2020 20:45:44 GMT  
		Size: 11.9 KB (11915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35a897edf97522141cb5ba6c49078b9e74a3973d60eb0b1b360f8174c64cd88`  
		Last Modified: Fri, 11 Dec 2020 20:45:43 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:14ada3c1e90b245a696c78cece45794bd1552f21a9f2b057e39abaa411d40036
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45398713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ab8e3d695a38f2bb83dbe697a16d924b6b22a9661aa2de7ac644ded523dc801`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:48:42 GMT
ADD file:2efe3cccad076777e72be01a4380984d961a457c67dad3041063307ce1519c4d in / 
# Fri, 11 Dec 2020 02:48:44 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 19:13:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 19:13:28 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 11 Dec 2020 19:13:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 19:13:41 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 19:13:42 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 19:13:42 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 19:13:43 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 19:13:44 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 19:13:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 19:13:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:15531941ccc12369b70088bb4e7b58263a2363c37d600f0ec7f4b7532efe6685`  
		Last Modified: Fri, 11 Dec 2020 02:56:00 GMT  
		Size: 20.4 MB (20387882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc6eef58f92eea9ce0ce34bd98afa24ba6e62ac9d993abbc6e19f386740a1cf`  
		Last Modified: Fri, 11 Dec 2020 19:15:44 GMT  
		Size: 6.0 MB (6028036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bac3f89be18b3a427d48cad79ddd6b69f6887f7eaf7e8128c9ad20a6eb6addd`  
		Last Modified: Fri, 11 Dec 2020 19:15:47 GMT  
		Size: 19.0 MB (18958394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00862f75c1e8b67eb484d473975df1bbbc7c51a78f5432c322bcb5e5f3c50f10`  
		Last Modified: Fri, 11 Dec 2020 19:15:43 GMT  
		Size: 12.3 KB (12252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc34cf61ecd11bd541c2e8ad659ad34e2330a2e8441b991a3fbb338ae262192c`  
		Last Modified: Fri, 11 Dec 2020 19:15:43 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cc74d146d1500252ed7513f794cb00b0a95e3dba618f70bc7de3eeead6a7c6`  
		Last Modified: Fri, 11 Dec 2020 19:15:43 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2`

```console
$ docker pull chronograf@sha256:f677cba47202c2be3c32f5d6275d6780e1a58fddd87637b0b1679845ce282bc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6.2` - linux; amd64

```console
$ docker pull chronograf@sha256:0c63a160dbccba212dc543e64158fab9a77b0a01f49a4c0bc0b0a00c7fef480d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49337463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2c9efc36b1b97e5bcacf38531931278106d9b34ce92f1e32f47c696760fa00c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:58 GMT
ADD file:f03e68a10b84e2342cfffbb8cdec1117c7f5e5d0dd004072e84efb62cfdf157c in / 
# Fri, 11 Dec 2020 02:08:58 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:51:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 02:51:29 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 11 Dec 2020 02:51:36 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 02:51:36 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 02:51:37 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 02:51:37 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 02:51:37 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 02:51:37 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 02:51:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 02:51:38 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e50c3c9ef5a201a24959788dcbc7ebf88d95c63e132a4d7396ce541127afd88e`  
		Last Modified: Fri, 11 Dec 2020 02:15:43 GMT  
		Size: 22.5 MB (22527860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121258f8a02a8e6785249c0e846752cef626dea7d69f721857d361346ce8c23d`  
		Last Modified: Fri, 11 Dec 2020 02:53:44 GMT  
		Size: 6.7 MB (6742130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382b5064a70659c8e793aeef613f2ea731cec998c7d9e4c707637c41a89c8fed`  
		Last Modified: Fri, 11 Dec 2020 02:53:47 GMT  
		Size: 20.0 MB (20043066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd0c76f546b92774dcb8835644ff2d7f0abe491f6fc6ac7162fbe76df76932c`  
		Last Modified: Fri, 11 Dec 2020 02:53:42 GMT  
		Size: 12.3 KB (12254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c0fceceb07b83e3ea939b7487539c31ecdcc20033330062996d01d58661ffa`  
		Last Modified: Fri, 11 Dec 2020 02:53:42 GMT  
		Size: 11.9 KB (11913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb2842f1e22040f350588f35db11e621a61c60246e008670652a12ea509fd43`  
		Last Modified: Fri, 11 Dec 2020 02:53:42 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:25d8e09268de99ca40364c857fed099eaf43de4055875e547fd5f3080abde562
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43918658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e318ffd9531bf0ba8f3001ff576506b7c8769ad19481a0c86c99a71711e2f8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:28:33 GMT
ADD file:a5ae44ff42f691e7afa1f743d1f05f6fd72d9c1737ae20b97977f9de76811260 in / 
# Fri, 11 Dec 2020 02:28:34 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 20:43:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 20:43:39 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 11 Dec 2020 20:43:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 20:43:54 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 20:43:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 20:43:55 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 20:43:56 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 20:43:57 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 20:43:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 20:43:58 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:3844aeda5f39338d766015a56d78b18d6d4d4b95b0e6b41f8d37105ee5b91a80`  
		Last Modified: Fri, 11 Dec 2020 02:37:12 GMT  
		Size: 19.3 MB (19313560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01f6f4ab74e3df5409e7c7b9fbf06f93ee005364bdfce72d9264eea24777ba9`  
		Last Modified: Fri, 11 Dec 2020 20:45:43 GMT  
		Size: 5.8 MB (5764540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218ada51ead5103b9eaeb308f58019e82eea9f1cef35677e443fd8ab78ce0a2b`  
		Last Modified: Fri, 11 Dec 2020 20:45:48 GMT  
		Size: 18.8 MB (18816147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3e03b88a119443fb24a1ebb8b3896df803101a9fa9ac46372bd0cc5a7e09a9`  
		Last Modified: Fri, 11 Dec 2020 20:45:42 GMT  
		Size: 12.3 KB (12256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69595d255f5bdff1636a1e39b5de4edb0bb8cae16b65539982c85d6f14d3f0b4`  
		Last Modified: Fri, 11 Dec 2020 20:45:44 GMT  
		Size: 11.9 KB (11915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35a897edf97522141cb5ba6c49078b9e74a3973d60eb0b1b360f8174c64cd88`  
		Last Modified: Fri, 11 Dec 2020 20:45:43 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:14ada3c1e90b245a696c78cece45794bd1552f21a9f2b057e39abaa411d40036
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45398713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ab8e3d695a38f2bb83dbe697a16d924b6b22a9661aa2de7ac644ded523dc801`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:48:42 GMT
ADD file:2efe3cccad076777e72be01a4380984d961a457c67dad3041063307ce1519c4d in / 
# Fri, 11 Dec 2020 02:48:44 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 19:13:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 19:13:28 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 11 Dec 2020 19:13:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 19:13:41 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 19:13:42 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 19:13:42 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 19:13:43 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 19:13:44 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 19:13:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 19:13:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:15531941ccc12369b70088bb4e7b58263a2363c37d600f0ec7f4b7532efe6685`  
		Last Modified: Fri, 11 Dec 2020 02:56:00 GMT  
		Size: 20.4 MB (20387882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc6eef58f92eea9ce0ce34bd98afa24ba6e62ac9d993abbc6e19f386740a1cf`  
		Last Modified: Fri, 11 Dec 2020 19:15:44 GMT  
		Size: 6.0 MB (6028036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bac3f89be18b3a427d48cad79ddd6b69f6887f7eaf7e8128c9ad20a6eb6addd`  
		Last Modified: Fri, 11 Dec 2020 19:15:47 GMT  
		Size: 19.0 MB (18958394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00862f75c1e8b67eb484d473975df1bbbc7c51a78f5432c322bcb5e5f3c50f10`  
		Last Modified: Fri, 11 Dec 2020 19:15:43 GMT  
		Size: 12.3 KB (12252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc34cf61ecd11bd541c2e8ad659ad34e2330a2e8441b991a3fbb338ae262192c`  
		Last Modified: Fri, 11 Dec 2020 19:15:43 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cc74d146d1500252ed7513f794cb00b0a95e3dba618f70bc7de3eeead6a7c6`  
		Last Modified: Fri, 11 Dec 2020 19:15:43 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2-alpine`

```console
$ docker pull chronograf@sha256:0096f188cb3a866e0872a11bc1ef13b1bc2941804c3bf47fc5899330cbf225b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.6.2-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:687ab05e612056f825d80fda6c5d7876eb4f19d40562ea1d3b63435c110b2057
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14839075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bac83c347dc8bb99ed7695c513333ac81f8b21c339ea1dbce25b17f790cb8e5a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:51:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:51:47 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 11 Dec 2020 02:51:47 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 11 Dec 2020 02:51:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 11 Dec 2020 02:51:50 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 02:51:50 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 02:51:50 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 02:51:51 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 02:51:51 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 11 Dec 2020 02:51:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 02:51:51 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9624996f533f5dfa6054365968149298c1183a1202c16061de0fc5093ad633f`  
		Last Modified: Fri, 11 Dec 2020 02:53:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714c102d667de25287e212434b418f887c3297d809db411374920f3d8b36201`  
		Last Modified: Fri, 11 Dec 2020 02:53:53 GMT  
		Size: 280.8 KB (280809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639b6ad3087a1b390bf386593b19eef656cd5017bf89fc28c9fabb19fa7e197e`  
		Last Modified: Fri, 11 Dec 2020 02:53:57 GMT  
		Size: 11.7 MB (11736791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25d3d11a6d3c0aae1277bc16c48a7232d1880ebb396c81b1529fb628691229c`  
		Last Modified: Fri, 11 Dec 2020 02:53:53 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b350b00e73e9cddede7cddd7a3947a2ea075e0d0aeb4ffb382509f9f721345f`  
		Last Modified: Fri, 11 Dec 2020 02:53:53 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77665e8af65cf8362afbb2c515c9d9019de43b275288baf5342e3226ea2d3921`  
		Last Modified: Fri, 11 Dec 2020 02:53:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6-alpine`

```console
$ docker pull chronograf@sha256:0096f188cb3a866e0872a11bc1ef13b1bc2941804c3bf47fc5899330cbf225b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.6-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:687ab05e612056f825d80fda6c5d7876eb4f19d40562ea1d3b63435c110b2057
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14839075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bac83c347dc8bb99ed7695c513333ac81f8b21c339ea1dbce25b17f790cb8e5a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:51:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:51:47 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 11 Dec 2020 02:51:47 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 11 Dec 2020 02:51:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 11 Dec 2020 02:51:50 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 02:51:50 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 02:51:50 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 02:51:51 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 02:51:51 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 11 Dec 2020 02:51:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 02:51:51 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9624996f533f5dfa6054365968149298c1183a1202c16061de0fc5093ad633f`  
		Last Modified: Fri, 11 Dec 2020 02:53:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714c102d667de25287e212434b418f887c3297d809db411374920f3d8b36201`  
		Last Modified: Fri, 11 Dec 2020 02:53:53 GMT  
		Size: 280.8 KB (280809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639b6ad3087a1b390bf386593b19eef656cd5017bf89fc28c9fabb19fa7e197e`  
		Last Modified: Fri, 11 Dec 2020 02:53:57 GMT  
		Size: 11.7 MB (11736791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25d3d11a6d3c0aae1277bc16c48a7232d1880ebb396c81b1529fb628691229c`  
		Last Modified: Fri, 11 Dec 2020 02:53:53 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b350b00e73e9cddede7cddd7a3947a2ea075e0d0aeb4ffb382509f9f721345f`  
		Last Modified: Fri, 11 Dec 2020 02:53:53 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77665e8af65cf8362afbb2c515c9d9019de43b275288baf5342e3226ea2d3921`  
		Last Modified: Fri, 11 Dec 2020 02:53:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7`

```console
$ docker pull chronograf@sha256:1f5556c54843eb07a696b591f85a6efe54ae8b27d59705f69cca61313f660641
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:c40e706a351a523fd64d2f784d1532a720cb515c76386ffc0051cd4898f237c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65365622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4edd59afe9a2bf5aa3b6cfb20cf4409a2d427177c780a4ed1aedc56cd8e56886`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:58 GMT
ADD file:f03e68a10b84e2342cfffbb8cdec1117c7f5e5d0dd004072e84efb62cfdf157c in / 
# Fri, 11 Dec 2020 02:08:58 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:52:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 02:52:04 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 11 Dec 2020 02:52:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 02:52:23 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 02:52:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 02:52:24 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 02:52:24 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 02:52:25 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 02:52:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 02:52:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e50c3c9ef5a201a24959788dcbc7ebf88d95c63e132a4d7396ce541127afd88e`  
		Last Modified: Fri, 11 Dec 2020 02:15:43 GMT  
		Size: 22.5 MB (22527860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b799f46775b8d30d301c1d88e0967c686e3002c590f8b63aa97a93d4e721577`  
		Last Modified: Fri, 11 Dec 2020 02:54:03 GMT  
		Size: 4.5 MB (4504642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ad401f2bb5c1c3dd9a2e985e21f602eb46925b55d4986887a559ccb45b9596`  
		Last Modified: Fri, 11 Dec 2020 02:54:11 GMT  
		Size: 38.3 MB (38308725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d62c20eeac3bd624d216fb91525469f1d64a874873ebd8ea40a8973c765baa`  
		Last Modified: Fri, 11 Dec 2020 02:54:03 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40db34109409a2719c7913fc5bac9e2889cb08a6620e4b14b38851192737aea5`  
		Last Modified: Fri, 11 Dec 2020 02:54:03 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e009bd9c6bee1445c4d2a67a0a01d2143e2e9434648d6c09e4003a8be0f2a11`  
		Last Modified: Fri, 11 Dec 2020 02:54:03 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:88f41dae1036e9f696f7a84cb004fa4ab361309ba55ba931dcc16bc7be70bdb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58969298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:382159da1acd0ab5e63c99936fd1393994048cbcee1851b2012ec946393375c0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:28:33 GMT
ADD file:a5ae44ff42f691e7afa1f743d1f05f6fd72d9c1737ae20b97977f9de76811260 in / 
# Fri, 11 Dec 2020 02:28:34 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 20:44:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 20:44:25 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 11 Dec 2020 20:44:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 20:44:46 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 20:44:47 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 20:44:48 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 20:44:48 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 20:44:49 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 20:44:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 20:44:51 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:3844aeda5f39338d766015a56d78b18d6d4d4b95b0e6b41f8d37105ee5b91a80`  
		Last Modified: Fri, 11 Dec 2020 02:37:12 GMT  
		Size: 19.3 MB (19313560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad418c5c5d3d52f029078c4eef5a00c392a2e9fe1c8d25f85481887fc848dbaf`  
		Last Modified: Fri, 11 Dec 2020 20:45:56 GMT  
		Size: 3.9 MB (3879432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408951802b02830b9a17f838db8f5a879b4d3c591f73a649e443775138b754ae`  
		Last Modified: Fri, 11 Dec 2020 20:46:05 GMT  
		Size: 35.8 MB (35751902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1acd70068162c8b6c7cb5d9c417da40fe0cfdd6753c063b138398cd1613221`  
		Last Modified: Fri, 11 Dec 2020 20:45:55 GMT  
		Size: 12.3 KB (12252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0d14d85ff0b40805a0155ebd3f8c0ed341bf588ebb91ae4dd22dfbc29ad8b6`  
		Last Modified: Fri, 11 Dec 2020 20:45:55 GMT  
		Size: 11.9 KB (11912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9ab1e75a9565c282e534694fe6b77c07b04e7d522482fb4b67ab724cbeb8cd`  
		Last Modified: Fri, 11 Dec 2020 20:45:57 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:3225915274bb6bf7f7dc7147d91fe7e959fe1a13ed065318270a6464cde72748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60456164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1977ebe4de743638890b7558f49d76a53f8ab57cb5d08f4e281098c8c10f8d37`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:48:42 GMT
ADD file:2efe3cccad076777e72be01a4380984d961a457c67dad3041063307ce1519c4d in / 
# Fri, 11 Dec 2020 02:48:44 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 19:14:20 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 19:14:22 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 11 Dec 2020 19:14:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 19:14:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 19:14:44 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 19:14:45 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 19:14:45 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 19:14:46 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 19:14:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 19:14:48 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:15531941ccc12369b70088bb4e7b58263a2363c37d600f0ec7f4b7532efe6685`  
		Last Modified: Fri, 11 Dec 2020 02:56:00 GMT  
		Size: 20.4 MB (20387882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7517de3bd6340ffc9245806134aad5e20933580bef5822a2e01b197a64dcd494`  
		Last Modified: Fri, 11 Dec 2020 19:15:58 GMT  
		Size: 4.1 MB (4082308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91c602536e96ff018a4443977fd6745cda94ee6455d50b555347c9a1f80f711`  
		Last Modified: Fri, 11 Dec 2020 19:16:05 GMT  
		Size: 36.0 MB (35961573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82951a98c1cb148cc4363e352820b61243fab1b0961cd1575364b75428dd6989`  
		Last Modified: Fri, 11 Dec 2020 19:15:57 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8225678c4b908a14dbb7cb9b025d4deb144f7c2e81178a26424356c1adea8236`  
		Last Modified: Fri, 11 Dec 2020 19:15:56 GMT  
		Size: 11.9 KB (11912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ad1b824158250f33ec33bba41dd485c3075672f537070e2d780cd6a1d85c1e`  
		Last Modified: Fri, 11 Dec 2020 19:15:56 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17`

```console
$ docker pull chronograf@sha256:1f5556c54843eb07a696b591f85a6efe54ae8b27d59705f69cca61313f660641
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:c40e706a351a523fd64d2f784d1532a720cb515c76386ffc0051cd4898f237c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65365622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4edd59afe9a2bf5aa3b6cfb20cf4409a2d427177c780a4ed1aedc56cd8e56886`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:58 GMT
ADD file:f03e68a10b84e2342cfffbb8cdec1117c7f5e5d0dd004072e84efb62cfdf157c in / 
# Fri, 11 Dec 2020 02:08:58 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:52:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 02:52:04 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 11 Dec 2020 02:52:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 02:52:23 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 02:52:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 02:52:24 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 02:52:24 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 02:52:25 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 02:52:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 02:52:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e50c3c9ef5a201a24959788dcbc7ebf88d95c63e132a4d7396ce541127afd88e`  
		Last Modified: Fri, 11 Dec 2020 02:15:43 GMT  
		Size: 22.5 MB (22527860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b799f46775b8d30d301c1d88e0967c686e3002c590f8b63aa97a93d4e721577`  
		Last Modified: Fri, 11 Dec 2020 02:54:03 GMT  
		Size: 4.5 MB (4504642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ad401f2bb5c1c3dd9a2e985e21f602eb46925b55d4986887a559ccb45b9596`  
		Last Modified: Fri, 11 Dec 2020 02:54:11 GMT  
		Size: 38.3 MB (38308725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d62c20eeac3bd624d216fb91525469f1d64a874873ebd8ea40a8973c765baa`  
		Last Modified: Fri, 11 Dec 2020 02:54:03 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40db34109409a2719c7913fc5bac9e2889cb08a6620e4b14b38851192737aea5`  
		Last Modified: Fri, 11 Dec 2020 02:54:03 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e009bd9c6bee1445c4d2a67a0a01d2143e2e9434648d6c09e4003a8be0f2a11`  
		Last Modified: Fri, 11 Dec 2020 02:54:03 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:88f41dae1036e9f696f7a84cb004fa4ab361309ba55ba931dcc16bc7be70bdb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58969298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:382159da1acd0ab5e63c99936fd1393994048cbcee1851b2012ec946393375c0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:28:33 GMT
ADD file:a5ae44ff42f691e7afa1f743d1f05f6fd72d9c1737ae20b97977f9de76811260 in / 
# Fri, 11 Dec 2020 02:28:34 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 20:44:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 20:44:25 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 11 Dec 2020 20:44:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 20:44:46 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 20:44:47 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 20:44:48 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 20:44:48 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 20:44:49 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 20:44:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 20:44:51 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:3844aeda5f39338d766015a56d78b18d6d4d4b95b0e6b41f8d37105ee5b91a80`  
		Last Modified: Fri, 11 Dec 2020 02:37:12 GMT  
		Size: 19.3 MB (19313560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad418c5c5d3d52f029078c4eef5a00c392a2e9fe1c8d25f85481887fc848dbaf`  
		Last Modified: Fri, 11 Dec 2020 20:45:56 GMT  
		Size: 3.9 MB (3879432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408951802b02830b9a17f838db8f5a879b4d3c591f73a649e443775138b754ae`  
		Last Modified: Fri, 11 Dec 2020 20:46:05 GMT  
		Size: 35.8 MB (35751902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1acd70068162c8b6c7cb5d9c417da40fe0cfdd6753c063b138398cd1613221`  
		Last Modified: Fri, 11 Dec 2020 20:45:55 GMT  
		Size: 12.3 KB (12252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0d14d85ff0b40805a0155ebd3f8c0ed341bf588ebb91ae4dd22dfbc29ad8b6`  
		Last Modified: Fri, 11 Dec 2020 20:45:55 GMT  
		Size: 11.9 KB (11912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9ab1e75a9565c282e534694fe6b77c07b04e7d522482fb4b67ab724cbeb8cd`  
		Last Modified: Fri, 11 Dec 2020 20:45:57 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:3225915274bb6bf7f7dc7147d91fe7e959fe1a13ed065318270a6464cde72748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60456164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1977ebe4de743638890b7558f49d76a53f8ab57cb5d08f4e281098c8c10f8d37`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:48:42 GMT
ADD file:2efe3cccad076777e72be01a4380984d961a457c67dad3041063307ce1519c4d in / 
# Fri, 11 Dec 2020 02:48:44 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 19:14:20 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 19:14:22 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 11 Dec 2020 19:14:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 19:14:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 19:14:44 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 19:14:45 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 19:14:45 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 19:14:46 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 19:14:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 19:14:48 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:15531941ccc12369b70088bb4e7b58263a2363c37d600f0ec7f4b7532efe6685`  
		Last Modified: Fri, 11 Dec 2020 02:56:00 GMT  
		Size: 20.4 MB (20387882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7517de3bd6340ffc9245806134aad5e20933580bef5822a2e01b197a64dcd494`  
		Last Modified: Fri, 11 Dec 2020 19:15:58 GMT  
		Size: 4.1 MB (4082308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91c602536e96ff018a4443977fd6745cda94ee6455d50b555347c9a1f80f711`  
		Last Modified: Fri, 11 Dec 2020 19:16:05 GMT  
		Size: 36.0 MB (35961573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82951a98c1cb148cc4363e352820b61243fab1b0961cd1575364b75428dd6989`  
		Last Modified: Fri, 11 Dec 2020 19:15:57 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8225678c4b908a14dbb7cb9b025d4deb144f7c2e81178a26424356c1adea8236`  
		Last Modified: Fri, 11 Dec 2020 19:15:56 GMT  
		Size: 11.9 KB (11912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ad1b824158250f33ec33bba41dd485c3075672f537070e2d780cd6a1d85c1e`  
		Last Modified: Fri, 11 Dec 2020 19:15:56 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17-alpine`

```console
$ docker pull chronograf@sha256:65a96aa283fef3e7a859923058cc8da592e2810cbf2c6ee913d292da9b013dc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.7.17-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:8ae102326e39dae85ad9c8baaeab76f5c1430a5a90a3df7744c622205c8b57c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22657539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a66cf8368b795c9b81fd7732bfd3dd024d6524bfde27047d2ff283bf2628dde`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:51:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:51:47 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 11 Dec 2020 02:52:33 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 11 Dec 2020 02:52:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 11 Dec 2020 02:52:39 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 02:52:40 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 02:52:40 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 02:52:40 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 02:52:41 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 11 Dec 2020 02:52:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 02:52:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9624996f533f5dfa6054365968149298c1183a1202c16061de0fc5093ad633f`  
		Last Modified: Fri, 11 Dec 2020 02:53:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714c102d667de25287e212434b418f887c3297d809db411374920f3d8b36201`  
		Last Modified: Fri, 11 Dec 2020 02:53:53 GMT  
		Size: 280.8 KB (280809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02aa34e34d0764615139c671d46ced46d882087f60733de71a5445cce7bf5f13`  
		Last Modified: Fri, 11 Dec 2020 02:54:23 GMT  
		Size: 19.6 MB (19555249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbd49540e07b3784da9d92d98e3af811b3015563c5b734dbef6a12517670d72`  
		Last Modified: Fri, 11 Dec 2020 02:54:17 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9ce994d80b9fed3e667377f4593d53b1bad5ee0b9bd08586d47a2eb0dbbcb0`  
		Last Modified: Fri, 11 Dec 2020 02:54:17 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0794cc62f9943fae6a48aa49873a3a9a5f8e686f80ae3ef5b1147a1178c96fc5`  
		Last Modified: Fri, 11 Dec 2020 02:54:17 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:65a96aa283fef3e7a859923058cc8da592e2810cbf2c6ee913d292da9b013dc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.7-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:8ae102326e39dae85ad9c8baaeab76f5c1430a5a90a3df7744c622205c8b57c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22657539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a66cf8368b795c9b81fd7732bfd3dd024d6524bfde27047d2ff283bf2628dde`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:51:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:51:47 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 11 Dec 2020 02:52:33 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 11 Dec 2020 02:52:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 11 Dec 2020 02:52:39 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 02:52:40 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 02:52:40 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 02:52:40 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 02:52:41 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 11 Dec 2020 02:52:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 02:52:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9624996f533f5dfa6054365968149298c1183a1202c16061de0fc5093ad633f`  
		Last Modified: Fri, 11 Dec 2020 02:53:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714c102d667de25287e212434b418f887c3297d809db411374920f3d8b36201`  
		Last Modified: Fri, 11 Dec 2020 02:53:53 GMT  
		Size: 280.8 KB (280809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02aa34e34d0764615139c671d46ced46d882087f60733de71a5445cce7bf5f13`  
		Last Modified: Fri, 11 Dec 2020 02:54:23 GMT  
		Size: 19.6 MB (19555249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbd49540e07b3784da9d92d98e3af811b3015563c5b734dbef6a12517670d72`  
		Last Modified: Fri, 11 Dec 2020 02:54:17 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9ce994d80b9fed3e667377f4593d53b1bad5ee0b9bd08586d47a2eb0dbbcb0`  
		Last Modified: Fri, 11 Dec 2020 02:54:17 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0794cc62f9943fae6a48aa49873a3a9a5f8e686f80ae3ef5b1147a1178c96fc5`  
		Last Modified: Fri, 11 Dec 2020 02:54:17 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8`

```console
$ docker pull chronograf@sha256:93a37d72f8c2d5fbd6a1e520a281e10ac2dd7393dd35cc28e012d2bc1144b6e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:05bef04499aa5453af082ce7a12b21b0ac5f8fb3654a557b740f6a46b9b1e9db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70422632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476583469caac9afa471c9a33bd2b5599b72b4a933a4e997de748cda23dfaf20`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:58 GMT
ADD file:f03e68a10b84e2342cfffbb8cdec1117c7f5e5d0dd004072e84efb62cfdf157c in / 
# Fri, 11 Dec 2020 02:08:58 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:51:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 02:52:48 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 11 Dec 2020 02:53:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 02:53:03 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 02:53:04 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 02:53:04 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 02:53:04 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 02:53:05 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 02:53:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 02:53:05 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e50c3c9ef5a201a24959788dcbc7ebf88d95c63e132a4d7396ce541127afd88e`  
		Last Modified: Fri, 11 Dec 2020 02:15:43 GMT  
		Size: 22.5 MB (22527860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121258f8a02a8e6785249c0e846752cef626dea7d69f721857d361346ce8c23d`  
		Last Modified: Fri, 11 Dec 2020 02:53:44 GMT  
		Size: 6.7 MB (6742130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a0113424375034b3f0290f4ee69045cdc6ca732fba10c9def6997f8dc33b6`  
		Last Modified: Fri, 11 Dec 2020 02:54:37 GMT  
		Size: 41.1 MB (41128244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a214ca128ad5b722e1d27cd275a8dd0d7d34e948ef513fc2c23487102693d51`  
		Last Modified: Fri, 11 Dec 2020 02:54:29 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095cb1201293ad3f4b622e03923fe84293b9e66966154bd3d93c30a188a94bab`  
		Last Modified: Fri, 11 Dec 2020 02:54:28 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249c743e560851f3e650b973febf0cc6c4d7cf358482e29333be1b9280407e51`  
		Last Modified: Fri, 11 Dec 2020 02:54:29 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:12f37367be4842518ee3fb92b1a65b1520319192830adac3e7e820cb025c4620
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63836361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03463f74641dd5b1c7482882250f7f752675583f9a5eac38887aca789c1198bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:28:33 GMT
ADD file:a5ae44ff42f691e7afa1f743d1f05f6fd72d9c1737ae20b97977f9de76811260 in / 
# Fri, 11 Dec 2020 02:28:34 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 20:43:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 20:45:01 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 11 Dec 2020 20:45:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 20:45:18 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 20:45:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 20:45:20 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 20:45:20 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 20:45:21 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 20:45:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 20:45:23 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:3844aeda5f39338d766015a56d78b18d6d4d4b95b0e6b41f8d37105ee5b91a80`  
		Last Modified: Fri, 11 Dec 2020 02:37:12 GMT  
		Size: 19.3 MB (19313560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01f6f4ab74e3df5409e7c7b9fbf06f93ee005364bdfce72d9264eea24777ba9`  
		Last Modified: Fri, 11 Dec 2020 20:45:43 GMT  
		Size: 5.8 MB (5764540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82d570cab3205e32109a10bcef81614fe8a984363fe5df290de9d3d784b80e1`  
		Last Modified: Fri, 11 Dec 2020 20:46:23 GMT  
		Size: 38.7 MB (38733867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b03b1bed98a56af66f496fe2a9e19cacf7b82c5a7d025a29d1ed5a5a2437e7`  
		Last Modified: Fri, 11 Dec 2020 20:46:13 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4870079f0c4ffb52818c543136005c8f786aba6bfbc996717c19ff5f378fc59c`  
		Last Modified: Fri, 11 Dec 2020 20:46:13 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21bbe3a4fc5282e777908e75a9d219d9c806d32682b122df6f4e709f34a10e95`  
		Last Modified: Fri, 11 Dec 2020 20:46:13 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:641a2478240e96d4b6fbb7dd48c90954218a06336053bf0c712813a09849911e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64942609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7986265ef928df9f8c7f640f7e5ac10567d52190c55be245735be4309551bc92`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:48:42 GMT
ADD file:2efe3cccad076777e72be01a4380984d961a457c67dad3041063307ce1519c4d in / 
# Fri, 11 Dec 2020 02:48:44 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 19:13:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 19:14:56 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 11 Dec 2020 19:15:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 19:15:19 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 19:15:20 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 19:15:21 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 19:15:22 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 19:15:22 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 19:15:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 19:15:24 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:15531941ccc12369b70088bb4e7b58263a2363c37d600f0ec7f4b7532efe6685`  
		Last Modified: Fri, 11 Dec 2020 02:56:00 GMT  
		Size: 20.4 MB (20387882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc6eef58f92eea9ce0ce34bd98afa24ba6e62ac9d993abbc6e19f386740a1cf`  
		Last Modified: Fri, 11 Dec 2020 19:15:44 GMT  
		Size: 6.0 MB (6028036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c310be4ce512120a0ffb1e668612dedaab93fd4a6c2c6db96a0e648c79f3ea36`  
		Last Modified: Fri, 11 Dec 2020 19:16:23 GMT  
		Size: 38.5 MB (38502290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70b7d321ae5610bbe16be1edd7aa33f31c9baef70f4e21bcb7d300cadac1c7c`  
		Last Modified: Fri, 11 Dec 2020 19:16:15 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a3fda20b10a2d6d351182191ce69690f6e5996cdf30a5a65c7ce571add0678`  
		Last Modified: Fri, 11 Dec 2020 19:16:14 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a131d50b0942b49599ee9252899bb800da1fb980ac5d1e9b86cce786ef3a0f1a`  
		Last Modified: Fri, 11 Dec 2020 19:16:14 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.8`

```console
$ docker pull chronograf@sha256:93a37d72f8c2d5fbd6a1e520a281e10ac2dd7393dd35cc28e012d2bc1144b6e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8.8` - linux; amd64

```console
$ docker pull chronograf@sha256:05bef04499aa5453af082ce7a12b21b0ac5f8fb3654a557b740f6a46b9b1e9db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70422632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476583469caac9afa471c9a33bd2b5599b72b4a933a4e997de748cda23dfaf20`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:58 GMT
ADD file:f03e68a10b84e2342cfffbb8cdec1117c7f5e5d0dd004072e84efb62cfdf157c in / 
# Fri, 11 Dec 2020 02:08:58 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:51:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 02:52:48 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 11 Dec 2020 02:53:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 02:53:03 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 02:53:04 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 02:53:04 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 02:53:04 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 02:53:05 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 02:53:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 02:53:05 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e50c3c9ef5a201a24959788dcbc7ebf88d95c63e132a4d7396ce541127afd88e`  
		Last Modified: Fri, 11 Dec 2020 02:15:43 GMT  
		Size: 22.5 MB (22527860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121258f8a02a8e6785249c0e846752cef626dea7d69f721857d361346ce8c23d`  
		Last Modified: Fri, 11 Dec 2020 02:53:44 GMT  
		Size: 6.7 MB (6742130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a0113424375034b3f0290f4ee69045cdc6ca732fba10c9def6997f8dc33b6`  
		Last Modified: Fri, 11 Dec 2020 02:54:37 GMT  
		Size: 41.1 MB (41128244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a214ca128ad5b722e1d27cd275a8dd0d7d34e948ef513fc2c23487102693d51`  
		Last Modified: Fri, 11 Dec 2020 02:54:29 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095cb1201293ad3f4b622e03923fe84293b9e66966154bd3d93c30a188a94bab`  
		Last Modified: Fri, 11 Dec 2020 02:54:28 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249c743e560851f3e650b973febf0cc6c4d7cf358482e29333be1b9280407e51`  
		Last Modified: Fri, 11 Dec 2020 02:54:29 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:12f37367be4842518ee3fb92b1a65b1520319192830adac3e7e820cb025c4620
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63836361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03463f74641dd5b1c7482882250f7f752675583f9a5eac38887aca789c1198bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:28:33 GMT
ADD file:a5ae44ff42f691e7afa1f743d1f05f6fd72d9c1737ae20b97977f9de76811260 in / 
# Fri, 11 Dec 2020 02:28:34 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 20:43:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 20:45:01 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 11 Dec 2020 20:45:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 20:45:18 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 20:45:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 20:45:20 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 20:45:20 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 20:45:21 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 20:45:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 20:45:23 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:3844aeda5f39338d766015a56d78b18d6d4d4b95b0e6b41f8d37105ee5b91a80`  
		Last Modified: Fri, 11 Dec 2020 02:37:12 GMT  
		Size: 19.3 MB (19313560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01f6f4ab74e3df5409e7c7b9fbf06f93ee005364bdfce72d9264eea24777ba9`  
		Last Modified: Fri, 11 Dec 2020 20:45:43 GMT  
		Size: 5.8 MB (5764540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82d570cab3205e32109a10bcef81614fe8a984363fe5df290de9d3d784b80e1`  
		Last Modified: Fri, 11 Dec 2020 20:46:23 GMT  
		Size: 38.7 MB (38733867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b03b1bed98a56af66f496fe2a9e19cacf7b82c5a7d025a29d1ed5a5a2437e7`  
		Last Modified: Fri, 11 Dec 2020 20:46:13 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4870079f0c4ffb52818c543136005c8f786aba6bfbc996717c19ff5f378fc59c`  
		Last Modified: Fri, 11 Dec 2020 20:46:13 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21bbe3a4fc5282e777908e75a9d219d9c806d32682b122df6f4e709f34a10e95`  
		Last Modified: Fri, 11 Dec 2020 20:46:13 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:641a2478240e96d4b6fbb7dd48c90954218a06336053bf0c712813a09849911e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64942609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7986265ef928df9f8c7f640f7e5ac10567d52190c55be245735be4309551bc92`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:48:42 GMT
ADD file:2efe3cccad076777e72be01a4380984d961a457c67dad3041063307ce1519c4d in / 
# Fri, 11 Dec 2020 02:48:44 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 19:13:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 19:14:56 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 11 Dec 2020 19:15:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 19:15:19 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 19:15:20 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 19:15:21 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 19:15:22 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 19:15:22 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 19:15:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 19:15:24 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:15531941ccc12369b70088bb4e7b58263a2363c37d600f0ec7f4b7532efe6685`  
		Last Modified: Fri, 11 Dec 2020 02:56:00 GMT  
		Size: 20.4 MB (20387882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc6eef58f92eea9ce0ce34bd98afa24ba6e62ac9d993abbc6e19f386740a1cf`  
		Last Modified: Fri, 11 Dec 2020 19:15:44 GMT  
		Size: 6.0 MB (6028036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c310be4ce512120a0ffb1e668612dedaab93fd4a6c2c6db96a0e648c79f3ea36`  
		Last Modified: Fri, 11 Dec 2020 19:16:23 GMT  
		Size: 38.5 MB (38502290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70b7d321ae5610bbe16be1edd7aa33f31c9baef70f4e21bcb7d300cadac1c7c`  
		Last Modified: Fri, 11 Dec 2020 19:16:15 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a3fda20b10a2d6d351182191ce69690f6e5996cdf30a5a65c7ce571add0678`  
		Last Modified: Fri, 11 Dec 2020 19:16:14 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a131d50b0942b49599ee9252899bb800da1fb980ac5d1e9b86cce786ef3a0f1a`  
		Last Modified: Fri, 11 Dec 2020 19:16:14 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.8-alpine`

```console
$ docker pull chronograf@sha256:154c60c2c97eab0dc68ec054c0374701d459f912832f998b00eda2434ebcab54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.8.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:4a16405e7df73ce95a6f5e763c2e899fd0110c45c62d6c6b0feb8e13c73a0773
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25347940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14e8b021a036a08ef030362109e5bc31baf829305f73f190161ef85d34dbc940`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:51:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:51:47 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 11 Dec 2020 02:53:12 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 11 Dec 2020 02:53:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 11 Dec 2020 02:53:19 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 02:53:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 02:53:20 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 02:53:20 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 02:53:20 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 11 Dec 2020 02:53:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 02:53:21 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9624996f533f5dfa6054365968149298c1183a1202c16061de0fc5093ad633f`  
		Last Modified: Fri, 11 Dec 2020 02:53:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714c102d667de25287e212434b418f887c3297d809db411374920f3d8b36201`  
		Last Modified: Fri, 11 Dec 2020 02:53:53 GMT  
		Size: 280.8 KB (280809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e15f09580a6d6bc3a7d5021387bae151f8aeeb0d67674ca7071c1776e333fcf`  
		Last Modified: Fri, 11 Dec 2020 02:54:50 GMT  
		Size: 22.2 MB (22245645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0253ae425b3a9037e3433731adfe4f96765b7fb1f1120d5fd7b58b16e6a76d`  
		Last Modified: Fri, 11 Dec 2020 02:54:45 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74299b6d2979ac9cf7ab80892733e71b7f74d53bf7a19964e98ccf306cb00344`  
		Last Modified: Fri, 11 Dec 2020 02:54:44 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414a8455403f624f4d1b945a48db62a2fdd5446d129a854e39cfd7df5eec1610`  
		Last Modified: Fri, 11 Dec 2020 02:54:45 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8-alpine`

```console
$ docker pull chronograf@sha256:154c60c2c97eab0dc68ec054c0374701d459f912832f998b00eda2434ebcab54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:4a16405e7df73ce95a6f5e763c2e899fd0110c45c62d6c6b0feb8e13c73a0773
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25347940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14e8b021a036a08ef030362109e5bc31baf829305f73f190161ef85d34dbc940`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:51:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:51:47 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 11 Dec 2020 02:53:12 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 11 Dec 2020 02:53:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 11 Dec 2020 02:53:19 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 02:53:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 02:53:20 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 02:53:20 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 02:53:20 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 11 Dec 2020 02:53:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 02:53:21 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9624996f533f5dfa6054365968149298c1183a1202c16061de0fc5093ad633f`  
		Last Modified: Fri, 11 Dec 2020 02:53:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714c102d667de25287e212434b418f887c3297d809db411374920f3d8b36201`  
		Last Modified: Fri, 11 Dec 2020 02:53:53 GMT  
		Size: 280.8 KB (280809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e15f09580a6d6bc3a7d5021387bae151f8aeeb0d67674ca7071c1776e333fcf`  
		Last Modified: Fri, 11 Dec 2020 02:54:50 GMT  
		Size: 22.2 MB (22245645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0253ae425b3a9037e3433731adfe4f96765b7fb1f1120d5fd7b58b16e6a76d`  
		Last Modified: Fri, 11 Dec 2020 02:54:45 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74299b6d2979ac9cf7ab80892733e71b7f74d53bf7a19964e98ccf306cb00344`  
		Last Modified: Fri, 11 Dec 2020 02:54:44 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414a8455403f624f4d1b945a48db62a2fdd5446d129a854e39cfd7df5eec1610`  
		Last Modified: Fri, 11 Dec 2020 02:54:45 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:154c60c2c97eab0dc68ec054c0374701d459f912832f998b00eda2434ebcab54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:4a16405e7df73ce95a6f5e763c2e899fd0110c45c62d6c6b0feb8e13c73a0773
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25347940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14e8b021a036a08ef030362109e5bc31baf829305f73f190161ef85d34dbc940`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:51:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:51:47 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 11 Dec 2020 02:53:12 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 11 Dec 2020 02:53:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 11 Dec 2020 02:53:19 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 02:53:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 02:53:20 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 02:53:20 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 02:53:20 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 11 Dec 2020 02:53:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 02:53:21 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9624996f533f5dfa6054365968149298c1183a1202c16061de0fc5093ad633f`  
		Last Modified: Fri, 11 Dec 2020 02:53:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714c102d667de25287e212434b418f887c3297d809db411374920f3d8b36201`  
		Last Modified: Fri, 11 Dec 2020 02:53:53 GMT  
		Size: 280.8 KB (280809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e15f09580a6d6bc3a7d5021387bae151f8aeeb0d67674ca7071c1776e333fcf`  
		Last Modified: Fri, 11 Dec 2020 02:54:50 GMT  
		Size: 22.2 MB (22245645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0253ae425b3a9037e3433731adfe4f96765b7fb1f1120d5fd7b58b16e6a76d`  
		Last Modified: Fri, 11 Dec 2020 02:54:45 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74299b6d2979ac9cf7ab80892733e71b7f74d53bf7a19964e98ccf306cb00344`  
		Last Modified: Fri, 11 Dec 2020 02:54:44 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414a8455403f624f4d1b945a48db62a2fdd5446d129a854e39cfd7df5eec1610`  
		Last Modified: Fri, 11 Dec 2020 02:54:45 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:latest`

```console
$ docker pull chronograf@sha256:93a37d72f8c2d5fbd6a1e520a281e10ac2dd7393dd35cc28e012d2bc1144b6e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:05bef04499aa5453af082ce7a12b21b0ac5f8fb3654a557b740f6a46b9b1e9db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70422632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476583469caac9afa471c9a33bd2b5599b72b4a933a4e997de748cda23dfaf20`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:58 GMT
ADD file:f03e68a10b84e2342cfffbb8cdec1117c7f5e5d0dd004072e84efb62cfdf157c in / 
# Fri, 11 Dec 2020 02:08:58 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:51:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 02:52:48 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 11 Dec 2020 02:53:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 02:53:03 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 02:53:04 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 02:53:04 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 02:53:04 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 02:53:05 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 02:53:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 02:53:05 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e50c3c9ef5a201a24959788dcbc7ebf88d95c63e132a4d7396ce541127afd88e`  
		Last Modified: Fri, 11 Dec 2020 02:15:43 GMT  
		Size: 22.5 MB (22527860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121258f8a02a8e6785249c0e846752cef626dea7d69f721857d361346ce8c23d`  
		Last Modified: Fri, 11 Dec 2020 02:53:44 GMT  
		Size: 6.7 MB (6742130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a0113424375034b3f0290f4ee69045cdc6ca732fba10c9def6997f8dc33b6`  
		Last Modified: Fri, 11 Dec 2020 02:54:37 GMT  
		Size: 41.1 MB (41128244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a214ca128ad5b722e1d27cd275a8dd0d7d34e948ef513fc2c23487102693d51`  
		Last Modified: Fri, 11 Dec 2020 02:54:29 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095cb1201293ad3f4b622e03923fe84293b9e66966154bd3d93c30a188a94bab`  
		Last Modified: Fri, 11 Dec 2020 02:54:28 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249c743e560851f3e650b973febf0cc6c4d7cf358482e29333be1b9280407e51`  
		Last Modified: Fri, 11 Dec 2020 02:54:29 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:12f37367be4842518ee3fb92b1a65b1520319192830adac3e7e820cb025c4620
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63836361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03463f74641dd5b1c7482882250f7f752675583f9a5eac38887aca789c1198bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:28:33 GMT
ADD file:a5ae44ff42f691e7afa1f743d1f05f6fd72d9c1737ae20b97977f9de76811260 in / 
# Fri, 11 Dec 2020 02:28:34 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 20:43:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 20:45:01 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 11 Dec 2020 20:45:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 20:45:18 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 20:45:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 20:45:20 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 20:45:20 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 20:45:21 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 20:45:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 20:45:23 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:3844aeda5f39338d766015a56d78b18d6d4d4b95b0e6b41f8d37105ee5b91a80`  
		Last Modified: Fri, 11 Dec 2020 02:37:12 GMT  
		Size: 19.3 MB (19313560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01f6f4ab74e3df5409e7c7b9fbf06f93ee005364bdfce72d9264eea24777ba9`  
		Last Modified: Fri, 11 Dec 2020 20:45:43 GMT  
		Size: 5.8 MB (5764540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82d570cab3205e32109a10bcef81614fe8a984363fe5df290de9d3d784b80e1`  
		Last Modified: Fri, 11 Dec 2020 20:46:23 GMT  
		Size: 38.7 MB (38733867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b03b1bed98a56af66f496fe2a9e19cacf7b82c5a7d025a29d1ed5a5a2437e7`  
		Last Modified: Fri, 11 Dec 2020 20:46:13 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4870079f0c4ffb52818c543136005c8f786aba6bfbc996717c19ff5f378fc59c`  
		Last Modified: Fri, 11 Dec 2020 20:46:13 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21bbe3a4fc5282e777908e75a9d219d9c806d32682b122df6f4e709f34a10e95`  
		Last Modified: Fri, 11 Dec 2020 20:46:13 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:641a2478240e96d4b6fbb7dd48c90954218a06336053bf0c712813a09849911e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64942609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7986265ef928df9f8c7f640f7e5ac10567d52190c55be245735be4309551bc92`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 11 Dec 2020 02:48:42 GMT
ADD file:2efe3cccad076777e72be01a4380984d961a457c67dad3041063307ce1519c4d in / 
# Fri, 11 Dec 2020 02:48:44 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 19:13:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 11 Dec 2020 19:14:56 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 11 Dec 2020 19:15:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 19:15:19 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 11 Dec 2020 19:15:20 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 11 Dec 2020 19:15:21 GMT
EXPOSE 8888
# Fri, 11 Dec 2020 19:15:22 GMT
VOLUME [/var/lib/chronograf]
# Fri, 11 Dec 2020 19:15:22 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 11 Dec 2020 19:15:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 19:15:24 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:15531941ccc12369b70088bb4e7b58263a2363c37d600f0ec7f4b7532efe6685`  
		Last Modified: Fri, 11 Dec 2020 02:56:00 GMT  
		Size: 20.4 MB (20387882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc6eef58f92eea9ce0ce34bd98afa24ba6e62ac9d993abbc6e19f386740a1cf`  
		Last Modified: Fri, 11 Dec 2020 19:15:44 GMT  
		Size: 6.0 MB (6028036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c310be4ce512120a0ffb1e668612dedaab93fd4a6c2c6db96a0e648c79f3ea36`  
		Last Modified: Fri, 11 Dec 2020 19:16:23 GMT  
		Size: 38.5 MB (38502290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70b7d321ae5610bbe16be1edd7aa33f31c9baef70f4e21bcb7d300cadac1c7c`  
		Last Modified: Fri, 11 Dec 2020 19:16:15 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a3fda20b10a2d6d351182191ce69690f6e5996cdf30a5a65c7ce571add0678`  
		Last Modified: Fri, 11 Dec 2020 19:16:14 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a131d50b0942b49599ee9252899bb800da1fb980ac5d1e9b86cce786ef3a0f1a`  
		Last Modified: Fri, 11 Dec 2020 19:16:14 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
