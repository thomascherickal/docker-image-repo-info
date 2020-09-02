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
-	[`chronograf:1.8.6`](#chronograf186)
-	[`chronograf:1.8.6-alpine`](#chronograf186-alpine)
-	[`chronograf:1.8-alpine`](#chronograf18-alpine)
-	[`chronograf:alpine`](#chronografalpine)
-	[`chronograf:latest`](#chronograflatest)

## `chronograf:1.6`

```console
$ docker pull chronograf@sha256:c8235bf58f386ef593c7a3218eb274f2dd310760ddcf6a599fca7395839fd350
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6` - linux; amd64

```console
$ docker pull chronograf@sha256:6dee39d2c3c194b9337433d500c07dcf9382e51f1a3f8258b6f38f97dd3f491b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49332242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:192949b21d728e0ab7f60d53c192775c01f6d4f83dffae08ca011a87bb2459bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Wed, 02 Sep 2020 00:08:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 02 Sep 2020 00:08:41 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 02 Sep 2020 00:08:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 02 Sep 2020 00:08:48 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 02 Sep 2020 00:08:48 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 02 Sep 2020 00:08:48 GMT
EXPOSE 8888
# Wed, 02 Sep 2020 00:08:48 GMT
VOLUME [/var/lib/chronograf]
# Wed, 02 Sep 2020 00:08:49 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 02 Sep 2020 00:08:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Sep 2020 00:08:49 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afff3f2fb3db7c061b33082931d5ba904dfd5cc528cc6d7e74e2d5d6821701c`  
		Last Modified: Wed, 02 Sep 2020 00:10:18 GMT  
		Size: 6.7 MB (6742093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd940f94a0f447d5ce837fcdba05941675190c7e6d1af3b2c8e66fe3d2ef87c`  
		Last Modified: Wed, 02 Sep 2020 00:10:20 GMT  
		Size: 20.0 MB (20043473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79714ed2b3ac2c73d6030f148362f4b685dbc2cfd96e81a67006aceb8f9aa3ee`  
		Last Modified: Wed, 02 Sep 2020 00:10:16 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7f09d8d576fa8be87ff1ffc474c8a0753b7e3ed787069a24cbb2fee275dcc5`  
		Last Modified: Wed, 02 Sep 2020 00:10:16 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c170cc72e6d1d0020d04344d26003a9406c4b8260e7092896497a2e5250f13c2`  
		Last Modified: Wed, 02 Sep 2020 00:10:16 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:b472157993683c6521c6a749dcaf5f738644f3f53d8052992f1d6f2a58241134
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43682171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5474e080ebd414279ac5cc1b391d09fd14f2c0f0f2b5d4163e2b7b511dc0bf63`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 05:01:30 GMT
ADD file:3d69e3d8fb19d3a9c5fc738b4c9b3c436f9ba10b16c057523360b3443dcd7570 in / 
# Tue, 04 Aug 2020 05:01:32 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:40:09 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 04 Aug 2020 08:40:21 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 04 Aug 2020 08:41:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 08:41:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 04 Aug 2020 08:41:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 04 Aug 2020 08:42:00 GMT
EXPOSE 8888
# Tue, 04 Aug 2020 08:42:09 GMT
VOLUME [/var/lib/chronograf]
# Tue, 04 Aug 2020 08:42:22 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 04 Aug 2020 08:42:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Aug 2020 08:42:35 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b33d4edf196b4a005f13932d074987a85eb6c927dc64b40989598b3ade8ebc5c`  
		Last Modified: Tue, 04 Aug 2020 05:09:01 GMT  
		Size: 19.3 MB (19304611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb933ad4bb85672991fffc11bb98b3d11d98ccd0523793e0699c1eb81ca6817e`  
		Last Modified: Tue, 04 Aug 2020 08:45:40 GMT  
		Size: 3.9 MB (3878320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e7f92e0d97f7611b2ea85e9ce43ed573114f4c05315e5d29761d14cf10d2b4`  
		Last Modified: Tue, 04 Aug 2020 08:45:46 GMT  
		Size: 20.5 MB (20474838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42b56a534c9cb1da08e138f42d23c5be9ffc1cbeacf3ec51a7866ad149101df`  
		Last Modified: Tue, 04 Aug 2020 08:45:39 GMT  
		Size: 12.3 KB (12252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bed665ba4db94e43d7a67f3fea32ee117825dcda905a01295961cd5ddad302f`  
		Last Modified: Tue, 04 Aug 2020 08:45:39 GMT  
		Size: 11.9 KB (11912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90ffec65b1574e6f5d51cbfcdf5db44742f82d7679002cd2222194163bc4a25`  
		Last Modified: Tue, 04 Aug 2020 08:45:39 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:90172255076fc052b7b997c30205d52bdf9801ff4aede8833d8685b371a5d944
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45387762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed0ed9d2af677eb32a03b81fa2e75e72378c51de6a0e9a89d96f1d90d9445868`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 07:00:02 GMT
ADD file:448eac8822629a9f212483d0e6123c797105b2ec368648e6f259b7d4cb83e0a1 in / 
# Tue, 04 Aug 2020 07:00:04 GMT
CMD ["bash"]
# Tue, 01 Sep 2020 23:34:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 01 Sep 2020 23:34:56 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 01 Sep 2020 23:36:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Sep 2020 23:36:09 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 01 Sep 2020 23:36:22 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 01 Sep 2020 23:36:32 GMT
EXPOSE 8888
# Tue, 01 Sep 2020 23:36:45 GMT
VOLUME [/var/lib/chronograf]
# Tue, 01 Sep 2020 23:36:46 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 01 Sep 2020 23:36:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Sep 2020 23:36:47 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:5984ce78d2759fcb147a7641f941b59e71e8c9f82aa5cb0e3d511c74c876a7e3`  
		Last Modified: Tue, 04 Aug 2020 07:06:31 GMT  
		Size: 20.4 MB (20377078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f266d2355710732ee4f239f9bce3a8c3e01e7a804b84421c3727e009a175dfd`  
		Last Modified: Tue, 01 Sep 2020 23:43:01 GMT  
		Size: 6.0 MB (6027754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5dfda5016a949361a1a43169e2b0affd58d6a8a885de52eedd622c194e109d`  
		Last Modified: Tue, 01 Sep 2020 23:43:07 GMT  
		Size: 19.0 MB (18958522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa3452dd26cc0cd409315803a64383dbe397e461378a594744c8e56afe10b37`  
		Last Modified: Tue, 01 Sep 2020 23:43:00 GMT  
		Size: 12.3 KB (12256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3fde642de8b237e4bb599b6049061c52cde751734228c5cf74cf490ec61eae`  
		Last Modified: Tue, 01 Sep 2020 23:42:58 GMT  
		Size: 11.9 KB (11913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6f9344378e14c2b52697fba7fc87d448c19ec97dd9003eb7196d908bf42e07`  
		Last Modified: Tue, 01 Sep 2020 23:42:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2`

```console
$ docker pull chronograf@sha256:c8235bf58f386ef593c7a3218eb274f2dd310760ddcf6a599fca7395839fd350
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6.2` - linux; amd64

```console
$ docker pull chronograf@sha256:6dee39d2c3c194b9337433d500c07dcf9382e51f1a3f8258b6f38f97dd3f491b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49332242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:192949b21d728e0ab7f60d53c192775c01f6d4f83dffae08ca011a87bb2459bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Wed, 02 Sep 2020 00:08:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 02 Sep 2020 00:08:41 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 02 Sep 2020 00:08:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 02 Sep 2020 00:08:48 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 02 Sep 2020 00:08:48 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 02 Sep 2020 00:08:48 GMT
EXPOSE 8888
# Wed, 02 Sep 2020 00:08:48 GMT
VOLUME [/var/lib/chronograf]
# Wed, 02 Sep 2020 00:08:49 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 02 Sep 2020 00:08:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Sep 2020 00:08:49 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afff3f2fb3db7c061b33082931d5ba904dfd5cc528cc6d7e74e2d5d6821701c`  
		Last Modified: Wed, 02 Sep 2020 00:10:18 GMT  
		Size: 6.7 MB (6742093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd940f94a0f447d5ce837fcdba05941675190c7e6d1af3b2c8e66fe3d2ef87c`  
		Last Modified: Wed, 02 Sep 2020 00:10:20 GMT  
		Size: 20.0 MB (20043473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79714ed2b3ac2c73d6030f148362f4b685dbc2cfd96e81a67006aceb8f9aa3ee`  
		Last Modified: Wed, 02 Sep 2020 00:10:16 GMT  
		Size: 12.3 KB (12251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7f09d8d576fa8be87ff1ffc474c8a0753b7e3ed787069a24cbb2fee275dcc5`  
		Last Modified: Wed, 02 Sep 2020 00:10:16 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c170cc72e6d1d0020d04344d26003a9406c4b8260e7092896497a2e5250f13c2`  
		Last Modified: Wed, 02 Sep 2020 00:10:16 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:b472157993683c6521c6a749dcaf5f738644f3f53d8052992f1d6f2a58241134
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43682171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5474e080ebd414279ac5cc1b391d09fd14f2c0f0f2b5d4163e2b7b511dc0bf63`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 05:01:30 GMT
ADD file:3d69e3d8fb19d3a9c5fc738b4c9b3c436f9ba10b16c057523360b3443dcd7570 in / 
# Tue, 04 Aug 2020 05:01:32 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:40:09 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 04 Aug 2020 08:40:21 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 04 Aug 2020 08:41:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 08:41:30 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 04 Aug 2020 08:41:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 04 Aug 2020 08:42:00 GMT
EXPOSE 8888
# Tue, 04 Aug 2020 08:42:09 GMT
VOLUME [/var/lib/chronograf]
# Tue, 04 Aug 2020 08:42:22 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 04 Aug 2020 08:42:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Aug 2020 08:42:35 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b33d4edf196b4a005f13932d074987a85eb6c927dc64b40989598b3ade8ebc5c`  
		Last Modified: Tue, 04 Aug 2020 05:09:01 GMT  
		Size: 19.3 MB (19304611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb933ad4bb85672991fffc11bb98b3d11d98ccd0523793e0699c1eb81ca6817e`  
		Last Modified: Tue, 04 Aug 2020 08:45:40 GMT  
		Size: 3.9 MB (3878320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e7f92e0d97f7611b2ea85e9ce43ed573114f4c05315e5d29761d14cf10d2b4`  
		Last Modified: Tue, 04 Aug 2020 08:45:46 GMT  
		Size: 20.5 MB (20474838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42b56a534c9cb1da08e138f42d23c5be9ffc1cbeacf3ec51a7866ad149101df`  
		Last Modified: Tue, 04 Aug 2020 08:45:39 GMT  
		Size: 12.3 KB (12252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bed665ba4db94e43d7a67f3fea32ee117825dcda905a01295961cd5ddad302f`  
		Last Modified: Tue, 04 Aug 2020 08:45:39 GMT  
		Size: 11.9 KB (11912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90ffec65b1574e6f5d51cbfcdf5db44742f82d7679002cd2222194163bc4a25`  
		Last Modified: Tue, 04 Aug 2020 08:45:39 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:90172255076fc052b7b997c30205d52bdf9801ff4aede8833d8685b371a5d944
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45387762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed0ed9d2af677eb32a03b81fa2e75e72378c51de6a0e9a89d96f1d90d9445868`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 07:00:02 GMT
ADD file:448eac8822629a9f212483d0e6123c797105b2ec368648e6f259b7d4cb83e0a1 in / 
# Tue, 04 Aug 2020 07:00:04 GMT
CMD ["bash"]
# Tue, 01 Sep 2020 23:34:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 01 Sep 2020 23:34:56 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Tue, 01 Sep 2020 23:36:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Sep 2020 23:36:09 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 01 Sep 2020 23:36:22 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 01 Sep 2020 23:36:32 GMT
EXPOSE 8888
# Tue, 01 Sep 2020 23:36:45 GMT
VOLUME [/var/lib/chronograf]
# Tue, 01 Sep 2020 23:36:46 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 01 Sep 2020 23:36:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Sep 2020 23:36:47 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:5984ce78d2759fcb147a7641f941b59e71e8c9f82aa5cb0e3d511c74c876a7e3`  
		Last Modified: Tue, 04 Aug 2020 07:06:31 GMT  
		Size: 20.4 MB (20377078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f266d2355710732ee4f239f9bce3a8c3e01e7a804b84421c3727e009a175dfd`  
		Last Modified: Tue, 01 Sep 2020 23:43:01 GMT  
		Size: 6.0 MB (6027754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5dfda5016a949361a1a43169e2b0affd58d6a8a885de52eedd622c194e109d`  
		Last Modified: Tue, 01 Sep 2020 23:43:07 GMT  
		Size: 19.0 MB (18958522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa3452dd26cc0cd409315803a64383dbe397e461378a594744c8e56afe10b37`  
		Last Modified: Tue, 01 Sep 2020 23:43:00 GMT  
		Size: 12.3 KB (12256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3fde642de8b237e4bb599b6049061c52cde751734228c5cf74cf490ec61eae`  
		Last Modified: Tue, 01 Sep 2020 23:42:58 GMT  
		Size: 11.9 KB (11913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6f9344378e14c2b52697fba7fc87d448c19ec97dd9003eb7196d908bf42e07`  
		Last Modified: Tue, 01 Sep 2020 23:42:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2-alpine`

```console
$ docker pull chronograf@sha256:e57907702a20b674dead075050a1343d3f19e9145cce45a5476f9a397e33b3ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.6.2-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:4a09f076901c8e93fd675920c8c815daf239daeb74bc7515f3de2f64563fc18a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14839707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01053d512100c074e0ff0c32e02e531dc031f94c2f116255fa69db72d2d4d933`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 23 Jul 2020 05:22:10 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:38:19 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 01 Sep 2020 00:38:19 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 02 Sep 2020 00:08:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 02 Sep 2020 00:08:58 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Wed, 02 Sep 2020 00:08:58 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 02 Sep 2020 00:08:58 GMT
EXPOSE 8888
# Wed, 02 Sep 2020 00:08:58 GMT
VOLUME [/var/lib/chronograf]
# Wed, 02 Sep 2020 00:08:59 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 02 Sep 2020 00:08:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Sep 2020 00:08:59 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ed77ee1a57b06efa2aeb4cc06845d93ce8c6e8b2ca507267000b5a6edddffa`  
		Last Modified: Thu, 23 Jul 2020 05:23:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61626b3b2d7f1da2eb5ae3486f7e2baf21fb5b7dd993595b8fe0fbe2a34445d6`  
		Last Modified: Tue, 01 Sep 2020 00:39:25 GMT  
		Size: 280.8 KB (280831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd21c10868843c1212c8450b499201f0be8a6f060d9babca97fc0935f18be556`  
		Last Modified: Wed, 02 Sep 2020 00:10:26 GMT  
		Size: 11.7 MB (11736804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf515696ab11ba9ab1a9fd88211b884b63eeab8afd0c706c875e9c9625c40618`  
		Last Modified: Wed, 02 Sep 2020 00:10:23 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90df5f0909da4b37414d999f07f6fb9310d55077d0d2714d1c2929b6520f5b9`  
		Last Modified: Wed, 02 Sep 2020 00:10:24 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3b5a611532769eb38fd565ed51950369f81e6309c4a1bdb66cf6906cfbaa48`  
		Last Modified: Wed, 02 Sep 2020 00:10:23 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6-alpine`

```console
$ docker pull chronograf@sha256:e57907702a20b674dead075050a1343d3f19e9145cce45a5476f9a397e33b3ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.6-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:4a09f076901c8e93fd675920c8c815daf239daeb74bc7515f3de2f64563fc18a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14839707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01053d512100c074e0ff0c32e02e531dc031f94c2f116255fa69db72d2d4d933`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 23 Jul 2020 05:22:10 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:38:19 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 01 Sep 2020 00:38:19 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Wed, 02 Sep 2020 00:08:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 02 Sep 2020 00:08:58 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Wed, 02 Sep 2020 00:08:58 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 02 Sep 2020 00:08:58 GMT
EXPOSE 8888
# Wed, 02 Sep 2020 00:08:58 GMT
VOLUME [/var/lib/chronograf]
# Wed, 02 Sep 2020 00:08:59 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 02 Sep 2020 00:08:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Sep 2020 00:08:59 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ed77ee1a57b06efa2aeb4cc06845d93ce8c6e8b2ca507267000b5a6edddffa`  
		Last Modified: Thu, 23 Jul 2020 05:23:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61626b3b2d7f1da2eb5ae3486f7e2baf21fb5b7dd993595b8fe0fbe2a34445d6`  
		Last Modified: Tue, 01 Sep 2020 00:39:25 GMT  
		Size: 280.8 KB (280831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd21c10868843c1212c8450b499201f0be8a6f060d9babca97fc0935f18be556`  
		Last Modified: Wed, 02 Sep 2020 00:10:26 GMT  
		Size: 11.7 MB (11736804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf515696ab11ba9ab1a9fd88211b884b63eeab8afd0c706c875e9c9625c40618`  
		Last Modified: Wed, 02 Sep 2020 00:10:23 GMT  
		Size: 12.2 KB (12241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90df5f0909da4b37414d999f07f6fb9310d55077d0d2714d1c2929b6520f5b9`  
		Last Modified: Wed, 02 Sep 2020 00:10:24 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3b5a611532769eb38fd565ed51950369f81e6309c4a1bdb66cf6906cfbaa48`  
		Last Modified: Wed, 02 Sep 2020 00:10:23 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7`

```console
$ docker pull chronograf@sha256:5eaf00ac6e9bce5f63d0b30cf2ff1fd7dca7afa8dc98de41c284f68240203337
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:5577c9fcfb376268267593f5f7e723a4621cf54c53222df4568c62641a36d11e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65360273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90fb77b17d580419c984fd77b5d291a0d1a2cb0f3700fc071c127e8b6d4fa096`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Wed, 02 Sep 2020 00:09:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 02 Sep 2020 00:09:10 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 02 Sep 2020 00:09:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 02 Sep 2020 00:09:21 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 02 Sep 2020 00:09:21 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 02 Sep 2020 00:09:21 GMT
EXPOSE 8888
# Wed, 02 Sep 2020 00:09:21 GMT
VOLUME [/var/lib/chronograf]
# Wed, 02 Sep 2020 00:09:21 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 02 Sep 2020 00:09:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Sep 2020 00:09:22 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f93ab8c834ff3edf8f966a7e4e5e2dfe6a0366deb5bb049901ca62f9c0dbbe`  
		Last Modified: Wed, 02 Sep 2020 00:10:30 GMT  
		Size: 4.5 MB (4504580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae77bd8c5b5e94c140cc539195f61c9564a1ff3bf79c737e531b6c2ae8bc2fc3`  
		Last Modified: Wed, 02 Sep 2020 00:10:35 GMT  
		Size: 38.3 MB (38309018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b55db1dfed515c97c617df4b9cf6352e34244573ae9765c4e93ae334416471`  
		Last Modified: Wed, 02 Sep 2020 00:10:30 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b392138da0ee70c6ec0334a041e221ecbe526116c298179fde0dfb3c014b9a`  
		Last Modified: Wed, 02 Sep 2020 00:10:29 GMT  
		Size: 11.9 KB (11912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe0d6b48a675838a0cd998e910896daa325cede286252fee3c24db8a83d978a`  
		Last Modified: Wed, 02 Sep 2020 00:10:29 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:9bfa82e88c4e414e26d3de28d4eccc868fadddfb7fe05a1a4f4e04334f69f36c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58959657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:728c488391ea19f9edcfb2c6a344c0478d602672053e1ab0240a288cc372c897`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 05:01:30 GMT
ADD file:3d69e3d8fb19d3a9c5fc738b4c9b3c436f9ba10b16c057523360b3443dcd7570 in / 
# Tue, 04 Aug 2020 05:01:32 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:40:09 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 04 Aug 2020 08:43:09 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 04 Aug 2020 08:44:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 08:44:21 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 04 Aug 2020 08:44:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 04 Aug 2020 08:44:23 GMT
EXPOSE 8888
# Tue, 04 Aug 2020 08:44:26 GMT
VOLUME [/var/lib/chronograf]
# Tue, 04 Aug 2020 08:44:29 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 04 Aug 2020 08:44:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Aug 2020 08:44:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b33d4edf196b4a005f13932d074987a85eb6c927dc64b40989598b3ade8ebc5c`  
		Last Modified: Tue, 04 Aug 2020 05:09:01 GMT  
		Size: 19.3 MB (19304611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb933ad4bb85672991fffc11bb98b3d11d98ccd0523793e0699c1eb81ca6817e`  
		Last Modified: Tue, 04 Aug 2020 08:45:40 GMT  
		Size: 3.9 MB (3878320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fa3e46c20d6342a32f4bd3473fe5daf746811c4063cb533a8e86344b016ea5`  
		Last Modified: Tue, 04 Aug 2020 08:46:07 GMT  
		Size: 35.8 MB (35752327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e3f2101a123761af772978b35c286415d31462d0e9d0762c721f241261eb7d`  
		Last Modified: Tue, 04 Aug 2020 08:45:53 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c29ae49c457f8714c437eac4d0befc8c927bd54fd383eb41ff112daa2c5a76`  
		Last Modified: Tue, 04 Aug 2020 08:45:53 GMT  
		Size: 11.9 KB (11911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e397f9f1bd96ce9ac240b8b1ec7c03c20b63c0d0de27a1637d00606ed2052ee6`  
		Last Modified: Tue, 04 Aug 2020 08:45:53 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:01f0aa43a1fb22fc1956c776293772318b916adf9ab04a3398c3dee89cd42564
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60444932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b8890ce936d4c4680bc13ac9cf44755c3831519a8135ee572799c880d1ea92`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 07:00:02 GMT
ADD file:448eac8822629a9f212483d0e6123c797105b2ec368648e6f259b7d4cb83e0a1 in / 
# Tue, 04 Aug 2020 07:00:04 GMT
CMD ["bash"]
# Tue, 01 Sep 2020 23:37:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 01 Sep 2020 23:37:42 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 01 Sep 2020 23:38:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Sep 2020 23:39:01 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 01 Sep 2020 23:39:09 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 01 Sep 2020 23:39:16 GMT
EXPOSE 8888
# Tue, 01 Sep 2020 23:39:31 GMT
VOLUME [/var/lib/chronograf]
# Tue, 01 Sep 2020 23:39:43 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 01 Sep 2020 23:40:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Sep 2020 23:40:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:5984ce78d2759fcb147a7641f941b59e71e8c9f82aa5cb0e3d511c74c876a7e3`  
		Last Modified: Tue, 04 Aug 2020 07:06:31 GMT  
		Size: 20.4 MB (20377078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8165183b47acbd3117b1d889ee5c8a78488c48be0e817a37c480248ef97679`  
		Last Modified: Tue, 01 Sep 2020 23:43:20 GMT  
		Size: 4.1 MB (4082049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d221a550fef5c44757a289be1e85910e33626d64a0a642a3611466d77048648`  
		Last Modified: Tue, 01 Sep 2020 23:43:29 GMT  
		Size: 36.0 MB (35961400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2e886b4d1c9321a1c819921b7ddce621eef3fd89c5a965bee46167484b570a`  
		Last Modified: Tue, 01 Sep 2020 23:43:17 GMT  
		Size: 12.3 KB (12253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b185042a25e2948de7a58dcf548e701b06a9886173d52d3a0b9522c733f94342`  
		Last Modified: Tue, 01 Sep 2020 23:43:17 GMT  
		Size: 11.9 KB (11913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903451520a8c22062b2f9c761751cb62f65753a0f0e85987dd73e354f484a9a9`  
		Last Modified: Tue, 01 Sep 2020 23:43:17 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17`

```console
$ docker pull chronograf@sha256:5eaf00ac6e9bce5f63d0b30cf2ff1fd7dca7afa8dc98de41c284f68240203337
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:5577c9fcfb376268267593f5f7e723a4621cf54c53222df4568c62641a36d11e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65360273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90fb77b17d580419c984fd77b5d291a0d1a2cb0f3700fc071c127e8b6d4fa096`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Wed, 02 Sep 2020 00:09:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 02 Sep 2020 00:09:10 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 02 Sep 2020 00:09:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 02 Sep 2020 00:09:21 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 02 Sep 2020 00:09:21 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 02 Sep 2020 00:09:21 GMT
EXPOSE 8888
# Wed, 02 Sep 2020 00:09:21 GMT
VOLUME [/var/lib/chronograf]
# Wed, 02 Sep 2020 00:09:21 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 02 Sep 2020 00:09:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Sep 2020 00:09:22 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f93ab8c834ff3edf8f966a7e4e5e2dfe6a0366deb5bb049901ca62f9c0dbbe`  
		Last Modified: Wed, 02 Sep 2020 00:10:30 GMT  
		Size: 4.5 MB (4504580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae77bd8c5b5e94c140cc539195f61c9564a1ff3bf79c737e531b6c2ae8bc2fc3`  
		Last Modified: Wed, 02 Sep 2020 00:10:35 GMT  
		Size: 38.3 MB (38309018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b55db1dfed515c97c617df4b9cf6352e34244573ae9765c4e93ae334416471`  
		Last Modified: Wed, 02 Sep 2020 00:10:30 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b392138da0ee70c6ec0334a041e221ecbe526116c298179fde0dfb3c014b9a`  
		Last Modified: Wed, 02 Sep 2020 00:10:29 GMT  
		Size: 11.9 KB (11912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe0d6b48a675838a0cd998e910896daa325cede286252fee3c24db8a83d978a`  
		Last Modified: Wed, 02 Sep 2020 00:10:29 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:9bfa82e88c4e414e26d3de28d4eccc868fadddfb7fe05a1a4f4e04334f69f36c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58959657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:728c488391ea19f9edcfb2c6a344c0478d602672053e1ab0240a288cc372c897`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 05:01:30 GMT
ADD file:3d69e3d8fb19d3a9c5fc738b4c9b3c436f9ba10b16c057523360b3443dcd7570 in / 
# Tue, 04 Aug 2020 05:01:32 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:40:09 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 04 Aug 2020 08:43:09 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 04 Aug 2020 08:44:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 08:44:21 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 04 Aug 2020 08:44:23 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 04 Aug 2020 08:44:23 GMT
EXPOSE 8888
# Tue, 04 Aug 2020 08:44:26 GMT
VOLUME [/var/lib/chronograf]
# Tue, 04 Aug 2020 08:44:29 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 04 Aug 2020 08:44:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Aug 2020 08:44:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b33d4edf196b4a005f13932d074987a85eb6c927dc64b40989598b3ade8ebc5c`  
		Last Modified: Tue, 04 Aug 2020 05:09:01 GMT  
		Size: 19.3 MB (19304611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb933ad4bb85672991fffc11bb98b3d11d98ccd0523793e0699c1eb81ca6817e`  
		Last Modified: Tue, 04 Aug 2020 08:45:40 GMT  
		Size: 3.9 MB (3878320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fa3e46c20d6342a32f4bd3473fe5daf746811c4063cb533a8e86344b016ea5`  
		Last Modified: Tue, 04 Aug 2020 08:46:07 GMT  
		Size: 35.8 MB (35752327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e3f2101a123761af772978b35c286415d31462d0e9d0762c721f241261eb7d`  
		Last Modified: Tue, 04 Aug 2020 08:45:53 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c29ae49c457f8714c437eac4d0befc8c927bd54fd383eb41ff112daa2c5a76`  
		Last Modified: Tue, 04 Aug 2020 08:45:53 GMT  
		Size: 11.9 KB (11911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e397f9f1bd96ce9ac240b8b1ec7c03c20b63c0d0de27a1637d00606ed2052ee6`  
		Last Modified: Tue, 04 Aug 2020 08:45:53 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:01f0aa43a1fb22fc1956c776293772318b916adf9ab04a3398c3dee89cd42564
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60444932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b8890ce936d4c4680bc13ac9cf44755c3831519a8135ee572799c880d1ea92`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 07:00:02 GMT
ADD file:448eac8822629a9f212483d0e6123c797105b2ec368648e6f259b7d4cb83e0a1 in / 
# Tue, 04 Aug 2020 07:00:04 GMT
CMD ["bash"]
# Tue, 01 Sep 2020 23:37:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 01 Sep 2020 23:37:42 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 01 Sep 2020 23:38:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Sep 2020 23:39:01 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 01 Sep 2020 23:39:09 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 01 Sep 2020 23:39:16 GMT
EXPOSE 8888
# Tue, 01 Sep 2020 23:39:31 GMT
VOLUME [/var/lib/chronograf]
# Tue, 01 Sep 2020 23:39:43 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 01 Sep 2020 23:40:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Sep 2020 23:40:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:5984ce78d2759fcb147a7641f941b59e71e8c9f82aa5cb0e3d511c74c876a7e3`  
		Last Modified: Tue, 04 Aug 2020 07:06:31 GMT  
		Size: 20.4 MB (20377078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8165183b47acbd3117b1d889ee5c8a78488c48be0e817a37c480248ef97679`  
		Last Modified: Tue, 01 Sep 2020 23:43:20 GMT  
		Size: 4.1 MB (4082049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d221a550fef5c44757a289be1e85910e33626d64a0a642a3611466d77048648`  
		Last Modified: Tue, 01 Sep 2020 23:43:29 GMT  
		Size: 36.0 MB (35961400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2e886b4d1c9321a1c819921b7ddce621eef3fd89c5a965bee46167484b570a`  
		Last Modified: Tue, 01 Sep 2020 23:43:17 GMT  
		Size: 12.3 KB (12253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b185042a25e2948de7a58dcf548e701b06a9886173d52d3a0b9522c733f94342`  
		Last Modified: Tue, 01 Sep 2020 23:43:17 GMT  
		Size: 11.9 KB (11913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903451520a8c22062b2f9c761751cb62f65753a0f0e85987dd73e354f484a9a9`  
		Last Modified: Tue, 01 Sep 2020 23:43:17 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17-alpine`

```console
$ docker pull chronograf@sha256:13b176957f590361ff83e6e41f4f150fdb1622f70a4d9bd5882c829ecc1c4e32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.7.17-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:3e6f71faadeb2978d22477a83cdaed7817a86dc26dc30585ffcb06fc65aaea53
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22658146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed9c760ca03e2302d49b9a0b101a83650f8bdbdd2ebc4cb2c06dbd3bb7685268`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 23 Jul 2020 05:22:10 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:38:19 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 01 Sep 2020 00:38:36 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 02 Sep 2020 00:09:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 02 Sep 2020 00:09:31 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 02 Sep 2020 00:09:31 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 02 Sep 2020 00:09:32 GMT
EXPOSE 8888
# Wed, 02 Sep 2020 00:09:32 GMT
VOLUME [/var/lib/chronograf]
# Wed, 02 Sep 2020 00:09:32 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 02 Sep 2020 00:09:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Sep 2020 00:09:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ed77ee1a57b06efa2aeb4cc06845d93ce8c6e8b2ca507267000b5a6edddffa`  
		Last Modified: Thu, 23 Jul 2020 05:23:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61626b3b2d7f1da2eb5ae3486f7e2baf21fb5b7dd993595b8fe0fbe2a34445d6`  
		Last Modified: Tue, 01 Sep 2020 00:39:25 GMT  
		Size: 280.8 KB (280831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3f1c77ac4aeaba4f3cd0cd6247ce60f264391306d4306146a64dfa3435e010`  
		Last Modified: Wed, 02 Sep 2020 00:10:43 GMT  
		Size: 19.6 MB (19555244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ad2284c373cd96c1693061cbddd4687c75ecc8dd4f208c25bfde4c7248d476`  
		Last Modified: Wed, 02 Sep 2020 00:10:39 GMT  
		Size: 12.2 KB (12239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec6c863fedc9d7061f93818178098b408576101c98d2c65d7bf935c5b4c79dd`  
		Last Modified: Wed, 02 Sep 2020 00:10:39 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8746e17c29b30757b2f7520eb1d936cbbbcbd55314fc394397d56c41376ef2`  
		Last Modified: Wed, 02 Sep 2020 00:10:39 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:13b176957f590361ff83e6e41f4f150fdb1622f70a4d9bd5882c829ecc1c4e32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.7-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:3e6f71faadeb2978d22477a83cdaed7817a86dc26dc30585ffcb06fc65aaea53
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22658146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed9c760ca03e2302d49b9a0b101a83650f8bdbdd2ebc4cb2c06dbd3bb7685268`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 23 Jul 2020 05:22:10 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:38:19 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 01 Sep 2020 00:38:36 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Wed, 02 Sep 2020 00:09:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 02 Sep 2020 00:09:31 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 02 Sep 2020 00:09:31 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 02 Sep 2020 00:09:32 GMT
EXPOSE 8888
# Wed, 02 Sep 2020 00:09:32 GMT
VOLUME [/var/lib/chronograf]
# Wed, 02 Sep 2020 00:09:32 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 02 Sep 2020 00:09:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Sep 2020 00:09:32 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ed77ee1a57b06efa2aeb4cc06845d93ce8c6e8b2ca507267000b5a6edddffa`  
		Last Modified: Thu, 23 Jul 2020 05:23:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61626b3b2d7f1da2eb5ae3486f7e2baf21fb5b7dd993595b8fe0fbe2a34445d6`  
		Last Modified: Tue, 01 Sep 2020 00:39:25 GMT  
		Size: 280.8 KB (280831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3f1c77ac4aeaba4f3cd0cd6247ce60f264391306d4306146a64dfa3435e010`  
		Last Modified: Wed, 02 Sep 2020 00:10:43 GMT  
		Size: 19.6 MB (19555244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ad2284c373cd96c1693061cbddd4687c75ecc8dd4f208c25bfde4c7248d476`  
		Last Modified: Wed, 02 Sep 2020 00:10:39 GMT  
		Size: 12.2 KB (12239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec6c863fedc9d7061f93818178098b408576101c98d2c65d7bf935c5b4c79dd`  
		Last Modified: Wed, 02 Sep 2020 00:10:39 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8746e17c29b30757b2f7520eb1d936cbbbcbd55314fc394397d56c41376ef2`  
		Last Modified: Wed, 02 Sep 2020 00:10:39 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8`

```console
$ docker pull chronograf@sha256:797e0bbfbe3b8e87ea1162c9f3196629591154f27a7a5c92f8de471b7e4a990a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:b8e62faea6e64c43994a865baf1372bd375e1d8dd118fee575a829415acd69a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70381672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2db75558813ceb5e5cf49e7fe3d835960f8ab9a9cc1e886452ab4eb57971cef3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Wed, 02 Sep 2020 00:08:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 02 Sep 2020 00:09:36 GMT
ENV CHRONOGRAF_VERSION=1.8.6
# Wed, 02 Sep 2020 00:09:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 02 Sep 2020 00:09:44 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 02 Sep 2020 00:09:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 02 Sep 2020 00:09:45 GMT
EXPOSE 8888
# Wed, 02 Sep 2020 00:09:45 GMT
VOLUME [/var/lib/chronograf]
# Wed, 02 Sep 2020 00:09:45 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 02 Sep 2020 00:09:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Sep 2020 00:09:45 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afff3f2fb3db7c061b33082931d5ba904dfd5cc528cc6d7e74e2d5d6821701c`  
		Last Modified: Wed, 02 Sep 2020 00:10:18 GMT  
		Size: 6.7 MB (6742093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1a03324aa2491c3efee74acc5b19036280e4fb0f12098fcad17c61d0371e19`  
		Last Modified: Wed, 02 Sep 2020 00:10:53 GMT  
		Size: 41.1 MB (41092910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8268eb360ba9dc00b977df5f766442acd3e82f69aa175c498caed155497d4a1`  
		Last Modified: Wed, 02 Sep 2020 00:10:46 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9810c23ed3920f02f1df96b8c340a7b13deeafeecddea1ddfd097393f2dab300`  
		Last Modified: Wed, 02 Sep 2020 00:10:46 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0bffc8124103c60bd00387121ba0e2e1a5ef5a80d3669293541484857a7f05`  
		Last Modified: Wed, 02 Sep 2020 00:10:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:c0803f5c98a9b606fea7ea6fa6fb50a2bc93750996bc83ffb304c47f528ad71c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63563753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9f9b03033028bf7afdee09c44e3a2f5ca551e4e125528907c13098da0d98858`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 05:01:30 GMT
ADD file:3d69e3d8fb19d3a9c5fc738b4c9b3c436f9ba10b16c057523360b3443dcd7570 in / 
# Tue, 04 Aug 2020 05:01:32 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:40:09 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 04 Aug 2020 08:44:50 GMT
ENV CHRONOGRAF_VERSION=1.8.4
# Tue, 04 Aug 2020 08:45:15 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 08:45:18 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 04 Aug 2020 08:45:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 04 Aug 2020 08:45:22 GMT
EXPOSE 8888
# Tue, 04 Aug 2020 08:45:22 GMT
VOLUME [/var/lib/chronograf]
# Tue, 04 Aug 2020 08:45:25 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 04 Aug 2020 08:45:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Aug 2020 08:45:28 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b33d4edf196b4a005f13932d074987a85eb6c927dc64b40989598b3ade8ebc5c`  
		Last Modified: Tue, 04 Aug 2020 05:09:01 GMT  
		Size: 19.3 MB (19304611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb933ad4bb85672991fffc11bb98b3d11d98ccd0523793e0699c1eb81ca6817e`  
		Last Modified: Tue, 04 Aug 2020 08:45:40 GMT  
		Size: 3.9 MB (3878320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56d04542cfbbb40ecceb3fb0857d765f0e9907bf4600635efb17582d63075af`  
		Last Modified: Tue, 04 Aug 2020 08:46:24 GMT  
		Size: 40.4 MB (40356413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc095732d5a67cce2400ab2414f1df138953b3f3dced02f04ef888cf7bca469`  
		Last Modified: Tue, 04 Aug 2020 08:46:13 GMT  
		Size: 12.3 KB (12255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd518336b8728bf95dafdf81b66d9663cbea4d2f4c704d43ae4c87a67e08f06`  
		Last Modified: Tue, 04 Aug 2020 08:46:14 GMT  
		Size: 11.9 KB (11915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5247c0d8a61cdbdcb822b8b41db097f237b43fcef962c21317e43f883533ec1d`  
		Last Modified: Tue, 04 Aug 2020 08:46:14 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:66df2a7e1a906b7bb7dbb86a9cbdf578129b51329d55de7a025fef28d30d8f60
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64887595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d9cd086cbb52293ca5bbd913eabbff46cd9b5e5c1e2cca48428cfbfaf6a3bf7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 07:00:02 GMT
ADD file:448eac8822629a9f212483d0e6123c797105b2ec368648e6f259b7d4cb83e0a1 in / 
# Tue, 04 Aug 2020 07:00:04 GMT
CMD ["bash"]
# Tue, 01 Sep 2020 23:34:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 01 Sep 2020 23:40:31 GMT
ENV CHRONOGRAF_VERSION=1.8.6
# Tue, 01 Sep 2020 23:41:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Sep 2020 23:41:36 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 01 Sep 2020 23:41:44 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 01 Sep 2020 23:41:54 GMT
EXPOSE 8888
# Tue, 01 Sep 2020 23:42:11 GMT
VOLUME [/var/lib/chronograf]
# Tue, 01 Sep 2020 23:42:26 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 01 Sep 2020 23:42:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Sep 2020 23:42:44 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:5984ce78d2759fcb147a7641f941b59e71e8c9f82aa5cb0e3d511c74c876a7e3`  
		Last Modified: Tue, 04 Aug 2020 07:06:31 GMT  
		Size: 20.4 MB (20377078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f266d2355710732ee4f239f9bce3a8c3e01e7a804b84421c3727e009a175dfd`  
		Last Modified: Tue, 01 Sep 2020 23:43:01 GMT  
		Size: 6.0 MB (6027754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6a994d6278ab68ad412716e576783a2c7b18d6c4017e16e4ead23a10401ae0`  
		Last Modified: Tue, 01 Sep 2020 23:43:51 GMT  
		Size: 38.5 MB (38458360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e30483204b6cb557fd9376a669f1dd91bb097e036f69bcf8919cc846bcc401f`  
		Last Modified: Tue, 01 Sep 2020 23:43:36 GMT  
		Size: 12.3 KB (12252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d969745c49ffdd93615791699ca3168313b9c274dbc44ea964866d4a43e16254`  
		Last Modified: Tue, 01 Sep 2020 23:43:36 GMT  
		Size: 11.9 KB (11912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93918a697a40dd750255a9320c43f040b7ac08513f1c3c59545c554db1457b5d`  
		Last Modified: Tue, 01 Sep 2020 23:43:36 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.6`

```console
$ docker pull chronograf@sha256:5ad51147a4325444814d798a3e8343acd1d5b66013440b78c90ea0daff2418b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `chronograf:1.8.6` - linux; amd64

```console
$ docker pull chronograf@sha256:b8e62faea6e64c43994a865baf1372bd375e1d8dd118fee575a829415acd69a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70381672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2db75558813ceb5e5cf49e7fe3d835960f8ab9a9cc1e886452ab4eb57971cef3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Wed, 02 Sep 2020 00:08:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 02 Sep 2020 00:09:36 GMT
ENV CHRONOGRAF_VERSION=1.8.6
# Wed, 02 Sep 2020 00:09:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 02 Sep 2020 00:09:44 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 02 Sep 2020 00:09:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 02 Sep 2020 00:09:45 GMT
EXPOSE 8888
# Wed, 02 Sep 2020 00:09:45 GMT
VOLUME [/var/lib/chronograf]
# Wed, 02 Sep 2020 00:09:45 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 02 Sep 2020 00:09:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Sep 2020 00:09:45 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afff3f2fb3db7c061b33082931d5ba904dfd5cc528cc6d7e74e2d5d6821701c`  
		Last Modified: Wed, 02 Sep 2020 00:10:18 GMT  
		Size: 6.7 MB (6742093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1a03324aa2491c3efee74acc5b19036280e4fb0f12098fcad17c61d0371e19`  
		Last Modified: Wed, 02 Sep 2020 00:10:53 GMT  
		Size: 41.1 MB (41092910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8268eb360ba9dc00b977df5f766442acd3e82f69aa175c498caed155497d4a1`  
		Last Modified: Wed, 02 Sep 2020 00:10:46 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9810c23ed3920f02f1df96b8c340a7b13deeafeecddea1ddfd097393f2dab300`  
		Last Modified: Wed, 02 Sep 2020 00:10:46 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0bffc8124103c60bd00387121ba0e2e1a5ef5a80d3669293541484857a7f05`  
		Last Modified: Wed, 02 Sep 2020 00:10:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.6` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:66df2a7e1a906b7bb7dbb86a9cbdf578129b51329d55de7a025fef28d30d8f60
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64887595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d9cd086cbb52293ca5bbd913eabbff46cd9b5e5c1e2cca48428cfbfaf6a3bf7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 07:00:02 GMT
ADD file:448eac8822629a9f212483d0e6123c797105b2ec368648e6f259b7d4cb83e0a1 in / 
# Tue, 04 Aug 2020 07:00:04 GMT
CMD ["bash"]
# Tue, 01 Sep 2020 23:34:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 01 Sep 2020 23:40:31 GMT
ENV CHRONOGRAF_VERSION=1.8.6
# Tue, 01 Sep 2020 23:41:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Sep 2020 23:41:36 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 01 Sep 2020 23:41:44 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 01 Sep 2020 23:41:54 GMT
EXPOSE 8888
# Tue, 01 Sep 2020 23:42:11 GMT
VOLUME [/var/lib/chronograf]
# Tue, 01 Sep 2020 23:42:26 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 01 Sep 2020 23:42:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Sep 2020 23:42:44 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:5984ce78d2759fcb147a7641f941b59e71e8c9f82aa5cb0e3d511c74c876a7e3`  
		Last Modified: Tue, 04 Aug 2020 07:06:31 GMT  
		Size: 20.4 MB (20377078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f266d2355710732ee4f239f9bce3a8c3e01e7a804b84421c3727e009a175dfd`  
		Last Modified: Tue, 01 Sep 2020 23:43:01 GMT  
		Size: 6.0 MB (6027754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6a994d6278ab68ad412716e576783a2c7b18d6c4017e16e4ead23a10401ae0`  
		Last Modified: Tue, 01 Sep 2020 23:43:51 GMT  
		Size: 38.5 MB (38458360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e30483204b6cb557fd9376a669f1dd91bb097e036f69bcf8919cc846bcc401f`  
		Last Modified: Tue, 01 Sep 2020 23:43:36 GMT  
		Size: 12.3 KB (12252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d969745c49ffdd93615791699ca3168313b9c274dbc44ea964866d4a43e16254`  
		Last Modified: Tue, 01 Sep 2020 23:43:36 GMT  
		Size: 11.9 KB (11912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93918a697a40dd750255a9320c43f040b7ac08513f1c3c59545c554db1457b5d`  
		Last Modified: Tue, 01 Sep 2020 23:43:36 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.6-alpine`

```console
$ docker pull chronograf@sha256:fefbf41da79fffccbbd941967d70392237f286fcc2df9d25dfe1fe45a58f8ddd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.8.6-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:a36e09c00ecb799786acea4e24a9c8da48acffa5d1f2fe86cfb1fb3aca5957c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25328335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c69feb5a82eacbc8d79467c5fc42fbbcb371a45a6fe2e9aafb3ba83725a0c3a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 23 Jul 2020 05:22:10 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:38:19 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 02 Sep 2020 00:09:51 GMT
ENV CHRONOGRAF_VERSION=1.8.6
# Wed, 02 Sep 2020 00:09:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 02 Sep 2020 00:09:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 02 Sep 2020 00:09:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 02 Sep 2020 00:09:55 GMT
EXPOSE 8888
# Wed, 02 Sep 2020 00:09:55 GMT
VOLUME [/var/lib/chronograf]
# Wed, 02 Sep 2020 00:09:55 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 02 Sep 2020 00:09:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Sep 2020 00:09:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ed77ee1a57b06efa2aeb4cc06845d93ce8c6e8b2ca507267000b5a6edddffa`  
		Last Modified: Thu, 23 Jul 2020 05:23:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61626b3b2d7f1da2eb5ae3486f7e2baf21fb5b7dd993595b8fe0fbe2a34445d6`  
		Last Modified: Tue, 01 Sep 2020 00:39:25 GMT  
		Size: 280.8 KB (280831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fea9bed343691db1570957996270f11b2b1d48eed66a868fb0755d9a2dd8f13`  
		Last Modified: Wed, 02 Sep 2020 00:11:01 GMT  
		Size: 22.2 MB (22225432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bd8075e11a081612e1f6d23566ea70bfe0dd2e08282b0f2c56f78b097f5088`  
		Last Modified: Wed, 02 Sep 2020 00:10:56 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8be9caf4702126c2554fa964ab06fa06c7f79e512634005342f8b68c5983c4`  
		Last Modified: Wed, 02 Sep 2020 00:10:56 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cfaf5406f7e90425cac0c325e66d5025d7cb98163d77a400f806c40f07335f5`  
		Last Modified: Wed, 02 Sep 2020 00:10:56 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8-alpine`

```console
$ docker pull chronograf@sha256:fefbf41da79fffccbbd941967d70392237f286fcc2df9d25dfe1fe45a58f8ddd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:a36e09c00ecb799786acea4e24a9c8da48acffa5d1f2fe86cfb1fb3aca5957c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25328335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c69feb5a82eacbc8d79467c5fc42fbbcb371a45a6fe2e9aafb3ba83725a0c3a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 23 Jul 2020 05:22:10 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:38:19 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 02 Sep 2020 00:09:51 GMT
ENV CHRONOGRAF_VERSION=1.8.6
# Wed, 02 Sep 2020 00:09:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 02 Sep 2020 00:09:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 02 Sep 2020 00:09:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 02 Sep 2020 00:09:55 GMT
EXPOSE 8888
# Wed, 02 Sep 2020 00:09:55 GMT
VOLUME [/var/lib/chronograf]
# Wed, 02 Sep 2020 00:09:55 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 02 Sep 2020 00:09:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Sep 2020 00:09:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ed77ee1a57b06efa2aeb4cc06845d93ce8c6e8b2ca507267000b5a6edddffa`  
		Last Modified: Thu, 23 Jul 2020 05:23:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61626b3b2d7f1da2eb5ae3486f7e2baf21fb5b7dd993595b8fe0fbe2a34445d6`  
		Last Modified: Tue, 01 Sep 2020 00:39:25 GMT  
		Size: 280.8 KB (280831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fea9bed343691db1570957996270f11b2b1d48eed66a868fb0755d9a2dd8f13`  
		Last Modified: Wed, 02 Sep 2020 00:11:01 GMT  
		Size: 22.2 MB (22225432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bd8075e11a081612e1f6d23566ea70bfe0dd2e08282b0f2c56f78b097f5088`  
		Last Modified: Wed, 02 Sep 2020 00:10:56 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8be9caf4702126c2554fa964ab06fa06c7f79e512634005342f8b68c5983c4`  
		Last Modified: Wed, 02 Sep 2020 00:10:56 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cfaf5406f7e90425cac0c325e66d5025d7cb98163d77a400f806c40f07335f5`  
		Last Modified: Wed, 02 Sep 2020 00:10:56 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:fefbf41da79fffccbbd941967d70392237f286fcc2df9d25dfe1fe45a58f8ddd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:a36e09c00ecb799786acea4e24a9c8da48acffa5d1f2fe86cfb1fb3aca5957c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25328335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c69feb5a82eacbc8d79467c5fc42fbbcb371a45a6fe2e9aafb3ba83725a0c3a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 23 Jul 2020 05:22:10 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:38:19 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 02 Sep 2020 00:09:51 GMT
ENV CHRONOGRAF_VERSION=1.8.6
# Wed, 02 Sep 2020 00:09:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 02 Sep 2020 00:09:55 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 02 Sep 2020 00:09:55 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 02 Sep 2020 00:09:55 GMT
EXPOSE 8888
# Wed, 02 Sep 2020 00:09:55 GMT
VOLUME [/var/lib/chronograf]
# Wed, 02 Sep 2020 00:09:55 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Wed, 02 Sep 2020 00:09:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Sep 2020 00:09:56 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ed77ee1a57b06efa2aeb4cc06845d93ce8c6e8b2ca507267000b5a6edddffa`  
		Last Modified: Thu, 23 Jul 2020 05:23:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61626b3b2d7f1da2eb5ae3486f7e2baf21fb5b7dd993595b8fe0fbe2a34445d6`  
		Last Modified: Tue, 01 Sep 2020 00:39:25 GMT  
		Size: 280.8 KB (280831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fea9bed343691db1570957996270f11b2b1d48eed66a868fb0755d9a2dd8f13`  
		Last Modified: Wed, 02 Sep 2020 00:11:01 GMT  
		Size: 22.2 MB (22225432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bd8075e11a081612e1f6d23566ea70bfe0dd2e08282b0f2c56f78b097f5088`  
		Last Modified: Wed, 02 Sep 2020 00:10:56 GMT  
		Size: 12.2 KB (12240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8be9caf4702126c2554fa964ab06fa06c7f79e512634005342f8b68c5983c4`  
		Last Modified: Wed, 02 Sep 2020 00:10:56 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cfaf5406f7e90425cac0c325e66d5025d7cb98163d77a400f806c40f07335f5`  
		Last Modified: Wed, 02 Sep 2020 00:10:56 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:latest`

```console
$ docker pull chronograf@sha256:797e0bbfbe3b8e87ea1162c9f3196629591154f27a7a5c92f8de471b7e4a990a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:b8e62faea6e64c43994a865baf1372bd375e1d8dd118fee575a829415acd69a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70381672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2db75558813ceb5e5cf49e7fe3d835960f8ab9a9cc1e886452ab4eb57971cef3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Wed, 02 Sep 2020 00:08:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 02 Sep 2020 00:09:36 GMT
ENV CHRONOGRAF_VERSION=1.8.6
# Wed, 02 Sep 2020 00:09:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Wed, 02 Sep 2020 00:09:44 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Wed, 02 Sep 2020 00:09:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Wed, 02 Sep 2020 00:09:45 GMT
EXPOSE 8888
# Wed, 02 Sep 2020 00:09:45 GMT
VOLUME [/var/lib/chronograf]
# Wed, 02 Sep 2020 00:09:45 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Wed, 02 Sep 2020 00:09:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Sep 2020 00:09:45 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afff3f2fb3db7c061b33082931d5ba904dfd5cc528cc6d7e74e2d5d6821701c`  
		Last Modified: Wed, 02 Sep 2020 00:10:18 GMT  
		Size: 6.7 MB (6742093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1a03324aa2491c3efee74acc5b19036280e4fb0f12098fcad17c61d0371e19`  
		Last Modified: Wed, 02 Sep 2020 00:10:53 GMT  
		Size: 41.1 MB (41092910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8268eb360ba9dc00b977df5f766442acd3e82f69aa175c498caed155497d4a1`  
		Last Modified: Wed, 02 Sep 2020 00:10:46 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9810c23ed3920f02f1df96b8c340a7b13deeafeecddea1ddfd097393f2dab300`  
		Last Modified: Wed, 02 Sep 2020 00:10:46 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0bffc8124103c60bd00387121ba0e2e1a5ef5a80d3669293541484857a7f05`  
		Last Modified: Wed, 02 Sep 2020 00:10:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:c0803f5c98a9b606fea7ea6fa6fb50a2bc93750996bc83ffb304c47f528ad71c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63563753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9f9b03033028bf7afdee09c44e3a2f5ca551e4e125528907c13098da0d98858`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 05:01:30 GMT
ADD file:3d69e3d8fb19d3a9c5fc738b4c9b3c436f9ba10b16c057523360b3443dcd7570 in / 
# Tue, 04 Aug 2020 05:01:32 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:40:09 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 04 Aug 2020 08:44:50 GMT
ENV CHRONOGRAF_VERSION=1.8.4
# Tue, 04 Aug 2020 08:45:15 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 08:45:18 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 04 Aug 2020 08:45:19 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 04 Aug 2020 08:45:22 GMT
EXPOSE 8888
# Tue, 04 Aug 2020 08:45:22 GMT
VOLUME [/var/lib/chronograf]
# Tue, 04 Aug 2020 08:45:25 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 04 Aug 2020 08:45:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Aug 2020 08:45:28 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:b33d4edf196b4a005f13932d074987a85eb6c927dc64b40989598b3ade8ebc5c`  
		Last Modified: Tue, 04 Aug 2020 05:09:01 GMT  
		Size: 19.3 MB (19304611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb933ad4bb85672991fffc11bb98b3d11d98ccd0523793e0699c1eb81ca6817e`  
		Last Modified: Tue, 04 Aug 2020 08:45:40 GMT  
		Size: 3.9 MB (3878320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56d04542cfbbb40ecceb3fb0857d765f0e9907bf4600635efb17582d63075af`  
		Last Modified: Tue, 04 Aug 2020 08:46:24 GMT  
		Size: 40.4 MB (40356413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc095732d5a67cce2400ab2414f1df138953b3f3dced02f04ef888cf7bca469`  
		Last Modified: Tue, 04 Aug 2020 08:46:13 GMT  
		Size: 12.3 KB (12255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd518336b8728bf95dafdf81b66d9663cbea4d2f4c704d43ae4c87a67e08f06`  
		Last Modified: Tue, 04 Aug 2020 08:46:14 GMT  
		Size: 11.9 KB (11915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5247c0d8a61cdbdcb822b8b41db097f237b43fcef962c21317e43f883533ec1d`  
		Last Modified: Tue, 04 Aug 2020 08:46:14 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:66df2a7e1a906b7bb7dbb86a9cbdf578129b51329d55de7a025fef28d30d8f60
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64887595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d9cd086cbb52293ca5bbd913eabbff46cd9b5e5c1e2cca48428cfbfaf6a3bf7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 04 Aug 2020 07:00:02 GMT
ADD file:448eac8822629a9f212483d0e6123c797105b2ec368648e6f259b7d4cb83e0a1 in / 
# Tue, 04 Aug 2020 07:00:04 GMT
CMD ["bash"]
# Tue, 01 Sep 2020 23:34:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 01 Sep 2020 23:40:31 GMT
ENV CHRONOGRAF_VERSION=1.8.6
# Tue, 01 Sep 2020 23:41:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Sep 2020 23:41:36 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 01 Sep 2020 23:41:44 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 01 Sep 2020 23:41:54 GMT
EXPOSE 8888
# Tue, 01 Sep 2020 23:42:11 GMT
VOLUME [/var/lib/chronograf]
# Tue, 01 Sep 2020 23:42:26 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 01 Sep 2020 23:42:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Sep 2020 23:42:44 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:5984ce78d2759fcb147a7641f941b59e71e8c9f82aa5cb0e3d511c74c876a7e3`  
		Last Modified: Tue, 04 Aug 2020 07:06:31 GMT  
		Size: 20.4 MB (20377078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f266d2355710732ee4f239f9bce3a8c3e01e7a804b84421c3727e009a175dfd`  
		Last Modified: Tue, 01 Sep 2020 23:43:01 GMT  
		Size: 6.0 MB (6027754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6a994d6278ab68ad412716e576783a2c7b18d6c4017e16e4ead23a10401ae0`  
		Last Modified: Tue, 01 Sep 2020 23:43:51 GMT  
		Size: 38.5 MB (38458360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e30483204b6cb557fd9376a669f1dd91bb097e036f69bcf8919cc846bcc401f`  
		Last Modified: Tue, 01 Sep 2020 23:43:36 GMT  
		Size: 12.3 KB (12252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d969745c49ffdd93615791699ca3168313b9c274dbc44ea964866d4a43e16254`  
		Last Modified: Tue, 01 Sep 2020 23:43:36 GMT  
		Size: 11.9 KB (11912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93918a697a40dd750255a9320c43f040b7ac08513f1c3c59545c554db1457b5d`  
		Last Modified: Tue, 01 Sep 2020 23:43:36 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
