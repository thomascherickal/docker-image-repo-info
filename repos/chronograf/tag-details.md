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
-	[`chronograf:1.8.4`](#chronograf184)
-	[`chronograf:1.8.4-alpine`](#chronograf184-alpine)
-	[`chronograf:1.8-alpine`](#chronograf18-alpine)
-	[`chronograf:alpine`](#chronografalpine)
-	[`chronograf:latest`](#chronograflatest)

## `chronograf:1.6`

```console
$ docker pull chronograf@sha256:a00baedceceeb662d156c978a56987fe11872ee59d111318bd16b083d486b418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6` - linux; amd64

```console
$ docker pull chronograf@sha256:ea9f94e792535e35a8b26a20d1d13479062746c92e80f566b1467925db0d2e8b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49141088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81df42a46d4b6cd3bd2d1c52db323c894316908e0703050fb327c4b0f0e73eec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:23:54 GMT
ADD file:3e0b81347262efc5a7401a531be7ab45cb8ab05ddab528fbb849bea0053865a0 in / 
# Wed, 13 May 2020 21:23:54 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:49:29 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 May 2020 21:49:29 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 13 May 2020 21:49:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 21:49:41 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 13 May 2020 21:49:41 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 13 May 2020 21:49:41 GMT
EXPOSE 8888
# Wed, 13 May 2020 21:49:42 GMT
VOLUME [/var/lib/chronograf]
# Wed, 13 May 2020 21:49:42 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 13 May 2020 21:49:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 May 2020 21:49:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e4f2068f62324fe92e80c472afb3742bf506f2a52712bf36ec0456de94c5b14e`  
		Last Modified: Wed, 13 May 2020 21:30:12 GMT  
		Size: 22.5 MB (22513438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38860158577867e1380349aea84937148611cf6b106ffb79d992e6a16ebc1ae6`  
		Last Modified: Wed, 13 May 2020 21:50:46 GMT  
		Size: 4.5 MB (4503528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0a5c27c9787ab99e4984a6b57c043194c0a6e7e35b04d29abbbda2ebf850f7`  
		Last Modified: Wed, 13 May 2020 21:50:50 GMT  
		Size: 22.1 MB (22099730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01cded31fa9196c56829a7e2604f2fa1f641e16a248922740017fd1f084c69d`  
		Last Modified: Wed, 13 May 2020 21:50:45 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c165ff53cb1a19afc2bba68abca2a2472c234c2e4bc5884efe6a0036e5de1a1`  
		Last Modified: Wed, 13 May 2020 21:50:45 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d408d330f207825389d991a9e03fbfeae4da3e3667e33c0f29bac64ea17e7fc`  
		Last Modified: Wed, 13 May 2020 21:50:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:2cd453d7194d04c86f140bbfb77e3695c58977b7188cb808151318339410bb82
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43725619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa74f6586254797b03088fdbe4cc55390ade0e80a6c7dcf53055c9a7ca6f0c57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:24:26 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 May 2020 22:24:27 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 13 May 2020 22:24:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 22:24:53 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 13 May 2020 22:24:54 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 13 May 2020 22:24:55 GMT
EXPOSE 8888
# Wed, 13 May 2020 22:24:57 GMT
VOLUME [/var/lib/chronograf]
# Wed, 13 May 2020 22:24:59 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 13 May 2020 22:25:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 May 2020 22:25:01 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b980babbd6be63c990cc1f3d2d047bc1565f0e663b62e0e6f3e9e93614c41c`  
		Last Modified: Wed, 13 May 2020 22:26:46 GMT  
		Size: 3.9 MB (3877340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b906800e634287d1696201d30f6915a9ec463c00492e559a5e197e4fcfa7a7`  
		Last Modified: Wed, 13 May 2020 22:26:53 GMT  
		Size: 20.5 MB (20525412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355d59d3b48e330a6c5ebb0e7c26650e572e4b08767387c5b0b80ee7a2c8c99d`  
		Last Modified: Wed, 13 May 2020 22:26:45 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fb6b121ce2691d40f4d595aa9de74188c6d5dab207ab626d5f3baf25278882`  
		Last Modified: Wed, 13 May 2020 22:26:45 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6651fd8a895cfc14faefb1f6231dd656436353d8107527d4e5ca930086c8ca`  
		Last Modified: Wed, 13 May 2020 22:26:45 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:fed9475f4cd4d79c68b80dec991ae9f68b52868ea435b5053c28e426ec290e07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45208453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7206b2d060c9eac85881cde2350f19b19c12362b14e5ac1a23939cef0db6c44`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:49:14 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 14 May 2020 00:49:16 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 14 May 2020 00:49:37 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 14 May 2020 00:49:39 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 14 May 2020 00:49:39 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 14 May 2020 00:49:40 GMT
EXPOSE 8888
# Thu, 14 May 2020 00:49:41 GMT
VOLUME [/var/lib/chronograf]
# Thu, 14 May 2020 00:49:42 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 14 May 2020 00:49:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 May 2020 00:49:43 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27009d9d4e56d600926f21a2fcea7fd9cd9faaf8a0aa1dc3d91e1bb89f5b654d`  
		Last Modified: Thu, 14 May 2020 00:51:01 GMT  
		Size: 4.1 MB (4080587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf47e7b747c276d01b53733036df33eba2f0eabf65dea09869dee864ad07787e`  
		Last Modified: Thu, 14 May 2020 00:51:06 GMT  
		Size: 20.7 MB (20733431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b256e82369d323e01fecf698494c7ff3c117bfe9783435a24e5aeb8dd91eaf6`  
		Last Modified: Thu, 14 May 2020 00:51:00 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c66fb83636d0fdfc873882b0bba3bc02302e493a9b690ebc15a51c123ac5bf`  
		Last Modified: Thu, 14 May 2020 00:51:00 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c2efdbfc1ed3b1806dfe80be3b4c43e62c5a97a0ad0570bc442307afe1866f`  
		Last Modified: Thu, 14 May 2020 00:51:00 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2`

```console
$ docker pull chronograf@sha256:a00baedceceeb662d156c978a56987fe11872ee59d111318bd16b083d486b418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6.2` - linux; amd64

```console
$ docker pull chronograf@sha256:ea9f94e792535e35a8b26a20d1d13479062746c92e80f566b1467925db0d2e8b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49141088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81df42a46d4b6cd3bd2d1c52db323c894316908e0703050fb327c4b0f0e73eec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:23:54 GMT
ADD file:3e0b81347262efc5a7401a531be7ab45cb8ab05ddab528fbb849bea0053865a0 in / 
# Wed, 13 May 2020 21:23:54 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:49:29 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 May 2020 21:49:29 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 13 May 2020 21:49:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 21:49:41 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 13 May 2020 21:49:41 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 13 May 2020 21:49:41 GMT
EXPOSE 8888
# Wed, 13 May 2020 21:49:42 GMT
VOLUME [/var/lib/chronograf]
# Wed, 13 May 2020 21:49:42 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 13 May 2020 21:49:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 May 2020 21:49:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e4f2068f62324fe92e80c472afb3742bf506f2a52712bf36ec0456de94c5b14e`  
		Last Modified: Wed, 13 May 2020 21:30:12 GMT  
		Size: 22.5 MB (22513438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38860158577867e1380349aea84937148611cf6b106ffb79d992e6a16ebc1ae6`  
		Last Modified: Wed, 13 May 2020 21:50:46 GMT  
		Size: 4.5 MB (4503528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0a5c27c9787ab99e4984a6b57c043194c0a6e7e35b04d29abbbda2ebf850f7`  
		Last Modified: Wed, 13 May 2020 21:50:50 GMT  
		Size: 22.1 MB (22099730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01cded31fa9196c56829a7e2604f2fa1f641e16a248922740017fd1f084c69d`  
		Last Modified: Wed, 13 May 2020 21:50:45 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c165ff53cb1a19afc2bba68abca2a2472c234c2e4bc5884efe6a0036e5de1a1`  
		Last Modified: Wed, 13 May 2020 21:50:45 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d408d330f207825389d991a9e03fbfeae4da3e3667e33c0f29bac64ea17e7fc`  
		Last Modified: Wed, 13 May 2020 21:50:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:2cd453d7194d04c86f140bbfb77e3695c58977b7188cb808151318339410bb82
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43725619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa74f6586254797b03088fdbe4cc55390ade0e80a6c7dcf53055c9a7ca6f0c57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:24:26 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 May 2020 22:24:27 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 13 May 2020 22:24:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 22:24:53 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 13 May 2020 22:24:54 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 13 May 2020 22:24:55 GMT
EXPOSE 8888
# Wed, 13 May 2020 22:24:57 GMT
VOLUME [/var/lib/chronograf]
# Wed, 13 May 2020 22:24:59 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 13 May 2020 22:25:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 May 2020 22:25:01 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b980babbd6be63c990cc1f3d2d047bc1565f0e663b62e0e6f3e9e93614c41c`  
		Last Modified: Wed, 13 May 2020 22:26:46 GMT  
		Size: 3.9 MB (3877340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b906800e634287d1696201d30f6915a9ec463c00492e559a5e197e4fcfa7a7`  
		Last Modified: Wed, 13 May 2020 22:26:53 GMT  
		Size: 20.5 MB (20525412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355d59d3b48e330a6c5ebb0e7c26650e572e4b08767387c5b0b80ee7a2c8c99d`  
		Last Modified: Wed, 13 May 2020 22:26:45 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fb6b121ce2691d40f4d595aa9de74188c6d5dab207ab626d5f3baf25278882`  
		Last Modified: Wed, 13 May 2020 22:26:45 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6651fd8a895cfc14faefb1f6231dd656436353d8107527d4e5ca930086c8ca`  
		Last Modified: Wed, 13 May 2020 22:26:45 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:fed9475f4cd4d79c68b80dec991ae9f68b52868ea435b5053c28e426ec290e07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45208453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7206b2d060c9eac85881cde2350f19b19c12362b14e5ac1a23939cef0db6c44`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:49:14 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 14 May 2020 00:49:16 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 14 May 2020 00:49:37 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 14 May 2020 00:49:39 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 14 May 2020 00:49:39 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 14 May 2020 00:49:40 GMT
EXPOSE 8888
# Thu, 14 May 2020 00:49:41 GMT
VOLUME [/var/lib/chronograf]
# Thu, 14 May 2020 00:49:42 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 14 May 2020 00:49:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 May 2020 00:49:43 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27009d9d4e56d600926f21a2fcea7fd9cd9faaf8a0aa1dc3d91e1bb89f5b654d`  
		Last Modified: Thu, 14 May 2020 00:51:01 GMT  
		Size: 4.1 MB (4080587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf47e7b747c276d01b53733036df33eba2f0eabf65dea09869dee864ad07787e`  
		Last Modified: Thu, 14 May 2020 00:51:06 GMT  
		Size: 20.7 MB (20733431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b256e82369d323e01fecf698494c7ff3c117bfe9783435a24e5aeb8dd91eaf6`  
		Last Modified: Thu, 14 May 2020 00:51:00 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c66fb83636d0fdfc873882b0bba3bc02302e493a9b690ebc15a51c123ac5bf`  
		Last Modified: Thu, 14 May 2020 00:51:00 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c2efdbfc1ed3b1806dfe80be3b4c43e62c5a97a0ad0570bc442307afe1866f`  
		Last Modified: Thu, 14 May 2020 00:51:00 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2-alpine`

```console
$ docker pull chronograf@sha256:ab9e909b2a6318701217d3f27b96c229ddfe381e3c99cfbc48c2b91df8d81d76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.6.2-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:3040d8f732544ed44f7908c19edf33c918ded367f988ee9175433f69e87a48c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14835872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db9289c1df02bab2c38655f41eb0aea2e277e8e961b19726cc9c70dafdc969d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:15:55 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 14:15:55 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 24 Apr 2020 14:15:58 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:15:58 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 24 Apr 2020 14:15:58 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 24 Apr 2020 14:15:59 GMT
EXPOSE 8888
# Fri, 24 Apr 2020 14:15:59 GMT
VOLUME [/var/lib/chronograf]
# Fri, 24 Apr 2020 14:15:59 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 24 Apr 2020 14:15:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:15:59 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c949b60b63fb4b31e70314aba2aff2223f42a54c0d76cdb28917f161840b03`  
		Last Modified: Fri, 24 Apr 2020 14:16:39 GMT  
		Size: 301.1 KB (301092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c82ab5090579d3291f9ed3ddd78c41f9ea5553454ae96b1bf426999afb054d8`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 11.7 MB (11736840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9942bb837dd1bcb4c7e3a5347942a16a2025ed26f2bac53491c93349ea073258`  
		Last Modified: Fri, 24 Apr 2020 14:16:39 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99129646db7665828c77148491e39759cc05105543b77dd789244f7b81e31674`  
		Last Modified: Fri, 24 Apr 2020 14:16:38 GMT  
		Size: 11.9 KB (11895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1456aec305d0c9a39b31f6c4d783e2f42198b7f0c6c6757607e8b397ee8044e5`  
		Last Modified: Fri, 24 Apr 2020 14:16:39 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6-alpine`

```console
$ docker pull chronograf@sha256:ab9e909b2a6318701217d3f27b96c229ddfe381e3c99cfbc48c2b91df8d81d76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.6-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:3040d8f732544ed44f7908c19edf33c918ded367f988ee9175433f69e87a48c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14835872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db9289c1df02bab2c38655f41eb0aea2e277e8e961b19726cc9c70dafdc969d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:15:55 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 14:15:55 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 24 Apr 2020 14:15:58 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:15:58 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 24 Apr 2020 14:15:58 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 24 Apr 2020 14:15:59 GMT
EXPOSE 8888
# Fri, 24 Apr 2020 14:15:59 GMT
VOLUME [/var/lib/chronograf]
# Fri, 24 Apr 2020 14:15:59 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 24 Apr 2020 14:15:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:15:59 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c949b60b63fb4b31e70314aba2aff2223f42a54c0d76cdb28917f161840b03`  
		Last Modified: Fri, 24 Apr 2020 14:16:39 GMT  
		Size: 301.1 KB (301092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c82ab5090579d3291f9ed3ddd78c41f9ea5553454ae96b1bf426999afb054d8`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 11.7 MB (11736840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9942bb837dd1bcb4c7e3a5347942a16a2025ed26f2bac53491c93349ea073258`  
		Last Modified: Fri, 24 Apr 2020 14:16:39 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99129646db7665828c77148491e39759cc05105543b77dd789244f7b81e31674`  
		Last Modified: Fri, 24 Apr 2020 14:16:38 GMT  
		Size: 11.9 KB (11895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1456aec305d0c9a39b31f6c4d783e2f42198b7f0c6c6757607e8b397ee8044e5`  
		Last Modified: Fri, 24 Apr 2020 14:16:39 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7`

```console
$ docker pull chronograf@sha256:876418ffa53380afbf39b9deb88ef5c6a1df870fc0cc56b2df606ea061ef614d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:35475fce8269e486b616658699600258de25563b8b1d5ac36395c8ffc90dcb95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65385983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae5c07cf19e050acca4055c3b371f9ff786d7ba8a6b922dec233f031aeb77ee1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:23:54 GMT
ADD file:3e0b81347262efc5a7401a531be7ab45cb8ab05ddab528fbb849bea0053865a0 in / 
# Wed, 13 May 2020 21:23:54 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:49:29 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 May 2020 21:49:52 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 13 May 2020 21:50:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 21:50:06 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 13 May 2020 21:50:06 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 13 May 2020 21:50:06 GMT
EXPOSE 8888
# Wed, 13 May 2020 21:50:06 GMT
VOLUME [/var/lib/chronograf]
# Wed, 13 May 2020 21:50:07 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 13 May 2020 21:50:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 May 2020 21:50:07 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e4f2068f62324fe92e80c472afb3742bf506f2a52712bf36ec0456de94c5b14e`  
		Last Modified: Wed, 13 May 2020 21:30:12 GMT  
		Size: 22.5 MB (22513438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38860158577867e1380349aea84937148611cf6b106ffb79d992e6a16ebc1ae6`  
		Last Modified: Wed, 13 May 2020 21:50:46 GMT  
		Size: 4.5 MB (4503528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc682dd5ff2849bb792d24710b5fd3afd1f9c68b9f957e99678ebf23a10efb70`  
		Last Modified: Wed, 13 May 2020 21:51:01 GMT  
		Size: 38.3 MB (38344635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047213c493f4c027952ca35d6bd2e4f831c35c3397515eda1353cd94fde3184b`  
		Last Modified: Wed, 13 May 2020 21:50:54 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de4811621ff0f2853573728d86e930297b6805ea19e3ba2b8d80a5f19a36173`  
		Last Modified: Wed, 13 May 2020 21:50:54 GMT  
		Size: 11.9 KB (11902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e06a277883d55a0ccff0d49ed938b3e3881cb00272e30b8e038f63c194885ec`  
		Last Modified: Wed, 13 May 2020 21:50:55 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:f66cfe2a4a9fd2a0ff9523889a58780822513f3dc0323cd215cf2e35608d5800
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (59002804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32d2c90d031983f43a64ddf28de788c30bfec0b7fb0e4d5cb4db202cedb79458`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:24:26 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 May 2020 22:25:15 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 13 May 2020 22:25:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 22:25:42 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 13 May 2020 22:25:43 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 13 May 2020 22:25:45 GMT
EXPOSE 8888
# Wed, 13 May 2020 22:25:46 GMT
VOLUME [/var/lib/chronograf]
# Wed, 13 May 2020 22:25:47 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 13 May 2020 22:25:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 May 2020 22:25:50 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b980babbd6be63c990cc1f3d2d047bc1565f0e663b62e0e6f3e9e93614c41c`  
		Last Modified: Wed, 13 May 2020 22:26:46 GMT  
		Size: 3.9 MB (3877340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570b76b5b9f178aa30225629246447b715f3d9f5a75007ddeb2efa0d7de96cb2`  
		Last Modified: Wed, 13 May 2020 22:27:09 GMT  
		Size: 35.8 MB (35802601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13db0290e6113566f051d8c3a3438d2b365f228e17f0ce4ef826c553daa9422`  
		Last Modified: Wed, 13 May 2020 22:26:59 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50066862e049bccaddb131a0aa5407e808d66a15acb2826e157fc5823199ae71`  
		Last Modified: Wed, 13 May 2020 22:26:58 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f0090c1bf0e023df18b4c200d1c7990d73ed8f5c01c63467e9a803bae638e7`  
		Last Modified: Wed, 13 May 2020 22:26:58 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:6c01d788687a8221bb183870e70de07a4eb2b0b9312b973d4150ea42f221dd02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60480786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a8f13155f2675c4cb96eae8ac36cd9f0914e7924ece624d1c59e3054634842`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:49:14 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 14 May 2020 00:49:50 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 14 May 2020 00:50:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 14 May 2020 00:50:10 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 14 May 2020 00:50:11 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 14 May 2020 00:50:12 GMT
EXPOSE 8888
# Thu, 14 May 2020 00:50:13 GMT
VOLUME [/var/lib/chronograf]
# Thu, 14 May 2020 00:50:13 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 14 May 2020 00:50:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 May 2020 00:50:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27009d9d4e56d600926f21a2fcea7fd9cd9faaf8a0aa1dc3d91e1bb89f5b654d`  
		Last Modified: Thu, 14 May 2020 00:51:01 GMT  
		Size: 4.1 MB (4080587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e81122c950dd7fdc9282e4ed74bee36eed68d1a9f995390e8e53bb90e606dc`  
		Last Modified: Thu, 14 May 2020 00:51:20 GMT  
		Size: 36.0 MB (36005767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191464e9bb4fb5422a38429dca6be229b35994bcd0a2d7e27fa497f1665d930c`  
		Last Modified: Thu, 14 May 2020 00:51:11 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c484957615594a2a17d77cdc9a295307feaa4b36cf515083d76a9c7d186aba`  
		Last Modified: Thu, 14 May 2020 00:51:12 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881fb7a4df76dbdc7d27501927dba4b1bf1b173a75f5a53d0c16b6b10270c20b`  
		Last Modified: Thu, 14 May 2020 00:51:11 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17`

```console
$ docker pull chronograf@sha256:876418ffa53380afbf39b9deb88ef5c6a1df870fc0cc56b2df606ea061ef614d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:35475fce8269e486b616658699600258de25563b8b1d5ac36395c8ffc90dcb95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65385983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae5c07cf19e050acca4055c3b371f9ff786d7ba8a6b922dec233f031aeb77ee1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:23:54 GMT
ADD file:3e0b81347262efc5a7401a531be7ab45cb8ab05ddab528fbb849bea0053865a0 in / 
# Wed, 13 May 2020 21:23:54 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:49:29 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 May 2020 21:49:52 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 13 May 2020 21:50:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 21:50:06 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 13 May 2020 21:50:06 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 13 May 2020 21:50:06 GMT
EXPOSE 8888
# Wed, 13 May 2020 21:50:06 GMT
VOLUME [/var/lib/chronograf]
# Wed, 13 May 2020 21:50:07 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 13 May 2020 21:50:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 May 2020 21:50:07 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e4f2068f62324fe92e80c472afb3742bf506f2a52712bf36ec0456de94c5b14e`  
		Last Modified: Wed, 13 May 2020 21:30:12 GMT  
		Size: 22.5 MB (22513438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38860158577867e1380349aea84937148611cf6b106ffb79d992e6a16ebc1ae6`  
		Last Modified: Wed, 13 May 2020 21:50:46 GMT  
		Size: 4.5 MB (4503528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc682dd5ff2849bb792d24710b5fd3afd1f9c68b9f957e99678ebf23a10efb70`  
		Last Modified: Wed, 13 May 2020 21:51:01 GMT  
		Size: 38.3 MB (38344635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047213c493f4c027952ca35d6bd2e4f831c35c3397515eda1353cd94fde3184b`  
		Last Modified: Wed, 13 May 2020 21:50:54 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de4811621ff0f2853573728d86e930297b6805ea19e3ba2b8d80a5f19a36173`  
		Last Modified: Wed, 13 May 2020 21:50:54 GMT  
		Size: 11.9 KB (11902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e06a277883d55a0ccff0d49ed938b3e3881cb00272e30b8e038f63c194885ec`  
		Last Modified: Wed, 13 May 2020 21:50:55 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:f66cfe2a4a9fd2a0ff9523889a58780822513f3dc0323cd215cf2e35608d5800
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (59002804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32d2c90d031983f43a64ddf28de788c30bfec0b7fb0e4d5cb4db202cedb79458`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:24:26 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 May 2020 22:25:15 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 13 May 2020 22:25:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 22:25:42 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 13 May 2020 22:25:43 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 13 May 2020 22:25:45 GMT
EXPOSE 8888
# Wed, 13 May 2020 22:25:46 GMT
VOLUME [/var/lib/chronograf]
# Wed, 13 May 2020 22:25:47 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 13 May 2020 22:25:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 May 2020 22:25:50 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b980babbd6be63c990cc1f3d2d047bc1565f0e663b62e0e6f3e9e93614c41c`  
		Last Modified: Wed, 13 May 2020 22:26:46 GMT  
		Size: 3.9 MB (3877340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570b76b5b9f178aa30225629246447b715f3d9f5a75007ddeb2efa0d7de96cb2`  
		Last Modified: Wed, 13 May 2020 22:27:09 GMT  
		Size: 35.8 MB (35802601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13db0290e6113566f051d8c3a3438d2b365f228e17f0ce4ef826c553daa9422`  
		Last Modified: Wed, 13 May 2020 22:26:59 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50066862e049bccaddb131a0aa5407e808d66a15acb2826e157fc5823199ae71`  
		Last Modified: Wed, 13 May 2020 22:26:58 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f0090c1bf0e023df18b4c200d1c7990d73ed8f5c01c63467e9a803bae638e7`  
		Last Modified: Wed, 13 May 2020 22:26:58 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:6c01d788687a8221bb183870e70de07a4eb2b0b9312b973d4150ea42f221dd02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60480786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a8f13155f2675c4cb96eae8ac36cd9f0914e7924ece624d1c59e3054634842`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:49:14 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 14 May 2020 00:49:50 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 14 May 2020 00:50:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 14 May 2020 00:50:10 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 14 May 2020 00:50:11 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 14 May 2020 00:50:12 GMT
EXPOSE 8888
# Thu, 14 May 2020 00:50:13 GMT
VOLUME [/var/lib/chronograf]
# Thu, 14 May 2020 00:50:13 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 14 May 2020 00:50:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 May 2020 00:50:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27009d9d4e56d600926f21a2fcea7fd9cd9faaf8a0aa1dc3d91e1bb89f5b654d`  
		Last Modified: Thu, 14 May 2020 00:51:01 GMT  
		Size: 4.1 MB (4080587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e81122c950dd7fdc9282e4ed74bee36eed68d1a9f995390e8e53bb90e606dc`  
		Last Modified: Thu, 14 May 2020 00:51:20 GMT  
		Size: 36.0 MB (36005767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191464e9bb4fb5422a38429dca6be229b35994bcd0a2d7e27fa497f1665d930c`  
		Last Modified: Thu, 14 May 2020 00:51:11 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c484957615594a2a17d77cdc9a295307feaa4b36cf515083d76a9c7d186aba`  
		Last Modified: Thu, 14 May 2020 00:51:12 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881fb7a4df76dbdc7d27501927dba4b1bf1b173a75f5a53d0c16b6b10270c20b`  
		Last Modified: Thu, 14 May 2020 00:51:11 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17-alpine`

```console
$ docker pull chronograf@sha256:faf77badf0d4c19aba77ce78fb35bc4ec21dfc34192d793d18e79f49821277c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.7.17-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:b678606f54ee20752ddd298914e0ad1d6723791eec7ec35591a055f0f956747c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22654463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3f1d7ad4936d18671d233511fe0de824e84ed7aaeb7c470db9f178fa1e07589`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:15:55 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 14:16:07 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 24 Apr 2020 14:16:11 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:16:11 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 24 Apr 2020 14:16:11 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 24 Apr 2020 14:16:11 GMT
EXPOSE 8888
# Fri, 24 Apr 2020 14:16:12 GMT
VOLUME [/var/lib/chronograf]
# Fri, 24 Apr 2020 14:16:12 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 24 Apr 2020 14:16:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:16:12 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c949b60b63fb4b31e70314aba2aff2223f42a54c0d76cdb28917f161840b03`  
		Last Modified: Fri, 24 Apr 2020 14:16:39 GMT  
		Size: 301.1 KB (301092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f8c2050a1f47854ba88cbd879481140d7d6e3c62be71ba05023e71cab520e6`  
		Last Modified: Fri, 24 Apr 2020 14:16:49 GMT  
		Size: 19.6 MB (19555428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb3d1a18058de1f5ee1b1e288c41e8c13c94a90b1903b1bb960cb9fdc2ac1fa`  
		Last Modified: Fri, 24 Apr 2020 14:16:44 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f961be2fc5445bd3dae3232f93f2bacb313d82895975cdf0df60356c2690f5c5`  
		Last Modified: Fri, 24 Apr 2020 14:16:44 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0175b6657939d4a3771a953b2ee386b25ebb4fd0f9067970338b16abb9532f6e`  
		Last Modified: Fri, 24 Apr 2020 14:16:44 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:faf77badf0d4c19aba77ce78fb35bc4ec21dfc34192d793d18e79f49821277c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.7-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:b678606f54ee20752ddd298914e0ad1d6723791eec7ec35591a055f0f956747c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22654463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3f1d7ad4936d18671d233511fe0de824e84ed7aaeb7c470db9f178fa1e07589`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:15:55 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 14:16:07 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 24 Apr 2020 14:16:11 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:16:11 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 24 Apr 2020 14:16:11 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 24 Apr 2020 14:16:11 GMT
EXPOSE 8888
# Fri, 24 Apr 2020 14:16:12 GMT
VOLUME [/var/lib/chronograf]
# Fri, 24 Apr 2020 14:16:12 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 24 Apr 2020 14:16:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:16:12 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c949b60b63fb4b31e70314aba2aff2223f42a54c0d76cdb28917f161840b03`  
		Last Modified: Fri, 24 Apr 2020 14:16:39 GMT  
		Size: 301.1 KB (301092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f8c2050a1f47854ba88cbd879481140d7d6e3c62be71ba05023e71cab520e6`  
		Last Modified: Fri, 24 Apr 2020 14:16:49 GMT  
		Size: 19.6 MB (19555428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb3d1a18058de1f5ee1b1e288c41e8c13c94a90b1903b1bb960cb9fdc2ac1fa`  
		Last Modified: Fri, 24 Apr 2020 14:16:44 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f961be2fc5445bd3dae3232f93f2bacb313d82895975cdf0df60356c2690f5c5`  
		Last Modified: Fri, 24 Apr 2020 14:16:44 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0175b6657939d4a3771a953b2ee386b25ebb4fd0f9067970338b16abb9532f6e`  
		Last Modified: Fri, 24 Apr 2020 14:16:44 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8`

```console
$ docker pull chronograf@sha256:c7f40088278d5a27cafb36beb0ac95635b1b4ac22ff49099657b350c19862572
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:ec6abdcd7f5b296740484abcc2c50808fac3ca8bab21e5197bae1d54e608fb4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70190648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b507b55579c8643f99c0e45087533bd4eea3a51b8fe13531d84200afa71c7c62`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:23:54 GMT
ADD file:3e0b81347262efc5a7401a531be7ab45cb8ab05ddab528fbb849bea0053865a0 in / 
# Wed, 13 May 2020 21:23:54 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:49:29 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 May 2020 21:50:14 GMT
ENV CHRONOGRAF_VERSION=1.8.4
# Wed, 13 May 2020 21:50:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 21:50:29 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 13 May 2020 21:50:29 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 13 May 2020 21:50:29 GMT
EXPOSE 8888
# Wed, 13 May 2020 21:50:29 GMT
VOLUME [/var/lib/chronograf]
# Wed, 13 May 2020 21:50:29 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 13 May 2020 21:50:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 May 2020 21:50:30 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e4f2068f62324fe92e80c472afb3742bf506f2a52712bf36ec0456de94c5b14e`  
		Last Modified: Wed, 13 May 2020 21:30:12 GMT  
		Size: 22.5 MB (22513438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38860158577867e1380349aea84937148611cf6b106ffb79d992e6a16ebc1ae6`  
		Last Modified: Wed, 13 May 2020 21:50:46 GMT  
		Size: 4.5 MB (4503528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94933266b7ae6468cd742a09a59f371990d4011115537da31cd50578069ffaa2`  
		Last Modified: Wed, 13 May 2020 21:51:16 GMT  
		Size: 43.1 MB (43149286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c505f60cd8d7c0ffd0216fa998dbf11bb7a99deaadb7a4e23cd5c56839177d4a`  
		Last Modified: Wed, 13 May 2020 21:51:08 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620985d2330acf8fd76beaec79d986c00a9569cd7f5367f398f388971c6451bf`  
		Last Modified: Wed, 13 May 2020 21:51:09 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e84220ec6583225f482e47f3786e86140e1384cd6550d4055301ed727407ce0`  
		Last Modified: Wed, 13 May 2020 21:51:09 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:b370d27051108c28aad8241bac9933bbc8a5a1aa595b66efa403e3fd9b6d7f27
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63604009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0e271719a01339c37a45578b291d4758efddb12e832fec09e9fb43eea837884`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:24:26 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 May 2020 22:25:57 GMT
ENV CHRONOGRAF_VERSION=1.8.4
# Wed, 13 May 2020 22:26:24 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 22:26:25 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 13 May 2020 22:26:27 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 13 May 2020 22:26:28 GMT
EXPOSE 8888
# Wed, 13 May 2020 22:26:29 GMT
VOLUME [/var/lib/chronograf]
# Wed, 13 May 2020 22:26:30 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 13 May 2020 22:26:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 May 2020 22:26:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b980babbd6be63c990cc1f3d2d047bc1565f0e663b62e0e6f3e9e93614c41c`  
		Last Modified: Wed, 13 May 2020 22:26:46 GMT  
		Size: 3.9 MB (3877340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1fb4e47638fe2863e805d69b4f04971ec7f081271bc32194dc6a925e291eac`  
		Last Modified: Wed, 13 May 2020 22:27:29 GMT  
		Size: 40.4 MB (40403801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a588b516876bed658396d4eb66ddf6a8bbabb9b5d281f131655035fafe2b43`  
		Last Modified: Wed, 13 May 2020 22:27:17 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4435550515dbdd574a03f7fde63e89aec97b1643312411a70af16917c23db5`  
		Last Modified: Wed, 13 May 2020 22:27:17 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb2cd4a1df1196c3949f80f4a9f6904bec5d072ebfc2b8a0e0222299692e770`  
		Last Modified: Wed, 13 May 2020 22:27:17 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:9369dc6d98735f8b79bc1076d9be8e1517452fa5a796be7c90186b5b77c15ac5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64714374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bc19e90c0f79e3da3fbf0d4892bfb01ff957566c7d97f0f0d0a5e29e7ae6d40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:49:14 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 14 May 2020 00:50:22 GMT
ENV CHRONOGRAF_VERSION=1.8.4
# Thu, 14 May 2020 00:50:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 14 May 2020 00:50:44 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 14 May 2020 00:50:44 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 14 May 2020 00:50:45 GMT
EXPOSE 8888
# Thu, 14 May 2020 00:50:46 GMT
VOLUME [/var/lib/chronograf]
# Thu, 14 May 2020 00:50:47 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 14 May 2020 00:50:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 May 2020 00:50:48 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27009d9d4e56d600926f21a2fcea7fd9cd9faaf8a0aa1dc3d91e1bb89f5b654d`  
		Last Modified: Thu, 14 May 2020 00:51:01 GMT  
		Size: 4.1 MB (4080587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a71fe07ad9b05ef55473a46159658ea8427311e4bc8b39a9ae6d384dd5c1f63`  
		Last Modified: Thu, 14 May 2020 00:51:36 GMT  
		Size: 40.2 MB (40239346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e534e3a2953b36d5d1ebc359f5338af4eaf36d7e709f31df4bf6a235e6ee20be`  
		Last Modified: Thu, 14 May 2020 00:51:27 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f34bd489cf7347846985910cb4e2513fd2760d84d00ea520c54686b14009813`  
		Last Modified: Thu, 14 May 2020 00:51:26 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8f7e28ce4718da060028d491bbb042da94690056e2c737956a4ca6ab891879`  
		Last Modified: Thu, 14 May 2020 00:51:26 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.4`

```console
$ docker pull chronograf@sha256:c7f40088278d5a27cafb36beb0ac95635b1b4ac22ff49099657b350c19862572
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8.4` - linux; amd64

```console
$ docker pull chronograf@sha256:ec6abdcd7f5b296740484abcc2c50808fac3ca8bab21e5197bae1d54e608fb4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70190648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b507b55579c8643f99c0e45087533bd4eea3a51b8fe13531d84200afa71c7c62`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:23:54 GMT
ADD file:3e0b81347262efc5a7401a531be7ab45cb8ab05ddab528fbb849bea0053865a0 in / 
# Wed, 13 May 2020 21:23:54 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:49:29 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 May 2020 21:50:14 GMT
ENV CHRONOGRAF_VERSION=1.8.4
# Wed, 13 May 2020 21:50:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 21:50:29 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 13 May 2020 21:50:29 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 13 May 2020 21:50:29 GMT
EXPOSE 8888
# Wed, 13 May 2020 21:50:29 GMT
VOLUME [/var/lib/chronograf]
# Wed, 13 May 2020 21:50:29 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 13 May 2020 21:50:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 May 2020 21:50:30 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e4f2068f62324fe92e80c472afb3742bf506f2a52712bf36ec0456de94c5b14e`  
		Last Modified: Wed, 13 May 2020 21:30:12 GMT  
		Size: 22.5 MB (22513438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38860158577867e1380349aea84937148611cf6b106ffb79d992e6a16ebc1ae6`  
		Last Modified: Wed, 13 May 2020 21:50:46 GMT  
		Size: 4.5 MB (4503528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94933266b7ae6468cd742a09a59f371990d4011115537da31cd50578069ffaa2`  
		Last Modified: Wed, 13 May 2020 21:51:16 GMT  
		Size: 43.1 MB (43149286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c505f60cd8d7c0ffd0216fa998dbf11bb7a99deaadb7a4e23cd5c56839177d4a`  
		Last Modified: Wed, 13 May 2020 21:51:08 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620985d2330acf8fd76beaec79d986c00a9569cd7f5367f398f388971c6451bf`  
		Last Modified: Wed, 13 May 2020 21:51:09 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e84220ec6583225f482e47f3786e86140e1384cd6550d4055301ed727407ce0`  
		Last Modified: Wed, 13 May 2020 21:51:09 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.4` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:b370d27051108c28aad8241bac9933bbc8a5a1aa595b66efa403e3fd9b6d7f27
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63604009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0e271719a01339c37a45578b291d4758efddb12e832fec09e9fb43eea837884`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:24:26 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 May 2020 22:25:57 GMT
ENV CHRONOGRAF_VERSION=1.8.4
# Wed, 13 May 2020 22:26:24 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 22:26:25 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 13 May 2020 22:26:27 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 13 May 2020 22:26:28 GMT
EXPOSE 8888
# Wed, 13 May 2020 22:26:29 GMT
VOLUME [/var/lib/chronograf]
# Wed, 13 May 2020 22:26:30 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 13 May 2020 22:26:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 May 2020 22:26:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b980babbd6be63c990cc1f3d2d047bc1565f0e663b62e0e6f3e9e93614c41c`  
		Last Modified: Wed, 13 May 2020 22:26:46 GMT  
		Size: 3.9 MB (3877340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1fb4e47638fe2863e805d69b4f04971ec7f081271bc32194dc6a925e291eac`  
		Last Modified: Wed, 13 May 2020 22:27:29 GMT  
		Size: 40.4 MB (40403801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a588b516876bed658396d4eb66ddf6a8bbabb9b5d281f131655035fafe2b43`  
		Last Modified: Wed, 13 May 2020 22:27:17 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4435550515dbdd574a03f7fde63e89aec97b1643312411a70af16917c23db5`  
		Last Modified: Wed, 13 May 2020 22:27:17 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb2cd4a1df1196c3949f80f4a9f6904bec5d072ebfc2b8a0e0222299692e770`  
		Last Modified: Wed, 13 May 2020 22:27:17 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.4` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:9369dc6d98735f8b79bc1076d9be8e1517452fa5a796be7c90186b5b77c15ac5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64714374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bc19e90c0f79e3da3fbf0d4892bfb01ff957566c7d97f0f0d0a5e29e7ae6d40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:49:14 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 14 May 2020 00:50:22 GMT
ENV CHRONOGRAF_VERSION=1.8.4
# Thu, 14 May 2020 00:50:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 14 May 2020 00:50:44 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 14 May 2020 00:50:44 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 14 May 2020 00:50:45 GMT
EXPOSE 8888
# Thu, 14 May 2020 00:50:46 GMT
VOLUME [/var/lib/chronograf]
# Thu, 14 May 2020 00:50:47 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 14 May 2020 00:50:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 May 2020 00:50:48 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27009d9d4e56d600926f21a2fcea7fd9cd9faaf8a0aa1dc3d91e1bb89f5b654d`  
		Last Modified: Thu, 14 May 2020 00:51:01 GMT  
		Size: 4.1 MB (4080587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a71fe07ad9b05ef55473a46159658ea8427311e4bc8b39a9ae6d384dd5c1f63`  
		Last Modified: Thu, 14 May 2020 00:51:36 GMT  
		Size: 40.2 MB (40239346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e534e3a2953b36d5d1ebc359f5338af4eaf36d7e709f31df4bf6a235e6ee20be`  
		Last Modified: Thu, 14 May 2020 00:51:27 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f34bd489cf7347846985910cb4e2513fd2760d84d00ea520c54686b14009813`  
		Last Modified: Thu, 14 May 2020 00:51:26 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8f7e28ce4718da060028d491bbb042da94690056e2c737956a4ca6ab891879`  
		Last Modified: Thu, 14 May 2020 00:51:26 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.4-alpine`

```console
$ docker pull chronograf@sha256:a98e8a764382260af789cf3fd24952e5a5e1eea2568eda7a60a51678662920e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.8.4-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:7b9fd4bfa461dd588069a6662e7a23eec428fbd0ed24382e7a80ec2dacbea40a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25332562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:424098e734c5096176c639a03764d77e23d8b41e93efd2283b5b4363b6a8b837`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:15:55 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Sat, 02 May 2020 01:26:58 GMT
ENV CHRONOGRAF_VERSION=1.8.4
# Sat, 02 May 2020 01:27:03 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 02 May 2020 01:27:03 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Sat, 02 May 2020 01:27:03 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Sat, 02 May 2020 01:27:03 GMT
EXPOSE 8888
# Sat, 02 May 2020 01:27:03 GMT
VOLUME [/var/lib/chronograf]
# Sat, 02 May 2020 01:27:04 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Sat, 02 May 2020 01:27:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 May 2020 01:27:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c949b60b63fb4b31e70314aba2aff2223f42a54c0d76cdb28917f161840b03`  
		Last Modified: Fri, 24 Apr 2020 14:16:39 GMT  
		Size: 301.1 KB (301092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9886928cc4adb52f7382fa144b66b2d2a8a508ee2a4327ed178a71ea5ea8d130`  
		Last Modified: Sat, 02 May 2020 01:27:31 GMT  
		Size: 22.2 MB (22233530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae424a8fe97aa2e30aa46019e00e82148076cded0664c8debe82ab7644110f70`  
		Last Modified: Sat, 02 May 2020 01:27:27 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7827a9189ac3387dea82ad1cd2d58d43376e50f63d167387049799e1ed4d3a6`  
		Last Modified: Sat, 02 May 2020 01:27:27 GMT  
		Size: 11.9 KB (11896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c01e2f7cf40f95c6fc4f1db94488161f473d4ed489b6ddf9ee36103412436b6`  
		Last Modified: Sat, 02 May 2020 01:27:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8-alpine`

```console
$ docker pull chronograf@sha256:a98e8a764382260af789cf3fd24952e5a5e1eea2568eda7a60a51678662920e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:7b9fd4bfa461dd588069a6662e7a23eec428fbd0ed24382e7a80ec2dacbea40a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25332562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:424098e734c5096176c639a03764d77e23d8b41e93efd2283b5b4363b6a8b837`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:15:55 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Sat, 02 May 2020 01:26:58 GMT
ENV CHRONOGRAF_VERSION=1.8.4
# Sat, 02 May 2020 01:27:03 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 02 May 2020 01:27:03 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Sat, 02 May 2020 01:27:03 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Sat, 02 May 2020 01:27:03 GMT
EXPOSE 8888
# Sat, 02 May 2020 01:27:03 GMT
VOLUME [/var/lib/chronograf]
# Sat, 02 May 2020 01:27:04 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Sat, 02 May 2020 01:27:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 May 2020 01:27:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c949b60b63fb4b31e70314aba2aff2223f42a54c0d76cdb28917f161840b03`  
		Last Modified: Fri, 24 Apr 2020 14:16:39 GMT  
		Size: 301.1 KB (301092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9886928cc4adb52f7382fa144b66b2d2a8a508ee2a4327ed178a71ea5ea8d130`  
		Last Modified: Sat, 02 May 2020 01:27:31 GMT  
		Size: 22.2 MB (22233530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae424a8fe97aa2e30aa46019e00e82148076cded0664c8debe82ab7644110f70`  
		Last Modified: Sat, 02 May 2020 01:27:27 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7827a9189ac3387dea82ad1cd2d58d43376e50f63d167387049799e1ed4d3a6`  
		Last Modified: Sat, 02 May 2020 01:27:27 GMT  
		Size: 11.9 KB (11896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c01e2f7cf40f95c6fc4f1db94488161f473d4ed489b6ddf9ee36103412436b6`  
		Last Modified: Sat, 02 May 2020 01:27:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:a98e8a764382260af789cf3fd24952e5a5e1eea2568eda7a60a51678662920e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:7b9fd4bfa461dd588069a6662e7a23eec428fbd0ed24382e7a80ec2dacbea40a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25332562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:424098e734c5096176c639a03764d77e23d8b41e93efd2283b5b4363b6a8b837`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:15:55 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Sat, 02 May 2020 01:26:58 GMT
ENV CHRONOGRAF_VERSION=1.8.4
# Sat, 02 May 2020 01:27:03 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 02 May 2020 01:27:03 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Sat, 02 May 2020 01:27:03 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Sat, 02 May 2020 01:27:03 GMT
EXPOSE 8888
# Sat, 02 May 2020 01:27:03 GMT
VOLUME [/var/lib/chronograf]
# Sat, 02 May 2020 01:27:04 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Sat, 02 May 2020 01:27:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 May 2020 01:27:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c949b60b63fb4b31e70314aba2aff2223f42a54c0d76cdb28917f161840b03`  
		Last Modified: Fri, 24 Apr 2020 14:16:39 GMT  
		Size: 301.1 KB (301092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9886928cc4adb52f7382fa144b66b2d2a8a508ee2a4327ed178a71ea5ea8d130`  
		Last Modified: Sat, 02 May 2020 01:27:31 GMT  
		Size: 22.2 MB (22233530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae424a8fe97aa2e30aa46019e00e82148076cded0664c8debe82ab7644110f70`  
		Last Modified: Sat, 02 May 2020 01:27:27 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7827a9189ac3387dea82ad1cd2d58d43376e50f63d167387049799e1ed4d3a6`  
		Last Modified: Sat, 02 May 2020 01:27:27 GMT  
		Size: 11.9 KB (11896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c01e2f7cf40f95c6fc4f1db94488161f473d4ed489b6ddf9ee36103412436b6`  
		Last Modified: Sat, 02 May 2020 01:27:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:latest`

```console
$ docker pull chronograf@sha256:c7f40088278d5a27cafb36beb0ac95635b1b4ac22ff49099657b350c19862572
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:ec6abdcd7f5b296740484abcc2c50808fac3ca8bab21e5197bae1d54e608fb4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70190648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b507b55579c8643f99c0e45087533bd4eea3a51b8fe13531d84200afa71c7c62`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:23:54 GMT
ADD file:3e0b81347262efc5a7401a531be7ab45cb8ab05ddab528fbb849bea0053865a0 in / 
# Wed, 13 May 2020 21:23:54 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:49:29 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 May 2020 21:50:14 GMT
ENV CHRONOGRAF_VERSION=1.8.4
# Wed, 13 May 2020 21:50:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 21:50:29 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 13 May 2020 21:50:29 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 13 May 2020 21:50:29 GMT
EXPOSE 8888
# Wed, 13 May 2020 21:50:29 GMT
VOLUME [/var/lib/chronograf]
# Wed, 13 May 2020 21:50:29 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 13 May 2020 21:50:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 May 2020 21:50:30 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:e4f2068f62324fe92e80c472afb3742bf506f2a52712bf36ec0456de94c5b14e`  
		Last Modified: Wed, 13 May 2020 21:30:12 GMT  
		Size: 22.5 MB (22513438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38860158577867e1380349aea84937148611cf6b106ffb79d992e6a16ebc1ae6`  
		Last Modified: Wed, 13 May 2020 21:50:46 GMT  
		Size: 4.5 MB (4503528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94933266b7ae6468cd742a09a59f371990d4011115537da31cd50578069ffaa2`  
		Last Modified: Wed, 13 May 2020 21:51:16 GMT  
		Size: 43.1 MB (43149286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c505f60cd8d7c0ffd0216fa998dbf11bb7a99deaadb7a4e23cd5c56839177d4a`  
		Last Modified: Wed, 13 May 2020 21:51:08 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620985d2330acf8fd76beaec79d986c00a9569cd7f5367f398f388971c6451bf`  
		Last Modified: Wed, 13 May 2020 21:51:09 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e84220ec6583225f482e47f3786e86140e1384cd6550d4055301ed727407ce0`  
		Last Modified: Wed, 13 May 2020 21:51:09 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:b370d27051108c28aad8241bac9933bbc8a5a1aa595b66efa403e3fd9b6d7f27
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63604009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0e271719a01339c37a45578b291d4758efddb12e832fec09e9fb43eea837884`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:24:26 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 May 2020 22:25:57 GMT
ENV CHRONOGRAF_VERSION=1.8.4
# Wed, 13 May 2020 22:26:24 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 22:26:25 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 13 May 2020 22:26:27 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 13 May 2020 22:26:28 GMT
EXPOSE 8888
# Wed, 13 May 2020 22:26:29 GMT
VOLUME [/var/lib/chronograf]
# Wed, 13 May 2020 22:26:30 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 13 May 2020 22:26:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 May 2020 22:26:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b980babbd6be63c990cc1f3d2d047bc1565f0e663b62e0e6f3e9e93614c41c`  
		Last Modified: Wed, 13 May 2020 22:26:46 GMT  
		Size: 3.9 MB (3877340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1fb4e47638fe2863e805d69b4f04971ec7f081271bc32194dc6a925e291eac`  
		Last Modified: Wed, 13 May 2020 22:27:29 GMT  
		Size: 40.4 MB (40403801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a588b516876bed658396d4eb66ddf6a8bbabb9b5d281f131655035fafe2b43`  
		Last Modified: Wed, 13 May 2020 22:27:17 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4435550515dbdd574a03f7fde63e89aec97b1643312411a70af16917c23db5`  
		Last Modified: Wed, 13 May 2020 22:27:17 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb2cd4a1df1196c3949f80f4a9f6904bec5d072ebfc2b8a0e0222299692e770`  
		Last Modified: Wed, 13 May 2020 22:27:17 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:9369dc6d98735f8b79bc1076d9be8e1517452fa5a796be7c90186b5b77c15ac5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64714374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bc19e90c0f79e3da3fbf0d4892bfb01ff957566c7d97f0f0d0a5e29e7ae6d40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:49:14 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 14 May 2020 00:50:22 GMT
ENV CHRONOGRAF_VERSION=1.8.4
# Thu, 14 May 2020 00:50:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 14 May 2020 00:50:44 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 14 May 2020 00:50:44 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 14 May 2020 00:50:45 GMT
EXPOSE 8888
# Thu, 14 May 2020 00:50:46 GMT
VOLUME [/var/lib/chronograf]
# Thu, 14 May 2020 00:50:47 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 14 May 2020 00:50:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 May 2020 00:50:48 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27009d9d4e56d600926f21a2fcea7fd9cd9faaf8a0aa1dc3d91e1bb89f5b654d`  
		Last Modified: Thu, 14 May 2020 00:51:01 GMT  
		Size: 4.1 MB (4080587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a71fe07ad9b05ef55473a46159658ea8427311e4bc8b39a9ae6d384dd5c1f63`  
		Last Modified: Thu, 14 May 2020 00:51:36 GMT  
		Size: 40.2 MB (40239346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e534e3a2953b36d5d1ebc359f5338af4eaf36d7e709f31df4bf6a235e6ee20be`  
		Last Modified: Thu, 14 May 2020 00:51:27 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f34bd489cf7347846985910cb4e2513fd2760d84d00ea520c54686b14009813`  
		Last Modified: Thu, 14 May 2020 00:51:26 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8f7e28ce4718da060028d491bbb042da94690056e2c737956a4ca6ab891879`  
		Last Modified: Thu, 14 May 2020 00:51:26 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
