<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `chronograf`

-	[`chronograf:1.5`](#chronograf15)
-	[`chronograf:1.5.0`](#chronograf150)
-	[`chronograf:1.5.0.1`](#chronograf1501)
-	[`chronograf:1.5.0.1-alpine`](#chronograf1501-alpine)
-	[`chronograf:1.5.0-alpine`](#chronograf150-alpine)
-	[`chronograf:1.5-alpine`](#chronograf15-alpine)
-	[`chronograf:1.6`](#chronograf16)
-	[`chronograf:1.6.2`](#chronograf162)
-	[`chronograf:1.6.2-alpine`](#chronograf162-alpine)
-	[`chronograf:1.6-alpine`](#chronograf16-alpine)
-	[`chronograf:1.7`](#chronograf17)
-	[`chronograf:1.7.16`](#chronograf1716)
-	[`chronograf:1.7.16-alpine`](#chronograf1716-alpine)
-	[`chronograf:1.7-alpine`](#chronograf17-alpine)
-	[`chronograf:alpine`](#chronografalpine)
-	[`chronograf:latest`](#chronograflatest)

## `chronograf:1.5`

```console
$ docker pull chronograf@sha256:481885709b73844d27ee267a0d8690ed59abed56fef71e096eabdc06cf0de3a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.5` - linux; amd64

```console
$ docker pull chronograf@sha256:2a8464114aee32a5a12e183f611fcb82562f6694b2e8eaa22caa2de823bd3b14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49096689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1494d113d56b9e011003427adec3c539bced291941fb89ae3ffaf27ae5e73ffb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:15:39 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 02:15:39 GMT
ENV CHRONOGRAF_VERSION=1.5.0.1
# Wed, 26 Feb 2020 02:15:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 02:15:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 02:15:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 02:15:56 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 02:15:56 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 02:15:56 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 02:15:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 02:15:57 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f878ed3f571cef34099acbbbb2582f64051e11e88b899a5cfe4ef47d003542f`  
		Last Modified: Wed, 26 Feb 2020 02:17:16 GMT  
		Size: 4.5 MB (4503576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adf1c1353cb928a2d0242c3674d5fe1ed26fb8ba7dfbeebaa8d27d17b4ebf65`  
		Last Modified: Wed, 26 Feb 2020 02:17:21 GMT  
		Size: 22.1 MB (22055362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a65427ab8626167561d2de92c49e400dc65fd78391a43fbb3e30f0ae597b98`  
		Last Modified: Wed, 26 Feb 2020 02:17:15 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e11dc5c4fcbd342b0ed074ed3731af92990b517e6b3e805ac9d9246f69833f`  
		Last Modified: Wed, 26 Feb 2020 02:17:15 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4028923d1a44248f38c144baad88dee46f1e6ae0814ec7f004947a4b2936acf2`  
		Last Modified: Wed, 26 Feb 2020 02:17:15 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.5` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:18e28d03207b8a5743e192a0e54e01145897b9e83889fa028202eabe4eaf0919
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43662183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83910a2164576ab70b7706fdc62a352f93c514e15e837e69bd7a76dd4c2808ad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:29:13 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 01:29:15 GMT
ENV CHRONOGRAF_VERSION=1.5.0.1
# Wed, 26 Feb 2020 01:29:37 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 01:29:38 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 01:29:38 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 01:29:39 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 01:29:40 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 01:29:41 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 01:29:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 01:29:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15634d01c3f3a1bece118d96c09deb143bac89f0f8ab71aeb0c0629360a460f`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 3.9 MB (3877306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbfb4b57a49ede05d50975f2ed04f4a50ae1a43e26fe75c49a2c1c5c0de0384`  
		Last Modified: Wed, 26 Feb 2020 01:31:45 GMT  
		Size: 20.5 MB (20462131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdb3488d3019554f469e0f950940c80d5b80b157a6b989191dd1c98e3cfaf8`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f6ef2dcdd1abb76ada64fef7667499685247929f93e80d74c9be13712eec99`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 11.9 KB (11911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663f8197381181b3bfcbbdcb29e7b4b6a5f251499899edd9be25be745e204dd1`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.5` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:d1c7cfd9525baeb779ff69008022af4a8852b444fa9ce24a7ca3af8988e49d10
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45144376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71675dd3717c00c37a5c96327d8efa9a3ee423655b056297e65f7618ed6ed01a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:10:29 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 04:10:30 GMT
ENV CHRONOGRAF_VERSION=1.5.0.1
# Wed, 26 Feb 2020 04:10:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 04:10:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 04:10:51 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 04:10:52 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 04:10:52 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 04:10:53 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 04:10:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 04:10:54 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f797dde9809216bf453cb02c743c00da5fed52ec53e5d746f9a7cfdb99720f`  
		Last Modified: Wed, 26 Feb 2020 04:12:22 GMT  
		Size: 4.1 MB (4080742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f24c30a55c846c930c556a974e8c2201f44d5d3cc88e7d45ceb3f11492e427`  
		Last Modified: Wed, 26 Feb 2020 04:12:27 GMT  
		Size: 20.7 MB (20669255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a51a2ca8e7f2d27cfef2a779ddc28d138d27b611405596adc1c2a99f4ab950d`  
		Last Modified: Wed, 26 Feb 2020 04:12:22 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43b6e28cf4bf0a81e95a6de1373b1e10d63e1bc63d373c9ea3bff1b74c4981d`  
		Last Modified: Wed, 26 Feb 2020 04:12:21 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e6df8db9fe0b5e910f535c95f696b93947cbac8b215257fea8dcdf91980b06`  
		Last Modified: Wed, 26 Feb 2020 04:12:22 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.5.0`

```console
$ docker pull chronograf@sha256:481885709b73844d27ee267a0d8690ed59abed56fef71e096eabdc06cf0de3a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.5.0` - linux; amd64

```console
$ docker pull chronograf@sha256:2a8464114aee32a5a12e183f611fcb82562f6694b2e8eaa22caa2de823bd3b14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49096689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1494d113d56b9e011003427adec3c539bced291941fb89ae3ffaf27ae5e73ffb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:15:39 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 02:15:39 GMT
ENV CHRONOGRAF_VERSION=1.5.0.1
# Wed, 26 Feb 2020 02:15:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 02:15:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 02:15:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 02:15:56 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 02:15:56 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 02:15:56 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 02:15:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 02:15:57 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f878ed3f571cef34099acbbbb2582f64051e11e88b899a5cfe4ef47d003542f`  
		Last Modified: Wed, 26 Feb 2020 02:17:16 GMT  
		Size: 4.5 MB (4503576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adf1c1353cb928a2d0242c3674d5fe1ed26fb8ba7dfbeebaa8d27d17b4ebf65`  
		Last Modified: Wed, 26 Feb 2020 02:17:21 GMT  
		Size: 22.1 MB (22055362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a65427ab8626167561d2de92c49e400dc65fd78391a43fbb3e30f0ae597b98`  
		Last Modified: Wed, 26 Feb 2020 02:17:15 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e11dc5c4fcbd342b0ed074ed3731af92990b517e6b3e805ac9d9246f69833f`  
		Last Modified: Wed, 26 Feb 2020 02:17:15 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4028923d1a44248f38c144baad88dee46f1e6ae0814ec7f004947a4b2936acf2`  
		Last Modified: Wed, 26 Feb 2020 02:17:15 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.5.0` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:18e28d03207b8a5743e192a0e54e01145897b9e83889fa028202eabe4eaf0919
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43662183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83910a2164576ab70b7706fdc62a352f93c514e15e837e69bd7a76dd4c2808ad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:29:13 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 01:29:15 GMT
ENV CHRONOGRAF_VERSION=1.5.0.1
# Wed, 26 Feb 2020 01:29:37 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 01:29:38 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 01:29:38 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 01:29:39 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 01:29:40 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 01:29:41 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 01:29:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 01:29:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15634d01c3f3a1bece118d96c09deb143bac89f0f8ab71aeb0c0629360a460f`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 3.9 MB (3877306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbfb4b57a49ede05d50975f2ed04f4a50ae1a43e26fe75c49a2c1c5c0de0384`  
		Last Modified: Wed, 26 Feb 2020 01:31:45 GMT  
		Size: 20.5 MB (20462131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdb3488d3019554f469e0f950940c80d5b80b157a6b989191dd1c98e3cfaf8`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f6ef2dcdd1abb76ada64fef7667499685247929f93e80d74c9be13712eec99`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 11.9 KB (11911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663f8197381181b3bfcbbdcb29e7b4b6a5f251499899edd9be25be745e204dd1`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.5.0` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:d1c7cfd9525baeb779ff69008022af4a8852b444fa9ce24a7ca3af8988e49d10
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45144376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71675dd3717c00c37a5c96327d8efa9a3ee423655b056297e65f7618ed6ed01a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:10:29 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 04:10:30 GMT
ENV CHRONOGRAF_VERSION=1.5.0.1
# Wed, 26 Feb 2020 04:10:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 04:10:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 04:10:51 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 04:10:52 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 04:10:52 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 04:10:53 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 04:10:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 04:10:54 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f797dde9809216bf453cb02c743c00da5fed52ec53e5d746f9a7cfdb99720f`  
		Last Modified: Wed, 26 Feb 2020 04:12:22 GMT  
		Size: 4.1 MB (4080742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f24c30a55c846c930c556a974e8c2201f44d5d3cc88e7d45ceb3f11492e427`  
		Last Modified: Wed, 26 Feb 2020 04:12:27 GMT  
		Size: 20.7 MB (20669255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a51a2ca8e7f2d27cfef2a779ddc28d138d27b611405596adc1c2a99f4ab950d`  
		Last Modified: Wed, 26 Feb 2020 04:12:22 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43b6e28cf4bf0a81e95a6de1373b1e10d63e1bc63d373c9ea3bff1b74c4981d`  
		Last Modified: Wed, 26 Feb 2020 04:12:21 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e6df8db9fe0b5e910f535c95f696b93947cbac8b215257fea8dcdf91980b06`  
		Last Modified: Wed, 26 Feb 2020 04:12:22 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.5.0.1`

```console
$ docker pull chronograf@sha256:481885709b73844d27ee267a0d8690ed59abed56fef71e096eabdc06cf0de3a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.5.0.1` - linux; amd64

```console
$ docker pull chronograf@sha256:2a8464114aee32a5a12e183f611fcb82562f6694b2e8eaa22caa2de823bd3b14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49096689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1494d113d56b9e011003427adec3c539bced291941fb89ae3ffaf27ae5e73ffb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:15:39 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 02:15:39 GMT
ENV CHRONOGRAF_VERSION=1.5.0.1
# Wed, 26 Feb 2020 02:15:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 02:15:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 02:15:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 02:15:56 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 02:15:56 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 02:15:56 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 02:15:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 02:15:57 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f878ed3f571cef34099acbbbb2582f64051e11e88b899a5cfe4ef47d003542f`  
		Last Modified: Wed, 26 Feb 2020 02:17:16 GMT  
		Size: 4.5 MB (4503576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adf1c1353cb928a2d0242c3674d5fe1ed26fb8ba7dfbeebaa8d27d17b4ebf65`  
		Last Modified: Wed, 26 Feb 2020 02:17:21 GMT  
		Size: 22.1 MB (22055362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a65427ab8626167561d2de92c49e400dc65fd78391a43fbb3e30f0ae597b98`  
		Last Modified: Wed, 26 Feb 2020 02:17:15 GMT  
		Size: 12.2 KB (12242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e11dc5c4fcbd342b0ed074ed3731af92990b517e6b3e805ac9d9246f69833f`  
		Last Modified: Wed, 26 Feb 2020 02:17:15 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4028923d1a44248f38c144baad88dee46f1e6ae0814ec7f004947a4b2936acf2`  
		Last Modified: Wed, 26 Feb 2020 02:17:15 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.5.0.1` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:18e28d03207b8a5743e192a0e54e01145897b9e83889fa028202eabe4eaf0919
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43662183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83910a2164576ab70b7706fdc62a352f93c514e15e837e69bd7a76dd4c2808ad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:29:13 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 01:29:15 GMT
ENV CHRONOGRAF_VERSION=1.5.0.1
# Wed, 26 Feb 2020 01:29:37 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 01:29:38 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 01:29:38 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 01:29:39 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 01:29:40 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 01:29:41 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 01:29:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 01:29:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15634d01c3f3a1bece118d96c09deb143bac89f0f8ab71aeb0c0629360a460f`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 3.9 MB (3877306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbfb4b57a49ede05d50975f2ed04f4a50ae1a43e26fe75c49a2c1c5c0de0384`  
		Last Modified: Wed, 26 Feb 2020 01:31:45 GMT  
		Size: 20.5 MB (20462131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdb3488d3019554f469e0f950940c80d5b80b157a6b989191dd1c98e3cfaf8`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f6ef2dcdd1abb76ada64fef7667499685247929f93e80d74c9be13712eec99`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 11.9 KB (11911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663f8197381181b3bfcbbdcb29e7b4b6a5f251499899edd9be25be745e204dd1`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.5.0.1` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:d1c7cfd9525baeb779ff69008022af4a8852b444fa9ce24a7ca3af8988e49d10
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45144376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71675dd3717c00c37a5c96327d8efa9a3ee423655b056297e65f7618ed6ed01a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:10:29 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 04:10:30 GMT
ENV CHRONOGRAF_VERSION=1.5.0.1
# Wed, 26 Feb 2020 04:10:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 04:10:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 04:10:51 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 04:10:52 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 04:10:52 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 04:10:53 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 04:10:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 04:10:54 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f797dde9809216bf453cb02c743c00da5fed52ec53e5d746f9a7cfdb99720f`  
		Last Modified: Wed, 26 Feb 2020 04:12:22 GMT  
		Size: 4.1 MB (4080742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f24c30a55c846c930c556a974e8c2201f44d5d3cc88e7d45ceb3f11492e427`  
		Last Modified: Wed, 26 Feb 2020 04:12:27 GMT  
		Size: 20.7 MB (20669255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a51a2ca8e7f2d27cfef2a779ddc28d138d27b611405596adc1c2a99f4ab950d`  
		Last Modified: Wed, 26 Feb 2020 04:12:22 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43b6e28cf4bf0a81e95a6de1373b1e10d63e1bc63d373c9ea3bff1b74c4981d`  
		Last Modified: Wed, 26 Feb 2020 04:12:21 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e6df8db9fe0b5e910f535c95f696b93947cbac8b215257fea8dcdf91980b06`  
		Last Modified: Wed, 26 Feb 2020 04:12:22 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.5.0.1-alpine`

```console
$ docker pull chronograf@sha256:96a8c2862d12647b69e69ea708919c174467a33bf9c4094c47c1c38b281d1362
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.5.0.1-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:f0e24b5af705a70ee5ec30f0ef3d899558ba84e9e0e28b6533eab0116a18447c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14714603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebbefd794b199d2e4334ff284913c3c11d573a264dbe2d966c56058ae41f057f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:03:46 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 23 Jan 2020 19:32:40 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 24 Jan 2020 06:18:07 GMT
ENV CHRONOGRAF_VERSION=1.5.0.1
# Fri, 24 Jan 2020 06:18:11 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Jan 2020 06:18:11 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 24 Jan 2020 06:18:11 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 24 Jan 2020 06:18:12 GMT
EXPOSE 8888
# Fri, 24 Jan 2020 06:18:12 GMT
VOLUME [/var/lib/chronograf]
# Fri, 24 Jan 2020 06:18:12 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 24 Jan 2020 06:18:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jan 2020 06:18:13 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0018c3785b24046a24095a1f9cf7f42642c3dfd6e8282b328a2e22ce10ebc0de`  
		Last Modified: Thu, 23 Jan 2020 19:07:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cabf7ae254f2fa160de4e52dde588a8ed9490a15fc92b06cc1c47b680ccdf4`  
		Last Modified: Thu, 23 Jan 2020 19:33:23 GMT  
		Size: 301.9 KB (301878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3b752cacd2c99d068949a8fa2863231a37be97894ff204e1aac95a3db46362`  
		Last Modified: Fri, 24 Jan 2020 06:19:00 GMT  
		Size: 11.6 MB (11624021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fa17657ce08f2051045c15e221d3a3d394406a34c5929e0f38043fab1708dc`  
		Last Modified: Fri, 24 Jan 2020 06:18:53 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1033b1186465e211fd59c1374233b0b6f8f03db586c35e2ea6f9a4566fdf9d9`  
		Last Modified: Fri, 24 Jan 2020 06:18:53 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411475a71eceec1dad8e44acb6a43adcffe4ed4c30aa9a0e952204231f9a9a01`  
		Last Modified: Fri, 24 Jan 2020 06:18:53 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.5.0-alpine`

```console
$ docker pull chronograf@sha256:96a8c2862d12647b69e69ea708919c174467a33bf9c4094c47c1c38b281d1362
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.5.0-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:f0e24b5af705a70ee5ec30f0ef3d899558ba84e9e0e28b6533eab0116a18447c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14714603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebbefd794b199d2e4334ff284913c3c11d573a264dbe2d966c56058ae41f057f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:03:46 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 23 Jan 2020 19:32:40 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 24 Jan 2020 06:18:07 GMT
ENV CHRONOGRAF_VERSION=1.5.0.1
# Fri, 24 Jan 2020 06:18:11 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Jan 2020 06:18:11 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 24 Jan 2020 06:18:11 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 24 Jan 2020 06:18:12 GMT
EXPOSE 8888
# Fri, 24 Jan 2020 06:18:12 GMT
VOLUME [/var/lib/chronograf]
# Fri, 24 Jan 2020 06:18:12 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 24 Jan 2020 06:18:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jan 2020 06:18:13 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0018c3785b24046a24095a1f9cf7f42642c3dfd6e8282b328a2e22ce10ebc0de`  
		Last Modified: Thu, 23 Jan 2020 19:07:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cabf7ae254f2fa160de4e52dde588a8ed9490a15fc92b06cc1c47b680ccdf4`  
		Last Modified: Thu, 23 Jan 2020 19:33:23 GMT  
		Size: 301.9 KB (301878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3b752cacd2c99d068949a8fa2863231a37be97894ff204e1aac95a3db46362`  
		Last Modified: Fri, 24 Jan 2020 06:19:00 GMT  
		Size: 11.6 MB (11624021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fa17657ce08f2051045c15e221d3a3d394406a34c5929e0f38043fab1708dc`  
		Last Modified: Fri, 24 Jan 2020 06:18:53 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1033b1186465e211fd59c1374233b0b6f8f03db586c35e2ea6f9a4566fdf9d9`  
		Last Modified: Fri, 24 Jan 2020 06:18:53 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411475a71eceec1dad8e44acb6a43adcffe4ed4c30aa9a0e952204231f9a9a01`  
		Last Modified: Fri, 24 Jan 2020 06:18:53 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.5-alpine`

```console
$ docker pull chronograf@sha256:96a8c2862d12647b69e69ea708919c174467a33bf9c4094c47c1c38b281d1362
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.5-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:f0e24b5af705a70ee5ec30f0ef3d899558ba84e9e0e28b6533eab0116a18447c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14714603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebbefd794b199d2e4334ff284913c3c11d573a264dbe2d966c56058ae41f057f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:03:46 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 23 Jan 2020 19:32:40 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 24 Jan 2020 06:18:07 GMT
ENV CHRONOGRAF_VERSION=1.5.0.1
# Fri, 24 Jan 2020 06:18:11 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Jan 2020 06:18:11 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 24 Jan 2020 06:18:11 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 24 Jan 2020 06:18:12 GMT
EXPOSE 8888
# Fri, 24 Jan 2020 06:18:12 GMT
VOLUME [/var/lib/chronograf]
# Fri, 24 Jan 2020 06:18:12 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 24 Jan 2020 06:18:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jan 2020 06:18:13 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0018c3785b24046a24095a1f9cf7f42642c3dfd6e8282b328a2e22ce10ebc0de`  
		Last Modified: Thu, 23 Jan 2020 19:07:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cabf7ae254f2fa160de4e52dde588a8ed9490a15fc92b06cc1c47b680ccdf4`  
		Last Modified: Thu, 23 Jan 2020 19:33:23 GMT  
		Size: 301.9 KB (301878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3b752cacd2c99d068949a8fa2863231a37be97894ff204e1aac95a3db46362`  
		Last Modified: Fri, 24 Jan 2020 06:19:00 GMT  
		Size: 11.6 MB (11624021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fa17657ce08f2051045c15e221d3a3d394406a34c5929e0f38043fab1708dc`  
		Last Modified: Fri, 24 Jan 2020 06:18:53 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1033b1186465e211fd59c1374233b0b6f8f03db586c35e2ea6f9a4566fdf9d9`  
		Last Modified: Fri, 24 Jan 2020 06:18:53 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411475a71eceec1dad8e44acb6a43adcffe4ed4c30aa9a0e952204231f9a9a01`  
		Last Modified: Fri, 24 Jan 2020 06:18:53 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6`

```console
$ docker pull chronograf@sha256:da6f1ca80e1299d4a53e3c0832f44b58e1375b46c54214166e381b8d6a1b73b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6` - linux; amd64

```console
$ docker pull chronograf@sha256:525df1e283b39214902f9573afda4240702201e7c1d7fc8224e4a212192e9d78
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49141097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d423aee4ef6df428ad8f6b4c26545daf4e43cc57747fb0da29bc2a5bb6540064`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:15:39 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 02:16:06 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 26 Feb 2020 02:16:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 02:16:23 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 02:16:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 02:16:24 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 02:16:24 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 02:16:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 02:16:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 02:16:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f878ed3f571cef34099acbbbb2582f64051e11e88b899a5cfe4ef47d003542f`  
		Last Modified: Wed, 26 Feb 2020 02:17:16 GMT  
		Size: 4.5 MB (4503576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03abdd98b7e7add053a6e84641890c1e8ea5d7b98824a0094a80de696297ed39`  
		Last Modified: Wed, 26 Feb 2020 02:17:33 GMT  
		Size: 22.1 MB (22099758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ab60ca6e02c6a80bbe7a26665268f6f1ebd25ea515b25865538153112bb6a8`  
		Last Modified: Wed, 26 Feb 2020 02:17:27 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c0a8a4eb7361e6cc7dfac10b224074dc3815cf2dca00420b0bfcf4f4d3873e`  
		Last Modified: Wed, 26 Feb 2020 02:17:27 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f86df364fcc995619828157895de0346f6038fd010d76b8e03cb4e739ba219`  
		Last Modified: Wed, 26 Feb 2020 02:17:27 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:ae63c72bacdc92d2891025a940c5846be420cd20999603afc0b9bc13c97dcaf9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43725358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f78bf7736604625294c7a65dbbaec0f8fd2f8f0dba64467e5c494cc20d52102`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:29:13 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 01:29:53 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 26 Feb 2020 01:30:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 01:30:13 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 01:30:14 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 01:30:15 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 01:30:17 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 01:30:18 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 01:30:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 01:30:20 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15634d01c3f3a1bece118d96c09deb143bac89f0f8ab71aeb0c0629360a460f`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 3.9 MB (3877306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e906e120466647231c285fa27ecc9be8cb19cc75e83d19b391b7608eefdc7b`  
		Last Modified: Wed, 26 Feb 2020 01:31:59 GMT  
		Size: 20.5 MB (20525314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17684c03781763995f92c0e11531b5558c0617cd50f0805164c039c65b52b1e0`  
		Last Modified: Wed, 26 Feb 2020 01:31:53 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a64f781b9ec1c0723ef52a1692d9c90643ba3f9af2828c0ad1985e3cfc0642`  
		Last Modified: Wed, 26 Feb 2020 01:31:53 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c7efdc3589128a06d0a9388f60c3141f9a94e1e93f5bd80558f39316adf279`  
		Last Modified: Wed, 26 Feb 2020 01:31:53 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:7173b34d6eee29870dbb286c337de20cc7e4f0d9e3aff35536e2ad94ee4db0b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45208580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc176aa969158749c9c685e3b3f5b34d19bb4792f9ed44d31fd88b1deeb780c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:10:29 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 04:11:01 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 26 Feb 2020 04:11:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 04:11:22 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 04:11:22 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 04:11:23 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 04:11:24 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 04:11:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 04:11:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 04:11:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f797dde9809216bf453cb02c743c00da5fed52ec53e5d746f9a7cfdb99720f`  
		Last Modified: Wed, 26 Feb 2020 04:12:22 GMT  
		Size: 4.1 MB (4080742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2378b44fa08285f9f6686d3e53b45afb6dbbed4c81d41ba811560d4e5eb1152`  
		Last Modified: Wed, 26 Feb 2020 04:12:42 GMT  
		Size: 20.7 MB (20733458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2bf4be9df591c56977ce6d8f013fb4304d0508b066ef299fc8e3543c57b745`  
		Last Modified: Wed, 26 Feb 2020 04:12:35 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a96c8ed531f5e471cecb1e286801bae331cb1aea35105264cdf0d43c1e9a07`  
		Last Modified: Wed, 26 Feb 2020 04:12:35 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2c86410b156355eff8190317b1b055b074860a1285a3eaf941217d3845556f`  
		Last Modified: Wed, 26 Feb 2020 04:12:35 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2`

```console
$ docker pull chronograf@sha256:da6f1ca80e1299d4a53e3c0832f44b58e1375b46c54214166e381b8d6a1b73b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6.2` - linux; amd64

```console
$ docker pull chronograf@sha256:525df1e283b39214902f9573afda4240702201e7c1d7fc8224e4a212192e9d78
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49141097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d423aee4ef6df428ad8f6b4c26545daf4e43cc57747fb0da29bc2a5bb6540064`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:15:39 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 02:16:06 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 26 Feb 2020 02:16:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 02:16:23 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 02:16:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 02:16:24 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 02:16:24 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 02:16:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 02:16:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 02:16:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f878ed3f571cef34099acbbbb2582f64051e11e88b899a5cfe4ef47d003542f`  
		Last Modified: Wed, 26 Feb 2020 02:17:16 GMT  
		Size: 4.5 MB (4503576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03abdd98b7e7add053a6e84641890c1e8ea5d7b98824a0094a80de696297ed39`  
		Last Modified: Wed, 26 Feb 2020 02:17:33 GMT  
		Size: 22.1 MB (22099758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ab60ca6e02c6a80bbe7a26665268f6f1ebd25ea515b25865538153112bb6a8`  
		Last Modified: Wed, 26 Feb 2020 02:17:27 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c0a8a4eb7361e6cc7dfac10b224074dc3815cf2dca00420b0bfcf4f4d3873e`  
		Last Modified: Wed, 26 Feb 2020 02:17:27 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f86df364fcc995619828157895de0346f6038fd010d76b8e03cb4e739ba219`  
		Last Modified: Wed, 26 Feb 2020 02:17:27 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:ae63c72bacdc92d2891025a940c5846be420cd20999603afc0b9bc13c97dcaf9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43725358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f78bf7736604625294c7a65dbbaec0f8fd2f8f0dba64467e5c494cc20d52102`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:29:13 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 01:29:53 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 26 Feb 2020 01:30:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 01:30:13 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 01:30:14 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 01:30:15 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 01:30:17 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 01:30:18 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 01:30:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 01:30:20 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15634d01c3f3a1bece118d96c09deb143bac89f0f8ab71aeb0c0629360a460f`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 3.9 MB (3877306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e906e120466647231c285fa27ecc9be8cb19cc75e83d19b391b7608eefdc7b`  
		Last Modified: Wed, 26 Feb 2020 01:31:59 GMT  
		Size: 20.5 MB (20525314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17684c03781763995f92c0e11531b5558c0617cd50f0805164c039c65b52b1e0`  
		Last Modified: Wed, 26 Feb 2020 01:31:53 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a64f781b9ec1c0723ef52a1692d9c90643ba3f9af2828c0ad1985e3cfc0642`  
		Last Modified: Wed, 26 Feb 2020 01:31:53 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c7efdc3589128a06d0a9388f60c3141f9a94e1e93f5bd80558f39316adf279`  
		Last Modified: Wed, 26 Feb 2020 01:31:53 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:7173b34d6eee29870dbb286c337de20cc7e4f0d9e3aff35536e2ad94ee4db0b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45208580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc176aa969158749c9c685e3b3f5b34d19bb4792f9ed44d31fd88b1deeb780c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:10:29 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 04:11:01 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 26 Feb 2020 04:11:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 04:11:22 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 04:11:22 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 04:11:23 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 04:11:24 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 04:11:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 04:11:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 04:11:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f797dde9809216bf453cb02c743c00da5fed52ec53e5d746f9a7cfdb99720f`  
		Last Modified: Wed, 26 Feb 2020 04:12:22 GMT  
		Size: 4.1 MB (4080742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2378b44fa08285f9f6686d3e53b45afb6dbbed4c81d41ba811560d4e5eb1152`  
		Last Modified: Wed, 26 Feb 2020 04:12:42 GMT  
		Size: 20.7 MB (20733458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2bf4be9df591c56977ce6d8f013fb4304d0508b066ef299fc8e3543c57b745`  
		Last Modified: Wed, 26 Feb 2020 04:12:35 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a96c8ed531f5e471cecb1e286801bae331cb1aea35105264cdf0d43c1e9a07`  
		Last Modified: Wed, 26 Feb 2020 04:12:35 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2c86410b156355eff8190317b1b055b074860a1285a3eaf941217d3845556f`  
		Last Modified: Wed, 26 Feb 2020 04:12:35 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2-alpine`

```console
$ docker pull chronograf@sha256:28a1724975f0d3d915fdd4437bb6dff1248fcba149af3263baacda8d0df53103
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.6.2-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:ad1c476ad7bceefac0abce84dddcc784f382d48a39c1e7ace47011c45ffca72e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14827436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffbd72c4a0ca324fa58904b89a1e3f7961c0c6f06d9fce279d56816a91dd9cc6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:03:46 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 23 Jan 2020 19:32:40 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 24 Jan 2020 06:18:20 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 24 Jan 2020 06:18:24 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Jan 2020 06:18:24 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 24 Jan 2020 06:18:24 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 24 Jan 2020 06:18:24 GMT
EXPOSE 8888
# Fri, 24 Jan 2020 06:18:25 GMT
VOLUME [/var/lib/chronograf]
# Fri, 24 Jan 2020 06:18:25 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 24 Jan 2020 06:18:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jan 2020 06:18:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0018c3785b24046a24095a1f9cf7f42642c3dfd6e8282b328a2e22ce10ebc0de`  
		Last Modified: Thu, 23 Jan 2020 19:07:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cabf7ae254f2fa160de4e52dde588a8ed9490a15fc92b06cc1c47b680ccdf4`  
		Last Modified: Thu, 23 Jan 2020 19:33:23 GMT  
		Size: 301.9 KB (301878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408f862d3a925084a8f20da4818facc02b5136b1c64af46aab594da9a00e6e2a`  
		Last Modified: Fri, 24 Jan 2020 06:19:15 GMT  
		Size: 11.7 MB (11736857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef248f2678020f581052347921213393abe2aef3bb16189ea7eb4feb23c7e819`  
		Last Modified: Fri, 24 Jan 2020 06:19:07 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d0e4328be0f0ee7718f9879334e0abb572bb8941d9baa29140bccb00388dc7`  
		Last Modified: Fri, 24 Jan 2020 06:19:07 GMT  
		Size: 11.9 KB (11896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0a0208ae33af327fb36eae423d4e90cabd9596b9d9b9f0b007ef0da70d8a78`  
		Last Modified: Fri, 24 Jan 2020 06:19:07 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6-alpine`

```console
$ docker pull chronograf@sha256:28a1724975f0d3d915fdd4437bb6dff1248fcba149af3263baacda8d0df53103
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.6-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:ad1c476ad7bceefac0abce84dddcc784f382d48a39c1e7ace47011c45ffca72e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14827436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffbd72c4a0ca324fa58904b89a1e3f7961c0c6f06d9fce279d56816a91dd9cc6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:03:46 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 23 Jan 2020 19:32:40 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 24 Jan 2020 06:18:20 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 24 Jan 2020 06:18:24 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Jan 2020 06:18:24 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 24 Jan 2020 06:18:24 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 24 Jan 2020 06:18:24 GMT
EXPOSE 8888
# Fri, 24 Jan 2020 06:18:25 GMT
VOLUME [/var/lib/chronograf]
# Fri, 24 Jan 2020 06:18:25 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 24 Jan 2020 06:18:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jan 2020 06:18:25 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0018c3785b24046a24095a1f9cf7f42642c3dfd6e8282b328a2e22ce10ebc0de`  
		Last Modified: Thu, 23 Jan 2020 19:07:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cabf7ae254f2fa160de4e52dde588a8ed9490a15fc92b06cc1c47b680ccdf4`  
		Last Modified: Thu, 23 Jan 2020 19:33:23 GMT  
		Size: 301.9 KB (301878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408f862d3a925084a8f20da4818facc02b5136b1c64af46aab594da9a00e6e2a`  
		Last Modified: Fri, 24 Jan 2020 06:19:15 GMT  
		Size: 11.7 MB (11736857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef248f2678020f581052347921213393abe2aef3bb16189ea7eb4feb23c7e819`  
		Last Modified: Fri, 24 Jan 2020 06:19:07 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d0e4328be0f0ee7718f9879334e0abb572bb8941d9baa29140bccb00388dc7`  
		Last Modified: Fri, 24 Jan 2020 06:19:07 GMT  
		Size: 11.9 KB (11896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0a0208ae33af327fb36eae423d4e90cabd9596b9d9b9f0b007ef0da70d8a78`  
		Last Modified: Fri, 24 Jan 2020 06:19:07 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7`

```console
$ docker pull chronograf@sha256:e15a4356281e58b0954836c1048046d0a08f13a478f471b5ad61fffe097b89c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:4af31a0c7af01ad359b72263144bdc51b0e6677b83f47911eb8700234031da78
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65385582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6369312ef45be54f22b95a64579668f5991288d4f8ede6572276146c6f71d0b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:15:39 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 02:16:35 GMT
ENV CHRONOGRAF_VERSION=1.7.16
# Wed, 26 Feb 2020 02:16:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 02:16:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 02:16:51 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 02:16:51 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 02:16:51 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 02:16:52 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 02:16:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 02:16:52 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f878ed3f571cef34099acbbbb2582f64051e11e88b899a5cfe4ef47d003542f`  
		Last Modified: Wed, 26 Feb 2020 02:17:16 GMT  
		Size: 4.5 MB (4503576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff5b5a73702847640aab781ee545a4b2077e73a4a85a517ee56088ea450864e`  
		Last Modified: Wed, 26 Feb 2020 02:18:05 GMT  
		Size: 38.3 MB (38344253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56056118acd55d7c10f5c53ab3a406e4f35aa68068db3bf8f8f6439e0c20e388`  
		Last Modified: Wed, 26 Feb 2020 02:17:38 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3f18a084f300ff69b4a084ea4a695ed721241ca542d77aeabcf95f7294773f`  
		Last Modified: Wed, 26 Feb 2020 02:17:38 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b553df81cc947753f2bec7411800d8512e4ea1ce6e47b225e7c0c3f9d7df2a`  
		Last Modified: Wed, 26 Feb 2020 02:17:39 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:8b9a6d6e4d1c828206936e89d77f6fa3276dccd467fabefae3d22956ba0b491c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (59000595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:734b2e9ac6697225cb9b6fbe4ec157c69c37d3441c8674e759f2934c6433690e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:29:13 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 01:30:28 GMT
ENV CHRONOGRAF_VERSION=1.7.16
# Wed, 26 Feb 2020 01:31:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 01:31:18 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 01:31:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 01:31:20 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 01:31:21 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 01:31:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 01:31:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 01:31:27 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15634d01c3f3a1bece118d96c09deb143bac89f0f8ab71aeb0c0629360a460f`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 3.9 MB (3877306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac8b2235deaa412d6bc31ce4908b924454a93527b924ccc7e44404b7abdfd65`  
		Last Modified: Wed, 26 Feb 2020 01:32:16 GMT  
		Size: 35.8 MB (35800543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60256e9073559fa19192595c43dd01c4ca6317eba445be882f5f228fe100b7b`  
		Last Modified: Wed, 26 Feb 2020 01:32:05 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5889ee4fb1874d8fd4296714e026d8fdce4387daa0428e2854ce703659b5c29`  
		Last Modified: Wed, 26 Feb 2020 01:32:05 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cb666d17fb2835e7b229f1fd07811a095318d900dabf6088618bcf1c4ac620`  
		Last Modified: Wed, 26 Feb 2020 01:32:06 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:3b501af8a2e799b0700a38ed53a30eb64e320f1df002bda54dc839d33f64f544
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60478450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e1fcb5e8de00b7840f34013444deffce779604286f2f0f83eadad52e8f46e14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:10:29 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 04:11:37 GMT
ENV CHRONOGRAF_VERSION=1.7.16
# Wed, 26 Feb 2020 04:11:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 04:12:00 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 04:12:01 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 04:12:01 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 04:12:02 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 04:12:03 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 04:12:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 04:12:06 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f797dde9809216bf453cb02c743c00da5fed52ec53e5d746f9a7cfdb99720f`  
		Last Modified: Wed, 26 Feb 2020 04:12:22 GMT  
		Size: 4.1 MB (4080742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91eca5753b74edb9cb9a58708cf147f0a04a551a576fe25b73081c73b5a0df61`  
		Last Modified: Wed, 26 Feb 2020 04:12:57 GMT  
		Size: 36.0 MB (36003328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427367104eb8e7bc23c10e1733ed32ee7b87515882d24bddc6e4be01426ab91`  
		Last Modified: Wed, 26 Feb 2020 04:12:48 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a947b04ef5079c9592e8f116def09bb3e79187b0b6261191ce28aa82554312a8`  
		Last Modified: Wed, 26 Feb 2020 04:12:48 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9269fe45d674fb606dce55b09b8c6e1933ee376f4bd255d96627a81d34113203`  
		Last Modified: Wed, 26 Feb 2020 04:12:48 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.16`

```console
$ docker pull chronograf@sha256:e15a4356281e58b0954836c1048046d0a08f13a478f471b5ad61fffe097b89c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.16` - linux; amd64

```console
$ docker pull chronograf@sha256:4af31a0c7af01ad359b72263144bdc51b0e6677b83f47911eb8700234031da78
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65385582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6369312ef45be54f22b95a64579668f5991288d4f8ede6572276146c6f71d0b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:15:39 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 02:16:35 GMT
ENV CHRONOGRAF_VERSION=1.7.16
# Wed, 26 Feb 2020 02:16:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 02:16:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 02:16:51 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 02:16:51 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 02:16:51 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 02:16:52 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 02:16:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 02:16:52 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f878ed3f571cef34099acbbbb2582f64051e11e88b899a5cfe4ef47d003542f`  
		Last Modified: Wed, 26 Feb 2020 02:17:16 GMT  
		Size: 4.5 MB (4503576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff5b5a73702847640aab781ee545a4b2077e73a4a85a517ee56088ea450864e`  
		Last Modified: Wed, 26 Feb 2020 02:18:05 GMT  
		Size: 38.3 MB (38344253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56056118acd55d7c10f5c53ab3a406e4f35aa68068db3bf8f8f6439e0c20e388`  
		Last Modified: Wed, 26 Feb 2020 02:17:38 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3f18a084f300ff69b4a084ea4a695ed721241ca542d77aeabcf95f7294773f`  
		Last Modified: Wed, 26 Feb 2020 02:17:38 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b553df81cc947753f2bec7411800d8512e4ea1ce6e47b225e7c0c3f9d7df2a`  
		Last Modified: Wed, 26 Feb 2020 02:17:39 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.16` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:8b9a6d6e4d1c828206936e89d77f6fa3276dccd467fabefae3d22956ba0b491c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (59000595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:734b2e9ac6697225cb9b6fbe4ec157c69c37d3441c8674e759f2934c6433690e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:29:13 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 01:30:28 GMT
ENV CHRONOGRAF_VERSION=1.7.16
# Wed, 26 Feb 2020 01:31:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 01:31:18 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 01:31:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 01:31:20 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 01:31:21 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 01:31:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 01:31:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 01:31:27 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15634d01c3f3a1bece118d96c09deb143bac89f0f8ab71aeb0c0629360a460f`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 3.9 MB (3877306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac8b2235deaa412d6bc31ce4908b924454a93527b924ccc7e44404b7abdfd65`  
		Last Modified: Wed, 26 Feb 2020 01:32:16 GMT  
		Size: 35.8 MB (35800543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60256e9073559fa19192595c43dd01c4ca6317eba445be882f5f228fe100b7b`  
		Last Modified: Wed, 26 Feb 2020 01:32:05 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5889ee4fb1874d8fd4296714e026d8fdce4387daa0428e2854ce703659b5c29`  
		Last Modified: Wed, 26 Feb 2020 01:32:05 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cb666d17fb2835e7b229f1fd07811a095318d900dabf6088618bcf1c4ac620`  
		Last Modified: Wed, 26 Feb 2020 01:32:06 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.16` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:3b501af8a2e799b0700a38ed53a30eb64e320f1df002bda54dc839d33f64f544
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60478450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e1fcb5e8de00b7840f34013444deffce779604286f2f0f83eadad52e8f46e14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:10:29 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 04:11:37 GMT
ENV CHRONOGRAF_VERSION=1.7.16
# Wed, 26 Feb 2020 04:11:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 04:12:00 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 04:12:01 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 04:12:01 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 04:12:02 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 04:12:03 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 04:12:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 04:12:06 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f797dde9809216bf453cb02c743c00da5fed52ec53e5d746f9a7cfdb99720f`  
		Last Modified: Wed, 26 Feb 2020 04:12:22 GMT  
		Size: 4.1 MB (4080742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91eca5753b74edb9cb9a58708cf147f0a04a551a576fe25b73081c73b5a0df61`  
		Last Modified: Wed, 26 Feb 2020 04:12:57 GMT  
		Size: 36.0 MB (36003328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427367104eb8e7bc23c10e1733ed32ee7b87515882d24bddc6e4be01426ab91`  
		Last Modified: Wed, 26 Feb 2020 04:12:48 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a947b04ef5079c9592e8f116def09bb3e79187b0b6261191ce28aa82554312a8`  
		Last Modified: Wed, 26 Feb 2020 04:12:48 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9269fe45d674fb606dce55b09b8c6e1933ee376f4bd255d96627a81d34113203`  
		Last Modified: Wed, 26 Feb 2020 04:12:48 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.16-alpine`

```console
$ docker pull chronograf@sha256:fb179947c124394dfe1ad86a69f8a5b3dbb71673c074a6274b9c3b0410291a13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.7.16-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:f3b9c76d16e20144dace9f0a8a00d95a82c05e5209407d52be8ae1fe45993d8a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22646541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a16d0f0f9db199994edeffe29a377125cf4c22db90b17980fb597280d987fcff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:03:46 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 23 Jan 2020 19:32:40 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 24 Jan 2020 06:18:32 GMT
ENV CHRONOGRAF_VERSION=1.7.16
# Fri, 24 Jan 2020 06:18:37 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Jan 2020 06:18:38 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 24 Jan 2020 06:18:38 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 24 Jan 2020 06:18:38 GMT
EXPOSE 8888
# Fri, 24 Jan 2020 06:18:38 GMT
VOLUME [/var/lib/chronograf]
# Fri, 24 Jan 2020 06:18:39 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 24 Jan 2020 06:18:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jan 2020 06:18:39 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0018c3785b24046a24095a1f9cf7f42642c3dfd6e8282b328a2e22ce10ebc0de`  
		Last Modified: Thu, 23 Jan 2020 19:07:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cabf7ae254f2fa160de4e52dde588a8ed9490a15fc92b06cc1c47b680ccdf4`  
		Last Modified: Thu, 23 Jan 2020 19:33:23 GMT  
		Size: 301.9 KB (301878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe71ecdd62685580afe85276ea2d0243a8a2577f1324e8c512f797fef9dee135`  
		Last Modified: Fri, 24 Jan 2020 06:19:28 GMT  
		Size: 19.6 MB (19555966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df31809678f6d8cc5fcbecb90b4ed64398630fca3dd3427ea594fcf812f1c10`  
		Last Modified: Fri, 24 Jan 2020 06:19:21 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0071045c16456ab436c57d69aa6c07a03b8c1a52956957647fbe6feab766cd5b`  
		Last Modified: Fri, 24 Jan 2020 06:19:20 GMT  
		Size: 11.9 KB (11893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b4b372df041bab39caf0f2afbc9fe8f703e3ccf9b5b826fab62077a7016d8e`  
		Last Modified: Fri, 24 Jan 2020 06:19:21 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:fb179947c124394dfe1ad86a69f8a5b3dbb71673c074a6274b9c3b0410291a13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.7-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:f3b9c76d16e20144dace9f0a8a00d95a82c05e5209407d52be8ae1fe45993d8a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22646541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a16d0f0f9db199994edeffe29a377125cf4c22db90b17980fb597280d987fcff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:03:46 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 23 Jan 2020 19:32:40 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 24 Jan 2020 06:18:32 GMT
ENV CHRONOGRAF_VERSION=1.7.16
# Fri, 24 Jan 2020 06:18:37 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Jan 2020 06:18:38 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 24 Jan 2020 06:18:38 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 24 Jan 2020 06:18:38 GMT
EXPOSE 8888
# Fri, 24 Jan 2020 06:18:38 GMT
VOLUME [/var/lib/chronograf]
# Fri, 24 Jan 2020 06:18:39 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 24 Jan 2020 06:18:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jan 2020 06:18:39 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0018c3785b24046a24095a1f9cf7f42642c3dfd6e8282b328a2e22ce10ebc0de`  
		Last Modified: Thu, 23 Jan 2020 19:07:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cabf7ae254f2fa160de4e52dde588a8ed9490a15fc92b06cc1c47b680ccdf4`  
		Last Modified: Thu, 23 Jan 2020 19:33:23 GMT  
		Size: 301.9 KB (301878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe71ecdd62685580afe85276ea2d0243a8a2577f1324e8c512f797fef9dee135`  
		Last Modified: Fri, 24 Jan 2020 06:19:28 GMT  
		Size: 19.6 MB (19555966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df31809678f6d8cc5fcbecb90b4ed64398630fca3dd3427ea594fcf812f1c10`  
		Last Modified: Fri, 24 Jan 2020 06:19:21 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0071045c16456ab436c57d69aa6c07a03b8c1a52956957647fbe6feab766cd5b`  
		Last Modified: Fri, 24 Jan 2020 06:19:20 GMT  
		Size: 11.9 KB (11893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b4b372df041bab39caf0f2afbc9fe8f703e3ccf9b5b826fab62077a7016d8e`  
		Last Modified: Fri, 24 Jan 2020 06:19:21 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:fb179947c124394dfe1ad86a69f8a5b3dbb71673c074a6274b9c3b0410291a13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:f3b9c76d16e20144dace9f0a8a00d95a82c05e5209407d52be8ae1fe45993d8a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22646541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a16d0f0f9db199994edeffe29a377125cf4c22db90b17980fb597280d987fcff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:03:46 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 23 Jan 2020 19:32:40 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 24 Jan 2020 06:18:32 GMT
ENV CHRONOGRAF_VERSION=1.7.16
# Fri, 24 Jan 2020 06:18:37 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Jan 2020 06:18:38 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 24 Jan 2020 06:18:38 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 24 Jan 2020 06:18:38 GMT
EXPOSE 8888
# Fri, 24 Jan 2020 06:18:38 GMT
VOLUME [/var/lib/chronograf]
# Fri, 24 Jan 2020 06:18:39 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 24 Jan 2020 06:18:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jan 2020 06:18:39 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0018c3785b24046a24095a1f9cf7f42642c3dfd6e8282b328a2e22ce10ebc0de`  
		Last Modified: Thu, 23 Jan 2020 19:07:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cabf7ae254f2fa160de4e52dde588a8ed9490a15fc92b06cc1c47b680ccdf4`  
		Last Modified: Thu, 23 Jan 2020 19:33:23 GMT  
		Size: 301.9 KB (301878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe71ecdd62685580afe85276ea2d0243a8a2577f1324e8c512f797fef9dee135`  
		Last Modified: Fri, 24 Jan 2020 06:19:28 GMT  
		Size: 19.6 MB (19555966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df31809678f6d8cc5fcbecb90b4ed64398630fca3dd3427ea594fcf812f1c10`  
		Last Modified: Fri, 24 Jan 2020 06:19:21 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0071045c16456ab436c57d69aa6c07a03b8c1a52956957647fbe6feab766cd5b`  
		Last Modified: Fri, 24 Jan 2020 06:19:20 GMT  
		Size: 11.9 KB (11893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b4b372df041bab39caf0f2afbc9fe8f703e3ccf9b5b826fab62077a7016d8e`  
		Last Modified: Fri, 24 Jan 2020 06:19:21 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:latest`

```console
$ docker pull chronograf@sha256:e15a4356281e58b0954836c1048046d0a08f13a478f471b5ad61fffe097b89c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:4af31a0c7af01ad359b72263144bdc51b0e6677b83f47911eb8700234031da78
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65385582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6369312ef45be54f22b95a64579668f5991288d4f8ede6572276146c6f71d0b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:15:39 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 02:16:35 GMT
ENV CHRONOGRAF_VERSION=1.7.16
# Wed, 26 Feb 2020 02:16:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 02:16:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 02:16:51 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 02:16:51 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 02:16:51 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 02:16:52 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 02:16:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 02:16:52 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f878ed3f571cef34099acbbbb2582f64051e11e88b899a5cfe4ef47d003542f`  
		Last Modified: Wed, 26 Feb 2020 02:17:16 GMT  
		Size: 4.5 MB (4503576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff5b5a73702847640aab781ee545a4b2077e73a4a85a517ee56088ea450864e`  
		Last Modified: Wed, 26 Feb 2020 02:18:05 GMT  
		Size: 38.3 MB (38344253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56056118acd55d7c10f5c53ab3a406e4f35aa68068db3bf8f8f6439e0c20e388`  
		Last Modified: Wed, 26 Feb 2020 02:17:38 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3f18a084f300ff69b4a084ea4a695ed721241ca542d77aeabcf95f7294773f`  
		Last Modified: Wed, 26 Feb 2020 02:17:38 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b553df81cc947753f2bec7411800d8512e4ea1ce6e47b225e7c0c3f9d7df2a`  
		Last Modified: Wed, 26 Feb 2020 02:17:39 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:8b9a6d6e4d1c828206936e89d77f6fa3276dccd467fabefae3d22956ba0b491c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (59000595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:734b2e9ac6697225cb9b6fbe4ec157c69c37d3441c8674e759f2934c6433690e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:29:13 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 01:30:28 GMT
ENV CHRONOGRAF_VERSION=1.7.16
# Wed, 26 Feb 2020 01:31:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 01:31:18 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 01:31:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 01:31:20 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 01:31:21 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 01:31:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 01:31:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 01:31:27 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15634d01c3f3a1bece118d96c09deb143bac89f0f8ab71aeb0c0629360a460f`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 3.9 MB (3877306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac8b2235deaa412d6bc31ce4908b924454a93527b924ccc7e44404b7abdfd65`  
		Last Modified: Wed, 26 Feb 2020 01:32:16 GMT  
		Size: 35.8 MB (35800543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60256e9073559fa19192595c43dd01c4ca6317eba445be882f5f228fe100b7b`  
		Last Modified: Wed, 26 Feb 2020 01:32:05 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5889ee4fb1874d8fd4296714e026d8fdce4387daa0428e2854ce703659b5c29`  
		Last Modified: Wed, 26 Feb 2020 01:32:05 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cb666d17fb2835e7b229f1fd07811a095318d900dabf6088618bcf1c4ac620`  
		Last Modified: Wed, 26 Feb 2020 01:32:06 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:3b501af8a2e799b0700a38ed53a30eb64e320f1df002bda54dc839d33f64f544
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60478450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e1fcb5e8de00b7840f34013444deffce779604286f2f0f83eadad52e8f46e14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:10:29 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 26 Feb 2020 04:11:37 GMT
ENV CHRONOGRAF_VERSION=1.7.16
# Wed, 26 Feb 2020 04:11:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Feb 2020 04:12:00 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 26 Feb 2020 04:12:01 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 26 Feb 2020 04:12:01 GMT
EXPOSE 8888
# Wed, 26 Feb 2020 04:12:02 GMT
VOLUME [/var/lib/chronograf]
# Wed, 26 Feb 2020 04:12:03 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 26 Feb 2020 04:12:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 04:12:06 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f797dde9809216bf453cb02c743c00da5fed52ec53e5d746f9a7cfdb99720f`  
		Last Modified: Wed, 26 Feb 2020 04:12:22 GMT  
		Size: 4.1 MB (4080742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91eca5753b74edb9cb9a58708cf147f0a04a551a576fe25b73081c73b5a0df61`  
		Last Modified: Wed, 26 Feb 2020 04:12:57 GMT  
		Size: 36.0 MB (36003328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427367104eb8e7bc23c10e1733ed32ee7b87515882d24bddc6e4be01426ab91`  
		Last Modified: Wed, 26 Feb 2020 04:12:48 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a947b04ef5079c9592e8f116def09bb3e79187b0b6261191ce28aa82554312a8`  
		Last Modified: Wed, 26 Feb 2020 04:12:48 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9269fe45d674fb606dce55b09b8c6e1933ee376f4bd255d96627a81d34113203`  
		Last Modified: Wed, 26 Feb 2020 04:12:48 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
