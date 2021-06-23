<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `influxdb`

-	[`influxdb:1.7`](#influxdb17)
-	[`influxdb:1.7-alpine`](#influxdb17-alpine)
-	[`influxdb:1.7-data`](#influxdb17-data)
-	[`influxdb:1.7-data-alpine`](#influxdb17-data-alpine)
-	[`influxdb:1.7-meta`](#influxdb17-meta)
-	[`influxdb:1.7-meta-alpine`](#influxdb17-meta-alpine)
-	[`influxdb:1.7.11`](#influxdb1711)
-	[`influxdb:1.7.11-alpine`](#influxdb1711-alpine)
-	[`influxdb:1.7.11-data`](#influxdb1711-data)
-	[`influxdb:1.7.11-data-alpine`](#influxdb1711-data-alpine)
-	[`influxdb:1.7.11-meta`](#influxdb1711-meta)
-	[`influxdb:1.7.11-meta-alpine`](#influxdb1711-meta-alpine)
-	[`influxdb:1.8`](#influxdb18)
-	[`influxdb:1.8-alpine`](#influxdb18-alpine)
-	[`influxdb:1.8-data`](#influxdb18-data)
-	[`influxdb:1.8-data-alpine`](#influxdb18-data-alpine)
-	[`influxdb:1.8-meta`](#influxdb18-meta)
-	[`influxdb:1.8-meta-alpine`](#influxdb18-meta-alpine)
-	[`influxdb:1.8.6`](#influxdb186)
-	[`influxdb:1.8.6-alpine`](#influxdb186-alpine)
-	[`influxdb:1.8.6-data`](#influxdb186-data)
-	[`influxdb:1.8.6-data-alpine`](#influxdb186-data-alpine)
-	[`influxdb:1.8.6-meta`](#influxdb186-meta)
-	[`influxdb:1.8.6-meta-alpine`](#influxdb186-meta-alpine)
-	[`influxdb:2.0`](#influxdb20)
-	[`influxdb:2.0-alpine`](#influxdb20-alpine)
-	[`influxdb:2.0.7`](#influxdb207)
-	[`influxdb:2.0.7-alpine`](#influxdb207-alpine)
-	[`influxdb:alpine`](#influxdbalpine)
-	[`influxdb:data`](#influxdbdata)
-	[`influxdb:data-alpine`](#influxdbdata-alpine)
-	[`influxdb:latest`](#influxdblatest)
-	[`influxdb:meta`](#influxdbmeta)
-	[`influxdb:meta-alpine`](#influxdbmeta-alpine)

## `influxdb:1.7`

```console
$ docker pull influxdb@sha256:b713f3175feb357bcab18ab3b4089f4d9e96c26ac96ef9f2010406de9ad3e628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7` - linux; amd64

```console
$ docker pull influxdb@sha256:14eb86bd7d5d9f4890eb28c4cc3b395c945ff6cdf8c33cf7d1dfb4e7060fa937
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122298666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2e1d3cdfb6ae42962cb933af30ac9d9bcc3ca1b67db2b3051a06c42e570f58a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:08:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 12 May 2021 20:08:58 GMT
ENV INFLUXDB_VERSION=1.7.11
# Wed, 12 May 2021 20:09:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 12 May 2021 20:09:04 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 12 May 2021 20:09:04 GMT
EXPOSE 8086
# Wed, 12 May 2021 20:09:04 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 May 2021 20:09:05 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 12 May 2021 20:09:05 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 12 May 2021 20:09:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 May 2021 20:09:06 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee65a07cb0cad7eedb6332aad83a593a46bbae0a453842817353e2cf9de28d`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa4069a83eb75714a88ef9978f1d9ea2340c13aeac69f95b2f531edcdbaa632`  
		Last Modified: Wed, 12 May 2021 20:11:23 GMT  
		Size: 61.3 MB (61285145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf0a1eba4744e1f82addad1553c1200421399d1b21ed9352a453dbfaf514ec1`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f4b54006e4b61473ed83cba4a79f5402a04aab12a0da20b78f9c653890503c`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7c01d64fbcae13e8b7ca53d9a11ae623f77e0adabf4da23fc9773c32899da8`  
		Last Modified: Wed, 12 May 2021 20:11:15 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:2d41a4f4a6c7b5f80848ac0bae2f9f039a5b6e746cc405401a83bf237f87231b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113465787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a6b234d298dfa36fc3a43d328e4f7e45cc067db11e5e6e1702e8d141dafbd24`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 May 2021 01:11:51 GMT
ADD file:81cfd4e746bdfcc19847240b77012487652be22dbd5741ccb2485a4207f2b73f in / 
# Wed, 12 May 2021 01:11:56 GMT
CMD ["bash"]
# Thu, 27 May 2021 00:45:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:45:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 15:25:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 27 May 2021 15:25:54 GMT
ENV INFLUXDB_VERSION=1.7.11
# Thu, 27 May 2021 15:26:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 27 May 2021 15:26:02 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 27 May 2021 15:26:02 GMT
EXPOSE 8086
# Thu, 27 May 2021 15:26:02 GMT
VOLUME [/var/lib/influxdb]
# Thu, 27 May 2021 15:26:02 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 27 May 2021 15:26:02 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 27 May 2021 15:26:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 May 2021 15:26:03 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:55b9a6b6b2552c5b2eac0a316e75a7bc18092819ee25c4f1d4d54700bcc1d3dc`  
		Last Modified: Wed, 12 May 2021 01:21:23 GMT  
		Size: 42.1 MB (42120307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba756a0ca8996787a145d62543ecf7cec523a638705be132f442d2013655149`  
		Last Modified: Thu, 27 May 2021 01:06:39 GMT  
		Size: 10.0 MB (9950803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61945aef6a8fee06fbe4dccead7cbad9da46ba174cee1eae1f813541ddb76b3`  
		Last Modified: Thu, 27 May 2021 01:06:38 GMT  
		Size: 3.9 MB (3921169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c677858c56844f5e94ad0349f4825fe826cbc6411776e4daf3ae7979e3ac45e`  
		Last Modified: Thu, 27 May 2021 15:26:40 GMT  
		Size: 2.9 KB (2851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a056d7c571efc6ffbd86f19bbae518ad117757ccb129174ace440fe8bafb4e6d`  
		Last Modified: Thu, 27 May 2021 15:26:50 GMT  
		Size: 57.5 MB (57468938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64eeedfce547a9cfad4d8fa7b0c55661d44a9627bcefc9baccf14385ed02d917`  
		Last Modified: Thu, 27 May 2021 15:26:40 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733282179c72da3557adeceb9426208fd7cf1916c9b3a5fc6d625c15b725b24c`  
		Last Modified: Thu, 27 May 2021 15:26:40 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2ebe7165580376dc2b77a3705fa668355a28c24c1f157d2d687f2b190e3072`  
		Last Modified: Thu, 27 May 2021 15:26:40 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:60e5937b13eb09466c3cc056f116ac89360c3e6b7532a077b2ef058568f5e994
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114697419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a93ba49ed4bb920119d6ce9cb682c489b5c8a7590ac8438e8f1bd8db11c7f80a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:55 GMT
ADD file:02285d0bd3ea996a7ebbe069a83e508701cbaf14f53fdeaa123775acd7e0537f in / 
# Tue, 22 Jun 2021 23:50:56 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:27:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:27:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 18:33:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 18:33:55 GMT
ENV INFLUXDB_VERSION=1.7.11
# Wed, 23 Jun 2021 18:33:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 23 Jun 2021 18:33:59 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 23 Jun 2021 18:33:59 GMT
EXPOSE 8086
# Wed, 23 Jun 2021 18:33:59 GMT
VOLUME [/var/lib/influxdb]
# Wed, 23 Jun 2021 18:33:59 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 23 Jun 2021 18:34:00 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 23 Jun 2021 18:34:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 18:34:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:0789e4a342a11c7c57a241829a41af53fbd194e6dede60c6d6f63d69e403b2cd`  
		Last Modified: Tue, 22 Jun 2021 23:57:52 GMT  
		Size: 43.2 MB (43177421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd2ed69368e8a7d296f1c91060e897753bed4a79ab68ed47c544e1f4d6fadcd`  
		Last Modified: Wed, 23 Jun 2021 00:35:58 GMT  
		Size: 10.2 MB (10214577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c76e514669ff971481e0d19dc0581f90d72eab2d0e117a5761ae016e14f213`  
		Last Modified: Wed, 23 Jun 2021 00:35:57 GMT  
		Size: 4.1 MB (4096534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6d3ae4d939261675d1e9409c3de9369a4e1d761bea9c9887f546c7086b325a`  
		Last Modified: Wed, 23 Jun 2021 18:35:06 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458964da7195c9931ac4ba4f2723f366390a4dc15162d47ab1ada4bad7cddc5d`  
		Last Modified: Wed, 23 Jun 2021 18:35:15 GMT  
		Size: 57.2 MB (57204318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec990cbc0dfc174ac62d30d4758ffd1f1ab3525f3af530480c564a04f02d486f`  
		Last Modified: Wed, 23 Jun 2021 18:35:06 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fc38215dcf9f65878829ccf1f551d3e1b7cb3395a4875b481775906c8ae8d2`  
		Last Modified: Wed, 23 Jun 2021 18:35:06 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ffcef61e67c9131cd095af6a81a8449604612a2e25ed979a2f1de6d7929fb1`  
		Last Modified: Wed, 23 Jun 2021 18:35:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-alpine`

```console
$ docker pull influxdb@sha256:019ffe9b1959d8a9a96ecb4d508e22024a0747008029265179be02b19b9c907d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:497cc2e6dd209b9cded65e0189ff389060f2786e7f2f1666889026a8beb0135d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65268062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88a2f90d367a1c53920888d296e840fd0924b4b2f020ed4afd70ebab0fd4084d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 22:56:19 GMT
ENV INFLUXDB_VERSION=1.7.11
# Wed, 14 Apr 2021 22:56:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:56:26 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 14 Apr 2021 22:56:26 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 22:56:26 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:56:26 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:56:26 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 14 Apr 2021 22:56:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:56:27 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffdfcbb00141ab55c6d38419b5322b874030c5aa73d693a598a2b28ce0e17081`  
		Last Modified: Wed, 14 Apr 2021 22:58:49 GMT  
		Size: 61.0 MB (61034818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19c2e634090909c8b92a0bc6963538e530570f798f2d9fed2be84648f6e66df`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512843e4c495158d090efbaa5625e4123a8aa5978df645e3a86e941f2c478a8`  
		Last Modified: Wed, 14 Apr 2021 22:58:44 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd288200021e8c620e82728a414657c33d78a2bd6f17adc456286e2c471c362`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data`

```console
$ docker pull influxdb@sha256:ed4bf75fda93d81d7212d2e5cb01fbd3549702d8f3c419a7958b44e85caa527c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-data` - linux; amd64

```console
$ docker pull influxdb@sha256:ddc6a1a374a233abf7192332b1b2dd58316658c4ba7cfca70d3ed39e85c4df9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (148962634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9eb629700047ef21ecf4ff1168db10c62a1a71151bb083ab37bdce2627ca73a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:08:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 12 May 2021 20:09:11 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Wed, 12 May 2021 20:09:19 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 12 May 2021 20:09:19 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 12 May 2021 20:09:20 GMT
EXPOSE 8086
# Wed, 12 May 2021 20:09:20 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 May 2021 20:09:20 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 12 May 2021 20:09:20 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 12 May 2021 20:09:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 May 2021 20:09:21 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee65a07cb0cad7eedb6332aad83a593a46bbae0a453842817353e2cf9de28d`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec20ebb0df2d0261a928fa2e775f7e47b1fbf489bd6e557e6e89b72d11e522eb`  
		Last Modified: Wed, 12 May 2021 20:11:49 GMT  
		Size: 87.9 MB (87949059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0820a4489a6108980883726bf6d7e5196dd9b42698603b5dd201c21efa87fe`  
		Last Modified: Wed, 12 May 2021 20:11:36 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b387507a918f61ed59e065e7321b85974b3e222cff40a36d0a036ad877a30c`  
		Last Modified: Wed, 12 May 2021 20:11:36 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df972cc3357c2211116b5b5bc0c66f2f9f4c4ba8a2ca41d1557eb1d2d602aac3`  
		Last Modified: Wed, 12 May 2021 20:11:36 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data-alpine`

```console
$ docker pull influxdb@sha256:953218e27826969473de77140a6e8e36635bc9598fb53e87520da576a4714697
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:59f66a260ca6ac25da45231834f1ba1f5cbd13db57112b39a1eaf3d89418eb1e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91872207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6de1bd45ba333a7fa2b42d112e649986e5df7ccfb6e5d61b4708ed0c96a95770`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 22:56:32 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Wed, 14 Apr 2021 22:56:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:56:42 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 14 Apr 2021 22:56:42 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 22:56:43 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:56:43 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:56:43 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 14 Apr 2021 22:56:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:56:43 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d72c8962115b8fbd20d5a78dd48e575abcd35f896096c95e0b579a8dbd4336`  
		Last Modified: Wed, 14 Apr 2021 22:59:12 GMT  
		Size: 87.6 MB (87638906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0493fd864febd60f65cd5502bd7fcba1d872989c033068c72632717ea9b5137c`  
		Last Modified: Wed, 14 Apr 2021 22:59:01 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd7b30f761adf01ac672b68e8634efcdbcaed5cadd4e8fd9b997c0537ec7a65`  
		Last Modified: Wed, 14 Apr 2021 22:59:00 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd0880938167776dea94134027e0bc04f2f881b2fab628ec37a41a325af8ed0`  
		Last Modified: Wed, 14 Apr 2021 22:59:01 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta`

```console
$ docker pull influxdb@sha256:290bdfe1d6a3e9dcdcde563dd29a68863dedbf6df0ae1c6746e8b3d6c43b82fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:86bc517da71c544988faa8626a800ee73e3d022f05a1764e2c502f6f096b32b7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.1 MB (84146008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:237cfc98f85a91551a3eb5ebe09f3055a08a63fde758d935adbe1e3ddcf06a47`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:08:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 12 May 2021 20:09:11 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Wed, 12 May 2021 20:09:30 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 12 May 2021 20:09:31 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 12 May 2021 20:09:31 GMT
EXPOSE 8091
# Wed, 12 May 2021 20:09:31 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 May 2021 20:09:31 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 12 May 2021 20:09:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 May 2021 20:09:32 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee65a07cb0cad7eedb6332aad83a593a46bbae0a453842817353e2cf9de28d`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570d53070a17d2b30fa2e02a53a1d95e5467c6ccd4140714d34094e8854b9856`  
		Last Modified: Wed, 12 May 2021 20:12:04 GMT  
		Size: 23.1 MB (23133637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d7691e645821a46af60cf56f867e46b6b2d2a4769589676aa8b77b5e161ff5`  
		Last Modified: Wed, 12 May 2021 20:12:00 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150b35b4a9758cb5fa65d465b0de0bfe033c96efc0a8ca6f526dfbad28a57e9c`  
		Last Modified: Wed, 12 May 2021 20:12:00 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta-alpine`

```console
$ docker pull influxdb@sha256:f997194721a978be18e2db6310fc4f20d4e8ae1a13158de1cd7dc6b042ebe98b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:88915c86ce7afd69b101ba5a4dd8d1dfce23bfa760dd74fbb8fec36b562a3909
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27235086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0485099136dd77a780e637f002a9399df5468f2609d126e85c977208798adaac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 22:56:32 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Wed, 14 Apr 2021 22:56:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:56:55 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 14 Apr 2021 22:56:55 GMT
EXPOSE 8091
# Wed, 14 Apr 2021 22:56:55 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:56:55 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:56:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:56:56 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8177497e45bcdf4f69a9c9e31aa09286c8157b7e3918ca418f2a8792b98791`  
		Last Modified: Wed, 14 Apr 2021 22:59:27 GMT  
		Size: 23.0 MB (23002988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ea6921490482ed769782ef5ab560e586b844b845bd40314224130d55910a45`  
		Last Modified: Wed, 14 Apr 2021 22:59:24 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bb5766ed91f5ba3565a638433f21786c10951ed30c32133153d1e11a7826c0`  
		Last Modified: Wed, 14 Apr 2021 22:59:28 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11`

```console
$ docker pull influxdb@sha256:b713f3175feb357bcab18ab3b4089f4d9e96c26ac96ef9f2010406de9ad3e628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7.11` - linux; amd64

```console
$ docker pull influxdb@sha256:14eb86bd7d5d9f4890eb28c4cc3b395c945ff6cdf8c33cf7d1dfb4e7060fa937
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122298666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2e1d3cdfb6ae42962cb933af30ac9d9bcc3ca1b67db2b3051a06c42e570f58a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:08:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 12 May 2021 20:08:58 GMT
ENV INFLUXDB_VERSION=1.7.11
# Wed, 12 May 2021 20:09:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 12 May 2021 20:09:04 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 12 May 2021 20:09:04 GMT
EXPOSE 8086
# Wed, 12 May 2021 20:09:04 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 May 2021 20:09:05 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 12 May 2021 20:09:05 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 12 May 2021 20:09:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 May 2021 20:09:06 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee65a07cb0cad7eedb6332aad83a593a46bbae0a453842817353e2cf9de28d`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa4069a83eb75714a88ef9978f1d9ea2340c13aeac69f95b2f531edcdbaa632`  
		Last Modified: Wed, 12 May 2021 20:11:23 GMT  
		Size: 61.3 MB (61285145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf0a1eba4744e1f82addad1553c1200421399d1b21ed9352a453dbfaf514ec1`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f4b54006e4b61473ed83cba4a79f5402a04aab12a0da20b78f9c653890503c`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7c01d64fbcae13e8b7ca53d9a11ae623f77e0adabf4da23fc9773c32899da8`  
		Last Modified: Wed, 12 May 2021 20:11:15 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.11` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:2d41a4f4a6c7b5f80848ac0bae2f9f039a5b6e746cc405401a83bf237f87231b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113465787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a6b234d298dfa36fc3a43d328e4f7e45cc067db11e5e6e1702e8d141dafbd24`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 May 2021 01:11:51 GMT
ADD file:81cfd4e746bdfcc19847240b77012487652be22dbd5741ccb2485a4207f2b73f in / 
# Wed, 12 May 2021 01:11:56 GMT
CMD ["bash"]
# Thu, 27 May 2021 00:45:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:45:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 15:25:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 27 May 2021 15:25:54 GMT
ENV INFLUXDB_VERSION=1.7.11
# Thu, 27 May 2021 15:26:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 27 May 2021 15:26:02 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 27 May 2021 15:26:02 GMT
EXPOSE 8086
# Thu, 27 May 2021 15:26:02 GMT
VOLUME [/var/lib/influxdb]
# Thu, 27 May 2021 15:26:02 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 27 May 2021 15:26:02 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 27 May 2021 15:26:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 May 2021 15:26:03 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:55b9a6b6b2552c5b2eac0a316e75a7bc18092819ee25c4f1d4d54700bcc1d3dc`  
		Last Modified: Wed, 12 May 2021 01:21:23 GMT  
		Size: 42.1 MB (42120307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba756a0ca8996787a145d62543ecf7cec523a638705be132f442d2013655149`  
		Last Modified: Thu, 27 May 2021 01:06:39 GMT  
		Size: 10.0 MB (9950803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61945aef6a8fee06fbe4dccead7cbad9da46ba174cee1eae1f813541ddb76b3`  
		Last Modified: Thu, 27 May 2021 01:06:38 GMT  
		Size: 3.9 MB (3921169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c677858c56844f5e94ad0349f4825fe826cbc6411776e4daf3ae7979e3ac45e`  
		Last Modified: Thu, 27 May 2021 15:26:40 GMT  
		Size: 2.9 KB (2851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a056d7c571efc6ffbd86f19bbae518ad117757ccb129174ace440fe8bafb4e6d`  
		Last Modified: Thu, 27 May 2021 15:26:50 GMT  
		Size: 57.5 MB (57468938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64eeedfce547a9cfad4d8fa7b0c55661d44a9627bcefc9baccf14385ed02d917`  
		Last Modified: Thu, 27 May 2021 15:26:40 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733282179c72da3557adeceb9426208fd7cf1916c9b3a5fc6d625c15b725b24c`  
		Last Modified: Thu, 27 May 2021 15:26:40 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2ebe7165580376dc2b77a3705fa668355a28c24c1f157d2d687f2b190e3072`  
		Last Modified: Thu, 27 May 2021 15:26:40 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.11` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:60e5937b13eb09466c3cc056f116ac89360c3e6b7532a077b2ef058568f5e994
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114697419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a93ba49ed4bb920119d6ce9cb682c489b5c8a7590ac8438e8f1bd8db11c7f80a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:55 GMT
ADD file:02285d0bd3ea996a7ebbe069a83e508701cbaf14f53fdeaa123775acd7e0537f in / 
# Tue, 22 Jun 2021 23:50:56 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:27:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:27:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 18:33:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 18:33:55 GMT
ENV INFLUXDB_VERSION=1.7.11
# Wed, 23 Jun 2021 18:33:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 23 Jun 2021 18:33:59 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 23 Jun 2021 18:33:59 GMT
EXPOSE 8086
# Wed, 23 Jun 2021 18:33:59 GMT
VOLUME [/var/lib/influxdb]
# Wed, 23 Jun 2021 18:33:59 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 23 Jun 2021 18:34:00 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 23 Jun 2021 18:34:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 18:34:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:0789e4a342a11c7c57a241829a41af53fbd194e6dede60c6d6f63d69e403b2cd`  
		Last Modified: Tue, 22 Jun 2021 23:57:52 GMT  
		Size: 43.2 MB (43177421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd2ed69368e8a7d296f1c91060e897753bed4a79ab68ed47c544e1f4d6fadcd`  
		Last Modified: Wed, 23 Jun 2021 00:35:58 GMT  
		Size: 10.2 MB (10214577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c76e514669ff971481e0d19dc0581f90d72eab2d0e117a5761ae016e14f213`  
		Last Modified: Wed, 23 Jun 2021 00:35:57 GMT  
		Size: 4.1 MB (4096534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6d3ae4d939261675d1e9409c3de9369a4e1d761bea9c9887f546c7086b325a`  
		Last Modified: Wed, 23 Jun 2021 18:35:06 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458964da7195c9931ac4ba4f2723f366390a4dc15162d47ab1ada4bad7cddc5d`  
		Last Modified: Wed, 23 Jun 2021 18:35:15 GMT  
		Size: 57.2 MB (57204318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec990cbc0dfc174ac62d30d4758ffd1f1ab3525f3af530480c564a04f02d486f`  
		Last Modified: Wed, 23 Jun 2021 18:35:06 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fc38215dcf9f65878829ccf1f551d3e1b7cb3395a4875b481775906c8ae8d2`  
		Last Modified: Wed, 23 Jun 2021 18:35:06 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ffcef61e67c9131cd095af6a81a8449604612a2e25ed979a2f1de6d7929fb1`  
		Last Modified: Wed, 23 Jun 2021 18:35:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-alpine`

```console
$ docker pull influxdb@sha256:019ffe9b1959d8a9a96ecb4d508e22024a0747008029265179be02b19b9c907d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.11-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:497cc2e6dd209b9cded65e0189ff389060f2786e7f2f1666889026a8beb0135d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65268062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88a2f90d367a1c53920888d296e840fd0924b4b2f020ed4afd70ebab0fd4084d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 22:56:19 GMT
ENV INFLUXDB_VERSION=1.7.11
# Wed, 14 Apr 2021 22:56:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:56:26 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 14 Apr 2021 22:56:26 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 22:56:26 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:56:26 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:56:26 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 14 Apr 2021 22:56:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:56:27 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffdfcbb00141ab55c6d38419b5322b874030c5aa73d693a598a2b28ce0e17081`  
		Last Modified: Wed, 14 Apr 2021 22:58:49 GMT  
		Size: 61.0 MB (61034818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19c2e634090909c8b92a0bc6963538e530570f798f2d9fed2be84648f6e66df`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512843e4c495158d090efbaa5625e4123a8aa5978df645e3a86e941f2c478a8`  
		Last Modified: Wed, 14 Apr 2021 22:58:44 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd288200021e8c620e82728a414657c33d78a2bd6f17adc456286e2c471c362`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-data`

```console
$ docker pull influxdb@sha256:ed4bf75fda93d81d7212d2e5cb01fbd3549702d8f3c419a7958b44e85caa527c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.11-data` - linux; amd64

```console
$ docker pull influxdb@sha256:ddc6a1a374a233abf7192332b1b2dd58316658c4ba7cfca70d3ed39e85c4df9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (148962634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9eb629700047ef21ecf4ff1168db10c62a1a71151bb083ab37bdce2627ca73a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:08:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 12 May 2021 20:09:11 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Wed, 12 May 2021 20:09:19 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 12 May 2021 20:09:19 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 12 May 2021 20:09:20 GMT
EXPOSE 8086
# Wed, 12 May 2021 20:09:20 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 May 2021 20:09:20 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 12 May 2021 20:09:20 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 12 May 2021 20:09:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 May 2021 20:09:21 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee65a07cb0cad7eedb6332aad83a593a46bbae0a453842817353e2cf9de28d`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec20ebb0df2d0261a928fa2e775f7e47b1fbf489bd6e557e6e89b72d11e522eb`  
		Last Modified: Wed, 12 May 2021 20:11:49 GMT  
		Size: 87.9 MB (87949059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0820a4489a6108980883726bf6d7e5196dd9b42698603b5dd201c21efa87fe`  
		Last Modified: Wed, 12 May 2021 20:11:36 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b387507a918f61ed59e065e7321b85974b3e222cff40a36d0a036ad877a30c`  
		Last Modified: Wed, 12 May 2021 20:11:36 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df972cc3357c2211116b5b5bc0c66f2f9f4c4ba8a2ca41d1557eb1d2d602aac3`  
		Last Modified: Wed, 12 May 2021 20:11:36 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-data-alpine`

```console
$ docker pull influxdb@sha256:953218e27826969473de77140a6e8e36635bc9598fb53e87520da576a4714697
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.11-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:59f66a260ca6ac25da45231834f1ba1f5cbd13db57112b39a1eaf3d89418eb1e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91872207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6de1bd45ba333a7fa2b42d112e649986e5df7ccfb6e5d61b4708ed0c96a95770`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 22:56:32 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Wed, 14 Apr 2021 22:56:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:56:42 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 14 Apr 2021 22:56:42 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 22:56:43 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:56:43 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:56:43 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 14 Apr 2021 22:56:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:56:43 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d72c8962115b8fbd20d5a78dd48e575abcd35f896096c95e0b579a8dbd4336`  
		Last Modified: Wed, 14 Apr 2021 22:59:12 GMT  
		Size: 87.6 MB (87638906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0493fd864febd60f65cd5502bd7fcba1d872989c033068c72632717ea9b5137c`  
		Last Modified: Wed, 14 Apr 2021 22:59:01 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd7b30f761adf01ac672b68e8634efcdbcaed5cadd4e8fd9b997c0537ec7a65`  
		Last Modified: Wed, 14 Apr 2021 22:59:00 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd0880938167776dea94134027e0bc04f2f881b2fab628ec37a41a325af8ed0`  
		Last Modified: Wed, 14 Apr 2021 22:59:01 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-meta`

```console
$ docker pull influxdb@sha256:290bdfe1d6a3e9dcdcde563dd29a68863dedbf6df0ae1c6746e8b3d6c43b82fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.11-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:86bc517da71c544988faa8626a800ee73e3d022f05a1764e2c502f6f096b32b7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.1 MB (84146008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:237cfc98f85a91551a3eb5ebe09f3055a08a63fde758d935adbe1e3ddcf06a47`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:08:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 12 May 2021 20:09:11 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Wed, 12 May 2021 20:09:30 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 12 May 2021 20:09:31 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 12 May 2021 20:09:31 GMT
EXPOSE 8091
# Wed, 12 May 2021 20:09:31 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 May 2021 20:09:31 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 12 May 2021 20:09:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 May 2021 20:09:32 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee65a07cb0cad7eedb6332aad83a593a46bbae0a453842817353e2cf9de28d`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570d53070a17d2b30fa2e02a53a1d95e5467c6ccd4140714d34094e8854b9856`  
		Last Modified: Wed, 12 May 2021 20:12:04 GMT  
		Size: 23.1 MB (23133637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d7691e645821a46af60cf56f867e46b6b2d2a4769589676aa8b77b5e161ff5`  
		Last Modified: Wed, 12 May 2021 20:12:00 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150b35b4a9758cb5fa65d465b0de0bfe033c96efc0a8ca6f526dfbad28a57e9c`  
		Last Modified: Wed, 12 May 2021 20:12:00 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-meta-alpine`

```console
$ docker pull influxdb@sha256:f997194721a978be18e2db6310fc4f20d4e8ae1a13158de1cd7dc6b042ebe98b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.11-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:88915c86ce7afd69b101ba5a4dd8d1dfce23bfa760dd74fbb8fec36b562a3909
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27235086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0485099136dd77a780e637f002a9399df5468f2609d126e85c977208798adaac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 22:56:32 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Wed, 14 Apr 2021 22:56:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:56:55 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 14 Apr 2021 22:56:55 GMT
EXPOSE 8091
# Wed, 14 Apr 2021 22:56:55 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:56:55 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:56:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:56:56 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8177497e45bcdf4f69a9c9e31aa09286c8157b7e3918ca418f2a8792b98791`  
		Last Modified: Wed, 14 Apr 2021 22:59:27 GMT  
		Size: 23.0 MB (23002988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ea6921490482ed769782ef5ab560e586b844b845bd40314224130d55910a45`  
		Last Modified: Wed, 14 Apr 2021 22:59:24 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bb5766ed91f5ba3565a638433f21786c10951ed30c32133153d1e11a7826c0`  
		Last Modified: Wed, 14 Apr 2021 22:59:28 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8`

```console
$ docker pull influxdb@sha256:4c10ce4aa692b4c3fcc27ea7d003c5cd2f999769150c76cdb3c096cbc5f7991e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:23d32e677af71e4519ed9bfb85723a828d01ac82c86389e2b9c37151ddd1fb2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126061236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6af31fae140af15e439f710b7579e2741ecf7e053cd9fec9bac7c252d55ee3c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:08:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Mon, 24 May 2021 19:20:37 GMT
ENV INFLUXDB_VERSION=1.8.6
# Mon, 24 May 2021 19:20:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Mon, 24 May 2021 19:20:45 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Mon, 24 May 2021 19:20:45 GMT
EXPOSE 8086
# Mon, 24 May 2021 19:20:46 GMT
VOLUME [/var/lib/influxdb]
# Mon, 24 May 2021 19:20:46 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Mon, 24 May 2021 19:20:46 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 24 May 2021 19:20:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 May 2021 19:20:46 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee65a07cb0cad7eedb6332aad83a593a46bbae0a453842817353e2cf9de28d`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17baf5a92309fcd575858ceff57924937cb52c1b51355c2ec76705a8a376522d`  
		Last Modified: Mon, 24 May 2021 19:22:39 GMT  
		Size: 65.0 MB (65047718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d07aa44165dee1218c34465f5684d5e4445fd2b2869a9d00de6963d5dc8c4d`  
		Last Modified: Mon, 24 May 2021 19:22:30 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e679c948a0d9394372b6f79352e44b4747b326dce04e1c0ff7692ae3ddcc6ad`  
		Last Modified: Mon, 24 May 2021 19:22:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab83d5924aa69d2a02add875492dd5b35009d46676c85ef4c7452af723c79a7`  
		Last Modified: Mon, 24 May 2021 19:22:30 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:cb1de27b7427e04c977c37b281fe25d8052ce629af73ce6d4fb78624f6b2e953
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.1 MB (117133004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29f31fb2110e482825565cc9a95546eef1160ca06723781ea3a070587c041087`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 May 2021 01:11:51 GMT
ADD file:81cfd4e746bdfcc19847240b77012487652be22dbd5741ccb2485a4207f2b73f in / 
# Wed, 12 May 2021 01:11:56 GMT
CMD ["bash"]
# Thu, 27 May 2021 00:45:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:45:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 15:25:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 27 May 2021 15:26:10 GMT
ENV INFLUXDB_VERSION=1.8.6
# Thu, 27 May 2021 15:26:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 27 May 2021 15:26:16 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 27 May 2021 15:26:17 GMT
EXPOSE 8086
# Thu, 27 May 2021 15:26:17 GMT
VOLUME [/var/lib/influxdb]
# Thu, 27 May 2021 15:26:17 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 27 May 2021 15:26:17 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 27 May 2021 15:26:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 May 2021 15:26:18 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:55b9a6b6b2552c5b2eac0a316e75a7bc18092819ee25c4f1d4d54700bcc1d3dc`  
		Last Modified: Wed, 12 May 2021 01:21:23 GMT  
		Size: 42.1 MB (42120307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba756a0ca8996787a145d62543ecf7cec523a638705be132f442d2013655149`  
		Last Modified: Thu, 27 May 2021 01:06:39 GMT  
		Size: 10.0 MB (9950803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61945aef6a8fee06fbe4dccead7cbad9da46ba174cee1eae1f813541ddb76b3`  
		Last Modified: Thu, 27 May 2021 01:06:38 GMT  
		Size: 3.9 MB (3921169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c677858c56844f5e94ad0349f4825fe826cbc6411776e4daf3ae7979e3ac45e`  
		Last Modified: Thu, 27 May 2021 15:26:40 GMT  
		Size: 2.9 KB (2851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa28ee3fd790cf2c401066384bdc26bca45d0d45b5e9afb16bb82d388445c99`  
		Last Modified: Thu, 27 May 2021 15:27:14 GMT  
		Size: 61.1 MB (61136157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce9393956a63f78dbe35955f9963b45543b9795ccdaf80f9adfb1b94af46eab`  
		Last Modified: Thu, 27 May 2021 15:27:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d07cb25a1da5ea3f1901e8bb2ac2ed797e183e1852e7786da813ecdd2ea12f`  
		Last Modified: Thu, 27 May 2021 15:27:03 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d30e0999373ce1db20ca0606505fa6e6dde294c1bac454989049e835025d5e`  
		Last Modified: Thu, 27 May 2021 15:27:03 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:3593251a5895534faa1841d1b26a22a2677cf37ea74413b4eec6ab6c2af297b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118189699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f27c8bbe8aa1d0e4ab14fe8c75e5529ddbc62b89897b64cfaa5a5e888222f41c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:55 GMT
ADD file:02285d0bd3ea996a7ebbe069a83e508701cbaf14f53fdeaa123775acd7e0537f in / 
# Tue, 22 Jun 2021 23:50:56 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:27:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:27:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 18:33:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 18:34:06 GMT
ENV INFLUXDB_VERSION=1.8.6
# Wed, 23 Jun 2021 18:34:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 23 Jun 2021 18:34:10 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 23 Jun 2021 18:34:10 GMT
EXPOSE 8086
# Wed, 23 Jun 2021 18:34:10 GMT
VOLUME [/var/lib/influxdb]
# Wed, 23 Jun 2021 18:34:11 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 23 Jun 2021 18:34:11 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 23 Jun 2021 18:34:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 18:34:11 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:0789e4a342a11c7c57a241829a41af53fbd194e6dede60c6d6f63d69e403b2cd`  
		Last Modified: Tue, 22 Jun 2021 23:57:52 GMT  
		Size: 43.2 MB (43177421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd2ed69368e8a7d296f1c91060e897753bed4a79ab68ed47c544e1f4d6fadcd`  
		Last Modified: Wed, 23 Jun 2021 00:35:58 GMT  
		Size: 10.2 MB (10214577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c76e514669ff971481e0d19dc0581f90d72eab2d0e117a5761ae016e14f213`  
		Last Modified: Wed, 23 Jun 2021 00:35:57 GMT  
		Size: 4.1 MB (4096534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6d3ae4d939261675d1e9409c3de9369a4e1d761bea9c9887f546c7086b325a`  
		Last Modified: Wed, 23 Jun 2021 18:35:06 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755a51f04c750f8be1b59a1c3cd62742dd3a30c0475de9bb6fcebd0c4db7fc32`  
		Last Modified: Wed, 23 Jun 2021 18:35:36 GMT  
		Size: 60.7 MB (60696598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03a16ef72b0463f07c9ee602e683a863c8936d7e5dedd2e1c1be2a1b712dbe6`  
		Last Modified: Wed, 23 Jun 2021 18:35:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca63296bbbac0183f1d5d949c9c012bc0cce81e8cb918b27a2337bfa920a52b8`  
		Last Modified: Wed, 23 Jun 2021 18:35:27 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d218c4c7b8cc3e25a078e9ad2c0aae9ddb0690efb98274c17c45b16dcb0489d7`  
		Last Modified: Wed, 23 Jun 2021 18:35:27 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-alpine`

```console
$ docker pull influxdb@sha256:174c55979a8f75e5c73eb8577ebd10f3cf15ec2a537d36720bf979dc4637acc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b6dd41e7fcf0c6e54619389ea1bb8f5f0ddac3c383772c8b698f570c2cc1e3cb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69024519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f03f71b7dafee03ac595905d2ce40a298f31d25171577ed99b00d1a600e96b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 24 May 2021 19:20:50 GMT
ENV INFLUXDB_VERSION=1.8.6
# Mon, 24 May 2021 19:20:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 24 May 2021 19:20:59 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Mon, 24 May 2021 19:20:59 GMT
EXPOSE 8086
# Mon, 24 May 2021 19:20:59 GMT
VOLUME [/var/lib/influxdb]
# Mon, 24 May 2021 19:21:00 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Mon, 24 May 2021 19:21:00 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 24 May 2021 19:21:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 May 2021 19:21:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5453a27c127086016d437494e880126fa294abf107506c213069720c8a07bab5`  
		Last Modified: Mon, 24 May 2021 19:22:59 GMT  
		Size: 64.8 MB (64791278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9552b4098165021fc55db600133f5f6dca90e013b0580bf7349194af0b51533f`  
		Last Modified: Mon, 24 May 2021 19:22:50 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27512febb70786ebe5a3b4b0ccd8e2c63259b9b77d168a2734bc17a6e0c33db3`  
		Last Modified: Mon, 24 May 2021 19:22:49 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2e117c0ac0e8595f7057b0158624321c7b87441a41ba545a807bbfea8cdb4d`  
		Last Modified: Mon, 24 May 2021 19:22:50 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data`

```console
$ docker pull influxdb@sha256:3ab29570c11851024e562dd3b17f3652040145c59e3bb3a16d57447740de1a4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:526e7102df9bedfd31b6cbcbfdc3ae31884f31e0d0c9ca2ef48f3cc84d85ec5f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127796276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:190b6b4a1f8faf9284e3d3e6b8c651e3b1caaf159587514aa07b2f50445ec473`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:08:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Mon, 24 May 2021 19:21:03 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Mon, 24 May 2021 19:21:11 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 24 May 2021 19:21:11 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 24 May 2021 19:21:12 GMT
EXPOSE 8086
# Mon, 24 May 2021 19:21:12 GMT
VOLUME [/var/lib/influxdb]
# Mon, 24 May 2021 19:21:12 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 24 May 2021 19:21:12 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 24 May 2021 19:21:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 May 2021 19:21:13 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee65a07cb0cad7eedb6332aad83a593a46bbae0a453842817353e2cf9de28d`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2773a7a98d7cff7012b04a6fd405bb45f072ce0f9984263ab559154b982cae`  
		Last Modified: Mon, 24 May 2021 19:23:18 GMT  
		Size: 66.8 MB (66782700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf345410be519d9f0751067be899e03bd987eac20a1ba875a2cd2748cdca3b4d`  
		Last Modified: Mon, 24 May 2021 19:23:10 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774ea1a99f05b930aa9e1fcc7138edd601a2c935b1c99d716b8543d7d1b706bb`  
		Last Modified: Mon, 24 May 2021 19:23:09 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33f603323ad9cb59df3614505a398877ea36e531cacd3268f881b929cc2ebe3`  
		Last Modified: Mon, 24 May 2021 19:23:10 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data-alpine`

```console
$ docker pull influxdb@sha256:3de2a6289300d1be88487af5fd2abacad7ca9ff2ec3d7353cfcbca129af892eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ef00d61d767fa488b5bfd38dd80c5269c5eddf8574dcddb9c02bb947573ce03e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70748316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c8a165e3b520020729746e784c1eb6041a4716205c5f5a4f4396ebf9e750b76`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 24 May 2021 19:21:17 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Mon, 24 May 2021 19:21:25 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 24 May 2021 19:21:26 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 24 May 2021 19:21:26 GMT
EXPOSE 8086
# Mon, 24 May 2021 19:21:26 GMT
VOLUME [/var/lib/influxdb]
# Mon, 24 May 2021 19:21:26 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 24 May 2021 19:21:27 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 24 May 2021 19:21:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 May 2021 19:21:27 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635793f5b48306dcab955aff9084c73aa36b911d9ecdd80fc6c0bda504313d8d`  
		Last Modified: Mon, 24 May 2021 19:23:42 GMT  
		Size: 66.5 MB (66515016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd3ce0e1057e72d11c9f915b709ac9b00f75c90f4288978eeb3d51857cae3a`  
		Last Modified: Mon, 24 May 2021 19:23:32 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2506c8ad21fbee3890d94e936ba78d5b9eb0691df595e6755694986231fc54`  
		Last Modified: Mon, 24 May 2021 19:23:33 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4d3e6c0b28abb9f6508c063df0648c3ee25886596d7a6157cae6adeb4767bf`  
		Last Modified: Mon, 24 May 2021 19:23:33 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta`

```console
$ docker pull influxdb@sha256:cfb5b01b5f8055f85824b84d2cbd92861af0fe230f2e5462c4aaa7d20e931f16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:e90ef2d58ad2113dcecbfdab6b0f62d435218e530bd358984b7181ed9f49e2bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84218334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8afaed1241b57683e2cc0bc2eb77fd3da57e14330cb69a0a935b56a2ee013321`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:08:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Mon, 24 May 2021 19:21:03 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Mon, 24 May 2021 19:21:34 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 24 May 2021 19:21:35 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 24 May 2021 19:21:35 GMT
EXPOSE 8091
# Mon, 24 May 2021 19:21:35 GMT
VOLUME [/var/lib/influxdb]
# Mon, 24 May 2021 19:21:35 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 24 May 2021 19:21:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 May 2021 19:21:36 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee65a07cb0cad7eedb6332aad83a593a46bbae0a453842817353e2cf9de28d`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df73b02e0adbf70adff8d7415e4e195b974a97b32c83a5dcbc8cf2314985fc5b`  
		Last Modified: Mon, 24 May 2021 19:23:57 GMT  
		Size: 23.2 MB (23205961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c59be4dda832c46c462ef85cacad8d242061f7e886398ac7f17668e5a880ba`  
		Last Modified: Mon, 24 May 2021 19:23:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1750d7e819bc72c58d2e341fd3a97759cf4f176db42e26e189273733c18b29d`  
		Last Modified: Mon, 24 May 2021 19:23:54 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta-alpine`

```console
$ docker pull influxdb@sha256:c5781a2ad82e23ecb77997b22d22a0f40b2d200e1d47bc9679bc5e6d5cef19a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:4adaa9b434a9cdeaf97111df8bc113633453db727ccc7623bf0a0d6f41b5646d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27306919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ba1ee0645cd12155610113100bb0564d95b9367c4ce88a91a77251d09568b7c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 24 May 2021 19:21:17 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Mon, 24 May 2021 19:21:43 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 24 May 2021 19:21:44 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 24 May 2021 19:21:44 GMT
EXPOSE 8091
# Mon, 24 May 2021 19:21:44 GMT
VOLUME [/var/lib/influxdb]
# Mon, 24 May 2021 19:21:44 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 24 May 2021 19:21:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 May 2021 19:21:45 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a0d200db7e6e767fb2b050a82e962f822da4d61122122a1d905d82be300dbe`  
		Last Modified: Mon, 24 May 2021 19:24:13 GMT  
		Size: 23.1 MB (23074821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084943cc8c5278875e6be6fd518a250ea14d19d4f4bb3174c8aa6f1db7521ae3`  
		Last Modified: Mon, 24 May 2021 19:24:10 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2187653745d63baa53dc6c0cd4cb5f83bd6c9c3f9fd92e4727a0394e09a5f5bf`  
		Last Modified: Mon, 24 May 2021 19:24:10 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.6`

```console
$ docker pull influxdb@sha256:4c10ce4aa692b4c3fcc27ea7d003c5cd2f999769150c76cdb3c096cbc5f7991e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.6` - linux; amd64

```console
$ docker pull influxdb@sha256:23d32e677af71e4519ed9bfb85723a828d01ac82c86389e2b9c37151ddd1fb2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126061236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6af31fae140af15e439f710b7579e2741ecf7e053cd9fec9bac7c252d55ee3c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:08:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Mon, 24 May 2021 19:20:37 GMT
ENV INFLUXDB_VERSION=1.8.6
# Mon, 24 May 2021 19:20:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Mon, 24 May 2021 19:20:45 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Mon, 24 May 2021 19:20:45 GMT
EXPOSE 8086
# Mon, 24 May 2021 19:20:46 GMT
VOLUME [/var/lib/influxdb]
# Mon, 24 May 2021 19:20:46 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Mon, 24 May 2021 19:20:46 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 24 May 2021 19:20:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 May 2021 19:20:46 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee65a07cb0cad7eedb6332aad83a593a46bbae0a453842817353e2cf9de28d`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17baf5a92309fcd575858ceff57924937cb52c1b51355c2ec76705a8a376522d`  
		Last Modified: Mon, 24 May 2021 19:22:39 GMT  
		Size: 65.0 MB (65047718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d07aa44165dee1218c34465f5684d5e4445fd2b2869a9d00de6963d5dc8c4d`  
		Last Modified: Mon, 24 May 2021 19:22:30 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e679c948a0d9394372b6f79352e44b4747b326dce04e1c0ff7692ae3ddcc6ad`  
		Last Modified: Mon, 24 May 2021 19:22:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab83d5924aa69d2a02add875492dd5b35009d46676c85ef4c7452af723c79a7`  
		Last Modified: Mon, 24 May 2021 19:22:30 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.6` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:cb1de27b7427e04c977c37b281fe25d8052ce629af73ce6d4fb78624f6b2e953
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.1 MB (117133004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29f31fb2110e482825565cc9a95546eef1160ca06723781ea3a070587c041087`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 May 2021 01:11:51 GMT
ADD file:81cfd4e746bdfcc19847240b77012487652be22dbd5741ccb2485a4207f2b73f in / 
# Wed, 12 May 2021 01:11:56 GMT
CMD ["bash"]
# Thu, 27 May 2021 00:45:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:45:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 15:25:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 27 May 2021 15:26:10 GMT
ENV INFLUXDB_VERSION=1.8.6
# Thu, 27 May 2021 15:26:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 27 May 2021 15:26:16 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 27 May 2021 15:26:17 GMT
EXPOSE 8086
# Thu, 27 May 2021 15:26:17 GMT
VOLUME [/var/lib/influxdb]
# Thu, 27 May 2021 15:26:17 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 27 May 2021 15:26:17 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 27 May 2021 15:26:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 May 2021 15:26:18 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:55b9a6b6b2552c5b2eac0a316e75a7bc18092819ee25c4f1d4d54700bcc1d3dc`  
		Last Modified: Wed, 12 May 2021 01:21:23 GMT  
		Size: 42.1 MB (42120307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba756a0ca8996787a145d62543ecf7cec523a638705be132f442d2013655149`  
		Last Modified: Thu, 27 May 2021 01:06:39 GMT  
		Size: 10.0 MB (9950803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61945aef6a8fee06fbe4dccead7cbad9da46ba174cee1eae1f813541ddb76b3`  
		Last Modified: Thu, 27 May 2021 01:06:38 GMT  
		Size: 3.9 MB (3921169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c677858c56844f5e94ad0349f4825fe826cbc6411776e4daf3ae7979e3ac45e`  
		Last Modified: Thu, 27 May 2021 15:26:40 GMT  
		Size: 2.9 KB (2851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa28ee3fd790cf2c401066384bdc26bca45d0d45b5e9afb16bb82d388445c99`  
		Last Modified: Thu, 27 May 2021 15:27:14 GMT  
		Size: 61.1 MB (61136157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce9393956a63f78dbe35955f9963b45543b9795ccdaf80f9adfb1b94af46eab`  
		Last Modified: Thu, 27 May 2021 15:27:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d07cb25a1da5ea3f1901e8bb2ac2ed797e183e1852e7786da813ecdd2ea12f`  
		Last Modified: Thu, 27 May 2021 15:27:03 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d30e0999373ce1db20ca0606505fa6e6dde294c1bac454989049e835025d5e`  
		Last Modified: Thu, 27 May 2021 15:27:03 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.6` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:3593251a5895534faa1841d1b26a22a2677cf37ea74413b4eec6ab6c2af297b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118189699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f27c8bbe8aa1d0e4ab14fe8c75e5529ddbc62b89897b64cfaa5a5e888222f41c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:55 GMT
ADD file:02285d0bd3ea996a7ebbe069a83e508701cbaf14f53fdeaa123775acd7e0537f in / 
# Tue, 22 Jun 2021 23:50:56 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:27:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:27:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 18:33:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 18:34:06 GMT
ENV INFLUXDB_VERSION=1.8.6
# Wed, 23 Jun 2021 18:34:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 23 Jun 2021 18:34:10 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 23 Jun 2021 18:34:10 GMT
EXPOSE 8086
# Wed, 23 Jun 2021 18:34:10 GMT
VOLUME [/var/lib/influxdb]
# Wed, 23 Jun 2021 18:34:11 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 23 Jun 2021 18:34:11 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 23 Jun 2021 18:34:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 18:34:11 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:0789e4a342a11c7c57a241829a41af53fbd194e6dede60c6d6f63d69e403b2cd`  
		Last Modified: Tue, 22 Jun 2021 23:57:52 GMT  
		Size: 43.2 MB (43177421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd2ed69368e8a7d296f1c91060e897753bed4a79ab68ed47c544e1f4d6fadcd`  
		Last Modified: Wed, 23 Jun 2021 00:35:58 GMT  
		Size: 10.2 MB (10214577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c76e514669ff971481e0d19dc0581f90d72eab2d0e117a5761ae016e14f213`  
		Last Modified: Wed, 23 Jun 2021 00:35:57 GMT  
		Size: 4.1 MB (4096534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6d3ae4d939261675d1e9409c3de9369a4e1d761bea9c9887f546c7086b325a`  
		Last Modified: Wed, 23 Jun 2021 18:35:06 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755a51f04c750f8be1b59a1c3cd62742dd3a30c0475de9bb6fcebd0c4db7fc32`  
		Last Modified: Wed, 23 Jun 2021 18:35:36 GMT  
		Size: 60.7 MB (60696598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03a16ef72b0463f07c9ee602e683a863c8936d7e5dedd2e1c1be2a1b712dbe6`  
		Last Modified: Wed, 23 Jun 2021 18:35:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca63296bbbac0183f1d5d949c9c012bc0cce81e8cb918b27a2337bfa920a52b8`  
		Last Modified: Wed, 23 Jun 2021 18:35:27 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d218c4c7b8cc3e25a078e9ad2c0aae9ddb0690efb98274c17c45b16dcb0489d7`  
		Last Modified: Wed, 23 Jun 2021 18:35:27 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.6-alpine`

```console
$ docker pull influxdb@sha256:174c55979a8f75e5c73eb8577ebd10f3cf15ec2a537d36720bf979dc4637acc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.6-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b6dd41e7fcf0c6e54619389ea1bb8f5f0ddac3c383772c8b698f570c2cc1e3cb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69024519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f03f71b7dafee03ac595905d2ce40a298f31d25171577ed99b00d1a600e96b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 24 May 2021 19:20:50 GMT
ENV INFLUXDB_VERSION=1.8.6
# Mon, 24 May 2021 19:20:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 24 May 2021 19:20:59 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Mon, 24 May 2021 19:20:59 GMT
EXPOSE 8086
# Mon, 24 May 2021 19:20:59 GMT
VOLUME [/var/lib/influxdb]
# Mon, 24 May 2021 19:21:00 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Mon, 24 May 2021 19:21:00 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 24 May 2021 19:21:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 May 2021 19:21:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5453a27c127086016d437494e880126fa294abf107506c213069720c8a07bab5`  
		Last Modified: Mon, 24 May 2021 19:22:59 GMT  
		Size: 64.8 MB (64791278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9552b4098165021fc55db600133f5f6dca90e013b0580bf7349194af0b51533f`  
		Last Modified: Mon, 24 May 2021 19:22:50 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27512febb70786ebe5a3b4b0ccd8e2c63259b9b77d168a2734bc17a6e0c33db3`  
		Last Modified: Mon, 24 May 2021 19:22:49 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2e117c0ac0e8595f7057b0158624321c7b87441a41ba545a807bbfea8cdb4d`  
		Last Modified: Mon, 24 May 2021 19:22:50 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.6-data`

```console
$ docker pull influxdb@sha256:3ab29570c11851024e562dd3b17f3652040145c59e3bb3a16d57447740de1a4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.6-data` - linux; amd64

```console
$ docker pull influxdb@sha256:526e7102df9bedfd31b6cbcbfdc3ae31884f31e0d0c9ca2ef48f3cc84d85ec5f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127796276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:190b6b4a1f8faf9284e3d3e6b8c651e3b1caaf159587514aa07b2f50445ec473`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:08:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Mon, 24 May 2021 19:21:03 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Mon, 24 May 2021 19:21:11 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 24 May 2021 19:21:11 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 24 May 2021 19:21:12 GMT
EXPOSE 8086
# Mon, 24 May 2021 19:21:12 GMT
VOLUME [/var/lib/influxdb]
# Mon, 24 May 2021 19:21:12 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 24 May 2021 19:21:12 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 24 May 2021 19:21:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 May 2021 19:21:13 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee65a07cb0cad7eedb6332aad83a593a46bbae0a453842817353e2cf9de28d`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2773a7a98d7cff7012b04a6fd405bb45f072ce0f9984263ab559154b982cae`  
		Last Modified: Mon, 24 May 2021 19:23:18 GMT  
		Size: 66.8 MB (66782700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf345410be519d9f0751067be899e03bd987eac20a1ba875a2cd2748cdca3b4d`  
		Last Modified: Mon, 24 May 2021 19:23:10 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774ea1a99f05b930aa9e1fcc7138edd601a2c935b1c99d716b8543d7d1b706bb`  
		Last Modified: Mon, 24 May 2021 19:23:09 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33f603323ad9cb59df3614505a398877ea36e531cacd3268f881b929cc2ebe3`  
		Last Modified: Mon, 24 May 2021 19:23:10 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.6-data-alpine`

```console
$ docker pull influxdb@sha256:3de2a6289300d1be88487af5fd2abacad7ca9ff2ec3d7353cfcbca129af892eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.6-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ef00d61d767fa488b5bfd38dd80c5269c5eddf8574dcddb9c02bb947573ce03e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70748316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c8a165e3b520020729746e784c1eb6041a4716205c5f5a4f4396ebf9e750b76`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 24 May 2021 19:21:17 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Mon, 24 May 2021 19:21:25 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 24 May 2021 19:21:26 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 24 May 2021 19:21:26 GMT
EXPOSE 8086
# Mon, 24 May 2021 19:21:26 GMT
VOLUME [/var/lib/influxdb]
# Mon, 24 May 2021 19:21:26 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 24 May 2021 19:21:27 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 24 May 2021 19:21:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 May 2021 19:21:27 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635793f5b48306dcab955aff9084c73aa36b911d9ecdd80fc6c0bda504313d8d`  
		Last Modified: Mon, 24 May 2021 19:23:42 GMT  
		Size: 66.5 MB (66515016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd3ce0e1057e72d11c9f915b709ac9b00f75c90f4288978eeb3d51857cae3a`  
		Last Modified: Mon, 24 May 2021 19:23:32 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2506c8ad21fbee3890d94e936ba78d5b9eb0691df595e6755694986231fc54`  
		Last Modified: Mon, 24 May 2021 19:23:33 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4d3e6c0b28abb9f6508c063df0648c3ee25886596d7a6157cae6adeb4767bf`  
		Last Modified: Mon, 24 May 2021 19:23:33 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.6-meta`

```console
$ docker pull influxdb@sha256:cfb5b01b5f8055f85824b84d2cbd92861af0fe230f2e5462c4aaa7d20e931f16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.6-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:e90ef2d58ad2113dcecbfdab6b0f62d435218e530bd358984b7181ed9f49e2bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84218334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8afaed1241b57683e2cc0bc2eb77fd3da57e14330cb69a0a935b56a2ee013321`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:08:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Mon, 24 May 2021 19:21:03 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Mon, 24 May 2021 19:21:34 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 24 May 2021 19:21:35 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 24 May 2021 19:21:35 GMT
EXPOSE 8091
# Mon, 24 May 2021 19:21:35 GMT
VOLUME [/var/lib/influxdb]
# Mon, 24 May 2021 19:21:35 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 24 May 2021 19:21:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 May 2021 19:21:36 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee65a07cb0cad7eedb6332aad83a593a46bbae0a453842817353e2cf9de28d`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df73b02e0adbf70adff8d7415e4e195b974a97b32c83a5dcbc8cf2314985fc5b`  
		Last Modified: Mon, 24 May 2021 19:23:57 GMT  
		Size: 23.2 MB (23205961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c59be4dda832c46c462ef85cacad8d242061f7e886398ac7f17668e5a880ba`  
		Last Modified: Mon, 24 May 2021 19:23:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1750d7e819bc72c58d2e341fd3a97759cf4f176db42e26e189273733c18b29d`  
		Last Modified: Mon, 24 May 2021 19:23:54 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.6-meta-alpine`

```console
$ docker pull influxdb@sha256:c5781a2ad82e23ecb77997b22d22a0f40b2d200e1d47bc9679bc5e6d5cef19a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.6-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:4adaa9b434a9cdeaf97111df8bc113633453db727ccc7623bf0a0d6f41b5646d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27306919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ba1ee0645cd12155610113100bb0564d95b9367c4ce88a91a77251d09568b7c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 24 May 2021 19:21:17 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Mon, 24 May 2021 19:21:43 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 24 May 2021 19:21:44 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 24 May 2021 19:21:44 GMT
EXPOSE 8091
# Mon, 24 May 2021 19:21:44 GMT
VOLUME [/var/lib/influxdb]
# Mon, 24 May 2021 19:21:44 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 24 May 2021 19:21:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 May 2021 19:21:45 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a0d200db7e6e767fb2b050a82e962f822da4d61122122a1d905d82be300dbe`  
		Last Modified: Mon, 24 May 2021 19:24:13 GMT  
		Size: 23.1 MB (23074821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084943cc8c5278875e6be6fd518a250ea14d19d4f4bb3174c8aa6f1db7521ae3`  
		Last Modified: Mon, 24 May 2021 19:24:10 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2187653745d63baa53dc6c0cd4cb5f83bd6c9c3f9fd92e4727a0394e09a5f5bf`  
		Last Modified: Mon, 24 May 2021 19:24:10 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0`

```console
$ docker pull influxdb@sha256:e80fe1f239c78881571d487d4356f3ae379dbedf44f2cf8dcb2444e2c3229222
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0` - linux; amd64

```console
$ docker pull influxdb@sha256:b50f219df32da917355b0db781150e6d0b89f149805663440a9e04c796ac13c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178697196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd6a4507399651c8d686cd4a63db7ef4312feb26e62846dc2398df2358bfbd63`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:10:17 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 12 May 2021 20:10:17 GMT
ENV GOSU_VER=1.12
# Wed, 12 May 2021 20:10:20 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 05 Jun 2021 00:31:22 GMT
ENV INFLUXDB_VERSION=2.0.7
# Sat, 05 Jun 2021 00:31:33 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 05 Jun 2021 00:31:35 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 05 Jun 2021 00:31:35 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 05 Jun 2021 00:31:35 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 05 Jun 2021 00:31:35 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Sat, 05 Jun 2021 00:31:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Jun 2021 00:31:36 GMT
CMD ["influxd"]
# Sat, 05 Jun 2021 00:31:36 GMT
EXPOSE 8086
# Sat, 05 Jun 2021 00:31:36 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 05 Jun 2021 00:31:36 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 05 Jun 2021 00:31:37 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b26e21cfb07a9a6fd606a130ce8206843d702e4f616d53df1321437a01a0ac0`  
		Last Modified: Wed, 12 May 2021 20:13:23 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77b907603e396f34b2bbb8229e1a740deabeb6537f737d78db0f2452f2504e8`  
		Last Modified: Wed, 12 May 2021 20:13:20 GMT  
		Size: 961.0 KB (960988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9591ed1fb6b3d71a7c4957993349963b5bf90e1a59c9104548b9c7afc65b1a08`  
		Last Modified: Sat, 05 Jun 2021 00:32:49 GMT  
		Size: 109.5 MB (109466216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba458e8eb79c92d9d076a9758c228a52d495388a8520755dbd5869f878de262c`  
		Last Modified: Sat, 05 Jun 2021 00:32:39 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac66788c54e9775c3aef47ef263022a66b957839916cb13f5750434938853cfa`  
		Last Modified: Sat, 05 Jun 2021 00:32:39 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608813173efe22b91f20d22d9f0056154ffdf93c54dbb83c2656215808797c30`  
		Last Modified: Sat, 05 Jun 2021 00:32:39 GMT  
		Size: 4.3 KB (4314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:d9825b3d372ad663f34bf92a3ebc1b9022906062b06986a0f203c5ab8670fec1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180628536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcdad0ed3f5fbd15e87467aad894389fa02f9ecb82c2710bc7bd62d50db96409`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:24:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:24:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 18:34:17 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 23 Jun 2021 18:34:17 GMT
ENV GOSU_VER=1.12
# Wed, 23 Jun 2021 18:34:20 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 23 Jun 2021 18:34:20 GMT
ENV INFLUXDB_VERSION=2.0.7
# Wed, 23 Jun 2021 18:34:28 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 23 Jun 2021 18:34:29 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 23 Jun 2021 18:34:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 23 Jun 2021 18:34:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 23 Jun 2021 18:34:30 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Wed, 23 Jun 2021 18:34:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 18:34:30 GMT
CMD ["influxd"]
# Wed, 23 Jun 2021 18:34:30 GMT
EXPOSE 8086
# Wed, 23 Jun 2021 18:34:30 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 23 Jun 2021 18:34:31 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 23 Jun 2021 18:34:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86422c44ee005c4d5ccb0e2fa32685229207b712728cd4b8c0ef97174f079df7`  
		Last Modified: Wed, 23 Jun 2021 00:33:16 GMT  
		Size: 7.7 MB (7694715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9137877e0c26a439a8954003b21876b6059de852c839631e8cf6fda5bd36434c`  
		Last Modified: Wed, 23 Jun 2021 00:33:17 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2b86f0fed5df426869e08ab884f79326e9a310498fb9c49929e08f9ef9002b`  
		Last Modified: Wed, 23 Jun 2021 18:35:51 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f865c284b0e6b32bd1f1dd14ec1e334cbadc7d6292712190efa42f4718b8dd`  
		Last Modified: Wed, 23 Jun 2021 18:35:48 GMT  
		Size: 896.4 KB (896380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea300fef38e2d57c2657aaad371813835137c72d9f2c258e56af5006e4e5797`  
		Last Modified: Wed, 23 Jun 2021 18:36:00 GMT  
		Size: 112.8 MB (112824510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0fc3d9ce52b5368331dd5726abd82bd12ed7c3e8a23a33cdc89f2fbf64ab73`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f091d2bde4f35ffdd2cb09c6e1bdce03228e14e72564adc636b11ddf9829ce`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b9b006308f765debe388af66277c827d88a43a1cc4a90dee951af142b3d1d0`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 4.3 KB (4315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0-alpine`

```console
$ docker pull influxdb@sha256:7630ad8caae177fe5442cce81068b944c13e2daa7ec289d6d3710b836824cd79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:9c2e3774aca3f2ee9675a1e0121836ab6b094f3ff4b2b0fae03dc2dd5c3f8378
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122946151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c5ab4e012ccdc738b8b78a3095905324f5e6e785f25dac93203a50321ca2039`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:57:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:57:47 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Wed, 14 Apr 2021 22:57:48 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 14 Apr 2021 22:57:49 GMT
ENV GOSU_VER=1.12
# Wed, 14 Apr 2021 22:57:52 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Jun 2021 00:31:40 GMT
ENV INFLUXDB_VERSION=2.0.7
# Sat, 05 Jun 2021 00:31:49 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 05 Jun 2021 00:31:50 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 05 Jun 2021 00:31:50 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 05 Jun 2021 00:31:50 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 05 Jun 2021 00:31:50 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Sat, 05 Jun 2021 00:31:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Jun 2021 00:31:51 GMT
CMD ["influxd"]
# Sat, 05 Jun 2021 00:31:51 GMT
EXPOSE 8086
# Sat, 05 Jun 2021 00:31:51 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 05 Jun 2021 00:31:51 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 05 Jun 2021 00:31:52 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70fcedbcfb9328a87e76b312a1996118fac6b73a1dea800c39df8d00207148`  
		Last Modified: Wed, 14 Apr 2021 23:01:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e50c2af4ce019b31b8f9df4781ebe41c99a903cd661ad9231e08773b029cfec`  
		Last Modified: Wed, 14 Apr 2021 23:01:05 GMT  
		Size: 9.7 MB (9701057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99cdb09e5aee3ab8869581dee7b389f6ebd9507ff9613cbc03683586b99eb96`  
		Last Modified: Wed, 14 Apr 2021 23:00:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4633d963d8e54bd89ef20119577189c164929c6451ec7be1f4cf45d26c3bb283`  
		Last Modified: Wed, 14 Apr 2021 23:00:56 GMT  
		Size: 960.6 KB (960616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8520535bd417b8e9823de3f2c784aaa5ee76600551afc6b859eeeba6f96d7687`  
		Last Modified: Sat, 05 Jun 2021 00:33:13 GMT  
		Size: 109.5 MB (109466245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c09337d0dcff42440f468734b71a602c359686958498e9880747a5ab008e47`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d17425d58200c18e5d27020d669313a6da4c073674fa9f07fa9618857b39f3`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67868fd95f4078c1eafb60e477d23b3c44ade51937a76f0854ebe16887fdd33`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 4.3 KB (4315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4eb31630932f0863ea90024beed6e95ad728eff5ff808ed860a9b6053e69e5ac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125980529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68e83b89b6cbd0d3cb85dd391739622d356bf8c255c4d79db34aaf80057183bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:52:29 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 16 Jun 2021 00:52:31 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Wed, 16 Jun 2021 00:52:32 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 16 Jun 2021 00:52:32 GMT
ENV GOSU_VER=1.12
# Wed, 16 Jun 2021 00:52:35 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Jun 2021 00:52:35 GMT
ENV INFLUXDB_VERSION=2.0.7
# Wed, 16 Jun 2021 00:53:07 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 16 Jun 2021 00:53:08 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 16 Jun 2021 00:53:08 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 16 Jun 2021 00:53:08 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 16 Jun 2021 00:53:09 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Wed, 16 Jun 2021 00:53:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Jun 2021 00:53:09 GMT
CMD ["influxd"]
# Wed, 16 Jun 2021 00:53:09 GMT
EXPOSE 8086
# Wed, 16 Jun 2021 00:53:09 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 16 Jun 2021 00:53:10 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 16 Jun 2021 00:53:10 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe30e69de6b45dfd810d5a55e1bca8f29e9400e80960f59b78b1b708d4870ce`  
		Last Modified: Wed, 16 Jun 2021 00:53:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db672e7bc210adf1e3b27670230d2aff87b3f7a7010d104a76386659263199a`  
		Last Modified: Wed, 16 Jun 2021 00:53:50 GMT  
		Size: 9.5 MB (9541646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bdc8b41c00d800f0b805f5e77f19a84e2ed27590d2bd4c4c6bd5f0acd42696`  
		Last Modified: Wed, 16 Jun 2021 00:53:48 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa53e1ed7ae59baa7209d2ea5fc38c68534e7c0874e5049a328d5773fa5fd52`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 896.1 KB (896102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363de3b3909450074472d83e29bdc1ed5bae16c0c7b418d2a6dd3a2fc7a6c4b9`  
		Last Modified: Wed, 16 Jun 2021 00:54:01 GMT  
		Size: 112.8 MB (112824492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5833ddaacbfb7d8dc60578a7fde752675eb2fe1afd84df0aa0e6f79376420237`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b25df44481a6e552072d4a95867ba255251639aaf14ce4541b3556623c8f87`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1e1ceabc2f222ffe7be59784f0bfe551e8e322ebe7c1b40967cfb50bb2f30c`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 4.3 KB (4314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.7`

```console
$ docker pull influxdb@sha256:e80fe1f239c78881571d487d4356f3ae379dbedf44f2cf8dcb2444e2c3229222
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.7` - linux; amd64

```console
$ docker pull influxdb@sha256:b50f219df32da917355b0db781150e6d0b89f149805663440a9e04c796ac13c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178697196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd6a4507399651c8d686cd4a63db7ef4312feb26e62846dc2398df2358bfbd63`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:10:17 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 12 May 2021 20:10:17 GMT
ENV GOSU_VER=1.12
# Wed, 12 May 2021 20:10:20 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 05 Jun 2021 00:31:22 GMT
ENV INFLUXDB_VERSION=2.0.7
# Sat, 05 Jun 2021 00:31:33 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 05 Jun 2021 00:31:35 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 05 Jun 2021 00:31:35 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 05 Jun 2021 00:31:35 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 05 Jun 2021 00:31:35 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Sat, 05 Jun 2021 00:31:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Jun 2021 00:31:36 GMT
CMD ["influxd"]
# Sat, 05 Jun 2021 00:31:36 GMT
EXPOSE 8086
# Sat, 05 Jun 2021 00:31:36 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 05 Jun 2021 00:31:36 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 05 Jun 2021 00:31:37 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b26e21cfb07a9a6fd606a130ce8206843d702e4f616d53df1321437a01a0ac0`  
		Last Modified: Wed, 12 May 2021 20:13:23 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77b907603e396f34b2bbb8229e1a740deabeb6537f737d78db0f2452f2504e8`  
		Last Modified: Wed, 12 May 2021 20:13:20 GMT  
		Size: 961.0 KB (960988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9591ed1fb6b3d71a7c4957993349963b5bf90e1a59c9104548b9c7afc65b1a08`  
		Last Modified: Sat, 05 Jun 2021 00:32:49 GMT  
		Size: 109.5 MB (109466216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba458e8eb79c92d9d076a9758c228a52d495388a8520755dbd5869f878de262c`  
		Last Modified: Sat, 05 Jun 2021 00:32:39 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac66788c54e9775c3aef47ef263022a66b957839916cb13f5750434938853cfa`  
		Last Modified: Sat, 05 Jun 2021 00:32:39 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608813173efe22b91f20d22d9f0056154ffdf93c54dbb83c2656215808797c30`  
		Last Modified: Sat, 05 Jun 2021 00:32:39 GMT  
		Size: 4.3 KB (4314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:d9825b3d372ad663f34bf92a3ebc1b9022906062b06986a0f203c5ab8670fec1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180628536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcdad0ed3f5fbd15e87467aad894389fa02f9ecb82c2710bc7bd62d50db96409`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:24:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:24:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 18:34:17 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 23 Jun 2021 18:34:17 GMT
ENV GOSU_VER=1.12
# Wed, 23 Jun 2021 18:34:20 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 23 Jun 2021 18:34:20 GMT
ENV INFLUXDB_VERSION=2.0.7
# Wed, 23 Jun 2021 18:34:28 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 23 Jun 2021 18:34:29 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 23 Jun 2021 18:34:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 23 Jun 2021 18:34:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 23 Jun 2021 18:34:30 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Wed, 23 Jun 2021 18:34:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 18:34:30 GMT
CMD ["influxd"]
# Wed, 23 Jun 2021 18:34:30 GMT
EXPOSE 8086
# Wed, 23 Jun 2021 18:34:30 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 23 Jun 2021 18:34:31 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 23 Jun 2021 18:34:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86422c44ee005c4d5ccb0e2fa32685229207b712728cd4b8c0ef97174f079df7`  
		Last Modified: Wed, 23 Jun 2021 00:33:16 GMT  
		Size: 7.7 MB (7694715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9137877e0c26a439a8954003b21876b6059de852c839631e8cf6fda5bd36434c`  
		Last Modified: Wed, 23 Jun 2021 00:33:17 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2b86f0fed5df426869e08ab884f79326e9a310498fb9c49929e08f9ef9002b`  
		Last Modified: Wed, 23 Jun 2021 18:35:51 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f865c284b0e6b32bd1f1dd14ec1e334cbadc7d6292712190efa42f4718b8dd`  
		Last Modified: Wed, 23 Jun 2021 18:35:48 GMT  
		Size: 896.4 KB (896380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea300fef38e2d57c2657aaad371813835137c72d9f2c258e56af5006e4e5797`  
		Last Modified: Wed, 23 Jun 2021 18:36:00 GMT  
		Size: 112.8 MB (112824510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0fc3d9ce52b5368331dd5726abd82bd12ed7c3e8a23a33cdc89f2fbf64ab73`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f091d2bde4f35ffdd2cb09c6e1bdce03228e14e72564adc636b11ddf9829ce`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b9b006308f765debe388af66277c827d88a43a1cc4a90dee951af142b3d1d0`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 4.3 KB (4315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.7-alpine`

```console
$ docker pull influxdb@sha256:7630ad8caae177fe5442cce81068b944c13e2daa7ec289d6d3710b836824cd79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.7-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:9c2e3774aca3f2ee9675a1e0121836ab6b094f3ff4b2b0fae03dc2dd5c3f8378
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122946151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c5ab4e012ccdc738b8b78a3095905324f5e6e785f25dac93203a50321ca2039`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:57:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:57:47 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Wed, 14 Apr 2021 22:57:48 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 14 Apr 2021 22:57:49 GMT
ENV GOSU_VER=1.12
# Wed, 14 Apr 2021 22:57:52 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Jun 2021 00:31:40 GMT
ENV INFLUXDB_VERSION=2.0.7
# Sat, 05 Jun 2021 00:31:49 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 05 Jun 2021 00:31:50 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 05 Jun 2021 00:31:50 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 05 Jun 2021 00:31:50 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 05 Jun 2021 00:31:50 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Sat, 05 Jun 2021 00:31:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Jun 2021 00:31:51 GMT
CMD ["influxd"]
# Sat, 05 Jun 2021 00:31:51 GMT
EXPOSE 8086
# Sat, 05 Jun 2021 00:31:51 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 05 Jun 2021 00:31:51 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 05 Jun 2021 00:31:52 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70fcedbcfb9328a87e76b312a1996118fac6b73a1dea800c39df8d00207148`  
		Last Modified: Wed, 14 Apr 2021 23:01:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e50c2af4ce019b31b8f9df4781ebe41c99a903cd661ad9231e08773b029cfec`  
		Last Modified: Wed, 14 Apr 2021 23:01:05 GMT  
		Size: 9.7 MB (9701057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99cdb09e5aee3ab8869581dee7b389f6ebd9507ff9613cbc03683586b99eb96`  
		Last Modified: Wed, 14 Apr 2021 23:00:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4633d963d8e54bd89ef20119577189c164929c6451ec7be1f4cf45d26c3bb283`  
		Last Modified: Wed, 14 Apr 2021 23:00:56 GMT  
		Size: 960.6 KB (960616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8520535bd417b8e9823de3f2c784aaa5ee76600551afc6b859eeeba6f96d7687`  
		Last Modified: Sat, 05 Jun 2021 00:33:13 GMT  
		Size: 109.5 MB (109466245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c09337d0dcff42440f468734b71a602c359686958498e9880747a5ab008e47`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d17425d58200c18e5d27020d669313a6da4c073674fa9f07fa9618857b39f3`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67868fd95f4078c1eafb60e477d23b3c44ade51937a76f0854ebe16887fdd33`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 4.3 KB (4315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.7-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4eb31630932f0863ea90024beed6e95ad728eff5ff808ed860a9b6053e69e5ac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125980529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68e83b89b6cbd0d3cb85dd391739622d356bf8c255c4d79db34aaf80057183bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:52:29 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 16 Jun 2021 00:52:31 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Wed, 16 Jun 2021 00:52:32 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 16 Jun 2021 00:52:32 GMT
ENV GOSU_VER=1.12
# Wed, 16 Jun 2021 00:52:35 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Jun 2021 00:52:35 GMT
ENV INFLUXDB_VERSION=2.0.7
# Wed, 16 Jun 2021 00:53:07 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 16 Jun 2021 00:53:08 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 16 Jun 2021 00:53:08 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 16 Jun 2021 00:53:08 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 16 Jun 2021 00:53:09 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Wed, 16 Jun 2021 00:53:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Jun 2021 00:53:09 GMT
CMD ["influxd"]
# Wed, 16 Jun 2021 00:53:09 GMT
EXPOSE 8086
# Wed, 16 Jun 2021 00:53:09 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 16 Jun 2021 00:53:10 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 16 Jun 2021 00:53:10 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe30e69de6b45dfd810d5a55e1bca8f29e9400e80960f59b78b1b708d4870ce`  
		Last Modified: Wed, 16 Jun 2021 00:53:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db672e7bc210adf1e3b27670230d2aff87b3f7a7010d104a76386659263199a`  
		Last Modified: Wed, 16 Jun 2021 00:53:50 GMT  
		Size: 9.5 MB (9541646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bdc8b41c00d800f0b805f5e77f19a84e2ed27590d2bd4c4c6bd5f0acd42696`  
		Last Modified: Wed, 16 Jun 2021 00:53:48 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa53e1ed7ae59baa7209d2ea5fc38c68534e7c0874e5049a328d5773fa5fd52`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 896.1 KB (896102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363de3b3909450074472d83e29bdc1ed5bae16c0c7b418d2a6dd3a2fc7a6c4b9`  
		Last Modified: Wed, 16 Jun 2021 00:54:01 GMT  
		Size: 112.8 MB (112824492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5833ddaacbfb7d8dc60578a7fde752675eb2fe1afd84df0aa0e6f79376420237`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b25df44481a6e552072d4a95867ba255251639aaf14ce4541b3556623c8f87`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1e1ceabc2f222ffe7be59784f0bfe551e8e322ebe7c1b40967cfb50bb2f30c`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 4.3 KB (4314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:7630ad8caae177fe5442cce81068b944c13e2daa7ec289d6d3710b836824cd79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:9c2e3774aca3f2ee9675a1e0121836ab6b094f3ff4b2b0fae03dc2dd5c3f8378
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122946151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c5ab4e012ccdc738b8b78a3095905324f5e6e785f25dac93203a50321ca2039`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:57:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:57:47 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Wed, 14 Apr 2021 22:57:48 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 14 Apr 2021 22:57:49 GMT
ENV GOSU_VER=1.12
# Wed, 14 Apr 2021 22:57:52 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Jun 2021 00:31:40 GMT
ENV INFLUXDB_VERSION=2.0.7
# Sat, 05 Jun 2021 00:31:49 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 05 Jun 2021 00:31:50 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 05 Jun 2021 00:31:50 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 05 Jun 2021 00:31:50 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 05 Jun 2021 00:31:50 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Sat, 05 Jun 2021 00:31:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Jun 2021 00:31:51 GMT
CMD ["influxd"]
# Sat, 05 Jun 2021 00:31:51 GMT
EXPOSE 8086
# Sat, 05 Jun 2021 00:31:51 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 05 Jun 2021 00:31:51 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 05 Jun 2021 00:31:52 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70fcedbcfb9328a87e76b312a1996118fac6b73a1dea800c39df8d00207148`  
		Last Modified: Wed, 14 Apr 2021 23:01:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e50c2af4ce019b31b8f9df4781ebe41c99a903cd661ad9231e08773b029cfec`  
		Last Modified: Wed, 14 Apr 2021 23:01:05 GMT  
		Size: 9.7 MB (9701057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99cdb09e5aee3ab8869581dee7b389f6ebd9507ff9613cbc03683586b99eb96`  
		Last Modified: Wed, 14 Apr 2021 23:00:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4633d963d8e54bd89ef20119577189c164929c6451ec7be1f4cf45d26c3bb283`  
		Last Modified: Wed, 14 Apr 2021 23:00:56 GMT  
		Size: 960.6 KB (960616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8520535bd417b8e9823de3f2c784aaa5ee76600551afc6b859eeeba6f96d7687`  
		Last Modified: Sat, 05 Jun 2021 00:33:13 GMT  
		Size: 109.5 MB (109466245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c09337d0dcff42440f468734b71a602c359686958498e9880747a5ab008e47`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d17425d58200c18e5d27020d669313a6da4c073674fa9f07fa9618857b39f3`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67868fd95f4078c1eafb60e477d23b3c44ade51937a76f0854ebe16887fdd33`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 4.3 KB (4315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4eb31630932f0863ea90024beed6e95ad728eff5ff808ed860a9b6053e69e5ac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125980529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68e83b89b6cbd0d3cb85dd391739622d356bf8c255c4d79db34aaf80057183bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:52:29 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 16 Jun 2021 00:52:31 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Wed, 16 Jun 2021 00:52:32 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 16 Jun 2021 00:52:32 GMT
ENV GOSU_VER=1.12
# Wed, 16 Jun 2021 00:52:35 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Jun 2021 00:52:35 GMT
ENV INFLUXDB_VERSION=2.0.7
# Wed, 16 Jun 2021 00:53:07 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 16 Jun 2021 00:53:08 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 16 Jun 2021 00:53:08 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 16 Jun 2021 00:53:08 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 16 Jun 2021 00:53:09 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Wed, 16 Jun 2021 00:53:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Jun 2021 00:53:09 GMT
CMD ["influxd"]
# Wed, 16 Jun 2021 00:53:09 GMT
EXPOSE 8086
# Wed, 16 Jun 2021 00:53:09 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 16 Jun 2021 00:53:10 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 16 Jun 2021 00:53:10 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe30e69de6b45dfd810d5a55e1bca8f29e9400e80960f59b78b1b708d4870ce`  
		Last Modified: Wed, 16 Jun 2021 00:53:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db672e7bc210adf1e3b27670230d2aff87b3f7a7010d104a76386659263199a`  
		Last Modified: Wed, 16 Jun 2021 00:53:50 GMT  
		Size: 9.5 MB (9541646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bdc8b41c00d800f0b805f5e77f19a84e2ed27590d2bd4c4c6bd5f0acd42696`  
		Last Modified: Wed, 16 Jun 2021 00:53:48 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa53e1ed7ae59baa7209d2ea5fc38c68534e7c0874e5049a328d5773fa5fd52`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 896.1 KB (896102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363de3b3909450074472d83e29bdc1ed5bae16c0c7b418d2a6dd3a2fc7a6c4b9`  
		Last Modified: Wed, 16 Jun 2021 00:54:01 GMT  
		Size: 112.8 MB (112824492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5833ddaacbfb7d8dc60578a7fde752675eb2fe1afd84df0aa0e6f79376420237`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b25df44481a6e552072d4a95867ba255251639aaf14ce4541b3556623c8f87`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1e1ceabc2f222ffe7be59784f0bfe551e8e322ebe7c1b40967cfb50bb2f30c`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 4.3 KB (4314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data`

```console
$ docker pull influxdb@sha256:3ab29570c11851024e562dd3b17f3652040145c59e3bb3a16d57447740de1a4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:526e7102df9bedfd31b6cbcbfdc3ae31884f31e0d0c9ca2ef48f3cc84d85ec5f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127796276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:190b6b4a1f8faf9284e3d3e6b8c651e3b1caaf159587514aa07b2f50445ec473`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:08:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Mon, 24 May 2021 19:21:03 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Mon, 24 May 2021 19:21:11 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 24 May 2021 19:21:11 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 24 May 2021 19:21:12 GMT
EXPOSE 8086
# Mon, 24 May 2021 19:21:12 GMT
VOLUME [/var/lib/influxdb]
# Mon, 24 May 2021 19:21:12 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 24 May 2021 19:21:12 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 24 May 2021 19:21:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 May 2021 19:21:13 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee65a07cb0cad7eedb6332aad83a593a46bbae0a453842817353e2cf9de28d`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2773a7a98d7cff7012b04a6fd405bb45f072ce0f9984263ab559154b982cae`  
		Last Modified: Mon, 24 May 2021 19:23:18 GMT  
		Size: 66.8 MB (66782700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf345410be519d9f0751067be899e03bd987eac20a1ba875a2cd2748cdca3b4d`  
		Last Modified: Mon, 24 May 2021 19:23:10 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774ea1a99f05b930aa9e1fcc7138edd601a2c935b1c99d716b8543d7d1b706bb`  
		Last Modified: Mon, 24 May 2021 19:23:09 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33f603323ad9cb59df3614505a398877ea36e531cacd3268f881b929cc2ebe3`  
		Last Modified: Mon, 24 May 2021 19:23:10 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data-alpine`

```console
$ docker pull influxdb@sha256:3de2a6289300d1be88487af5fd2abacad7ca9ff2ec3d7353cfcbca129af892eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ef00d61d767fa488b5bfd38dd80c5269c5eddf8574dcddb9c02bb947573ce03e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70748316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c8a165e3b520020729746e784c1eb6041a4716205c5f5a4f4396ebf9e750b76`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 24 May 2021 19:21:17 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Mon, 24 May 2021 19:21:25 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 24 May 2021 19:21:26 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 24 May 2021 19:21:26 GMT
EXPOSE 8086
# Mon, 24 May 2021 19:21:26 GMT
VOLUME [/var/lib/influxdb]
# Mon, 24 May 2021 19:21:26 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 24 May 2021 19:21:27 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 24 May 2021 19:21:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 May 2021 19:21:27 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635793f5b48306dcab955aff9084c73aa36b911d9ecdd80fc6c0bda504313d8d`  
		Last Modified: Mon, 24 May 2021 19:23:42 GMT  
		Size: 66.5 MB (66515016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd3ce0e1057e72d11c9f915b709ac9b00f75c90f4288978eeb3d51857cae3a`  
		Last Modified: Mon, 24 May 2021 19:23:32 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2506c8ad21fbee3890d94e936ba78d5b9eb0691df595e6755694986231fc54`  
		Last Modified: Mon, 24 May 2021 19:23:33 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4d3e6c0b28abb9f6508c063df0648c3ee25886596d7a6157cae6adeb4767bf`  
		Last Modified: Mon, 24 May 2021 19:23:33 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:latest`

```console
$ docker pull influxdb@sha256:e80fe1f239c78881571d487d4356f3ae379dbedf44f2cf8dcb2444e2c3229222
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:b50f219df32da917355b0db781150e6d0b89f149805663440a9e04c796ac13c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178697196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd6a4507399651c8d686cd4a63db7ef4312feb26e62846dc2398df2358bfbd63`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:10:17 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 12 May 2021 20:10:17 GMT
ENV GOSU_VER=1.12
# Wed, 12 May 2021 20:10:20 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 05 Jun 2021 00:31:22 GMT
ENV INFLUXDB_VERSION=2.0.7
# Sat, 05 Jun 2021 00:31:33 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 05 Jun 2021 00:31:35 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 05 Jun 2021 00:31:35 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 05 Jun 2021 00:31:35 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 05 Jun 2021 00:31:35 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Sat, 05 Jun 2021 00:31:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Jun 2021 00:31:36 GMT
CMD ["influxd"]
# Sat, 05 Jun 2021 00:31:36 GMT
EXPOSE 8086
# Sat, 05 Jun 2021 00:31:36 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 05 Jun 2021 00:31:36 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 05 Jun 2021 00:31:37 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b26e21cfb07a9a6fd606a130ce8206843d702e4f616d53df1321437a01a0ac0`  
		Last Modified: Wed, 12 May 2021 20:13:23 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77b907603e396f34b2bbb8229e1a740deabeb6537f737d78db0f2452f2504e8`  
		Last Modified: Wed, 12 May 2021 20:13:20 GMT  
		Size: 961.0 KB (960988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9591ed1fb6b3d71a7c4957993349963b5bf90e1a59c9104548b9c7afc65b1a08`  
		Last Modified: Sat, 05 Jun 2021 00:32:49 GMT  
		Size: 109.5 MB (109466216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba458e8eb79c92d9d076a9758c228a52d495388a8520755dbd5869f878de262c`  
		Last Modified: Sat, 05 Jun 2021 00:32:39 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac66788c54e9775c3aef47ef263022a66b957839916cb13f5750434938853cfa`  
		Last Modified: Sat, 05 Jun 2021 00:32:39 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608813173efe22b91f20d22d9f0056154ffdf93c54dbb83c2656215808797c30`  
		Last Modified: Sat, 05 Jun 2021 00:32:39 GMT  
		Size: 4.3 KB (4314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:d9825b3d372ad663f34bf92a3ebc1b9022906062b06986a0f203c5ab8670fec1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180628536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcdad0ed3f5fbd15e87467aad894389fa02f9ecb82c2710bc7bd62d50db96409`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:24:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:24:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 18:34:17 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 23 Jun 2021 18:34:17 GMT
ENV GOSU_VER=1.12
# Wed, 23 Jun 2021 18:34:20 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 23 Jun 2021 18:34:20 GMT
ENV INFLUXDB_VERSION=2.0.7
# Wed, 23 Jun 2021 18:34:28 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 23 Jun 2021 18:34:29 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 23 Jun 2021 18:34:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 23 Jun 2021 18:34:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 23 Jun 2021 18:34:30 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Wed, 23 Jun 2021 18:34:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 18:34:30 GMT
CMD ["influxd"]
# Wed, 23 Jun 2021 18:34:30 GMT
EXPOSE 8086
# Wed, 23 Jun 2021 18:34:30 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 23 Jun 2021 18:34:31 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 23 Jun 2021 18:34:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86422c44ee005c4d5ccb0e2fa32685229207b712728cd4b8c0ef97174f079df7`  
		Last Modified: Wed, 23 Jun 2021 00:33:16 GMT  
		Size: 7.7 MB (7694715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9137877e0c26a439a8954003b21876b6059de852c839631e8cf6fda5bd36434c`  
		Last Modified: Wed, 23 Jun 2021 00:33:17 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2b86f0fed5df426869e08ab884f79326e9a310498fb9c49929e08f9ef9002b`  
		Last Modified: Wed, 23 Jun 2021 18:35:51 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f865c284b0e6b32bd1f1dd14ec1e334cbadc7d6292712190efa42f4718b8dd`  
		Last Modified: Wed, 23 Jun 2021 18:35:48 GMT  
		Size: 896.4 KB (896380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea300fef38e2d57c2657aaad371813835137c72d9f2c258e56af5006e4e5797`  
		Last Modified: Wed, 23 Jun 2021 18:36:00 GMT  
		Size: 112.8 MB (112824510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0fc3d9ce52b5368331dd5726abd82bd12ed7c3e8a23a33cdc89f2fbf64ab73`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f091d2bde4f35ffdd2cb09c6e1bdce03228e14e72564adc636b11ddf9829ce`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b9b006308f765debe388af66277c827d88a43a1cc4a90dee951af142b3d1d0`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 4.3 KB (4315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:cfb5b01b5f8055f85824b84d2cbd92861af0fe230f2e5462c4aaa7d20e931f16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:e90ef2d58ad2113dcecbfdab6b0f62d435218e530bd358984b7181ed9f49e2bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84218334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8afaed1241b57683e2cc0bc2eb77fd3da57e14330cb69a0a935b56a2ee013321`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:08:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Mon, 24 May 2021 19:21:03 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Mon, 24 May 2021 19:21:34 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 24 May 2021 19:21:35 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 24 May 2021 19:21:35 GMT
EXPOSE 8091
# Mon, 24 May 2021 19:21:35 GMT
VOLUME [/var/lib/influxdb]
# Mon, 24 May 2021 19:21:35 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 24 May 2021 19:21:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 May 2021 19:21:36 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee65a07cb0cad7eedb6332aad83a593a46bbae0a453842817353e2cf9de28d`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df73b02e0adbf70adff8d7415e4e195b974a97b32c83a5dcbc8cf2314985fc5b`  
		Last Modified: Mon, 24 May 2021 19:23:57 GMT  
		Size: 23.2 MB (23205961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c59be4dda832c46c462ef85cacad8d242061f7e886398ac7f17668e5a880ba`  
		Last Modified: Mon, 24 May 2021 19:23:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1750d7e819bc72c58d2e341fd3a97759cf4f176db42e26e189273733c18b29d`  
		Last Modified: Mon, 24 May 2021 19:23:54 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta-alpine`

```console
$ docker pull influxdb@sha256:c5781a2ad82e23ecb77997b22d22a0f40b2d200e1d47bc9679bc5e6d5cef19a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:4adaa9b434a9cdeaf97111df8bc113633453db727ccc7623bf0a0d6f41b5646d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27306919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ba1ee0645cd12155610113100bb0564d95b9367c4ce88a91a77251d09568b7c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 24 May 2021 19:21:17 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Mon, 24 May 2021 19:21:43 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 24 May 2021 19:21:44 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 24 May 2021 19:21:44 GMT
EXPOSE 8091
# Mon, 24 May 2021 19:21:44 GMT
VOLUME [/var/lib/influxdb]
# Mon, 24 May 2021 19:21:44 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 24 May 2021 19:21:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 May 2021 19:21:45 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a0d200db7e6e767fb2b050a82e962f822da4d61122122a1d905d82be300dbe`  
		Last Modified: Mon, 24 May 2021 19:24:13 GMT  
		Size: 23.1 MB (23074821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084943cc8c5278875e6be6fd518a250ea14d19d4f4bb3174c8aa6f1db7521ae3`  
		Last Modified: Mon, 24 May 2021 19:24:10 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2187653745d63baa53dc6c0cd4cb5f83bd6c9c3f9fd92e4727a0394e09a5f5bf`  
		Last Modified: Mon, 24 May 2021 19:24:10 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
