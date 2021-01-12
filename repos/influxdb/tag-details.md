<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `influxdb`

-	[`influxdb:1.7`](#influxdb17)
-	[`influxdb:1.7.10`](#influxdb1710)
-	[`influxdb:1.7.10-alpine`](#influxdb1710-alpine)
-	[`influxdb:1.7.10-data`](#influxdb1710-data)
-	[`influxdb:1.7.10-data-alpine`](#influxdb1710-data-alpine)
-	[`influxdb:1.7.10-meta`](#influxdb1710-meta)
-	[`influxdb:1.7.10-meta-alpine`](#influxdb1710-meta-alpine)
-	[`influxdb:1.7-alpine`](#influxdb17-alpine)
-	[`influxdb:1.7-data`](#influxdb17-data)
-	[`influxdb:1.7-data-alpine`](#influxdb17-data-alpine)
-	[`influxdb:1.7-meta`](#influxdb17-meta)
-	[`influxdb:1.7-meta-alpine`](#influxdb17-meta-alpine)
-	[`influxdb:1.8`](#influxdb18)
-	[`influxdb:1.8.3`](#influxdb183)
-	[`influxdb:1.8.3-alpine`](#influxdb183-alpine)
-	[`influxdb:1.8.3-data`](#influxdb183-data)
-	[`influxdb:1.8.3-data-alpine`](#influxdb183-data-alpine)
-	[`influxdb:1.8.3-meta`](#influxdb183-meta)
-	[`influxdb:1.8.3-meta-alpine`](#influxdb183-meta-alpine)
-	[`influxdb:1.8-alpine`](#influxdb18-alpine)
-	[`influxdb:1.8-data`](#influxdb18-data)
-	[`influxdb:1.8-data-alpine`](#influxdb18-data-alpine)
-	[`influxdb:1.8-meta`](#influxdb18-meta)
-	[`influxdb:1.8-meta-alpine`](#influxdb18-meta-alpine)
-	[`influxdb:alpine`](#influxdbalpine)
-	[`influxdb:data`](#influxdbdata)
-	[`influxdb:data-alpine`](#influxdbdata-alpine)
-	[`influxdb:latest`](#influxdblatest)
-	[`influxdb:meta`](#influxdbmeta)
-	[`influxdb:meta-alpine`](#influxdbmeta-alpine)

## `influxdb:1.7`

```console
$ docker pull influxdb@sha256:fa3b37c1b08392c1496d577f2fb3e9d218ad8ef720c2ce5268ba2b82edb24489
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7` - linux; amd64

```console
$ docker pull influxdb@sha256:d77847fb924bbefed25deb8a68b70c4afb6e630e71214c553b22b30fbcabd748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124572545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4961ecf8c6fd31017f050d2156d5fbbb36c04b2b689652e8d75bf4bb5068daa7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 17:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 17:01:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 02:42:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 18 Dec 2020 02:42:38 GMT
ENV INFLUXDB_VERSION=1.7.10
# Fri, 18 Dec 2020 02:42:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 18 Dec 2020 02:42:44 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 18 Dec 2020 02:42:44 GMT
EXPOSE 8086
# Fri, 18 Dec 2020 02:42:45 GMT
VOLUME [/var/lib/influxdb]
# Fri, 18 Dec 2020 02:42:45 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 18 Dec 2020 02:42:45 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 18 Dec 2020 02:42:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Dec 2020 02:42:45 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072739d44e4fe2316d3bda5b6e0944796b1824cb2dee521ef06bf11e4f5db0fe`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 10.8 MB (10752737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5111f27e9600a1fa0a3a8660e8518294729a41abcd648bbf0ec9f60dcfb02b73`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 4.3 MB (4340690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8edcaa1ed5e299a41dda2ec21e02bcffc9984be150078569bf9537b855e2f`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b70972a5fd4e4a0bde1b5202f336f542093e98cb568db6852f308634f43c79`  
		Last Modified: Fri, 18 Dec 2020 02:44:49 GMT  
		Size: 64.1 MB (64096968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b648f8b79e2fa0303fdebe324471a3171c4f67fe655c8d5cb241a0afc8a386a4`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea3c1edbc61e5f9b83d99275e12d7f136951c7a4d7cabafd2dd49ecf08c3f05`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b574f8b4de22bd3f4cc0249d82b7a60cc64e91b11aab3849220ec5144821b95e`  
		Last Modified: Fri, 18 Dec 2020 02:44:37 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:373b4abf2625eb55fedf8e0044da07fa6d1641158089b2d90370abfa3534d0a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.1 MB (116126235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:760c5db290ae58a35faa0f19670cc7833722d87596520bd472491567f7664c2a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:19 GMT
ADD file:9c744a203d36aa8c515bbc11873a4a479cdf3fe9f020ca1ef207b53e6b3a251e in / 
# Tue, 12 Jan 2021 00:05:23 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:21:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 17:20:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 17:20:19 GMT
ENV INFLUXDB_VERSION=1.7.10
# Tue, 12 Jan 2021 17:20:31 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 12 Jan 2021 17:20:32 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 12 Jan 2021 17:20:33 GMT
EXPOSE 8086
# Tue, 12 Jan 2021 17:20:33 GMT
VOLUME [/var/lib/influxdb]
# Tue, 12 Jan 2021 17:20:34 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 12 Jan 2021 17:20:35 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 12 Jan 2021 17:20:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 17:20:36 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f5de2649c1cd9091872f81b8ceb6a67890124f113d9fce9c52bf60d5a6e19f43`  
		Last Modified: Tue, 12 Jan 2021 00:15:23 GMT  
		Size: 42.1 MB (42119951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cae60aac6e598935e2b14216dc4265434ba03d17c82f622b18abb712577d2c`  
		Last Modified: Tue, 12 Jan 2021 01:34:01 GMT  
		Size: 9.4 MB (9446203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9694e28a75917ff08caeaee5ed8729a2f12d2110bf203781d578006a0ef2f7`  
		Last Modified: Tue, 12 Jan 2021 01:33:59 GMT  
		Size: 3.9 MB (3919958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9af4291e32292c1b3e0baa3521c9903226273223480ec660c81d82cec54e2b`  
		Last Modified: Tue, 12 Jan 2021 17:21:15 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1fe691cbf6d58c61c06b4b154037abf1c59528fbcd06edb0b8647fbaa480bf`  
		Last Modified: Tue, 12 Jan 2021 17:21:38 GMT  
		Size: 60.6 MB (60635552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7d2fe33bfbd793722159f43468b29fefa606ca3266c9d4d1441ba7970a71fe`  
		Last Modified: Tue, 12 Jan 2021 17:21:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b086b775b90d6b7f96f199d301aa3ed95cfa9a29949b3b64f2ea0d7e7bff2e3`  
		Last Modified: Tue, 12 Jan 2021 17:21:15 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ebd71ed5826cf3773c334df649adfd2a23033924953f406da52aa762533ba4`  
		Last Modified: Tue, 12 Jan 2021 17:21:15 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:d6d11517e7235585eff40bf4b69b6dcc52fd9ba093f654cadfa32f77eb18f19c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.1 MB (117106672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0282426d0ee6b4914cf033416b66e6bbbb06fdd7b257382df33339d6123683e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 11 Dec 2020 02:48:16 GMT
ADD file:48e44714f486662ed380343e556f0f7411bd6600d916440063753c55d1f94b45 in / 
# Fri, 11 Dec 2020 02:48:17 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 10:13:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 10:13:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 15:25:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 17 Dec 2020 15:25:55 GMT
ENV INFLUXDB_VERSION=1.7.10
# Thu, 17 Dec 2020 15:26:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 17 Dec 2020 15:26:17 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 17 Dec 2020 15:26:28 GMT
EXPOSE 8086
# Thu, 17 Dec 2020 15:26:36 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 15:26:36 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 17 Dec 2020 15:26:38 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Dec 2020 15:26:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 15:26:43 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:ecefb91918e846819df74a1beb8e41f454bef156738373818c20656a3a46d5f7`  
		Last Modified: Fri, 11 Dec 2020 02:55:36 GMT  
		Size: 43.2 MB (43175941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda9a63f37e7beb33012f80c0f66755ce6d87a51fde0a283a06dbdf2857ce533`  
		Last Modified: Thu, 17 Dec 2020 10:41:45 GMT  
		Size: 9.7 MB (9702906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0c493446fd68c6abee0df0169e849bcb73aa61a86ba5e30783c9b5298007b7`  
		Last Modified: Thu, 17 Dec 2020 10:41:43 GMT  
		Size: 4.1 MB (4095483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a00a8a57199af4c15740e382214257dc71414c8a40b544ffcd0d9f53ce2404c`  
		Last Modified: Thu, 17 Dec 2020 15:27:23 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d88dd8ced803e32c54afaa6262ab6169811fc45acb4b5e968cbdac3cf0bce9`  
		Last Modified: Thu, 17 Dec 2020 15:27:37 GMT  
		Size: 60.1 MB (60127768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07894f945b444bbf8ee411e2392a8dbe778491d1d778b7441035737d6802675`  
		Last Modified: Thu, 17 Dec 2020 15:27:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f51f444571a0f64dba2812230df34a24b62e4233f4a7fae5c9e73d3684d6aa6`  
		Last Modified: Thu, 17 Dec 2020 15:27:24 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da68ae98baa462fb810d05bc890fdadc71895cbdae37fdf8874452d7c1907cb`  
		Last Modified: Thu, 17 Dec 2020 15:27:23 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.10`

```console
$ docker pull influxdb@sha256:fa3b37c1b08392c1496d577f2fb3e9d218ad8ef720c2ce5268ba2b82edb24489
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7.10` - linux; amd64

```console
$ docker pull influxdb@sha256:d77847fb924bbefed25deb8a68b70c4afb6e630e71214c553b22b30fbcabd748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124572545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4961ecf8c6fd31017f050d2156d5fbbb36c04b2b689652e8d75bf4bb5068daa7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 17:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 17:01:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 02:42:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 18 Dec 2020 02:42:38 GMT
ENV INFLUXDB_VERSION=1.7.10
# Fri, 18 Dec 2020 02:42:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 18 Dec 2020 02:42:44 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 18 Dec 2020 02:42:44 GMT
EXPOSE 8086
# Fri, 18 Dec 2020 02:42:45 GMT
VOLUME [/var/lib/influxdb]
# Fri, 18 Dec 2020 02:42:45 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 18 Dec 2020 02:42:45 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 18 Dec 2020 02:42:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Dec 2020 02:42:45 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072739d44e4fe2316d3bda5b6e0944796b1824cb2dee521ef06bf11e4f5db0fe`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 10.8 MB (10752737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5111f27e9600a1fa0a3a8660e8518294729a41abcd648bbf0ec9f60dcfb02b73`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 4.3 MB (4340690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8edcaa1ed5e299a41dda2ec21e02bcffc9984be150078569bf9537b855e2f`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b70972a5fd4e4a0bde1b5202f336f542093e98cb568db6852f308634f43c79`  
		Last Modified: Fri, 18 Dec 2020 02:44:49 GMT  
		Size: 64.1 MB (64096968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b648f8b79e2fa0303fdebe324471a3171c4f67fe655c8d5cb241a0afc8a386a4`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea3c1edbc61e5f9b83d99275e12d7f136951c7a4d7cabafd2dd49ecf08c3f05`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b574f8b4de22bd3f4cc0249d82b7a60cc64e91b11aab3849220ec5144821b95e`  
		Last Modified: Fri, 18 Dec 2020 02:44:37 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:373b4abf2625eb55fedf8e0044da07fa6d1641158089b2d90370abfa3534d0a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.1 MB (116126235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:760c5db290ae58a35faa0f19670cc7833722d87596520bd472491567f7664c2a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:19 GMT
ADD file:9c744a203d36aa8c515bbc11873a4a479cdf3fe9f020ca1ef207b53e6b3a251e in / 
# Tue, 12 Jan 2021 00:05:23 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:21:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 17:20:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 17:20:19 GMT
ENV INFLUXDB_VERSION=1.7.10
# Tue, 12 Jan 2021 17:20:31 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 12 Jan 2021 17:20:32 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 12 Jan 2021 17:20:33 GMT
EXPOSE 8086
# Tue, 12 Jan 2021 17:20:33 GMT
VOLUME [/var/lib/influxdb]
# Tue, 12 Jan 2021 17:20:34 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 12 Jan 2021 17:20:35 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 12 Jan 2021 17:20:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 17:20:36 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f5de2649c1cd9091872f81b8ceb6a67890124f113d9fce9c52bf60d5a6e19f43`  
		Last Modified: Tue, 12 Jan 2021 00:15:23 GMT  
		Size: 42.1 MB (42119951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cae60aac6e598935e2b14216dc4265434ba03d17c82f622b18abb712577d2c`  
		Last Modified: Tue, 12 Jan 2021 01:34:01 GMT  
		Size: 9.4 MB (9446203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9694e28a75917ff08caeaee5ed8729a2f12d2110bf203781d578006a0ef2f7`  
		Last Modified: Tue, 12 Jan 2021 01:33:59 GMT  
		Size: 3.9 MB (3919958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9af4291e32292c1b3e0baa3521c9903226273223480ec660c81d82cec54e2b`  
		Last Modified: Tue, 12 Jan 2021 17:21:15 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1fe691cbf6d58c61c06b4b154037abf1c59528fbcd06edb0b8647fbaa480bf`  
		Last Modified: Tue, 12 Jan 2021 17:21:38 GMT  
		Size: 60.6 MB (60635552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7d2fe33bfbd793722159f43468b29fefa606ca3266c9d4d1441ba7970a71fe`  
		Last Modified: Tue, 12 Jan 2021 17:21:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b086b775b90d6b7f96f199d301aa3ed95cfa9a29949b3b64f2ea0d7e7bff2e3`  
		Last Modified: Tue, 12 Jan 2021 17:21:15 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ebd71ed5826cf3773c334df649adfd2a23033924953f406da52aa762533ba4`  
		Last Modified: Tue, 12 Jan 2021 17:21:15 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:d6d11517e7235585eff40bf4b69b6dcc52fd9ba093f654cadfa32f77eb18f19c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.1 MB (117106672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0282426d0ee6b4914cf033416b66e6bbbb06fdd7b257382df33339d6123683e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 11 Dec 2020 02:48:16 GMT
ADD file:48e44714f486662ed380343e556f0f7411bd6600d916440063753c55d1f94b45 in / 
# Fri, 11 Dec 2020 02:48:17 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 10:13:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 10:13:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 15:25:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 17 Dec 2020 15:25:55 GMT
ENV INFLUXDB_VERSION=1.7.10
# Thu, 17 Dec 2020 15:26:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 17 Dec 2020 15:26:17 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 17 Dec 2020 15:26:28 GMT
EXPOSE 8086
# Thu, 17 Dec 2020 15:26:36 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 15:26:36 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 17 Dec 2020 15:26:38 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Dec 2020 15:26:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 15:26:43 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:ecefb91918e846819df74a1beb8e41f454bef156738373818c20656a3a46d5f7`  
		Last Modified: Fri, 11 Dec 2020 02:55:36 GMT  
		Size: 43.2 MB (43175941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda9a63f37e7beb33012f80c0f66755ce6d87a51fde0a283a06dbdf2857ce533`  
		Last Modified: Thu, 17 Dec 2020 10:41:45 GMT  
		Size: 9.7 MB (9702906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0c493446fd68c6abee0df0169e849bcb73aa61a86ba5e30783c9b5298007b7`  
		Last Modified: Thu, 17 Dec 2020 10:41:43 GMT  
		Size: 4.1 MB (4095483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a00a8a57199af4c15740e382214257dc71414c8a40b544ffcd0d9f53ce2404c`  
		Last Modified: Thu, 17 Dec 2020 15:27:23 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d88dd8ced803e32c54afaa6262ab6169811fc45acb4b5e968cbdac3cf0bce9`  
		Last Modified: Thu, 17 Dec 2020 15:27:37 GMT  
		Size: 60.1 MB (60127768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07894f945b444bbf8ee411e2392a8dbe778491d1d778b7441035737d6802675`  
		Last Modified: Thu, 17 Dec 2020 15:27:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f51f444571a0f64dba2812230df34a24b62e4233f4a7fae5c9e73d3684d6aa6`  
		Last Modified: Thu, 17 Dec 2020 15:27:24 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da68ae98baa462fb810d05bc890fdadc71895cbdae37fdf8874452d7c1907cb`  
		Last Modified: Thu, 17 Dec 2020 15:27:23 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.10-alpine`

```console
$ docker pull influxdb@sha256:775e645de86f5fa045d5f2395c2ca79ec4816d635edb3a3eb3d48b3b0e78d4ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.10-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:d51c6106662f02e811faf97bcef6a2a6913a0ef3d676b776f00e1afbcafc513c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68070188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:946ee76bbc80ab07f2bc3dbb5934eb7c4de7f58024d5ac5cdf9e3dca8b888130`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:47:22 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:47:22 GMT
ENV INFLUXDB_VERSION=1.7.10
# Thu, 17 Dec 2020 13:47:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:47:30 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 17 Dec 2020 13:47:31 GMT
EXPOSE 8086
# Thu, 17 Dec 2020 13:47:31 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 13:47:31 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:47:31 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Dec 2020 13:47:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:47:32 GMT
CMD ["influxd"]
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
	-	`sha256:1924738bc6407d8319fdb7d3fca610b5972213dee7ad608f4d801b3990f11a21`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 1.4 MB (1428296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511d29ff60a150f0c897cbabbca1e1db59493a51bb5991ff7e87be68d032a2d9`  
		Last Modified: Thu, 17 Dec 2020 13:49:46 GMT  
		Size: 63.8 MB (63840959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5de96d55cbf03bad33a1be3c6ce83dff929a7ebef24ac93154aabbb30674490`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f599f84c2c5eb886cceb5fb9d190dac3a4bca360f7085bdb97c83dfadbebbc6b`  
		Last Modified: Thu, 17 Dec 2020 13:49:34 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9945b200342d04735e6160898c3882898c4a1570b22b27157d72854b8d566e68`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.10-data`

```console
$ docker pull influxdb@sha256:e3a09474bca0f0e914b72aeec8a49278f7ee3779519a4700f70bea5b3875eca7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:6584e35b0dda8c3ad4299cac53e72a5d36bcc30d9fd01f18f4690a8eb16b86e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.4 MB (148387967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37c94e5fcd3877b596e75b4e56121cea14e0ef3f1b2dff51425c2efe203966e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 17:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 17:01:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 02:42:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 18 Dec 2020 02:42:54 GMT
ENV INFLUXDB_VERSION=1.7.10-c1.7.10
# Fri, 18 Dec 2020 02:43:03 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 18 Dec 2020 02:43:03 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 18 Dec 2020 02:43:03 GMT
EXPOSE 8086
# Fri, 18 Dec 2020 02:43:03 GMT
VOLUME [/var/lib/influxdb]
# Fri, 18 Dec 2020 02:43:03 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 18 Dec 2020 02:43:04 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 18 Dec 2020 02:43:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Dec 2020 02:43:04 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072739d44e4fe2316d3bda5b6e0944796b1824cb2dee521ef06bf11e4f5db0fe`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 10.8 MB (10752737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5111f27e9600a1fa0a3a8660e8518294729a41abcd648bbf0ec9f60dcfb02b73`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 4.3 MB (4340690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8edcaa1ed5e299a41dda2ec21e02bcffc9984be150078569bf9537b855e2f`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92638418a20efb974a62e8eda469df911c434b189fca40bf441f2a00365f903e`  
		Last Modified: Fri, 18 Dec 2020 02:45:10 GMT  
		Size: 87.9 MB (87912333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdbbb2913df668846827d723c0c446523c9a33a381f242d5952bf78108e8d39`  
		Last Modified: Fri, 18 Dec 2020 02:44:57 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c72fa2dec2177c27fc7352ac5eb91006c4241ae38313361254205f50fff94f7`  
		Last Modified: Fri, 18 Dec 2020 02:44:57 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b97339beb7cc625779908640a191270b5acd6e2a3df85499424c973e8c5624`  
		Last Modified: Fri, 18 Dec 2020 02:44:56 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.10-data-alpine`

```console
$ docker pull influxdb@sha256:2b8174c4527c4344779a259b65f1e994d610c22e48d0e9ef08159fa1879db538
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.10-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:1aada19288a09e51e979d64d825416c9c4019a5d54a73d1d86ecd92b5ed4d936
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.8 MB (91833013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e846d9cdf372741355f7ff7a345adc7bf12038650298d2d65eada44bd6b1597`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:47:22 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:47:40 GMT
ENV INFLUXDB_VERSION=1.7.10-c1.7.10
# Thu, 17 Dec 2020 13:47:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:47:50 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 17 Dec 2020 13:47:50 GMT
EXPOSE 8086
# Thu, 17 Dec 2020 13:47:51 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 13:47:51 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:47:51 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Dec 2020 13:47:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:47:52 GMT
CMD ["influxd"]
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
	-	`sha256:1924738bc6407d8319fdb7d3fca610b5972213dee7ad608f4d801b3990f11a21`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 1.4 MB (1428296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65dd6e6ca392bfd9c0443ca825222f9caa722e13a8d0f97181d82b9336666f56`  
		Last Modified: Thu, 17 Dec 2020 13:50:09 GMT  
		Size: 87.6 MB (87603725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd248e147bc17ad4584e1373ca1406b31caca773d6cabe1c3f05ef36410cb66`  
		Last Modified: Thu, 17 Dec 2020 13:49:53 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79190b655b57c228c95a7fa6fdc71fe5db4a4fb3ee6d015ad3e521a7da7d3844`  
		Last Modified: Thu, 17 Dec 2020 13:49:53 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc067c0916f35d8ae60aa3959d71eb5903c389839000e351a4c184ff39585f2`  
		Last Modified: Thu, 17 Dec 2020 13:49:54 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.10-meta`

```console
$ docker pull influxdb@sha256:56f41362cde4a919b66d80b38920e440ce9b95038659e815cc85b789703c01b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:93fa6165faf4d0174bd3613ac7ae3ac73655cdf87388a97cf5e780211f88095b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.6 MB (83607089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f610b77dfb9465ae48c0e3209f05c0927bc7fa7aa7afebfe97ceec6dbddf52`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 17:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 17:01:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 02:42:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 18 Dec 2020 02:42:54 GMT
ENV INFLUXDB_VERSION=1.7.10-c1.7.10
# Fri, 18 Dec 2020 02:43:14 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 18 Dec 2020 02:43:15 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 18 Dec 2020 02:43:15 GMT
EXPOSE 8091
# Fri, 18 Dec 2020 02:43:15 GMT
VOLUME [/var/lib/influxdb]
# Fri, 18 Dec 2020 02:43:15 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 18 Dec 2020 02:43:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Dec 2020 02:43:16 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072739d44e4fe2316d3bda5b6e0944796b1824cb2dee521ef06bf11e4f5db0fe`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 10.8 MB (10752737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5111f27e9600a1fa0a3a8660e8518294729a41abcd648bbf0ec9f60dcfb02b73`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 4.3 MB (4340690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8edcaa1ed5e299a41dda2ec21e02bcffc9984be150078569bf9537b855e2f`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8ac203dfae9af5a917933f9fd0fd75133b08b509c0f9931c980e51db484930`  
		Last Modified: Fri, 18 Dec 2020 02:45:21 GMT  
		Size: 23.1 MB (23132660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f76e3cbf34396af02fd40002cf9410897ab417a2cf4b6c7e8a1cd983438e67`  
		Last Modified: Fri, 18 Dec 2020 02:45:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37854094312e951542a51432c0d0b9faf8ec3d4f27a5fc037dfe31e7c583373a`  
		Last Modified: Fri, 18 Dec 2020 02:45:17 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.10-meta-alpine`

```console
$ docker pull influxdb@sha256:de16392636e76e08ab574dd858057a6b975c782c8b5c0b416733e029ce25b5e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.10-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:156abf7250306d6f8dcbff15092cef2b76844b7c018d606fc6a62116e89f4f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27230754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d7485cab53b185859b0e6762551835468f6f52cc194a69b4e734ddebcf905f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:47:22 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:47:40 GMT
ENV INFLUXDB_VERSION=1.7.10-c1.7.10
# Thu, 17 Dec 2020 13:48:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:48:04 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 17 Dec 2020 13:48:04 GMT
EXPOSE 8091
# Thu, 17 Dec 2020 13:48:05 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 13:48:05 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:48:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:48:05 GMT
CMD ["influxd-meta"]
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
	-	`sha256:1924738bc6407d8319fdb7d3fca610b5972213dee7ad608f4d801b3990f11a21`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 1.4 MB (1428296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810893317995e32ec408ab5a96f97680ed29491804e058a06afc02b4f9764fe9`  
		Last Modified: Thu, 17 Dec 2020 13:50:21 GMT  
		Size: 23.0 MB (23002670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a373124bdc8b99e201610f79430294e29f7444345987bb5ca2c4042360d2f539`  
		Last Modified: Thu, 17 Dec 2020 13:50:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fcd2ae59d54ca79585f5a7888535850738abff6ce791ed0b1061ba560ffda83`  
		Last Modified: Thu, 17 Dec 2020 13:50:18 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-alpine`

```console
$ docker pull influxdb@sha256:775e645de86f5fa045d5f2395c2ca79ec4816d635edb3a3eb3d48b3b0e78d4ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:d51c6106662f02e811faf97bcef6a2a6913a0ef3d676b776f00e1afbcafc513c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68070188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:946ee76bbc80ab07f2bc3dbb5934eb7c4de7f58024d5ac5cdf9e3dca8b888130`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:47:22 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:47:22 GMT
ENV INFLUXDB_VERSION=1.7.10
# Thu, 17 Dec 2020 13:47:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:47:30 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 17 Dec 2020 13:47:31 GMT
EXPOSE 8086
# Thu, 17 Dec 2020 13:47:31 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 13:47:31 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:47:31 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Dec 2020 13:47:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:47:32 GMT
CMD ["influxd"]
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
	-	`sha256:1924738bc6407d8319fdb7d3fca610b5972213dee7ad608f4d801b3990f11a21`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 1.4 MB (1428296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511d29ff60a150f0c897cbabbca1e1db59493a51bb5991ff7e87be68d032a2d9`  
		Last Modified: Thu, 17 Dec 2020 13:49:46 GMT  
		Size: 63.8 MB (63840959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5de96d55cbf03bad33a1be3c6ce83dff929a7ebef24ac93154aabbb30674490`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f599f84c2c5eb886cceb5fb9d190dac3a4bca360f7085bdb97c83dfadbebbc6b`  
		Last Modified: Thu, 17 Dec 2020 13:49:34 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9945b200342d04735e6160898c3882898c4a1570b22b27157d72854b8d566e68`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data`

```console
$ docker pull influxdb@sha256:e3a09474bca0f0e914b72aeec8a49278f7ee3779519a4700f70bea5b3875eca7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-data` - linux; amd64

```console
$ docker pull influxdb@sha256:6584e35b0dda8c3ad4299cac53e72a5d36bcc30d9fd01f18f4690a8eb16b86e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.4 MB (148387967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37c94e5fcd3877b596e75b4e56121cea14e0ef3f1b2dff51425c2efe203966e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 17:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 17:01:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 02:42:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 18 Dec 2020 02:42:54 GMT
ENV INFLUXDB_VERSION=1.7.10-c1.7.10
# Fri, 18 Dec 2020 02:43:03 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 18 Dec 2020 02:43:03 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 18 Dec 2020 02:43:03 GMT
EXPOSE 8086
# Fri, 18 Dec 2020 02:43:03 GMT
VOLUME [/var/lib/influxdb]
# Fri, 18 Dec 2020 02:43:03 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 18 Dec 2020 02:43:04 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 18 Dec 2020 02:43:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Dec 2020 02:43:04 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072739d44e4fe2316d3bda5b6e0944796b1824cb2dee521ef06bf11e4f5db0fe`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 10.8 MB (10752737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5111f27e9600a1fa0a3a8660e8518294729a41abcd648bbf0ec9f60dcfb02b73`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 4.3 MB (4340690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8edcaa1ed5e299a41dda2ec21e02bcffc9984be150078569bf9537b855e2f`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92638418a20efb974a62e8eda469df911c434b189fca40bf441f2a00365f903e`  
		Last Modified: Fri, 18 Dec 2020 02:45:10 GMT  
		Size: 87.9 MB (87912333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdbbb2913df668846827d723c0c446523c9a33a381f242d5952bf78108e8d39`  
		Last Modified: Fri, 18 Dec 2020 02:44:57 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c72fa2dec2177c27fc7352ac5eb91006c4241ae38313361254205f50fff94f7`  
		Last Modified: Fri, 18 Dec 2020 02:44:57 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b97339beb7cc625779908640a191270b5acd6e2a3df85499424c973e8c5624`  
		Last Modified: Fri, 18 Dec 2020 02:44:56 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data-alpine`

```console
$ docker pull influxdb@sha256:2b8174c4527c4344779a259b65f1e994d610c22e48d0e9ef08159fa1879db538
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:1aada19288a09e51e979d64d825416c9c4019a5d54a73d1d86ecd92b5ed4d936
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.8 MB (91833013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e846d9cdf372741355f7ff7a345adc7bf12038650298d2d65eada44bd6b1597`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:47:22 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:47:40 GMT
ENV INFLUXDB_VERSION=1.7.10-c1.7.10
# Thu, 17 Dec 2020 13:47:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:47:50 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 17 Dec 2020 13:47:50 GMT
EXPOSE 8086
# Thu, 17 Dec 2020 13:47:51 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 13:47:51 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:47:51 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Dec 2020 13:47:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:47:52 GMT
CMD ["influxd"]
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
	-	`sha256:1924738bc6407d8319fdb7d3fca610b5972213dee7ad608f4d801b3990f11a21`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 1.4 MB (1428296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65dd6e6ca392bfd9c0443ca825222f9caa722e13a8d0f97181d82b9336666f56`  
		Last Modified: Thu, 17 Dec 2020 13:50:09 GMT  
		Size: 87.6 MB (87603725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd248e147bc17ad4584e1373ca1406b31caca773d6cabe1c3f05ef36410cb66`  
		Last Modified: Thu, 17 Dec 2020 13:49:53 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79190b655b57c228c95a7fa6fdc71fe5db4a4fb3ee6d015ad3e521a7da7d3844`  
		Last Modified: Thu, 17 Dec 2020 13:49:53 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc067c0916f35d8ae60aa3959d71eb5903c389839000e351a4c184ff39585f2`  
		Last Modified: Thu, 17 Dec 2020 13:49:54 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta`

```console
$ docker pull influxdb@sha256:56f41362cde4a919b66d80b38920e440ce9b95038659e815cc85b789703c01b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:93fa6165faf4d0174bd3613ac7ae3ac73655cdf87388a97cf5e780211f88095b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.6 MB (83607089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f610b77dfb9465ae48c0e3209f05c0927bc7fa7aa7afebfe97ceec6dbddf52`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 17:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 17:01:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 02:42:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 18 Dec 2020 02:42:54 GMT
ENV INFLUXDB_VERSION=1.7.10-c1.7.10
# Fri, 18 Dec 2020 02:43:14 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 18 Dec 2020 02:43:15 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 18 Dec 2020 02:43:15 GMT
EXPOSE 8091
# Fri, 18 Dec 2020 02:43:15 GMT
VOLUME [/var/lib/influxdb]
# Fri, 18 Dec 2020 02:43:15 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 18 Dec 2020 02:43:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Dec 2020 02:43:16 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072739d44e4fe2316d3bda5b6e0944796b1824cb2dee521ef06bf11e4f5db0fe`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 10.8 MB (10752737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5111f27e9600a1fa0a3a8660e8518294729a41abcd648bbf0ec9f60dcfb02b73`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 4.3 MB (4340690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8edcaa1ed5e299a41dda2ec21e02bcffc9984be150078569bf9537b855e2f`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8ac203dfae9af5a917933f9fd0fd75133b08b509c0f9931c980e51db484930`  
		Last Modified: Fri, 18 Dec 2020 02:45:21 GMT  
		Size: 23.1 MB (23132660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f76e3cbf34396af02fd40002cf9410897ab417a2cf4b6c7e8a1cd983438e67`  
		Last Modified: Fri, 18 Dec 2020 02:45:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37854094312e951542a51432c0d0b9faf8ec3d4f27a5fc037dfe31e7c583373a`  
		Last Modified: Fri, 18 Dec 2020 02:45:17 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta-alpine`

```console
$ docker pull influxdb@sha256:de16392636e76e08ab574dd858057a6b975c782c8b5c0b416733e029ce25b5e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:156abf7250306d6f8dcbff15092cef2b76844b7c018d606fc6a62116e89f4f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27230754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d7485cab53b185859b0e6762551835468f6f52cc194a69b4e734ddebcf905f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:47:22 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:47:40 GMT
ENV INFLUXDB_VERSION=1.7.10-c1.7.10
# Thu, 17 Dec 2020 13:48:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:48:04 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 17 Dec 2020 13:48:04 GMT
EXPOSE 8091
# Thu, 17 Dec 2020 13:48:05 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 13:48:05 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:48:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:48:05 GMT
CMD ["influxd-meta"]
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
	-	`sha256:1924738bc6407d8319fdb7d3fca610b5972213dee7ad608f4d801b3990f11a21`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 1.4 MB (1428296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810893317995e32ec408ab5a96f97680ed29491804e058a06afc02b4f9764fe9`  
		Last Modified: Thu, 17 Dec 2020 13:50:21 GMT  
		Size: 23.0 MB (23002670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a373124bdc8b99e201610f79430294e29f7444345987bb5ca2c4042360d2f539`  
		Last Modified: Thu, 17 Dec 2020 13:50:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fcd2ae59d54ca79585f5a7888535850738abff6ce791ed0b1061ba560ffda83`  
		Last Modified: Thu, 17 Dec 2020 13:50:18 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8`

```console
$ docker pull influxdb@sha256:c73a90a14b49d71412c9603bca9b16994a41957f894d888fd02a9d7d43ce279f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:b89938115d631b406fca51de2eac0612cd41d34220977a9006a7641c06abfe92
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125441510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09375fea906ebb5b85e95c778da27b7af699c7e7990ffb4efb2f2bb9257c0fb2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 17:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 17:01:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 02:42:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 18 Dec 2020 02:43:23 GMT
ENV INFLUXDB_VERSION=1.8.3
# Fri, 18 Dec 2020 02:43:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 18 Dec 2020 02:43:30 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 18 Dec 2020 02:43:30 GMT
EXPOSE 8086
# Fri, 18 Dec 2020 02:43:30 GMT
VOLUME [/var/lib/influxdb]
# Fri, 18 Dec 2020 02:43:30 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 18 Dec 2020 02:43:31 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 18 Dec 2020 02:43:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Dec 2020 02:43:31 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072739d44e4fe2316d3bda5b6e0944796b1824cb2dee521ef06bf11e4f5db0fe`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 10.8 MB (10752737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5111f27e9600a1fa0a3a8660e8518294729a41abcd648bbf0ec9f60dcfb02b73`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 4.3 MB (4340690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8edcaa1ed5e299a41dda2ec21e02bcffc9984be150078569bf9537b855e2f`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13ba5490d638739d7649f595d300d9e5f3a94a9e8fccc862882ea39072091c3`  
		Last Modified: Fri, 18 Dec 2020 02:45:49 GMT  
		Size: 65.0 MB (64965934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad98b997807bdc5f0ba2dbc2b2d99209a2d4e967f4bd9b63091b9a3f02199b9`  
		Last Modified: Fri, 18 Dec 2020 02:45:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecdc57b1fad2cc5801e5f52560444b5d2456d8ae182a19591622d5938c81e074`  
		Last Modified: Fri, 18 Dec 2020 02:45:28 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bab1f0411eb3ce399ff56a568974c24d992a1015771229c5a2343560d68497e`  
		Last Modified: Fri, 18 Dec 2020 02:45:28 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:b099bdd1f4306689fd11c02f83b3de7fc11eccd8debf5f345e9be11d0a7cd7dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116548072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e315d6ff66902df2ef37f85938d60bf8e96760230a8d5ee593ad7f0f6e7e80`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:19 GMT
ADD file:9c744a203d36aa8c515bbc11873a4a479cdf3fe9f020ca1ef207b53e6b3a251e in / 
# Tue, 12 Jan 2021 00:05:23 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:21:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 17:20:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 17:20:45 GMT
ENV INFLUXDB_VERSION=1.8.3
# Tue, 12 Jan 2021 17:20:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 12 Jan 2021 17:20:56 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 12 Jan 2021 17:20:57 GMT
EXPOSE 8086
# Tue, 12 Jan 2021 17:20:58 GMT
VOLUME [/var/lib/influxdb]
# Tue, 12 Jan 2021 17:20:58 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 12 Jan 2021 17:20:59 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 12 Jan 2021 17:21:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 17:21:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f5de2649c1cd9091872f81b8ceb6a67890124f113d9fce9c52bf60d5a6e19f43`  
		Last Modified: Tue, 12 Jan 2021 00:15:23 GMT  
		Size: 42.1 MB (42119951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cae60aac6e598935e2b14216dc4265434ba03d17c82f622b18abb712577d2c`  
		Last Modified: Tue, 12 Jan 2021 01:34:01 GMT  
		Size: 9.4 MB (9446203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9694e28a75917ff08caeaee5ed8729a2f12d2110bf203781d578006a0ef2f7`  
		Last Modified: Tue, 12 Jan 2021 01:33:59 GMT  
		Size: 3.9 MB (3919958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9af4291e32292c1b3e0baa3521c9903226273223480ec660c81d82cec54e2b`  
		Last Modified: Tue, 12 Jan 2021 17:21:15 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc25c2db575e35a675a00c4c4a6d0f737064cc0789ae70ad0fa214115eac480`  
		Last Modified: Tue, 12 Jan 2021 17:22:04 GMT  
		Size: 61.1 MB (61057389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309ce3cfceae39ef043c05cbcaf2d3443f8d4b6d2e7bbb35acdab440f655b62d`  
		Last Modified: Tue, 12 Jan 2021 17:21:48 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0848e4c0b723e7b1c138100af0c50a5197705e68c522c35815519c5c4b64610d`  
		Last Modified: Tue, 12 Jan 2021 17:21:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e532b4cfca353c580548792aea8a7e5dc17fdbed3b8606c0ec3640fd6d0524`  
		Last Modified: Tue, 12 Jan 2021 17:21:48 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:116afd3662c995818965acbc3f515851eb8b59b081852ee633b6516d83a343bd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117605732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a83e931cfa467a4db3127999749502aa87a922ddb52333257a88cfe89e012dde`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 11 Dec 2020 02:48:16 GMT
ADD file:48e44714f486662ed380343e556f0f7411bd6600d916440063753c55d1f94b45 in / 
# Fri, 11 Dec 2020 02:48:17 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 10:13:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 10:13:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 15:25:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 17 Dec 2020 15:26:52 GMT
ENV INFLUXDB_VERSION=1.8.3
# Thu, 17 Dec 2020 15:27:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 17 Dec 2020 15:27:02 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 17 Dec 2020 15:27:03 GMT
EXPOSE 8086
# Thu, 17 Dec 2020 15:27:03 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 15:27:04 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 17 Dec 2020 15:27:05 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Dec 2020 15:27:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 15:27:07 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:ecefb91918e846819df74a1beb8e41f454bef156738373818c20656a3a46d5f7`  
		Last Modified: Fri, 11 Dec 2020 02:55:36 GMT  
		Size: 43.2 MB (43175941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda9a63f37e7beb33012f80c0f66755ce6d87a51fde0a283a06dbdf2857ce533`  
		Last Modified: Thu, 17 Dec 2020 10:41:45 GMT  
		Size: 9.7 MB (9702906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0c493446fd68c6abee0df0169e849bcb73aa61a86ba5e30783c9b5298007b7`  
		Last Modified: Thu, 17 Dec 2020 10:41:43 GMT  
		Size: 4.1 MB (4095483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a00a8a57199af4c15740e382214257dc71414c8a40b544ffcd0d9f53ce2404c`  
		Last Modified: Thu, 17 Dec 2020 15:27:23 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ed1589af262d0f6104eceb471392d09eff5421d4669f06e2c9054545965652`  
		Last Modified: Thu, 17 Dec 2020 15:27:58 GMT  
		Size: 60.6 MB (60626832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4054772c2c83698fb81c7e810b3698c46ad0ee08ad658c2d70ab1481f90ca177`  
		Last Modified: Thu, 17 Dec 2020 15:27:46 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0f7491941e8bc9638ce33e93b5d9e88ace69570e4a88ca8f0d2a2125969333`  
		Last Modified: Thu, 17 Dec 2020 15:27:45 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db28bc4ec64e21181ce4865c49ef34edec20ff9c09a4166fd920a2fe64950ebc`  
		Last Modified: Thu, 17 Dec 2020 15:27:45 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.3`

```console
$ docker pull influxdb@sha256:c73a90a14b49d71412c9603bca9b16994a41957f894d888fd02a9d7d43ce279f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.3` - linux; amd64

```console
$ docker pull influxdb@sha256:b89938115d631b406fca51de2eac0612cd41d34220977a9006a7641c06abfe92
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125441510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09375fea906ebb5b85e95c778da27b7af699c7e7990ffb4efb2f2bb9257c0fb2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 17:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 17:01:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 02:42:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 18 Dec 2020 02:43:23 GMT
ENV INFLUXDB_VERSION=1.8.3
# Fri, 18 Dec 2020 02:43:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 18 Dec 2020 02:43:30 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 18 Dec 2020 02:43:30 GMT
EXPOSE 8086
# Fri, 18 Dec 2020 02:43:30 GMT
VOLUME [/var/lib/influxdb]
# Fri, 18 Dec 2020 02:43:30 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 18 Dec 2020 02:43:31 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 18 Dec 2020 02:43:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Dec 2020 02:43:31 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072739d44e4fe2316d3bda5b6e0944796b1824cb2dee521ef06bf11e4f5db0fe`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 10.8 MB (10752737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5111f27e9600a1fa0a3a8660e8518294729a41abcd648bbf0ec9f60dcfb02b73`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 4.3 MB (4340690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8edcaa1ed5e299a41dda2ec21e02bcffc9984be150078569bf9537b855e2f`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13ba5490d638739d7649f595d300d9e5f3a94a9e8fccc862882ea39072091c3`  
		Last Modified: Fri, 18 Dec 2020 02:45:49 GMT  
		Size: 65.0 MB (64965934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad98b997807bdc5f0ba2dbc2b2d99209a2d4e967f4bd9b63091b9a3f02199b9`  
		Last Modified: Fri, 18 Dec 2020 02:45:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecdc57b1fad2cc5801e5f52560444b5d2456d8ae182a19591622d5938c81e074`  
		Last Modified: Fri, 18 Dec 2020 02:45:28 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bab1f0411eb3ce399ff56a568974c24d992a1015771229c5a2343560d68497e`  
		Last Modified: Fri, 18 Dec 2020 02:45:28 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.3` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:b099bdd1f4306689fd11c02f83b3de7fc11eccd8debf5f345e9be11d0a7cd7dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116548072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e315d6ff66902df2ef37f85938d60bf8e96760230a8d5ee593ad7f0f6e7e80`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:19 GMT
ADD file:9c744a203d36aa8c515bbc11873a4a479cdf3fe9f020ca1ef207b53e6b3a251e in / 
# Tue, 12 Jan 2021 00:05:23 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:21:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 17:20:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 17:20:45 GMT
ENV INFLUXDB_VERSION=1.8.3
# Tue, 12 Jan 2021 17:20:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 12 Jan 2021 17:20:56 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 12 Jan 2021 17:20:57 GMT
EXPOSE 8086
# Tue, 12 Jan 2021 17:20:58 GMT
VOLUME [/var/lib/influxdb]
# Tue, 12 Jan 2021 17:20:58 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 12 Jan 2021 17:20:59 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 12 Jan 2021 17:21:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 17:21:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f5de2649c1cd9091872f81b8ceb6a67890124f113d9fce9c52bf60d5a6e19f43`  
		Last Modified: Tue, 12 Jan 2021 00:15:23 GMT  
		Size: 42.1 MB (42119951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cae60aac6e598935e2b14216dc4265434ba03d17c82f622b18abb712577d2c`  
		Last Modified: Tue, 12 Jan 2021 01:34:01 GMT  
		Size: 9.4 MB (9446203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9694e28a75917ff08caeaee5ed8729a2f12d2110bf203781d578006a0ef2f7`  
		Last Modified: Tue, 12 Jan 2021 01:33:59 GMT  
		Size: 3.9 MB (3919958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9af4291e32292c1b3e0baa3521c9903226273223480ec660c81d82cec54e2b`  
		Last Modified: Tue, 12 Jan 2021 17:21:15 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc25c2db575e35a675a00c4c4a6d0f737064cc0789ae70ad0fa214115eac480`  
		Last Modified: Tue, 12 Jan 2021 17:22:04 GMT  
		Size: 61.1 MB (61057389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309ce3cfceae39ef043c05cbcaf2d3443f8d4b6d2e7bbb35acdab440f655b62d`  
		Last Modified: Tue, 12 Jan 2021 17:21:48 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0848e4c0b723e7b1c138100af0c50a5197705e68c522c35815519c5c4b64610d`  
		Last Modified: Tue, 12 Jan 2021 17:21:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e532b4cfca353c580548792aea8a7e5dc17fdbed3b8606c0ec3640fd6d0524`  
		Last Modified: Tue, 12 Jan 2021 17:21:48 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.3` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:116afd3662c995818965acbc3f515851eb8b59b081852ee633b6516d83a343bd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117605732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a83e931cfa467a4db3127999749502aa87a922ddb52333257a88cfe89e012dde`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 11 Dec 2020 02:48:16 GMT
ADD file:48e44714f486662ed380343e556f0f7411bd6600d916440063753c55d1f94b45 in / 
# Fri, 11 Dec 2020 02:48:17 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 10:13:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 10:13:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 15:25:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 17 Dec 2020 15:26:52 GMT
ENV INFLUXDB_VERSION=1.8.3
# Thu, 17 Dec 2020 15:27:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 17 Dec 2020 15:27:02 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 17 Dec 2020 15:27:03 GMT
EXPOSE 8086
# Thu, 17 Dec 2020 15:27:03 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 15:27:04 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 17 Dec 2020 15:27:05 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Dec 2020 15:27:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 15:27:07 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:ecefb91918e846819df74a1beb8e41f454bef156738373818c20656a3a46d5f7`  
		Last Modified: Fri, 11 Dec 2020 02:55:36 GMT  
		Size: 43.2 MB (43175941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda9a63f37e7beb33012f80c0f66755ce6d87a51fde0a283a06dbdf2857ce533`  
		Last Modified: Thu, 17 Dec 2020 10:41:45 GMT  
		Size: 9.7 MB (9702906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0c493446fd68c6abee0df0169e849bcb73aa61a86ba5e30783c9b5298007b7`  
		Last Modified: Thu, 17 Dec 2020 10:41:43 GMT  
		Size: 4.1 MB (4095483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a00a8a57199af4c15740e382214257dc71414c8a40b544ffcd0d9f53ce2404c`  
		Last Modified: Thu, 17 Dec 2020 15:27:23 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ed1589af262d0f6104eceb471392d09eff5421d4669f06e2c9054545965652`  
		Last Modified: Thu, 17 Dec 2020 15:27:58 GMT  
		Size: 60.6 MB (60626832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4054772c2c83698fb81c7e810b3698c46ad0ee08ad658c2d70ab1481f90ca177`  
		Last Modified: Thu, 17 Dec 2020 15:27:46 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0f7491941e8bc9638ce33e93b5d9e88ace69570e4a88ca8f0d2a2125969333`  
		Last Modified: Thu, 17 Dec 2020 15:27:45 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db28bc4ec64e21181ce4865c49ef34edec20ff9c09a4166fd920a2fe64950ebc`  
		Last Modified: Thu, 17 Dec 2020 15:27:45 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.3-alpine`

```console
$ docker pull influxdb@sha256:65cb0a80cab9744a2892c9720867fdbd1a61784529c599fd37105893d8a6a6e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.3-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:2f73472a38b0fadb41399fcd111877b762b9088fe891e4060ae842c9a3c0e4ed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68935837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79d626945ed3abd9dc0fefe18c4f2334be0c05873ffc296139c902819fccdb51`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:47:22 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:48:13 GMT
ENV INFLUXDB_VERSION=1.8.3
# Thu, 17 Dec 2020 13:48:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:48:23 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 17 Dec 2020 13:48:23 GMT
EXPOSE 8086
# Thu, 17 Dec 2020 13:48:23 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 13:48:23 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:48:23 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Dec 2020 13:48:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:48:24 GMT
CMD ["influxd"]
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
	-	`sha256:1924738bc6407d8319fdb7d3fca610b5972213dee7ad608f4d801b3990f11a21`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 1.4 MB (1428296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12eb60e6cd81240f7cfece2cd78c24800a82105bb0ccc15d8f108a11b392ed`  
		Last Modified: Thu, 17 Dec 2020 13:50:49 GMT  
		Size: 64.7 MB (64706606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f99d25b1ceb07bd2d7e2314d83eff49e3838acc35cc1b8fad1e4e758087d10`  
		Last Modified: Thu, 17 Dec 2020 13:50:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52690e3b2d969a7bc60dc1b366d40383d4f1573e778c8d9f4643ba117afa24f`  
		Last Modified: Thu, 17 Dec 2020 13:50:31 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3383a0f6861a3a14514428c363a8d2acfc4ab75797c887d79458cb7708641d`  
		Last Modified: Thu, 17 Dec 2020 13:50:30 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.3-data`

```console
$ docker pull influxdb@sha256:81117df76aca30d2b9453dd190a317c224dc340e0a3b5d5d4fd917285cacc6ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.3-data` - linux; amd64

```console
$ docker pull influxdb@sha256:858e6c3de06ea8dcd4687a533da5caa057b5a2486c72281e00bad9f3c096ef2b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.3 MB (126271600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82114e01d2026118e0b6f6f774acef8a9e98bb5710dab1e307f3e0ef955e3c8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 17:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 17:01:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 02:42:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 18 Dec 2020 02:43:39 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Fri, 18 Dec 2020 02:43:46 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 18 Dec 2020 02:43:46 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 18 Dec 2020 02:43:46 GMT
EXPOSE 8086
# Fri, 18 Dec 2020 02:43:46 GMT
VOLUME [/var/lib/influxdb]
# Fri, 18 Dec 2020 02:43:47 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 18 Dec 2020 02:43:47 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 18 Dec 2020 02:43:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Dec 2020 02:43:47 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072739d44e4fe2316d3bda5b6e0944796b1824cb2dee521ef06bf11e4f5db0fe`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 10.8 MB (10752737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5111f27e9600a1fa0a3a8660e8518294729a41abcd648bbf0ec9f60dcfb02b73`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 4.3 MB (4340690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8edcaa1ed5e299a41dda2ec21e02bcffc9984be150078569bf9537b855e2f`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449c6310804ea1b27f8c9db90a4c35e53609e049e934da5c9a3cda312a2bf140`  
		Last Modified: Fri, 18 Dec 2020 02:46:09 GMT  
		Size: 65.8 MB (65795967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94e9d69309ce033b79f1260379862696ba2c3b18163e17ee039a605a89ac925`  
		Last Modified: Fri, 18 Dec 2020 02:45:59 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e762457fa50e4dc37ba028893e64501eb49ccba483a292dbd1f25b8566b8e982`  
		Last Modified: Fri, 18 Dec 2020 02:45:59 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48207ae20b5db2e6f2211be396d6d59a880f832ddf8e518a210b8f37cf614b72`  
		Last Modified: Fri, 18 Dec 2020 02:45:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.3-data-alpine`

```console
$ docker pull influxdb@sha256:1f76bcc17b25bea15aa83eba37ae79913bb097973c16510c29426683554ffa78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.3-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ca8eb83702c42e6842af42682894c786ed7df4ccad01039da5e44b25987f621e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69770238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c93b32605cb2f94cf639d1f32c08a983526c4557abd14fe6292fc0d2fa3607`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:47:22 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:48:32 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Thu, 17 Dec 2020 13:48:39 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:48:39 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 17 Dec 2020 13:48:39 GMT
EXPOSE 8086
# Thu, 17 Dec 2020 13:48:39 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 13:48:39 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:48:40 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Dec 2020 13:48:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:48:40 GMT
CMD ["influxd"]
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
	-	`sha256:1924738bc6407d8319fdb7d3fca610b5972213dee7ad608f4d801b3990f11a21`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 1.4 MB (1428296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6edf7ef0639b641e2a6c111b20bb8d65c63a939fb49f70007b70b6a18cd225`  
		Last Modified: Thu, 17 Dec 2020 13:51:10 GMT  
		Size: 65.5 MB (65540953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976d9c1bb701d9b9686a9c72d1711cb0e6b27061b3f6950efbadbbab20dad7bf`  
		Last Modified: Thu, 17 Dec 2020 13:50:58 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d3881e28e4b6909bfc1fd929606827018b6dfb44e91a07edf855afb0f7e856`  
		Last Modified: Thu, 17 Dec 2020 13:50:58 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a300eda57a9818ae4a90aaf183c2476f4e828cbc9073271ec5bffdc644b6e7b2`  
		Last Modified: Thu, 17 Dec 2020 13:50:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.3-meta`

```console
$ docker pull influxdb@sha256:ae646819f963fb00e7c01984626b8442efbfb5e1ab3dddde58e0d5f6c3f15899
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.3-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:556ccc3ace6d88c6c9739b8e27ab5e88f1a22cfc302a2444b95379cd8d6ea303
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83339700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd04b7b31146bbc9d25c819dcc0a5841a8fc12d4bc0da47a5113d35a962a06c1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 17:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 17:01:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 02:42:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 18 Dec 2020 02:43:39 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Fri, 18 Dec 2020 02:43:58 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 18 Dec 2020 02:43:58 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 18 Dec 2020 02:43:58 GMT
EXPOSE 8091
# Fri, 18 Dec 2020 02:43:59 GMT
VOLUME [/var/lib/influxdb]
# Fri, 18 Dec 2020 02:43:59 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 18 Dec 2020 02:43:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Dec 2020 02:43:59 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072739d44e4fe2316d3bda5b6e0944796b1824cb2dee521ef06bf11e4f5db0fe`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 10.8 MB (10752737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5111f27e9600a1fa0a3a8660e8518294729a41abcd648bbf0ec9f60dcfb02b73`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 4.3 MB (4340690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8edcaa1ed5e299a41dda2ec21e02bcffc9984be150078569bf9537b855e2f`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82550fa0125499a3c848b35ecfd0a5d0ece26c5ffd8b6b88657b4199e945327f`  
		Last Modified: Fri, 18 Dec 2020 02:46:20 GMT  
		Size: 22.9 MB (22865271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a106d8f0f18ca0e190aede94b9ab2b2adf418d5d5544aaf340c86af12ee445ed`  
		Last Modified: Fri, 18 Dec 2020 02:46:16 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798fd3ed5f538287b703b25f8c9a0a1094be537cca8d259f802eb64c2a6efbb3`  
		Last Modified: Fri, 18 Dec 2020 02:46:16 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.3-meta-alpine`

```console
$ docker pull influxdb@sha256:4c29eac32909a131cfaff0592d154d70dd7dfe0478cb9540c2901ddf0da5fae7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.3-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:dca974575db512c53831bde49ddf78ac0dcf4d82dc22079be452c62da4ba5682
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (26963560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8881cbf80321dc2a4ebdf2195439034efa5d7c8d21b315de81395c705b9129c8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:47:22 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:48:32 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Thu, 17 Dec 2020 13:48:52 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:48:52 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 17 Dec 2020 13:48:53 GMT
EXPOSE 8091
# Thu, 17 Dec 2020 13:48:53 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 13:48:54 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:48:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:48:54 GMT
CMD ["influxd-meta"]
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
	-	`sha256:1924738bc6407d8319fdb7d3fca610b5972213dee7ad608f4d801b3990f11a21`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 1.4 MB (1428296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160bf10769c16bdb7542730ceba295bdfb41ccdcc94aad7899def6ebc89b50f5`  
		Last Modified: Thu, 17 Dec 2020 13:51:26 GMT  
		Size: 22.7 MB (22735478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc8f9cb3bd7cd3e189107cbd62ad4c10e03619dda2334334e9472e68bed697b`  
		Last Modified: Thu, 17 Dec 2020 13:51:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74170b5ea5a39ad5a9878ee9a90ab8f39e7d7331d10ead82b0ed7f28cd4f007`  
		Last Modified: Thu, 17 Dec 2020 13:51:22 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-alpine`

```console
$ docker pull influxdb@sha256:65cb0a80cab9744a2892c9720867fdbd1a61784529c599fd37105893d8a6a6e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:2f73472a38b0fadb41399fcd111877b762b9088fe891e4060ae842c9a3c0e4ed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68935837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79d626945ed3abd9dc0fefe18c4f2334be0c05873ffc296139c902819fccdb51`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:47:22 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:48:13 GMT
ENV INFLUXDB_VERSION=1.8.3
# Thu, 17 Dec 2020 13:48:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:48:23 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 17 Dec 2020 13:48:23 GMT
EXPOSE 8086
# Thu, 17 Dec 2020 13:48:23 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 13:48:23 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:48:23 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Dec 2020 13:48:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:48:24 GMT
CMD ["influxd"]
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
	-	`sha256:1924738bc6407d8319fdb7d3fca610b5972213dee7ad608f4d801b3990f11a21`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 1.4 MB (1428296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12eb60e6cd81240f7cfece2cd78c24800a82105bb0ccc15d8f108a11b392ed`  
		Last Modified: Thu, 17 Dec 2020 13:50:49 GMT  
		Size: 64.7 MB (64706606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f99d25b1ceb07bd2d7e2314d83eff49e3838acc35cc1b8fad1e4e758087d10`  
		Last Modified: Thu, 17 Dec 2020 13:50:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52690e3b2d969a7bc60dc1b366d40383d4f1573e778c8d9f4643ba117afa24f`  
		Last Modified: Thu, 17 Dec 2020 13:50:31 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3383a0f6861a3a14514428c363a8d2acfc4ab75797c887d79458cb7708641d`  
		Last Modified: Thu, 17 Dec 2020 13:50:30 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data`

```console
$ docker pull influxdb@sha256:81117df76aca30d2b9453dd190a317c224dc340e0a3b5d5d4fd917285cacc6ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:858e6c3de06ea8dcd4687a533da5caa057b5a2486c72281e00bad9f3c096ef2b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.3 MB (126271600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82114e01d2026118e0b6f6f774acef8a9e98bb5710dab1e307f3e0ef955e3c8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 17:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 17:01:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 02:42:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 18 Dec 2020 02:43:39 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Fri, 18 Dec 2020 02:43:46 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 18 Dec 2020 02:43:46 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 18 Dec 2020 02:43:46 GMT
EXPOSE 8086
# Fri, 18 Dec 2020 02:43:46 GMT
VOLUME [/var/lib/influxdb]
# Fri, 18 Dec 2020 02:43:47 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 18 Dec 2020 02:43:47 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 18 Dec 2020 02:43:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Dec 2020 02:43:47 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072739d44e4fe2316d3bda5b6e0944796b1824cb2dee521ef06bf11e4f5db0fe`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 10.8 MB (10752737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5111f27e9600a1fa0a3a8660e8518294729a41abcd648bbf0ec9f60dcfb02b73`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 4.3 MB (4340690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8edcaa1ed5e299a41dda2ec21e02bcffc9984be150078569bf9537b855e2f`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449c6310804ea1b27f8c9db90a4c35e53609e049e934da5c9a3cda312a2bf140`  
		Last Modified: Fri, 18 Dec 2020 02:46:09 GMT  
		Size: 65.8 MB (65795967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94e9d69309ce033b79f1260379862696ba2c3b18163e17ee039a605a89ac925`  
		Last Modified: Fri, 18 Dec 2020 02:45:59 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e762457fa50e4dc37ba028893e64501eb49ccba483a292dbd1f25b8566b8e982`  
		Last Modified: Fri, 18 Dec 2020 02:45:59 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48207ae20b5db2e6f2211be396d6d59a880f832ddf8e518a210b8f37cf614b72`  
		Last Modified: Fri, 18 Dec 2020 02:45:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data-alpine`

```console
$ docker pull influxdb@sha256:1f76bcc17b25bea15aa83eba37ae79913bb097973c16510c29426683554ffa78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ca8eb83702c42e6842af42682894c786ed7df4ccad01039da5e44b25987f621e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69770238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c93b32605cb2f94cf639d1f32c08a983526c4557abd14fe6292fc0d2fa3607`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:47:22 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:48:32 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Thu, 17 Dec 2020 13:48:39 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:48:39 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 17 Dec 2020 13:48:39 GMT
EXPOSE 8086
# Thu, 17 Dec 2020 13:48:39 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 13:48:39 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:48:40 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Dec 2020 13:48:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:48:40 GMT
CMD ["influxd"]
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
	-	`sha256:1924738bc6407d8319fdb7d3fca610b5972213dee7ad608f4d801b3990f11a21`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 1.4 MB (1428296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6edf7ef0639b641e2a6c111b20bb8d65c63a939fb49f70007b70b6a18cd225`  
		Last Modified: Thu, 17 Dec 2020 13:51:10 GMT  
		Size: 65.5 MB (65540953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976d9c1bb701d9b9686a9c72d1711cb0e6b27061b3f6950efbadbbab20dad7bf`  
		Last Modified: Thu, 17 Dec 2020 13:50:58 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d3881e28e4b6909bfc1fd929606827018b6dfb44e91a07edf855afb0f7e856`  
		Last Modified: Thu, 17 Dec 2020 13:50:58 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a300eda57a9818ae4a90aaf183c2476f4e828cbc9073271ec5bffdc644b6e7b2`  
		Last Modified: Thu, 17 Dec 2020 13:50:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta`

```console
$ docker pull influxdb@sha256:ae646819f963fb00e7c01984626b8442efbfb5e1ab3dddde58e0d5f6c3f15899
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:556ccc3ace6d88c6c9739b8e27ab5e88f1a22cfc302a2444b95379cd8d6ea303
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83339700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd04b7b31146bbc9d25c819dcc0a5841a8fc12d4bc0da47a5113d35a962a06c1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 17:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 17:01:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 02:42:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 18 Dec 2020 02:43:39 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Fri, 18 Dec 2020 02:43:58 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 18 Dec 2020 02:43:58 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 18 Dec 2020 02:43:58 GMT
EXPOSE 8091
# Fri, 18 Dec 2020 02:43:59 GMT
VOLUME [/var/lib/influxdb]
# Fri, 18 Dec 2020 02:43:59 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 18 Dec 2020 02:43:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Dec 2020 02:43:59 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072739d44e4fe2316d3bda5b6e0944796b1824cb2dee521ef06bf11e4f5db0fe`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 10.8 MB (10752737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5111f27e9600a1fa0a3a8660e8518294729a41abcd648bbf0ec9f60dcfb02b73`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 4.3 MB (4340690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8edcaa1ed5e299a41dda2ec21e02bcffc9984be150078569bf9537b855e2f`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82550fa0125499a3c848b35ecfd0a5d0ece26c5ffd8b6b88657b4199e945327f`  
		Last Modified: Fri, 18 Dec 2020 02:46:20 GMT  
		Size: 22.9 MB (22865271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a106d8f0f18ca0e190aede94b9ab2b2adf418d5d5544aaf340c86af12ee445ed`  
		Last Modified: Fri, 18 Dec 2020 02:46:16 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798fd3ed5f538287b703b25f8c9a0a1094be537cca8d259f802eb64c2a6efbb3`  
		Last Modified: Fri, 18 Dec 2020 02:46:16 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta-alpine`

```console
$ docker pull influxdb@sha256:4c29eac32909a131cfaff0592d154d70dd7dfe0478cb9540c2901ddf0da5fae7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:dca974575db512c53831bde49ddf78ac0dcf4d82dc22079be452c62da4ba5682
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (26963560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8881cbf80321dc2a4ebdf2195439034efa5d7c8d21b315de81395c705b9129c8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:47:22 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:48:32 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Thu, 17 Dec 2020 13:48:52 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:48:52 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 17 Dec 2020 13:48:53 GMT
EXPOSE 8091
# Thu, 17 Dec 2020 13:48:53 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 13:48:54 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:48:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:48:54 GMT
CMD ["influxd-meta"]
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
	-	`sha256:1924738bc6407d8319fdb7d3fca610b5972213dee7ad608f4d801b3990f11a21`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 1.4 MB (1428296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160bf10769c16bdb7542730ceba295bdfb41ccdcc94aad7899def6ebc89b50f5`  
		Last Modified: Thu, 17 Dec 2020 13:51:26 GMT  
		Size: 22.7 MB (22735478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc8f9cb3bd7cd3e189107cbd62ad4c10e03619dda2334334e9472e68bed697b`  
		Last Modified: Thu, 17 Dec 2020 13:51:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74170b5ea5a39ad5a9878ee9a90ab8f39e7d7331d10ead82b0ed7f28cd4f007`  
		Last Modified: Thu, 17 Dec 2020 13:51:22 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:65cb0a80cab9744a2892c9720867fdbd1a61784529c599fd37105893d8a6a6e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:2f73472a38b0fadb41399fcd111877b762b9088fe891e4060ae842c9a3c0e4ed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68935837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79d626945ed3abd9dc0fefe18c4f2334be0c05873ffc296139c902819fccdb51`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:47:22 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:48:13 GMT
ENV INFLUXDB_VERSION=1.8.3
# Thu, 17 Dec 2020 13:48:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:48:23 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 17 Dec 2020 13:48:23 GMT
EXPOSE 8086
# Thu, 17 Dec 2020 13:48:23 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 13:48:23 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:48:23 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Dec 2020 13:48:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:48:24 GMT
CMD ["influxd"]
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
	-	`sha256:1924738bc6407d8319fdb7d3fca610b5972213dee7ad608f4d801b3990f11a21`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 1.4 MB (1428296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12eb60e6cd81240f7cfece2cd78c24800a82105bb0ccc15d8f108a11b392ed`  
		Last Modified: Thu, 17 Dec 2020 13:50:49 GMT  
		Size: 64.7 MB (64706606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f99d25b1ceb07bd2d7e2314d83eff49e3838acc35cc1b8fad1e4e758087d10`  
		Last Modified: Thu, 17 Dec 2020 13:50:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52690e3b2d969a7bc60dc1b366d40383d4f1573e778c8d9f4643ba117afa24f`  
		Last Modified: Thu, 17 Dec 2020 13:50:31 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3383a0f6861a3a14514428c363a8d2acfc4ab75797c887d79458cb7708641d`  
		Last Modified: Thu, 17 Dec 2020 13:50:30 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data`

```console
$ docker pull influxdb@sha256:81117df76aca30d2b9453dd190a317c224dc340e0a3b5d5d4fd917285cacc6ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:858e6c3de06ea8dcd4687a533da5caa057b5a2486c72281e00bad9f3c096ef2b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.3 MB (126271600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82114e01d2026118e0b6f6f774acef8a9e98bb5710dab1e307f3e0ef955e3c8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 17:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 17:01:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 02:42:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 18 Dec 2020 02:43:39 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Fri, 18 Dec 2020 02:43:46 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 18 Dec 2020 02:43:46 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 18 Dec 2020 02:43:46 GMT
EXPOSE 8086
# Fri, 18 Dec 2020 02:43:46 GMT
VOLUME [/var/lib/influxdb]
# Fri, 18 Dec 2020 02:43:47 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 18 Dec 2020 02:43:47 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 18 Dec 2020 02:43:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Dec 2020 02:43:47 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072739d44e4fe2316d3bda5b6e0944796b1824cb2dee521ef06bf11e4f5db0fe`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 10.8 MB (10752737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5111f27e9600a1fa0a3a8660e8518294729a41abcd648bbf0ec9f60dcfb02b73`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 4.3 MB (4340690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8edcaa1ed5e299a41dda2ec21e02bcffc9984be150078569bf9537b855e2f`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449c6310804ea1b27f8c9db90a4c35e53609e049e934da5c9a3cda312a2bf140`  
		Last Modified: Fri, 18 Dec 2020 02:46:09 GMT  
		Size: 65.8 MB (65795967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94e9d69309ce033b79f1260379862696ba2c3b18163e17ee039a605a89ac925`  
		Last Modified: Fri, 18 Dec 2020 02:45:59 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e762457fa50e4dc37ba028893e64501eb49ccba483a292dbd1f25b8566b8e982`  
		Last Modified: Fri, 18 Dec 2020 02:45:59 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48207ae20b5db2e6f2211be396d6d59a880f832ddf8e518a210b8f37cf614b72`  
		Last Modified: Fri, 18 Dec 2020 02:45:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data-alpine`

```console
$ docker pull influxdb@sha256:1f76bcc17b25bea15aa83eba37ae79913bb097973c16510c29426683554ffa78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ca8eb83702c42e6842af42682894c786ed7df4ccad01039da5e44b25987f621e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69770238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c93b32605cb2f94cf639d1f32c08a983526c4557abd14fe6292fc0d2fa3607`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:47:22 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:48:32 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Thu, 17 Dec 2020 13:48:39 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:48:39 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 17 Dec 2020 13:48:39 GMT
EXPOSE 8086
# Thu, 17 Dec 2020 13:48:39 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 13:48:39 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:48:40 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Dec 2020 13:48:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:48:40 GMT
CMD ["influxd"]
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
	-	`sha256:1924738bc6407d8319fdb7d3fca610b5972213dee7ad608f4d801b3990f11a21`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 1.4 MB (1428296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6edf7ef0639b641e2a6c111b20bb8d65c63a939fb49f70007b70b6a18cd225`  
		Last Modified: Thu, 17 Dec 2020 13:51:10 GMT  
		Size: 65.5 MB (65540953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976d9c1bb701d9b9686a9c72d1711cb0e6b27061b3f6950efbadbbab20dad7bf`  
		Last Modified: Thu, 17 Dec 2020 13:50:58 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d3881e28e4b6909bfc1fd929606827018b6dfb44e91a07edf855afb0f7e856`  
		Last Modified: Thu, 17 Dec 2020 13:50:58 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a300eda57a9818ae4a90aaf183c2476f4e828cbc9073271ec5bffdc644b6e7b2`  
		Last Modified: Thu, 17 Dec 2020 13:50:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:latest`

```console
$ docker pull influxdb@sha256:c73a90a14b49d71412c9603bca9b16994a41957f894d888fd02a9d7d43ce279f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:b89938115d631b406fca51de2eac0612cd41d34220977a9006a7641c06abfe92
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125441510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09375fea906ebb5b85e95c778da27b7af699c7e7990ffb4efb2f2bb9257c0fb2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 17:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 17:01:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 02:42:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 18 Dec 2020 02:43:23 GMT
ENV INFLUXDB_VERSION=1.8.3
# Fri, 18 Dec 2020 02:43:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 18 Dec 2020 02:43:30 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 18 Dec 2020 02:43:30 GMT
EXPOSE 8086
# Fri, 18 Dec 2020 02:43:30 GMT
VOLUME [/var/lib/influxdb]
# Fri, 18 Dec 2020 02:43:30 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 18 Dec 2020 02:43:31 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 18 Dec 2020 02:43:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Dec 2020 02:43:31 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072739d44e4fe2316d3bda5b6e0944796b1824cb2dee521ef06bf11e4f5db0fe`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 10.8 MB (10752737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5111f27e9600a1fa0a3a8660e8518294729a41abcd648bbf0ec9f60dcfb02b73`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 4.3 MB (4340690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8edcaa1ed5e299a41dda2ec21e02bcffc9984be150078569bf9537b855e2f`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13ba5490d638739d7649f595d300d9e5f3a94a9e8fccc862882ea39072091c3`  
		Last Modified: Fri, 18 Dec 2020 02:45:49 GMT  
		Size: 65.0 MB (64965934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad98b997807bdc5f0ba2dbc2b2d99209a2d4e967f4bd9b63091b9a3f02199b9`  
		Last Modified: Fri, 18 Dec 2020 02:45:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecdc57b1fad2cc5801e5f52560444b5d2456d8ae182a19591622d5938c81e074`  
		Last Modified: Fri, 18 Dec 2020 02:45:28 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bab1f0411eb3ce399ff56a568974c24d992a1015771229c5a2343560d68497e`  
		Last Modified: Fri, 18 Dec 2020 02:45:28 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:b099bdd1f4306689fd11c02f83b3de7fc11eccd8debf5f345e9be11d0a7cd7dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116548072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e315d6ff66902df2ef37f85938d60bf8e96760230a8d5ee593ad7f0f6e7e80`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:19 GMT
ADD file:9c744a203d36aa8c515bbc11873a4a479cdf3fe9f020ca1ef207b53e6b3a251e in / 
# Tue, 12 Jan 2021 00:05:23 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:21:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 17:20:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 17:20:45 GMT
ENV INFLUXDB_VERSION=1.8.3
# Tue, 12 Jan 2021 17:20:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 12 Jan 2021 17:20:56 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 12 Jan 2021 17:20:57 GMT
EXPOSE 8086
# Tue, 12 Jan 2021 17:20:58 GMT
VOLUME [/var/lib/influxdb]
# Tue, 12 Jan 2021 17:20:58 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 12 Jan 2021 17:20:59 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 12 Jan 2021 17:21:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 17:21:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f5de2649c1cd9091872f81b8ceb6a67890124f113d9fce9c52bf60d5a6e19f43`  
		Last Modified: Tue, 12 Jan 2021 00:15:23 GMT  
		Size: 42.1 MB (42119951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cae60aac6e598935e2b14216dc4265434ba03d17c82f622b18abb712577d2c`  
		Last Modified: Tue, 12 Jan 2021 01:34:01 GMT  
		Size: 9.4 MB (9446203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9694e28a75917ff08caeaee5ed8729a2f12d2110bf203781d578006a0ef2f7`  
		Last Modified: Tue, 12 Jan 2021 01:33:59 GMT  
		Size: 3.9 MB (3919958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9af4291e32292c1b3e0baa3521c9903226273223480ec660c81d82cec54e2b`  
		Last Modified: Tue, 12 Jan 2021 17:21:15 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc25c2db575e35a675a00c4c4a6d0f737064cc0789ae70ad0fa214115eac480`  
		Last Modified: Tue, 12 Jan 2021 17:22:04 GMT  
		Size: 61.1 MB (61057389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309ce3cfceae39ef043c05cbcaf2d3443f8d4b6d2e7bbb35acdab440f655b62d`  
		Last Modified: Tue, 12 Jan 2021 17:21:48 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0848e4c0b723e7b1c138100af0c50a5197705e68c522c35815519c5c4b64610d`  
		Last Modified: Tue, 12 Jan 2021 17:21:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e532b4cfca353c580548792aea8a7e5dc17fdbed3b8606c0ec3640fd6d0524`  
		Last Modified: Tue, 12 Jan 2021 17:21:48 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:116afd3662c995818965acbc3f515851eb8b59b081852ee633b6516d83a343bd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117605732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a83e931cfa467a4db3127999749502aa87a922ddb52333257a88cfe89e012dde`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 11 Dec 2020 02:48:16 GMT
ADD file:48e44714f486662ed380343e556f0f7411bd6600d916440063753c55d1f94b45 in / 
# Fri, 11 Dec 2020 02:48:17 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 10:13:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 10:13:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 15:25:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 17 Dec 2020 15:26:52 GMT
ENV INFLUXDB_VERSION=1.8.3
# Thu, 17 Dec 2020 15:27:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 17 Dec 2020 15:27:02 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 17 Dec 2020 15:27:03 GMT
EXPOSE 8086
# Thu, 17 Dec 2020 15:27:03 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 15:27:04 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 17 Dec 2020 15:27:05 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Dec 2020 15:27:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 15:27:07 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:ecefb91918e846819df74a1beb8e41f454bef156738373818c20656a3a46d5f7`  
		Last Modified: Fri, 11 Dec 2020 02:55:36 GMT  
		Size: 43.2 MB (43175941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda9a63f37e7beb33012f80c0f66755ce6d87a51fde0a283a06dbdf2857ce533`  
		Last Modified: Thu, 17 Dec 2020 10:41:45 GMT  
		Size: 9.7 MB (9702906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0c493446fd68c6abee0df0169e849bcb73aa61a86ba5e30783c9b5298007b7`  
		Last Modified: Thu, 17 Dec 2020 10:41:43 GMT  
		Size: 4.1 MB (4095483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a00a8a57199af4c15740e382214257dc71414c8a40b544ffcd0d9f53ce2404c`  
		Last Modified: Thu, 17 Dec 2020 15:27:23 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ed1589af262d0f6104eceb471392d09eff5421d4669f06e2c9054545965652`  
		Last Modified: Thu, 17 Dec 2020 15:27:58 GMT  
		Size: 60.6 MB (60626832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4054772c2c83698fb81c7e810b3698c46ad0ee08ad658c2d70ab1481f90ca177`  
		Last Modified: Thu, 17 Dec 2020 15:27:46 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0f7491941e8bc9638ce33e93b5d9e88ace69570e4a88ca8f0d2a2125969333`  
		Last Modified: Thu, 17 Dec 2020 15:27:45 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db28bc4ec64e21181ce4865c49ef34edec20ff9c09a4166fd920a2fe64950ebc`  
		Last Modified: Thu, 17 Dec 2020 15:27:45 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:ae646819f963fb00e7c01984626b8442efbfb5e1ab3dddde58e0d5f6c3f15899
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:556ccc3ace6d88c6c9739b8e27ab5e88f1a22cfc302a2444b95379cd8d6ea303
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83339700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd04b7b31146bbc9d25c819dcc0a5841a8fc12d4bc0da47a5113d35a962a06c1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 17:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 17:01:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 02:42:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 18 Dec 2020 02:43:39 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Fri, 18 Dec 2020 02:43:58 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 18 Dec 2020 02:43:58 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 18 Dec 2020 02:43:58 GMT
EXPOSE 8091
# Fri, 18 Dec 2020 02:43:59 GMT
VOLUME [/var/lib/influxdb]
# Fri, 18 Dec 2020 02:43:59 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 18 Dec 2020 02:43:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Dec 2020 02:43:59 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072739d44e4fe2316d3bda5b6e0944796b1824cb2dee521ef06bf11e4f5db0fe`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 10.8 MB (10752737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5111f27e9600a1fa0a3a8660e8518294729a41abcd648bbf0ec9f60dcfb02b73`  
		Last Modified: Thu, 17 Dec 2020 17:27:45 GMT  
		Size: 4.3 MB (4340690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8edcaa1ed5e299a41dda2ec21e02bcffc9984be150078569bf9537b855e2f`  
		Last Modified: Fri, 18 Dec 2020 02:44:38 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82550fa0125499a3c848b35ecfd0a5d0ece26c5ffd8b6b88657b4199e945327f`  
		Last Modified: Fri, 18 Dec 2020 02:46:20 GMT  
		Size: 22.9 MB (22865271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a106d8f0f18ca0e190aede94b9ab2b2adf418d5d5544aaf340c86af12ee445ed`  
		Last Modified: Fri, 18 Dec 2020 02:46:16 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798fd3ed5f538287b703b25f8c9a0a1094be537cca8d259f802eb64c2a6efbb3`  
		Last Modified: Fri, 18 Dec 2020 02:46:16 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta-alpine`

```console
$ docker pull influxdb@sha256:4c29eac32909a131cfaff0592d154d70dd7dfe0478cb9540c2901ddf0da5fae7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:dca974575db512c53831bde49ddf78ac0dcf4d82dc22079be452c62da4ba5682
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (26963560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8881cbf80321dc2a4ebdf2195439034efa5d7c8d21b315de81395c705b9129c8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:47:22 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 17 Dec 2020 13:48:32 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Thu, 17 Dec 2020 13:48:52 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:48:52 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 17 Dec 2020 13:48:53 GMT
EXPOSE 8091
# Thu, 17 Dec 2020 13:48:53 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Dec 2020 13:48:54 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:48:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:48:54 GMT
CMD ["influxd-meta"]
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
	-	`sha256:1924738bc6407d8319fdb7d3fca610b5972213dee7ad608f4d801b3990f11a21`  
		Last Modified: Thu, 17 Dec 2020 13:49:35 GMT  
		Size: 1.4 MB (1428296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160bf10769c16bdb7542730ceba295bdfb41ccdcc94aad7899def6ebc89b50f5`  
		Last Modified: Thu, 17 Dec 2020 13:51:26 GMT  
		Size: 22.7 MB (22735478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc8f9cb3bd7cd3e189107cbd62ad4c10e03619dda2334334e9472e68bed697b`  
		Last Modified: Thu, 17 Dec 2020 13:51:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74170b5ea5a39ad5a9878ee9a90ab8f39e7d7331d10ead82b0ed7f28cd4f007`  
		Last Modified: Thu, 17 Dec 2020 13:51:22 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
