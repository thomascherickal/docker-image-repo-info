## `chronograf:latest`

```console
$ docker pull chronograf@sha256:750ca1c63b4c3ef1acc99d4a2cf8320f78b19c653403c4f69ec3a3bc5e67ecb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:dbc2c61a84e72db77fa9f2da381c0268db8dc74dbb6820b76d08b10b1988db1e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70443794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f07c735db5e077a7ae57f6216fec094bc3b975979ab304a059604dc5f145faf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:17 GMT
ADD file:55a25b93e8f2940a796f3cbf1e78bddf5f49c46b1b89b63b9b5673cbed9483ca in / 
# Thu, 22 Jul 2021 00:47:17 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:24:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 01:24:53 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Thu, 22 Jul 2021 01:25:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 01:25:01 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 22 Jul 2021 01:25:02 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Jul 2021 01:25:02 GMT
EXPOSE 8888
# Thu, 22 Jul 2021 01:25:02 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Jul 2021 01:25:02 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 22 Jul 2021 01:25:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 01:25:03 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:778066204fb734c2fb80cb8127cb35d67d742806a4eaf1aba0b5393c4ae6f2a4`  
		Last Modified: Thu, 22 Jul 2021 00:53:22 GMT  
		Size: 22.5 MB (22527428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ff0af07da1ef7cf177b743e7ad0a7624265bf35374bcd2570af99c1be4eea9`  
		Last Modified: Thu, 22 Jul 2021 01:25:27 GMT  
		Size: 6.8 MB (6760219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f0c0740080eb1beb0bafc38e6302c80ab58a56cd623d417c394b231d55d2a9`  
		Last Modified: Thu, 22 Jul 2021 01:26:04 GMT  
		Size: 41.1 MB (41131759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87cfa89e6cb17bd471dd756aad021cff94fe738e0b8908ebedaeb2496916554`  
		Last Modified: Thu, 22 Jul 2021 01:25:58 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bfeee62a671086588e9c04f66c454fb68ecee8c66dbe508743ef70e5974b66`  
		Last Modified: Thu, 22 Jul 2021 01:25:59 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d1ef1a0aa9a111a5fd29bfab71dae1eb2f860cdb6745adbca31962564a9d08`  
		Last Modified: Thu, 22 Jul 2021 01:25:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:aaa12f3421fbcc2da74abf990ee7e7515ef96f85710f3361d890a52991d3d8d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59617640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065f7eaeabb6ce83c6ac6cb1cfe4e40568460463aa8b45664a6797fbec021dee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 02:07:27 GMT
ADD file:86bd875241ca751f2f50a9c3504cfca4ce772411fed23fe6893299a271c275e3 in / 
# Thu, 22 Jul 2021 02:07:28 GMT
CMD ["bash"]
# Tue, 10 Aug 2021 23:00:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 10 Aug 2021 23:02:02 GMT
ENV CHRONOGRAF_VERSION=1.8.9
# Tue, 10 Aug 2021 23:02:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 10 Aug 2021 23:02:22 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 10 Aug 2021 23:02:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 10 Aug 2021 23:02:23 GMT
EXPOSE 8888
# Tue, 10 Aug 2021 23:02:24 GMT
VOLUME [/var/lib/chronograf]
# Tue, 10 Aug 2021 23:02:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 10 Aug 2021 23:02:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Aug 2021 23:02:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:37325b08023150a9e16c0c8d98d10daa998ce21ec3b9226cc6f0148a245a8a57`  
		Last Modified: Thu, 22 Jul 2021 02:21:16 GMT  
		Size: 19.3 MB (19315955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84236a4145013894eb753d54367ba39e700f41448379d11fb8acf79e2100e630`  
		Last Modified: Tue, 10 Aug 2021 23:03:14 GMT  
		Size: 5.8 MB (5779562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563aa1050ffeff783f5c0ace0c0d4c26bf42c55be8a64652b976ba2242844480`  
		Last Modified: Tue, 10 Aug 2021 23:04:29 GMT  
		Size: 34.5 MB (34497735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33390c7d3a170ef269b4e0664ab92012f5e8a0be393ea68452543bc3805dd86`  
		Last Modified: Tue, 10 Aug 2021 23:04:10 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63513570675210dbda0283a576386daa6c1305131230de9124c5a42c5b9ede1`  
		Last Modified: Tue, 10 Aug 2021 23:04:11 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001f573921c3e4fda4891864bdc68ad985bbec2316df915bf5b962fb9cc9cced`  
		Last Modified: Tue, 10 Aug 2021 23:04:10 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:f16a60124e199840257f215b25bf2347840a341f56c2b50eb6ccfb47740c6c47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64970233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7e052aba53be0451400f0ec90d1cbd1cf089dfe6b31480453fcc5f21a74d8d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:40 GMT
ADD file:b39a01b3af7a531df3592571b7f6eaa7efd20919858f7f0cd2ddf1c1eceb078d in / 
# Thu, 22 Jul 2021 00:41:40 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:11:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 01:12:23 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Thu, 22 Jul 2021 01:12:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 22 Jul 2021 01:12:31 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 22 Jul 2021 01:12:31 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 22 Jul 2021 01:12:31 GMT
EXPOSE 8888
# Thu, 22 Jul 2021 01:12:31 GMT
VOLUME [/var/lib/chronograf]
# Thu, 22 Jul 2021 01:12:31 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 22 Jul 2021 01:12:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 01:12:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9e7a560784c85cb9624bff5b6e479fbb95d5e265873987014f8aec75d509a530`  
		Last Modified: Thu, 22 Jul 2021 00:48:50 GMT  
		Size: 20.4 MB (20389427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58364f3e37bf6b8fd81d518b8f7e5a5c8b7e7ac6f79faf0c99101ffcef189204`  
		Last Modified: Thu, 22 Jul 2021 01:12:56 GMT  
		Size: 6.0 MB (6047477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4b587acd1b705f40e13a6f37bde0255703ed113b71c608ddd2f398cbe2f40e`  
		Last Modified: Thu, 22 Jul 2021 01:13:36 GMT  
		Size: 38.5 MB (38508940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2161d973333f7691e631e2063f505a6e800edf211cca030fd5cf083eeb62ed5`  
		Last Modified: Thu, 22 Jul 2021 01:13:30 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0bf9aa56a41dfc971d38fa9b8c9fdcacbe80ea7f7bed40138fc47a30072709`  
		Last Modified: Thu, 22 Jul 2021 01:13:30 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145897592d2b460b30d22c92b220ab150f0af94c742f79505897d3c5c386124d`  
		Last Modified: Thu, 22 Jul 2021 01:13:31 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
