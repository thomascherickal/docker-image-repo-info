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
$ docker pull chronograf@sha256:837209ffbc9c2152f9c7517ea8f479cc83ad9d6a9e4b472c9a0f8f84c5bd4cb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6` - linux; amd64

```console
$ docker pull chronograf@sha256:15d69f88c78fc993e239344a667d867a16cf3036fa85bb9c0ef0978d6350f73f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49339213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbc24ccb5be15bf65bde27ae4676d1113a0ca2bdfce97c1e16fc68c83e4bab4d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:30 GMT
ADD file:da0c935ddc86ca9e44bdd5f61b46c7b43a115ee4bc356324265a7ad6323f61ae in / 
# Tue, 09 Feb 2021 02:23:30 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:46:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Feb 2021 02:46:21 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 09 Feb 2021 02:46:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 02:46:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Feb 2021 02:46:31 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Feb 2021 02:46:31 GMT
EXPOSE 8888
# Tue, 09 Feb 2021 02:46:31 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Feb 2021 02:46:31 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 09 Feb 2021 02:46:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Feb 2021 02:46:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:cae7303ade7f17f84fe86b2a44880e9725cf7d6dcd17f79485360712b6af6dcd`  
		Last Modified: Tue, 09 Feb 2021 02:29:36 GMT  
		Size: 22.5 MB (22528600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603c713cc31395a01337edc5ae784741dda2d7aefb303bb93f7577486b1d1bbe`  
		Last Modified: Tue, 09 Feb 2021 02:47:56 GMT  
		Size: 6.7 MB (6742606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb264800cecf8165052770994afd137d006aca9ea58eb935e938faaf37456785`  
		Last Modified: Tue, 09 Feb 2021 02:47:58 GMT  
		Size: 20.0 MB (20043609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad14277e20368ba850ae45ad74343b73253d0b2e09955b70547cea209e15bc9`  
		Last Modified: Tue, 09 Feb 2021 02:47:53 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e230d3bd4c856bf3fd0f2235b0fb0b77a153d617f6a49a43a974aa2bae66485c`  
		Last Modified: Tue, 09 Feb 2021 02:47:53 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee67c6ec7750a2447c2f9b027624c9aa158255f2f6ebed9f0eab3044b4a887f`  
		Last Modified: Tue, 09 Feb 2021 02:47:53 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:d0d3b9d07ddecd6a78a3340619110666e7e5dd72401503c70ec548cbc98b0880
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43921665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:566476e1edf92fe35d41a805b26f6a80220cda7818ed0ba960c5753793bc9f29`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:44 GMT
ADD file:31b268030b071d84c09e225f80f0552bc4869000d8be3321e1046de8ff0f44e2 in / 
# Tue, 12 Jan 2021 00:05:47 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:07:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 01:07:37 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 12 Jan 2021 01:07:51 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 01:07:52 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 12 Jan 2021 01:07:53 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 12 Jan 2021 01:07:54 GMT
EXPOSE 8888
# Tue, 12 Jan 2021 01:07:55 GMT
VOLUME [/var/lib/chronograf]
# Tue, 12 Jan 2021 01:07:55 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 12 Jan 2021 01:07:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 01:07:57 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0528b39c7eddf3a960919da4e91c41f304ecd9b26b5d04a6f7e80aedf265e78c`  
		Last Modified: Tue, 12 Jan 2021 00:15:54 GMT  
		Size: 19.3 MB (19315991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f4127298f0c323dd5825d1a04aac0766454af692c736bb4e0f694997674d13`  
		Last Modified: Tue, 12 Jan 2021 01:09:37 GMT  
		Size: 5.8 MB (5764894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da7ba5e30310b9ba619b0f0a3806ef0ada977759d811b944750632ec4184b70`  
		Last Modified: Tue, 12 Jan 2021 01:09:42 GMT  
		Size: 18.8 MB (18816387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ba999b35380400d3e7b31576420bc90e9f4d8cfddf42c34cd1fd550dd33e10`  
		Last Modified: Tue, 12 Jan 2021 01:09:36 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a895344d2dc5b82aa293cc3cd0d437ab2f529a31af3b45d154730a7ae4d7d1`  
		Last Modified: Tue, 12 Jan 2021 01:09:35 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b9bac54f8223f05a4dde78c899cbfd8a81c55d9cdf86eedb54e4fff0e93203`  
		Last Modified: Tue, 12 Jan 2021 01:09:35 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:01be822b7493fdefdb31df8567ea281109692b8294f0811865deed3697665cbe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45400388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3decb9b5aee14ca5d09e6573ee01e398a359543365c58b48862b88a274983a2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Feb 2021 02:43:38 GMT
ADD file:ec0f3f5aad51202b992acbfa7ec19738608d022983bc1918d7d9eecdd35e4800 in / 
# Tue, 09 Feb 2021 02:43:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:28:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Feb 2021 04:28:55 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 09 Feb 2021 04:29:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 04:29:09 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Feb 2021 04:29:10 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Feb 2021 04:29:11 GMT
EXPOSE 8888
# Tue, 09 Feb 2021 04:29:12 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Feb 2021 04:29:13 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 09 Feb 2021 04:29:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Feb 2021 04:29:14 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b373a42fa9174db1e441a19411c9622d41f6db219878945ed0cb256efa32c8a6`  
		Last Modified: Tue, 09 Feb 2021 02:50:08 GMT  
		Size: 20.4 MB (20389427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b4b210d138fd2393967f174396ed44ec8cbf98472a90f6928614b79905e1c7`  
		Last Modified: Tue, 09 Feb 2021 04:31:00 GMT  
		Size: 6.0 MB (6028114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92463e9a64f743107a35bac7cfcedc0470f56389efb30c60810b31b7474d418`  
		Last Modified: Tue, 09 Feb 2021 04:31:04 GMT  
		Size: 19.0 MB (18958459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56eb95e3ddaeefa987c0beedb2b0ed5644c5fd82be58396027e8fdb0bb9499cc`  
		Last Modified: Tue, 09 Feb 2021 04:30:58 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc12ab819f226c9f8e8bc5caa63d917b2801e29fafac3d4273b943c56018701`  
		Last Modified: Tue, 09 Feb 2021 04:30:58 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec61cd44099f0548fdb0ee56ca7b5004eb7c68d7fbc0313990476590501f455`  
		Last Modified: Tue, 09 Feb 2021 04:30:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2`

```console
$ docker pull chronograf@sha256:837209ffbc9c2152f9c7517ea8f479cc83ad9d6a9e4b472c9a0f8f84c5bd4cb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6.2` - linux; amd64

```console
$ docker pull chronograf@sha256:15d69f88c78fc993e239344a667d867a16cf3036fa85bb9c0ef0978d6350f73f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49339213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbc24ccb5be15bf65bde27ae4676d1113a0ca2bdfce97c1e16fc68c83e4bab4d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:30 GMT
ADD file:da0c935ddc86ca9e44bdd5f61b46c7b43a115ee4bc356324265a7ad6323f61ae in / 
# Tue, 09 Feb 2021 02:23:30 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:46:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Feb 2021 02:46:21 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 09 Feb 2021 02:46:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 02:46:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Feb 2021 02:46:31 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Feb 2021 02:46:31 GMT
EXPOSE 8888
# Tue, 09 Feb 2021 02:46:31 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Feb 2021 02:46:31 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 09 Feb 2021 02:46:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Feb 2021 02:46:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:cae7303ade7f17f84fe86b2a44880e9725cf7d6dcd17f79485360712b6af6dcd`  
		Last Modified: Tue, 09 Feb 2021 02:29:36 GMT  
		Size: 22.5 MB (22528600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603c713cc31395a01337edc5ae784741dda2d7aefb303bb93f7577486b1d1bbe`  
		Last Modified: Tue, 09 Feb 2021 02:47:56 GMT  
		Size: 6.7 MB (6742606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb264800cecf8165052770994afd137d006aca9ea58eb935e938faaf37456785`  
		Last Modified: Tue, 09 Feb 2021 02:47:58 GMT  
		Size: 20.0 MB (20043609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad14277e20368ba850ae45ad74343b73253d0b2e09955b70547cea209e15bc9`  
		Last Modified: Tue, 09 Feb 2021 02:47:53 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e230d3bd4c856bf3fd0f2235b0fb0b77a153d617f6a49a43a974aa2bae66485c`  
		Last Modified: Tue, 09 Feb 2021 02:47:53 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee67c6ec7750a2447c2f9b027624c9aa158255f2f6ebed9f0eab3044b4a887f`  
		Last Modified: Tue, 09 Feb 2021 02:47:53 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:d0d3b9d07ddecd6a78a3340619110666e7e5dd72401503c70ec548cbc98b0880
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43921665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:566476e1edf92fe35d41a805b26f6a80220cda7818ed0ba960c5753793bc9f29`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:44 GMT
ADD file:31b268030b071d84c09e225f80f0552bc4869000d8be3321e1046de8ff0f44e2 in / 
# Tue, 12 Jan 2021 00:05:47 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:07:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 01:07:37 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 12 Jan 2021 01:07:51 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 01:07:52 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 12 Jan 2021 01:07:53 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 12 Jan 2021 01:07:54 GMT
EXPOSE 8888
# Tue, 12 Jan 2021 01:07:55 GMT
VOLUME [/var/lib/chronograf]
# Tue, 12 Jan 2021 01:07:55 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 12 Jan 2021 01:07:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 01:07:57 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0528b39c7eddf3a960919da4e91c41f304ecd9b26b5d04a6f7e80aedf265e78c`  
		Last Modified: Tue, 12 Jan 2021 00:15:54 GMT  
		Size: 19.3 MB (19315991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f4127298f0c323dd5825d1a04aac0766454af692c736bb4e0f694997674d13`  
		Last Modified: Tue, 12 Jan 2021 01:09:37 GMT  
		Size: 5.8 MB (5764894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da7ba5e30310b9ba619b0f0a3806ef0ada977759d811b944750632ec4184b70`  
		Last Modified: Tue, 12 Jan 2021 01:09:42 GMT  
		Size: 18.8 MB (18816387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ba999b35380400d3e7b31576420bc90e9f4d8cfddf42c34cd1fd550dd33e10`  
		Last Modified: Tue, 12 Jan 2021 01:09:36 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a895344d2dc5b82aa293cc3cd0d437ab2f529a31af3b45d154730a7ae4d7d1`  
		Last Modified: Tue, 12 Jan 2021 01:09:35 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b9bac54f8223f05a4dde78c899cbfd8a81c55d9cdf86eedb54e4fff0e93203`  
		Last Modified: Tue, 12 Jan 2021 01:09:35 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:01be822b7493fdefdb31df8567ea281109692b8294f0811865deed3697665cbe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45400388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3decb9b5aee14ca5d09e6573ee01e398a359543365c58b48862b88a274983a2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Feb 2021 02:43:38 GMT
ADD file:ec0f3f5aad51202b992acbfa7ec19738608d022983bc1918d7d9eecdd35e4800 in / 
# Tue, 09 Feb 2021 02:43:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:28:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Feb 2021 04:28:55 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 09 Feb 2021 04:29:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 04:29:09 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Feb 2021 04:29:10 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Feb 2021 04:29:11 GMT
EXPOSE 8888
# Tue, 09 Feb 2021 04:29:12 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Feb 2021 04:29:13 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 09 Feb 2021 04:29:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Feb 2021 04:29:14 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b373a42fa9174db1e441a19411c9622d41f6db219878945ed0cb256efa32c8a6`  
		Last Modified: Tue, 09 Feb 2021 02:50:08 GMT  
		Size: 20.4 MB (20389427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b4b210d138fd2393967f174396ed44ec8cbf98472a90f6928614b79905e1c7`  
		Last Modified: Tue, 09 Feb 2021 04:31:00 GMT  
		Size: 6.0 MB (6028114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92463e9a64f743107a35bac7cfcedc0470f56389efb30c60810b31b7474d418`  
		Last Modified: Tue, 09 Feb 2021 04:31:04 GMT  
		Size: 19.0 MB (18958459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56eb95e3ddaeefa987c0beedb2b0ed5644c5fd82be58396027e8fdb0bb9499cc`  
		Last Modified: Tue, 09 Feb 2021 04:30:58 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc12ab819f226c9f8e8bc5caa63d917b2801e29fafac3d4273b943c56018701`  
		Last Modified: Tue, 09 Feb 2021 04:30:58 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec61cd44099f0548fdb0ee56ca7b5004eb7c68d7fbc0313990476590501f455`  
		Last Modified: Tue, 09 Feb 2021 04:30:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2-alpine`

```console
$ docker pull chronograf@sha256:bd7d078f68d37dae6c306bb60381931b31ffe20e8f05a61403799ddb964b2b80
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.6.2-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:aa8153e9564955c6440b2e9f3fbd01b3b56353d85d4507606f089481d64e5846
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14841160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1fab9bc646ca060d41a5475ff0f189c919fe6c6972d60ad848096a4b195cc70`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:07:54 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:07:54 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 17 Dec 2020 13:07:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:07:58 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Thu, 17 Dec 2020 13:07:58 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Dec 2020 13:07:58 GMT
EXPOSE 8888
# Thu, 17 Dec 2020 13:07:59 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Dec 2020 13:07:59 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:07:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:08:00 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac210e4df99beaffbde65dfe580e9923c2bef3b5dd07f0ac7d364e47dc2fac52`  
		Last Modified: Thu, 17 Dec 2020 13:09:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2a689ddee3aadca4971508078c3d8f60b8fdbeb3ee260f4212e3b37c6548cf`  
		Last Modified: Thu, 17 Dec 2020 13:09:08 GMT  
		Size: 280.8 KB (280803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830afd193f17a2708e0e0aed04bc824eaf599194e09caf8127dc1bbcbf8ece4a`  
		Last Modified: Thu, 17 Dec 2020 13:09:10 GMT  
		Size: 11.7 MB (11736759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568e1862a75c54417677f0c9d54e5a43babc8f3c1f95b290ed038759a38fa2b5`  
		Last Modified: Thu, 17 Dec 2020 13:09:08 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4073eade77f18f605f564f645f9193c2cdd47d3de4c6c58212c1e1509bfcbc`  
		Last Modified: Thu, 17 Dec 2020 13:09:07 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8429486153b5eb8648d218ae483630085735e59481e96257695f4d3accdd43`  
		Last Modified: Thu, 17 Dec 2020 13:09:07 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6-alpine`

```console
$ docker pull chronograf@sha256:bd7d078f68d37dae6c306bb60381931b31ffe20e8f05a61403799ddb964b2b80
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.6-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:aa8153e9564955c6440b2e9f3fbd01b3b56353d85d4507606f089481d64e5846
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14841160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1fab9bc646ca060d41a5475ff0f189c919fe6c6972d60ad848096a4b195cc70`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:07:54 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:07:54 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Thu, 17 Dec 2020 13:07:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:07:58 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Thu, 17 Dec 2020 13:07:58 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Dec 2020 13:07:58 GMT
EXPOSE 8888
# Thu, 17 Dec 2020 13:07:59 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Dec 2020 13:07:59 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:07:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:08:00 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac210e4df99beaffbde65dfe580e9923c2bef3b5dd07f0ac7d364e47dc2fac52`  
		Last Modified: Thu, 17 Dec 2020 13:09:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2a689ddee3aadca4971508078c3d8f60b8fdbeb3ee260f4212e3b37c6548cf`  
		Last Modified: Thu, 17 Dec 2020 13:09:08 GMT  
		Size: 280.8 KB (280803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830afd193f17a2708e0e0aed04bc824eaf599194e09caf8127dc1bbcbf8ece4a`  
		Last Modified: Thu, 17 Dec 2020 13:09:10 GMT  
		Size: 11.7 MB (11736759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568e1862a75c54417677f0c9d54e5a43babc8f3c1f95b290ed038759a38fa2b5`  
		Last Modified: Thu, 17 Dec 2020 13:09:08 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4073eade77f18f605f564f645f9193c2cdd47d3de4c6c58212c1e1509bfcbc`  
		Last Modified: Thu, 17 Dec 2020 13:09:07 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8429486153b5eb8648d218ae483630085735e59481e96257695f4d3accdd43`  
		Last Modified: Thu, 17 Dec 2020 13:09:07 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7`

```console
$ docker pull chronograf@sha256:c67074a3a174b0074b95af9315e4150d72c0944b5962e846c96130f1989f3c95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:922cb1501665af987f94a25294737445d1e750cfa3f8eaabf2c331be1d54e6d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65367021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68daff9cf85806cd4af73110736d39c50ee36742dc4d63a14fb2fda186a72cb3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:30 GMT
ADD file:da0c935ddc86ca9e44bdd5f61b46c7b43a115ee4bc356324265a7ad6323f61ae in / 
# Tue, 09 Feb 2021 02:23:30 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:46:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Feb 2021 02:46:52 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 09 Feb 2021 02:47:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 02:47:05 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Feb 2021 02:47:05 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Feb 2021 02:47:05 GMT
EXPOSE 8888
# Tue, 09 Feb 2021 02:47:06 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Feb 2021 02:47:06 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 09 Feb 2021 02:47:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Feb 2021 02:47:06 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:cae7303ade7f17f84fe86b2a44880e9725cf7d6dcd17f79485360712b6af6dcd`  
		Last Modified: Tue, 09 Feb 2021 02:29:36 GMT  
		Size: 22.5 MB (22528600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4311468ad10eee51ca97c75df7615a5d0af76d156b6824a7dfb244b8694016a2`  
		Last Modified: Tue, 09 Feb 2021 02:48:08 GMT  
		Size: 4.5 MB (4504899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da961c36214e89fbf909b0c9fb9a969ec955522bcb12630f37000ea4fde1777`  
		Last Modified: Tue, 09 Feb 2021 02:48:22 GMT  
		Size: 38.3 MB (38309126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750f9108344712250c9e2212694c183c2a1ab46aa21d48358cf9d5fd13ce2960`  
		Last Modified: Tue, 09 Feb 2021 02:48:07 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815008e187db7862ee0c7be568d20df2ef54553814a42b16b8355e95d5c8d896`  
		Last Modified: Tue, 09 Feb 2021 02:48:07 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3755893fcd8e74505c6b1ac0f7b0d69ac72d8cf813930d4bee368b9199a6be`  
		Last Modified: Tue, 09 Feb 2021 02:48:10 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:08340123b60d3fa2b987502b8b4e1108eff8b615b48b06a347007dc9af8da16c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58972179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e481a6fc11a52cd2c7ced262c0876a6cac4ccf370a9159b1dd690c8dcb487a14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:44 GMT
ADD file:31b268030b071d84c09e225f80f0552bc4869000d8be3321e1046de8ff0f44e2 in / 
# Tue, 12 Jan 2021 00:05:47 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:08:20 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 01:08:21 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 12 Jan 2021 01:08:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 01:08:41 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 12 Jan 2021 01:08:42 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 12 Jan 2021 01:08:43 GMT
EXPOSE 8888
# Tue, 12 Jan 2021 01:08:43 GMT
VOLUME [/var/lib/chronograf]
# Tue, 12 Jan 2021 01:08:44 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 12 Jan 2021 01:08:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 01:08:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0528b39c7eddf3a960919da4e91c41f304ecd9b26b5d04a6f7e80aedf265e78c`  
		Last Modified: Tue, 12 Jan 2021 00:15:54 GMT  
		Size: 19.3 MB (19315991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568f26d93b85c4004aab1a3540235786cac21ea3e6514faaaca5369446bd64db`  
		Last Modified: Tue, 12 Jan 2021 01:09:54 GMT  
		Size: 3.9 MB (3879477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bc73fc1b5186a81777e07417e261242112304faaec88b04d15d169cd4772cf`  
		Last Modified: Tue, 12 Jan 2021 01:10:01 GMT  
		Size: 35.8 MB (35752308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd758e1cd8e12d8963c1a0d44e2f20dbc00d2dcc3b4ea4579f1aaa740f3140c`  
		Last Modified: Tue, 12 Jan 2021 01:09:51 GMT  
		Size: 12.3 KB (12252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552a83f1ce379b388f365955c03d5fc3e9bfb5fc3d7d750bff1cc4ae73ab58e3`  
		Last Modified: Tue, 12 Jan 2021 01:09:51 GMT  
		Size: 11.9 KB (11912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:babbe8404c4602a657d969a4173bfe3e751f1f417eee397e729929dbe3c13cb7`  
		Last Modified: Tue, 12 Jan 2021 01:09:51 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:3fe817594497ba687c2c1e536381b429784146e989519d4c49aa9ec613d6bd7e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60457732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cf446bcaf7b66b3e70ecefcf89d426013ae7c91f98fb26cb84d3f127c7744e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Feb 2021 02:43:38 GMT
ADD file:ec0f3f5aad51202b992acbfa7ec19738608d022983bc1918d7d9eecdd35e4800 in / 
# Tue, 09 Feb 2021 02:43:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:29:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Feb 2021 04:29:40 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 09 Feb 2021 04:30:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 04:30:01 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Feb 2021 04:30:02 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Feb 2021 04:30:03 GMT
EXPOSE 8888
# Tue, 09 Feb 2021 04:30:04 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Feb 2021 04:30:05 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 09 Feb 2021 04:30:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Feb 2021 04:30:07 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b373a42fa9174db1e441a19411c9622d41f6db219878945ed0cb256efa32c8a6`  
		Last Modified: Tue, 09 Feb 2021 02:50:08 GMT  
		Size: 20.4 MB (20389427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f91f32ad810e3079afdb3990c2c5ea83a15f72ef79ce69080270a9d31808669`  
		Last Modified: Tue, 09 Feb 2021 04:31:13 GMT  
		Size: 4.1 MB (4082249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b58ac22f8956909038475f6de337b94e8c5515c3af8b2e002f64c573e6e39fe`  
		Last Modified: Tue, 09 Feb 2021 04:31:21 GMT  
		Size: 36.0 MB (35961660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2af3f87c317846b7282ade6031f461325b19d98ebd130777821ade96277a7e`  
		Last Modified: Tue, 09 Feb 2021 04:31:13 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9f2202400c8c35fbb38c5af4a2374c5001e193477d61489db80655e5c8f0ff`  
		Last Modified: Tue, 09 Feb 2021 04:31:13 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbda7d2fb58e598338ffad6c22fb43c0b845ae194e2513624332d8fe8ad0a50`  
		Last Modified: Tue, 09 Feb 2021 04:31:12 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17`

```console
$ docker pull chronograf@sha256:c67074a3a174b0074b95af9315e4150d72c0944b5962e846c96130f1989f3c95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:922cb1501665af987f94a25294737445d1e750cfa3f8eaabf2c331be1d54e6d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65367021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68daff9cf85806cd4af73110736d39c50ee36742dc4d63a14fb2fda186a72cb3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:30 GMT
ADD file:da0c935ddc86ca9e44bdd5f61b46c7b43a115ee4bc356324265a7ad6323f61ae in / 
# Tue, 09 Feb 2021 02:23:30 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:46:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Feb 2021 02:46:52 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 09 Feb 2021 02:47:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 02:47:05 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Feb 2021 02:47:05 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Feb 2021 02:47:05 GMT
EXPOSE 8888
# Tue, 09 Feb 2021 02:47:06 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Feb 2021 02:47:06 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 09 Feb 2021 02:47:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Feb 2021 02:47:06 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:cae7303ade7f17f84fe86b2a44880e9725cf7d6dcd17f79485360712b6af6dcd`  
		Last Modified: Tue, 09 Feb 2021 02:29:36 GMT  
		Size: 22.5 MB (22528600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4311468ad10eee51ca97c75df7615a5d0af76d156b6824a7dfb244b8694016a2`  
		Last Modified: Tue, 09 Feb 2021 02:48:08 GMT  
		Size: 4.5 MB (4504899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da961c36214e89fbf909b0c9fb9a969ec955522bcb12630f37000ea4fde1777`  
		Last Modified: Tue, 09 Feb 2021 02:48:22 GMT  
		Size: 38.3 MB (38309126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750f9108344712250c9e2212694c183c2a1ab46aa21d48358cf9d5fd13ce2960`  
		Last Modified: Tue, 09 Feb 2021 02:48:07 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815008e187db7862ee0c7be568d20df2ef54553814a42b16b8355e95d5c8d896`  
		Last Modified: Tue, 09 Feb 2021 02:48:07 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3755893fcd8e74505c6b1ac0f7b0d69ac72d8cf813930d4bee368b9199a6be`  
		Last Modified: Tue, 09 Feb 2021 02:48:10 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:08340123b60d3fa2b987502b8b4e1108eff8b615b48b06a347007dc9af8da16c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58972179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e481a6fc11a52cd2c7ced262c0876a6cac4ccf370a9159b1dd690c8dcb487a14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:44 GMT
ADD file:31b268030b071d84c09e225f80f0552bc4869000d8be3321e1046de8ff0f44e2 in / 
# Tue, 12 Jan 2021 00:05:47 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:08:20 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 01:08:21 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 12 Jan 2021 01:08:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 01:08:41 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 12 Jan 2021 01:08:42 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 12 Jan 2021 01:08:43 GMT
EXPOSE 8888
# Tue, 12 Jan 2021 01:08:43 GMT
VOLUME [/var/lib/chronograf]
# Tue, 12 Jan 2021 01:08:44 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 12 Jan 2021 01:08:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 01:08:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0528b39c7eddf3a960919da4e91c41f304ecd9b26b5d04a6f7e80aedf265e78c`  
		Last Modified: Tue, 12 Jan 2021 00:15:54 GMT  
		Size: 19.3 MB (19315991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568f26d93b85c4004aab1a3540235786cac21ea3e6514faaaca5369446bd64db`  
		Last Modified: Tue, 12 Jan 2021 01:09:54 GMT  
		Size: 3.9 MB (3879477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bc73fc1b5186a81777e07417e261242112304faaec88b04d15d169cd4772cf`  
		Last Modified: Tue, 12 Jan 2021 01:10:01 GMT  
		Size: 35.8 MB (35752308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd758e1cd8e12d8963c1a0d44e2f20dbc00d2dcc3b4ea4579f1aaa740f3140c`  
		Last Modified: Tue, 12 Jan 2021 01:09:51 GMT  
		Size: 12.3 KB (12252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552a83f1ce379b388f365955c03d5fc3e9bfb5fc3d7d750bff1cc4ae73ab58e3`  
		Last Modified: Tue, 12 Jan 2021 01:09:51 GMT  
		Size: 11.9 KB (11912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:babbe8404c4602a657d969a4173bfe3e751f1f417eee397e729929dbe3c13cb7`  
		Last Modified: Tue, 12 Jan 2021 01:09:51 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:3fe817594497ba687c2c1e536381b429784146e989519d4c49aa9ec613d6bd7e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60457732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cf446bcaf7b66b3e70ecefcf89d426013ae7c91f98fb26cb84d3f127c7744e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Feb 2021 02:43:38 GMT
ADD file:ec0f3f5aad51202b992acbfa7ec19738608d022983bc1918d7d9eecdd35e4800 in / 
# Tue, 09 Feb 2021 02:43:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:29:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Feb 2021 04:29:40 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 09 Feb 2021 04:30:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 04:30:01 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Feb 2021 04:30:02 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Feb 2021 04:30:03 GMT
EXPOSE 8888
# Tue, 09 Feb 2021 04:30:04 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Feb 2021 04:30:05 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 09 Feb 2021 04:30:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Feb 2021 04:30:07 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b373a42fa9174db1e441a19411c9622d41f6db219878945ed0cb256efa32c8a6`  
		Last Modified: Tue, 09 Feb 2021 02:50:08 GMT  
		Size: 20.4 MB (20389427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f91f32ad810e3079afdb3990c2c5ea83a15f72ef79ce69080270a9d31808669`  
		Last Modified: Tue, 09 Feb 2021 04:31:13 GMT  
		Size: 4.1 MB (4082249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b58ac22f8956909038475f6de337b94e8c5515c3af8b2e002f64c573e6e39fe`  
		Last Modified: Tue, 09 Feb 2021 04:31:21 GMT  
		Size: 36.0 MB (35961660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2af3f87c317846b7282ade6031f461325b19d98ebd130777821ade96277a7e`  
		Last Modified: Tue, 09 Feb 2021 04:31:13 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9f2202400c8c35fbb38c5af4a2374c5001e193477d61489db80655e5c8f0ff`  
		Last Modified: Tue, 09 Feb 2021 04:31:13 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbda7d2fb58e598338ffad6c22fb43c0b845ae194e2513624332d8fe8ad0a50`  
		Last Modified: Tue, 09 Feb 2021 04:31:12 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17-alpine`

```console
$ docker pull chronograf@sha256:54fad03f8e069f7e70f040ce4c04de5fe587c3352c583e793d8555285526a6f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.7.17-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:d21af2c2d95e6db6999599ea80679e913ba9baddcb577fc185a6d7754cbb536d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22659644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae046a801abe2133da5e53d9ef4f2de4d327a5d31164f730f3bbc19726424ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:07:54 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:08:09 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 17 Dec 2020 13:08:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:08:15 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Dec 2020 13:08:15 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Dec 2020 13:08:16 GMT
EXPOSE 8888
# Thu, 17 Dec 2020 13:08:16 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Dec 2020 13:08:16 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:08:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:08:17 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac210e4df99beaffbde65dfe580e9923c2bef3b5dd07f0ac7d364e47dc2fac52`  
		Last Modified: Thu, 17 Dec 2020 13:09:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2a689ddee3aadca4971508078c3d8f60b8fdbeb3ee260f4212e3b37c6548cf`  
		Last Modified: Thu, 17 Dec 2020 13:09:08 GMT  
		Size: 280.8 KB (280803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f571a84c04c28e8a3810d586fb2b53322a1354a23bfa19cb77479a31431fe0`  
		Last Modified: Thu, 17 Dec 2020 13:09:27 GMT  
		Size: 19.6 MB (19555253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0367630ab9f7b67fc28dd908761fbc3410b5fb5184af54da530638c2f34658e`  
		Last Modified: Thu, 17 Dec 2020 13:09:20 GMT  
		Size: 12.2 KB (12234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e38591aa1abadf0a47ade4223ef0b3aeb95c267e441f391233dab229f5ae333`  
		Last Modified: Thu, 17 Dec 2020 13:09:19 GMT  
		Size: 11.9 KB (11897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbec67c014f65c027243bee64c9406f31452e71822868852e1beb0b4e334fa7`  
		Last Modified: Thu, 17 Dec 2020 13:09:20 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:54fad03f8e069f7e70f040ce4c04de5fe587c3352c583e793d8555285526a6f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.7-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:d21af2c2d95e6db6999599ea80679e913ba9baddcb577fc185a6d7754cbb536d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22659644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae046a801abe2133da5e53d9ef4f2de4d327a5d31164f730f3bbc19726424ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:07:54 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:08:09 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 17 Dec 2020 13:08:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:08:15 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Dec 2020 13:08:15 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Dec 2020 13:08:16 GMT
EXPOSE 8888
# Thu, 17 Dec 2020 13:08:16 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Dec 2020 13:08:16 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:08:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:08:17 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac210e4df99beaffbde65dfe580e9923c2bef3b5dd07f0ac7d364e47dc2fac52`  
		Last Modified: Thu, 17 Dec 2020 13:09:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2a689ddee3aadca4971508078c3d8f60b8fdbeb3ee260f4212e3b37c6548cf`  
		Last Modified: Thu, 17 Dec 2020 13:09:08 GMT  
		Size: 280.8 KB (280803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f571a84c04c28e8a3810d586fb2b53322a1354a23bfa19cb77479a31431fe0`  
		Last Modified: Thu, 17 Dec 2020 13:09:27 GMT  
		Size: 19.6 MB (19555253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0367630ab9f7b67fc28dd908761fbc3410b5fb5184af54da530638c2f34658e`  
		Last Modified: Thu, 17 Dec 2020 13:09:20 GMT  
		Size: 12.2 KB (12234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e38591aa1abadf0a47ade4223ef0b3aeb95c267e441f391233dab229f5ae333`  
		Last Modified: Thu, 17 Dec 2020 13:09:19 GMT  
		Size: 11.9 KB (11897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbec67c014f65c027243bee64c9406f31452e71822868852e1beb0b4e334fa7`  
		Last Modified: Thu, 17 Dec 2020 13:09:20 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8`

```console
$ docker pull chronograf@sha256:8d9ce545ee8f8a543dc71e30ad59341e9c56069bf4d02581f600e8f411c1aa72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:6bbfbbd73180964dbe313647223e80ee0e165ae05015db86639ba20f0f78931d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70424385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82d0154a00f46e5c1657d665aa2fc18c9c0242b2db7f64caa4e6658ed6b4ef60`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:30 GMT
ADD file:da0c935ddc86ca9e44bdd5f61b46c7b43a115ee4bc356324265a7ad6323f61ae in / 
# Tue, 09 Feb 2021 02:23:30 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:46:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Feb 2021 02:47:17 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 09 Feb 2021 02:47:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 02:47:27 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Feb 2021 02:47:27 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Feb 2021 02:47:28 GMT
EXPOSE 8888
# Tue, 09 Feb 2021 02:47:28 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Feb 2021 02:47:28 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 09 Feb 2021 02:47:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Feb 2021 02:47:29 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:cae7303ade7f17f84fe86b2a44880e9725cf7d6dcd17f79485360712b6af6dcd`  
		Last Modified: Tue, 09 Feb 2021 02:29:36 GMT  
		Size: 22.5 MB (22528600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603c713cc31395a01337edc5ae784741dda2d7aefb303bb93f7577486b1d1bbe`  
		Last Modified: Tue, 09 Feb 2021 02:47:56 GMT  
		Size: 6.7 MB (6742606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63600abc06b0687e4b24afa150d2da557c51a85b33e91502d51071591e5e6d82`  
		Last Modified: Tue, 09 Feb 2021 02:48:34 GMT  
		Size: 41.1 MB (41128782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3b434ef96cd8f4643d0c998ec73edb0b44c26d4e31cd5bca7c5f29b9400a0d`  
		Last Modified: Tue, 09 Feb 2021 02:48:27 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8145a040da7204ae6decb8f85b3096c06ade1972f6b6d4ab0496b789a24ce2`  
		Last Modified: Tue, 09 Feb 2021 02:48:27 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391ffb32b78cc26585c3ddd4ecc5590a8961c93e839ed73b88da29e4ad507ee7`  
		Last Modified: Tue, 09 Feb 2021 02:48:27 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:3da13b6796ebefd8fc57f33f36f900b12749991889ca27a55b92e61df695d0d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63839375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6afe2319f4923872211dd1c6fb7d6f7f1cf4ee339b6ee56524ea2152687f147b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:44 GMT
ADD file:31b268030b071d84c09e225f80f0552bc4869000d8be3321e1046de8ff0f44e2 in / 
# Tue, 12 Jan 2021 00:05:47 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:07:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 01:08:56 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 12 Jan 2021 01:09:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 01:09:12 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 12 Jan 2021 01:09:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 12 Jan 2021 01:09:13 GMT
EXPOSE 8888
# Tue, 12 Jan 2021 01:09:14 GMT
VOLUME [/var/lib/chronograf]
# Tue, 12 Jan 2021 01:09:14 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 12 Jan 2021 01:09:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 01:09:16 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0528b39c7eddf3a960919da4e91c41f304ecd9b26b5d04a6f7e80aedf265e78c`  
		Last Modified: Tue, 12 Jan 2021 00:15:54 GMT  
		Size: 19.3 MB (19315991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f4127298f0c323dd5825d1a04aac0766454af692c736bb4e0f694997674d13`  
		Last Modified: Tue, 12 Jan 2021 01:09:37 GMT  
		Size: 5.8 MB (5764894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0824f2b6d2aa3df50a37e3ed82740c40490fbe272791899b764d8d4f4eda7363`  
		Last Modified: Tue, 12 Jan 2021 01:10:30 GMT  
		Size: 38.7 MB (38734094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9885ddc2631790171fabbacd8dc66c012dbce273625e9e4342b549b81b7a79e2`  
		Last Modified: Tue, 12 Jan 2021 01:10:11 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6077683d07b03d236ca914eea776e4a2c8783a01d501982ce3d996bda1f1f8db`  
		Last Modified: Tue, 12 Jan 2021 01:10:12 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0f55ebb4c1531ff64981cf258a9d98f23e8eca98f28c825fe297296a9fc797`  
		Last Modified: Tue, 12 Jan 2021 01:10:12 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:772e41408e685093b75eb7142c04a1c337d06f7eef0429d4342ba20ed1469690
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64944529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1063ec2d69ccd4c96f32b1317a570c7f26af9bf8d91f4af4c21fbfdb1f9dee70`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 12 Jan 2021 00:45:57 GMT
ADD file:1dbf496d4adcfe7f12aea3440df891e77dfc1ebe060293de4f1ce37805fa65dc in / 
# Tue, 12 Jan 2021 00:46:05 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:44:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 01:46:01 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 12 Jan 2021 01:46:15 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 01:46:16 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 12 Jan 2021 01:46:17 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 12 Jan 2021 01:46:18 GMT
EXPOSE 8888
# Tue, 12 Jan 2021 01:46:19 GMT
VOLUME [/var/lib/chronograf]
# Tue, 12 Jan 2021 01:46:20 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 12 Jan 2021 01:46:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 01:46:23 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f5ae4cb78f788ad985447f014f2a5d2a878b9aa7496e12d4f62aaab1069093da`  
		Last Modified: Tue, 12 Jan 2021 00:55:18 GMT  
		Size: 20.4 MB (20389454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5b2a9df7f21c90351b107bab5a43b12f7050b083a2b6ea45344e6c2a11d8d1`  
		Last Modified: Tue, 12 Jan 2021 01:46:47 GMT  
		Size: 6.0 MB (6028288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74610bcba12f8039f16f242b33711e94b08613319f3be703c5f69c27403f975`  
		Last Modified: Tue, 12 Jan 2021 01:47:44 GMT  
		Size: 38.5 MB (38502389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922b0b85414cee401a0104e4ca7e8b3b0d7122f2728eaf6b2a4819375d0f1461`  
		Last Modified: Tue, 12 Jan 2021 01:47:26 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75d59b8a3efcc7e1c45e33112dd475d07e867492c71f280b7767210d40367c6`  
		Last Modified: Tue, 12 Jan 2021 01:47:27 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01429ece6f867a273ade23497f62653f3e5f14b47e5bab2c44da69fbb1c2b52`  
		Last Modified: Tue, 12 Jan 2021 01:47:27 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.8`

```console
$ docker pull chronograf@sha256:743696cac24f2466bd182701e39c3b1156531aa49c9ef828d9ecc9471bec5aa0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8.8` - linux; amd64

```console
$ docker pull chronograf@sha256:6bbfbbd73180964dbe313647223e80ee0e165ae05015db86639ba20f0f78931d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70424385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82d0154a00f46e5c1657d665aa2fc18c9c0242b2db7f64caa4e6658ed6b4ef60`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:30 GMT
ADD file:da0c935ddc86ca9e44bdd5f61b46c7b43a115ee4bc356324265a7ad6323f61ae in / 
# Tue, 09 Feb 2021 02:23:30 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:46:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Feb 2021 02:47:17 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 09 Feb 2021 02:47:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 02:47:27 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Feb 2021 02:47:27 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Feb 2021 02:47:28 GMT
EXPOSE 8888
# Tue, 09 Feb 2021 02:47:28 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Feb 2021 02:47:28 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 09 Feb 2021 02:47:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Feb 2021 02:47:29 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:cae7303ade7f17f84fe86b2a44880e9725cf7d6dcd17f79485360712b6af6dcd`  
		Last Modified: Tue, 09 Feb 2021 02:29:36 GMT  
		Size: 22.5 MB (22528600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603c713cc31395a01337edc5ae784741dda2d7aefb303bb93f7577486b1d1bbe`  
		Last Modified: Tue, 09 Feb 2021 02:47:56 GMT  
		Size: 6.7 MB (6742606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63600abc06b0687e4b24afa150d2da557c51a85b33e91502d51071591e5e6d82`  
		Last Modified: Tue, 09 Feb 2021 02:48:34 GMT  
		Size: 41.1 MB (41128782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3b434ef96cd8f4643d0c998ec73edb0b44c26d4e31cd5bca7c5f29b9400a0d`  
		Last Modified: Tue, 09 Feb 2021 02:48:27 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8145a040da7204ae6decb8f85b3096c06ade1972f6b6d4ab0496b789a24ce2`  
		Last Modified: Tue, 09 Feb 2021 02:48:27 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391ffb32b78cc26585c3ddd4ecc5590a8961c93e839ed73b88da29e4ad507ee7`  
		Last Modified: Tue, 09 Feb 2021 02:48:27 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:3da13b6796ebefd8fc57f33f36f900b12749991889ca27a55b92e61df695d0d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63839375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6afe2319f4923872211dd1c6fb7d6f7f1cf4ee339b6ee56524ea2152687f147b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:44 GMT
ADD file:31b268030b071d84c09e225f80f0552bc4869000d8be3321e1046de8ff0f44e2 in / 
# Tue, 12 Jan 2021 00:05:47 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:07:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 01:08:56 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 12 Jan 2021 01:09:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 01:09:12 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 12 Jan 2021 01:09:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 12 Jan 2021 01:09:13 GMT
EXPOSE 8888
# Tue, 12 Jan 2021 01:09:14 GMT
VOLUME [/var/lib/chronograf]
# Tue, 12 Jan 2021 01:09:14 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 12 Jan 2021 01:09:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 01:09:16 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0528b39c7eddf3a960919da4e91c41f304ecd9b26b5d04a6f7e80aedf265e78c`  
		Last Modified: Tue, 12 Jan 2021 00:15:54 GMT  
		Size: 19.3 MB (19315991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f4127298f0c323dd5825d1a04aac0766454af692c736bb4e0f694997674d13`  
		Last Modified: Tue, 12 Jan 2021 01:09:37 GMT  
		Size: 5.8 MB (5764894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0824f2b6d2aa3df50a37e3ed82740c40490fbe272791899b764d8d4f4eda7363`  
		Last Modified: Tue, 12 Jan 2021 01:10:30 GMT  
		Size: 38.7 MB (38734094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9885ddc2631790171fabbacd8dc66c012dbce273625e9e4342b549b81b7a79e2`  
		Last Modified: Tue, 12 Jan 2021 01:10:11 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6077683d07b03d236ca914eea776e4a2c8783a01d501982ce3d996bda1f1f8db`  
		Last Modified: Tue, 12 Jan 2021 01:10:12 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0f55ebb4c1531ff64981cf258a9d98f23e8eca98f28c825fe297296a9fc797`  
		Last Modified: Tue, 12 Jan 2021 01:10:12 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:7f130666c6361906f40355f639d52098ddfb14057bc887b3fb0624dc46f071cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64944267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e2a6436ea35a9248cd7a1fab7947bda22ebd1b384802f92f4381c3a4ab5995b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Feb 2021 02:43:38 GMT
ADD file:ec0f3f5aad51202b992acbfa7ec19738608d022983bc1918d7d9eecdd35e4800 in / 
# Tue, 09 Feb 2021 02:43:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:28:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Feb 2021 04:30:15 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 09 Feb 2021 04:30:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 04:30:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Feb 2021 04:30:30 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Feb 2021 04:30:31 GMT
EXPOSE 8888
# Tue, 09 Feb 2021 04:30:32 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Feb 2021 04:30:32 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 09 Feb 2021 04:30:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Feb 2021 04:30:34 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b373a42fa9174db1e441a19411c9622d41f6db219878945ed0cb256efa32c8a6`  
		Last Modified: Tue, 09 Feb 2021 02:50:08 GMT  
		Size: 20.4 MB (20389427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b4b210d138fd2393967f174396ed44ec8cbf98472a90f6928614b79905e1c7`  
		Last Modified: Tue, 09 Feb 2021 04:31:00 GMT  
		Size: 6.0 MB (6028114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97054239d5610218f0d05723d441a14db8468a06c13285a97f969709773d4178`  
		Last Modified: Tue, 09 Feb 2021 04:31:38 GMT  
		Size: 38.5 MB (38502341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f43bc65242ba82f02506f64d85701f9c77545eb0b27c358b4485d6904721ad`  
		Last Modified: Tue, 09 Feb 2021 04:31:29 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adfc4f590d599d4ffcc7b0942e21ba4bf06a0e9406b85dd3984a80066badaa0`  
		Last Modified: Tue, 09 Feb 2021 04:31:29 GMT  
		Size: 11.9 KB (11902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa90b76c984b1fd857a54f0cf52b49a189c1e0989ba0d5daba83447beb7041e2`  
		Last Modified: Tue, 09 Feb 2021 04:31:29 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.8-alpine`

```console
$ docker pull chronograf@sha256:2a643fee634453db985e763817c488d98114a8b22baeaebfc54f4ed309eebfac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.8.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:a69e7c6203bc95089dbe494c7563fb2ce77184bb4a0cda4b8ba989fb3407d5d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25350029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636966db36b11e40f9eebfb328048cabf4963a3f8e3efb7d4bd911ad64441dc3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:07:54 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:08:27 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Thu, 17 Dec 2020 13:08:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:08:32 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Dec 2020 13:08:33 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Dec 2020 13:08:33 GMT
EXPOSE 8888
# Thu, 17 Dec 2020 13:08:33 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Dec 2020 13:08:34 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:08:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:08:34 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac210e4df99beaffbde65dfe580e9923c2bef3b5dd07f0ac7d364e47dc2fac52`  
		Last Modified: Thu, 17 Dec 2020 13:09:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2a689ddee3aadca4971508078c3d8f60b8fdbeb3ee260f4212e3b37c6548cf`  
		Last Modified: Thu, 17 Dec 2020 13:09:08 GMT  
		Size: 280.8 KB (280803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165d18ddb83e7b234ae8c9bbd89bd90fe43a0d4e1ec5cd07a343bcd2e67fdc56`  
		Last Modified: Thu, 17 Dec 2020 13:09:43 GMT  
		Size: 22.2 MB (22245630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0f441fa8e0bc088be4728eefe678d20621b1c8bc6ed6eaaba1e5a8ebe9fbf6`  
		Last Modified: Thu, 17 Dec 2020 13:09:37 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb2589e467992d5e57c582fd71f1f6dbe6c1d26775e19e99ad778696d636c3b`  
		Last Modified: Thu, 17 Dec 2020 13:09:37 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affda9312202e2ee28e4be258174dd31e64c9c8ef0e414de15948aa57c8b5e13`  
		Last Modified: Thu, 17 Dec 2020 13:09:37 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8-alpine`

```console
$ docker pull chronograf@sha256:2a643fee634453db985e763817c488d98114a8b22baeaebfc54f4ed309eebfac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:a69e7c6203bc95089dbe494c7563fb2ce77184bb4a0cda4b8ba989fb3407d5d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25350029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636966db36b11e40f9eebfb328048cabf4963a3f8e3efb7d4bd911ad64441dc3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:07:54 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:08:27 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Thu, 17 Dec 2020 13:08:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:08:32 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Dec 2020 13:08:33 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Dec 2020 13:08:33 GMT
EXPOSE 8888
# Thu, 17 Dec 2020 13:08:33 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Dec 2020 13:08:34 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:08:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:08:34 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac210e4df99beaffbde65dfe580e9923c2bef3b5dd07f0ac7d364e47dc2fac52`  
		Last Modified: Thu, 17 Dec 2020 13:09:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2a689ddee3aadca4971508078c3d8f60b8fdbeb3ee260f4212e3b37c6548cf`  
		Last Modified: Thu, 17 Dec 2020 13:09:08 GMT  
		Size: 280.8 KB (280803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165d18ddb83e7b234ae8c9bbd89bd90fe43a0d4e1ec5cd07a343bcd2e67fdc56`  
		Last Modified: Thu, 17 Dec 2020 13:09:43 GMT  
		Size: 22.2 MB (22245630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0f441fa8e0bc088be4728eefe678d20621b1c8bc6ed6eaaba1e5a8ebe9fbf6`  
		Last Modified: Thu, 17 Dec 2020 13:09:37 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb2589e467992d5e57c582fd71f1f6dbe6c1d26775e19e99ad778696d636c3b`  
		Last Modified: Thu, 17 Dec 2020 13:09:37 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affda9312202e2ee28e4be258174dd31e64c9c8ef0e414de15948aa57c8b5e13`  
		Last Modified: Thu, 17 Dec 2020 13:09:37 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:2a643fee634453db985e763817c488d98114a8b22baeaebfc54f4ed309eebfac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:a69e7c6203bc95089dbe494c7563fb2ce77184bb4a0cda4b8ba989fb3407d5d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25350029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636966db36b11e40f9eebfb328048cabf4963a3f8e3efb7d4bd911ad64441dc3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:07:54 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:08:27 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Thu, 17 Dec 2020 13:08:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:08:32 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 17 Dec 2020 13:08:33 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 17 Dec 2020 13:08:33 GMT
EXPOSE 8888
# Thu, 17 Dec 2020 13:08:33 GMT
VOLUME [/var/lib/chronograf]
# Thu, 17 Dec 2020 13:08:34 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:08:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:08:34 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac210e4df99beaffbde65dfe580e9923c2bef3b5dd07f0ac7d364e47dc2fac52`  
		Last Modified: Thu, 17 Dec 2020 13:09:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2a689ddee3aadca4971508078c3d8f60b8fdbeb3ee260f4212e3b37c6548cf`  
		Last Modified: Thu, 17 Dec 2020 13:09:08 GMT  
		Size: 280.8 KB (280803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165d18ddb83e7b234ae8c9bbd89bd90fe43a0d4e1ec5cd07a343bcd2e67fdc56`  
		Last Modified: Thu, 17 Dec 2020 13:09:43 GMT  
		Size: 22.2 MB (22245630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0f441fa8e0bc088be4728eefe678d20621b1c8bc6ed6eaaba1e5a8ebe9fbf6`  
		Last Modified: Thu, 17 Dec 2020 13:09:37 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb2589e467992d5e57c582fd71f1f6dbe6c1d26775e19e99ad778696d636c3b`  
		Last Modified: Thu, 17 Dec 2020 13:09:37 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affda9312202e2ee28e4be258174dd31e64c9c8ef0e414de15948aa57c8b5e13`  
		Last Modified: Thu, 17 Dec 2020 13:09:37 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:latest`

```console
$ docker pull chronograf@sha256:743696cac24f2466bd182701e39c3b1156531aa49c9ef828d9ecc9471bec5aa0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:6bbfbbd73180964dbe313647223e80ee0e165ae05015db86639ba20f0f78931d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70424385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82d0154a00f46e5c1657d665aa2fc18c9c0242b2db7f64caa4e6658ed6b4ef60`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:30 GMT
ADD file:da0c935ddc86ca9e44bdd5f61b46c7b43a115ee4bc356324265a7ad6323f61ae in / 
# Tue, 09 Feb 2021 02:23:30 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:46:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Feb 2021 02:47:17 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 09 Feb 2021 02:47:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 02:47:27 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Feb 2021 02:47:27 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Feb 2021 02:47:28 GMT
EXPOSE 8888
# Tue, 09 Feb 2021 02:47:28 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Feb 2021 02:47:28 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 09 Feb 2021 02:47:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Feb 2021 02:47:29 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:cae7303ade7f17f84fe86b2a44880e9725cf7d6dcd17f79485360712b6af6dcd`  
		Last Modified: Tue, 09 Feb 2021 02:29:36 GMT  
		Size: 22.5 MB (22528600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603c713cc31395a01337edc5ae784741dda2d7aefb303bb93f7577486b1d1bbe`  
		Last Modified: Tue, 09 Feb 2021 02:47:56 GMT  
		Size: 6.7 MB (6742606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63600abc06b0687e4b24afa150d2da557c51a85b33e91502d51071591e5e6d82`  
		Last Modified: Tue, 09 Feb 2021 02:48:34 GMT  
		Size: 41.1 MB (41128782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3b434ef96cd8f4643d0c998ec73edb0b44c26d4e31cd5bca7c5f29b9400a0d`  
		Last Modified: Tue, 09 Feb 2021 02:48:27 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8145a040da7204ae6decb8f85b3096c06ade1972f6b6d4ab0496b789a24ce2`  
		Last Modified: Tue, 09 Feb 2021 02:48:27 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391ffb32b78cc26585c3ddd4ecc5590a8961c93e839ed73b88da29e4ad507ee7`  
		Last Modified: Tue, 09 Feb 2021 02:48:27 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:3da13b6796ebefd8fc57f33f36f900b12749991889ca27a55b92e61df695d0d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63839375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6afe2319f4923872211dd1c6fb7d6f7f1cf4ee339b6ee56524ea2152687f147b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:44 GMT
ADD file:31b268030b071d84c09e225f80f0552bc4869000d8be3321e1046de8ff0f44e2 in / 
# Tue, 12 Jan 2021 00:05:47 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:07:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 01:08:56 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 12 Jan 2021 01:09:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 01:09:12 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 12 Jan 2021 01:09:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 12 Jan 2021 01:09:13 GMT
EXPOSE 8888
# Tue, 12 Jan 2021 01:09:14 GMT
VOLUME [/var/lib/chronograf]
# Tue, 12 Jan 2021 01:09:14 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 12 Jan 2021 01:09:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 01:09:16 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0528b39c7eddf3a960919da4e91c41f304ecd9b26b5d04a6f7e80aedf265e78c`  
		Last Modified: Tue, 12 Jan 2021 00:15:54 GMT  
		Size: 19.3 MB (19315991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f4127298f0c323dd5825d1a04aac0766454af692c736bb4e0f694997674d13`  
		Last Modified: Tue, 12 Jan 2021 01:09:37 GMT  
		Size: 5.8 MB (5764894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0824f2b6d2aa3df50a37e3ed82740c40490fbe272791899b764d8d4f4eda7363`  
		Last Modified: Tue, 12 Jan 2021 01:10:30 GMT  
		Size: 38.7 MB (38734094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9885ddc2631790171fabbacd8dc66c012dbce273625e9e4342b549b81b7a79e2`  
		Last Modified: Tue, 12 Jan 2021 01:10:11 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6077683d07b03d236ca914eea776e4a2c8783a01d501982ce3d996bda1f1f8db`  
		Last Modified: Tue, 12 Jan 2021 01:10:12 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0f55ebb4c1531ff64981cf258a9d98f23e8eca98f28c825fe297296a9fc797`  
		Last Modified: Tue, 12 Jan 2021 01:10:12 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:7f130666c6361906f40355f639d52098ddfb14057bc887b3fb0624dc46f071cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64944267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e2a6436ea35a9248cd7a1fab7947bda22ebd1b384802f92f4381c3a4ab5995b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Feb 2021 02:43:38 GMT
ADD file:ec0f3f5aad51202b992acbfa7ec19738608d022983bc1918d7d9eecdd35e4800 in / 
# Tue, 09 Feb 2021 02:43:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:28:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Feb 2021 04:30:15 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Tue, 09 Feb 2021 04:30:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 04:30:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Feb 2021 04:30:30 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Feb 2021 04:30:31 GMT
EXPOSE 8888
# Tue, 09 Feb 2021 04:30:32 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Feb 2021 04:30:32 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 09 Feb 2021 04:30:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Feb 2021 04:30:34 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b373a42fa9174db1e441a19411c9622d41f6db219878945ed0cb256efa32c8a6`  
		Last Modified: Tue, 09 Feb 2021 02:50:08 GMT  
		Size: 20.4 MB (20389427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b4b210d138fd2393967f174396ed44ec8cbf98472a90f6928614b79905e1c7`  
		Last Modified: Tue, 09 Feb 2021 04:31:00 GMT  
		Size: 6.0 MB (6028114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97054239d5610218f0d05723d441a14db8468a06c13285a97f969709773d4178`  
		Last Modified: Tue, 09 Feb 2021 04:31:38 GMT  
		Size: 38.5 MB (38502341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f43bc65242ba82f02506f64d85701f9c77545eb0b27c358b4485d6904721ad`  
		Last Modified: Tue, 09 Feb 2021 04:31:29 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adfc4f590d599d4ffcc7b0942e21ba4bf06a0e9406b85dd3984a80066badaa0`  
		Last Modified: Tue, 09 Feb 2021 04:31:29 GMT  
		Size: 11.9 KB (11902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa90b76c984b1fd857a54f0cf52b49a189c1e0989ba0d5daba83447beb7041e2`  
		Last Modified: Tue, 09 Feb 2021 04:31:29 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
