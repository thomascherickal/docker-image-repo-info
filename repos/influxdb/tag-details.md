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
-	[`influxdb:1.8.1`](#influxdb181)
-	[`influxdb:1.8.1-alpine`](#influxdb181-alpine)
-	[`influxdb:1.8.1-data`](#influxdb181-data)
-	[`influxdb:1.8.1-data-alpine`](#influxdb181-data-alpine)
-	[`influxdb:1.8.1-meta`](#influxdb181-meta)
-	[`influxdb:1.8.1-meta-alpine`](#influxdb181-meta-alpine)
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
$ docker pull influxdb@sha256:719906adf2d0f83961de6c32858265044873b6644379b1c54b6903f558bf8b0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7` - linux; amd64

```console
$ docker pull influxdb@sha256:ab949daf5024bf57e4cba186e9d6026e94dd01c4181591a0462b8d92dd1c1cf0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124566140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82fde2c0e9a081066f7d9495a362056a72e83194b70b9368004bd0faad84d82e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:43:24 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 10 Jun 2020 02:43:24 GMT
ENV INFLUXDB_VERSION=1.7.10
# Wed, 10 Jun 2020 02:43:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 10 Jun 2020 02:43:32 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 10 Jun 2020 02:43:32 GMT
EXPOSE 8086
# Wed, 10 Jun 2020 02:43:32 GMT
VOLUME [/var/lib/influxdb]
# Wed, 10 Jun 2020 02:43:32 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 10 Jun 2020 02:43:33 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 10 Jun 2020 02:43:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 02:43:33 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e4835694e137bd4973eca79a9bb485066fb4b944fe90b33abadbdf75863b4a`  
		Last Modified: Wed, 10 Jun 2020 02:45:11 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79df916ec569f85f61591b10c9612bcd41b06820e04d6219b580dd4a8669ac95`  
		Last Modified: Wed, 10 Jun 2020 02:45:20 GMT  
		Size: 64.1 MB (64096946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7cac0fe28688c9ea936fac8734f24c4b6afe4a38bbb11a7bf4b4f30faa70f1`  
		Last Modified: Wed, 10 Jun 2020 02:45:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9dfbe934719c8e11a78ebfae40f7388ba515bdd84253265ff2dcc8f7e2ec71`  
		Last Modified: Wed, 10 Jun 2020 02:45:10 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e806aeeedbdfc28a4d54843de1d95559ed2f03a9630c7c019d3fc095967a33bb`  
		Last Modified: Wed, 10 Jun 2020 02:45:11 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:316f506c80f71789e78ac98b5236987d4773f466b899a9693c37e84013ae835d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.1 MB (116104309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aad8052c631089f7fc01c018fc9b98441ec8f0d0c4a226363c7e5d336e7dcfae`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:07 GMT
ADD file:c0b9ed1244ec0acfc9054c7cb80c768878e3da99740f981ba3a82bdd854305db in / 
# Tue, 09 Jun 2020 01:06:09 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:02:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:02:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 18:42:50 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Jun 2020 18:42:51 GMT
ENV INFLUXDB_VERSION=1.7.10
# Tue, 09 Jun 2020 18:43:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 09 Jun 2020 18:43:02 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 09 Jun 2020 18:43:03 GMT
EXPOSE 8086
# Tue, 09 Jun 2020 18:43:03 GMT
VOLUME [/var/lib/influxdb]
# Tue, 09 Jun 2020 18:43:04 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 09 Jun 2020 18:43:05 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 09 Jun 2020 18:43:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Jun 2020 18:43:06 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:2566ca784846d2d0d4f9105084d94d68d8ea1a82a06a76c5bcd991ce5a10cda1`  
		Last Modified: Tue, 09 Jun 2020 01:13:35 GMT  
		Size: 42.1 MB (42102504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f976b5a12722f5e6e115157695654d36452b713c7fa64a860f8c9e14859402`  
		Last Modified: Tue, 09 Jun 2020 02:15:15 GMT  
		Size: 9.4 MB (9443335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35142ef6ea6c722cd0397799ab151e5da354eabc784b3acef29def7fa34e9bc`  
		Last Modified: Tue, 09 Jun 2020 02:15:13 GMT  
		Size: 3.9 MB (3918433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c8981f961756294156fe1f662892a0a0ab88baf5d457700d5fade1752d133`  
		Last Modified: Tue, 09 Jun 2020 18:43:39 GMT  
		Size: 2.8 KB (2801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1450f8816523df3085384145b8aa97820eefa981b7d3c8c64bb5d647874ec8ed`  
		Last Modified: Tue, 09 Jun 2020 18:43:58 GMT  
		Size: 60.6 MB (60635520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff3800bad7aedc077150df5c6acf4adfb9acac67eeca49c24dfe402bbfaad23`  
		Last Modified: Tue, 09 Jun 2020 18:43:39 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be33424cd202a051045696740451eaededc2619f9b7be438f947486ed6d91a38`  
		Last Modified: Tue, 09 Jun 2020 18:43:39 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3efe3a68df7de2c7d8c5597b3c3f25579df4d3d9053c10cd800cd1b308bcf9`  
		Last Modified: Tue, 09 Jun 2020 18:43:39 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4cf2bbefe215c9e6dee3faa5a502289ee45ea2e4431e3b12e096a8758cb767e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.1 MB (117086934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe20eb3597b293334cb9d26c773867c08adad74956f83176c6ee69d20f86f093`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:22 GMT
ADD file:5cbf00485aed776e940988cadfad6853c640c13635ae54fb2b00aafccfe81a73 in / 
# Tue, 09 Jun 2020 01:54:25 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 21:50:27 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Jun 2020 21:50:28 GMT
ENV INFLUXDB_VERSION=1.7.10
# Tue, 09 Jun 2020 21:50:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 09 Jun 2020 21:50:42 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 09 Jun 2020 21:50:44 GMT
EXPOSE 8086
# Tue, 09 Jun 2020 21:50:46 GMT
VOLUME [/var/lib/influxdb]
# Tue, 09 Jun 2020 21:50:47 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 09 Jun 2020 21:50:48 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 09 Jun 2020 21:50:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Jun 2020 21:50:56 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:4c4f692ec920eecb1f30d9ef8e50125217decc872d7ada6eeccc36c6dcb49e4d`  
		Last Modified: Tue, 09 Jun 2020 02:00:09 GMT  
		Size: 43.2 MB (43160923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0990c417a21ef9e268cc0822cd23968c4b17cded8170cce0c4d8f7e020e6fd`  
		Last Modified: Tue, 09 Jun 2020 02:50:17 GMT  
		Size: 9.7 MB (9699635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6b83fd41426d182f67fdac882a6bfcd3aad22d7226a653ae58d3046bd46b5e`  
		Last Modified: Tue, 09 Jun 2020 02:50:15 GMT  
		Size: 4.1 MB (4094104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039c1b8b197fb87df9fbb2ea446d6a6608957e69c6af971e06bf2040595482aa`  
		Last Modified: Tue, 09 Jun 2020 21:51:40 GMT  
		Size: 2.8 KB (2803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f28e5fe788b39b28bf311da9c135972dcfb196e686be2485ddce88c0a491261`  
		Last Modified: Tue, 09 Jun 2020 21:51:58 GMT  
		Size: 60.1 MB (60127754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fde6264cfd17f853a1c45eb2d3a11457fb48f34357a1194558ed7ffd5294ff`  
		Last Modified: Tue, 09 Jun 2020 21:51:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6dc9ca58d502d398c5b2dff153aeefe7803eaadde66c3c7750148f7f01078b`  
		Last Modified: Tue, 09 Jun 2020 21:51:40 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ace20a8141eba141018690c41f177091ace88da271d26fbbde05cbf603702ca`  
		Last Modified: Tue, 09 Jun 2020 21:51:40 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.10`

```console
$ docker pull influxdb@sha256:719906adf2d0f83961de6c32858265044873b6644379b1c54b6903f558bf8b0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7.10` - linux; amd64

```console
$ docker pull influxdb@sha256:ab949daf5024bf57e4cba186e9d6026e94dd01c4181591a0462b8d92dd1c1cf0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124566140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82fde2c0e9a081066f7d9495a362056a72e83194b70b9368004bd0faad84d82e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:43:24 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 10 Jun 2020 02:43:24 GMT
ENV INFLUXDB_VERSION=1.7.10
# Wed, 10 Jun 2020 02:43:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 10 Jun 2020 02:43:32 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 10 Jun 2020 02:43:32 GMT
EXPOSE 8086
# Wed, 10 Jun 2020 02:43:32 GMT
VOLUME [/var/lib/influxdb]
# Wed, 10 Jun 2020 02:43:32 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 10 Jun 2020 02:43:33 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 10 Jun 2020 02:43:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 02:43:33 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e4835694e137bd4973eca79a9bb485066fb4b944fe90b33abadbdf75863b4a`  
		Last Modified: Wed, 10 Jun 2020 02:45:11 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79df916ec569f85f61591b10c9612bcd41b06820e04d6219b580dd4a8669ac95`  
		Last Modified: Wed, 10 Jun 2020 02:45:20 GMT  
		Size: 64.1 MB (64096946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7cac0fe28688c9ea936fac8734f24c4b6afe4a38bbb11a7bf4b4f30faa70f1`  
		Last Modified: Wed, 10 Jun 2020 02:45:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9dfbe934719c8e11a78ebfae40f7388ba515bdd84253265ff2dcc8f7e2ec71`  
		Last Modified: Wed, 10 Jun 2020 02:45:10 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e806aeeedbdfc28a4d54843de1d95559ed2f03a9630c7c019d3fc095967a33bb`  
		Last Modified: Wed, 10 Jun 2020 02:45:11 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:316f506c80f71789e78ac98b5236987d4773f466b899a9693c37e84013ae835d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.1 MB (116104309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aad8052c631089f7fc01c018fc9b98441ec8f0d0c4a226363c7e5d336e7dcfae`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:07 GMT
ADD file:c0b9ed1244ec0acfc9054c7cb80c768878e3da99740f981ba3a82bdd854305db in / 
# Tue, 09 Jun 2020 01:06:09 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:02:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:02:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 18:42:50 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Jun 2020 18:42:51 GMT
ENV INFLUXDB_VERSION=1.7.10
# Tue, 09 Jun 2020 18:43:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 09 Jun 2020 18:43:02 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 09 Jun 2020 18:43:03 GMT
EXPOSE 8086
# Tue, 09 Jun 2020 18:43:03 GMT
VOLUME [/var/lib/influxdb]
# Tue, 09 Jun 2020 18:43:04 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 09 Jun 2020 18:43:05 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 09 Jun 2020 18:43:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Jun 2020 18:43:06 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:2566ca784846d2d0d4f9105084d94d68d8ea1a82a06a76c5bcd991ce5a10cda1`  
		Last Modified: Tue, 09 Jun 2020 01:13:35 GMT  
		Size: 42.1 MB (42102504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f976b5a12722f5e6e115157695654d36452b713c7fa64a860f8c9e14859402`  
		Last Modified: Tue, 09 Jun 2020 02:15:15 GMT  
		Size: 9.4 MB (9443335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35142ef6ea6c722cd0397799ab151e5da354eabc784b3acef29def7fa34e9bc`  
		Last Modified: Tue, 09 Jun 2020 02:15:13 GMT  
		Size: 3.9 MB (3918433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c8981f961756294156fe1f662892a0a0ab88baf5d457700d5fade1752d133`  
		Last Modified: Tue, 09 Jun 2020 18:43:39 GMT  
		Size: 2.8 KB (2801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1450f8816523df3085384145b8aa97820eefa981b7d3c8c64bb5d647874ec8ed`  
		Last Modified: Tue, 09 Jun 2020 18:43:58 GMT  
		Size: 60.6 MB (60635520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff3800bad7aedc077150df5c6acf4adfb9acac67eeca49c24dfe402bbfaad23`  
		Last Modified: Tue, 09 Jun 2020 18:43:39 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be33424cd202a051045696740451eaededc2619f9b7be438f947486ed6d91a38`  
		Last Modified: Tue, 09 Jun 2020 18:43:39 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3efe3a68df7de2c7d8c5597b3c3f25579df4d3d9053c10cd800cd1b308bcf9`  
		Last Modified: Tue, 09 Jun 2020 18:43:39 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4cf2bbefe215c9e6dee3faa5a502289ee45ea2e4431e3b12e096a8758cb767e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.1 MB (117086934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe20eb3597b293334cb9d26c773867c08adad74956f83176c6ee69d20f86f093`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:22 GMT
ADD file:5cbf00485aed776e940988cadfad6853c640c13635ae54fb2b00aafccfe81a73 in / 
# Tue, 09 Jun 2020 01:54:25 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 21:50:27 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Jun 2020 21:50:28 GMT
ENV INFLUXDB_VERSION=1.7.10
# Tue, 09 Jun 2020 21:50:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 09 Jun 2020 21:50:42 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 09 Jun 2020 21:50:44 GMT
EXPOSE 8086
# Tue, 09 Jun 2020 21:50:46 GMT
VOLUME [/var/lib/influxdb]
# Tue, 09 Jun 2020 21:50:47 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 09 Jun 2020 21:50:48 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 09 Jun 2020 21:50:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Jun 2020 21:50:56 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:4c4f692ec920eecb1f30d9ef8e50125217decc872d7ada6eeccc36c6dcb49e4d`  
		Last Modified: Tue, 09 Jun 2020 02:00:09 GMT  
		Size: 43.2 MB (43160923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0990c417a21ef9e268cc0822cd23968c4b17cded8170cce0c4d8f7e020e6fd`  
		Last Modified: Tue, 09 Jun 2020 02:50:17 GMT  
		Size: 9.7 MB (9699635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6b83fd41426d182f67fdac882a6bfcd3aad22d7226a653ae58d3046bd46b5e`  
		Last Modified: Tue, 09 Jun 2020 02:50:15 GMT  
		Size: 4.1 MB (4094104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039c1b8b197fb87df9fbb2ea446d6a6608957e69c6af971e06bf2040595482aa`  
		Last Modified: Tue, 09 Jun 2020 21:51:40 GMT  
		Size: 2.8 KB (2803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f28e5fe788b39b28bf311da9c135972dcfb196e686be2485ddce88c0a491261`  
		Last Modified: Tue, 09 Jun 2020 21:51:58 GMT  
		Size: 60.1 MB (60127754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fde6264cfd17f853a1c45eb2d3a11457fb48f34357a1194558ed7ffd5294ff`  
		Last Modified: Tue, 09 Jun 2020 21:51:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6dc9ca58d502d398c5b2dff153aeefe7803eaadde66c3c7750148f7f01078b`  
		Last Modified: Tue, 09 Jun 2020 21:51:40 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ace20a8141eba141018690c41f177091ace88da271d26fbbde05cbf603702ca`  
		Last Modified: Tue, 09 Jun 2020 21:51:40 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.10-alpine`

```console
$ docker pull influxdb@sha256:d8ea9d1d96dd69eb63d0c6f7c848604df8a3e5d3c193051e2b825d3856ba30fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.10-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:849cc2ab7ef9942f036c052f0f3d3bc4cd0695438655d0b9b5460bec52603d0a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68530277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e25540c816202585a6fae4637c76572d11fb7b5876158b668aaa6a104ac2cfb2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 15:28:09 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 15:28:09 GMT
ENV INFLUXDB_VERSION=1.7.10
# Fri, 24 Apr 2020 15:28:18 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 15:28:18 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 24 Apr 2020 15:28:18 GMT
EXPOSE 8086
# Fri, 24 Apr 2020 15:28:18 GMT
VOLUME [/var/lib/influxdb]
# Fri, 24 Apr 2020 15:28:19 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 24 Apr 2020 15:28:19 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 24 Apr 2020 15:28:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 15:28:19 GMT
CMD ["influxd"]
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
	-	`sha256:c9984b0a697389d40ad58252364c9cbb4e4a5258602767230a8f149134746718`  
		Last Modified: Fri, 24 Apr 2020 15:30:04 GMT  
		Size: 1.9 MB (1863602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3deadc9a03ce9d7f0df4d8daeb5c1c14bed2da992ea25959d92429347c3a7750`  
		Last Modified: Fri, 24 Apr 2020 15:30:13 GMT  
		Size: 63.9 MB (63891399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e03c842a2b43e7a3e90fc111f9a31b46a3c571602ff6c88d68f0cb83031487f`  
		Last Modified: Fri, 24 Apr 2020 15:30:03 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db77010b7e69bbb82798640c2a5592f7b3b061034f82ec952f5d40194306016`  
		Last Modified: Fri, 24 Apr 2020 15:30:04 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f9223aa73b313d67a35777833eb832c3207ee6b6f2331d8491abde40ebf22e`  
		Last Modified: Fri, 24 Apr 2020 15:30:04 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.10-data`

```console
$ docker pull influxdb@sha256:077630b6d1af956d11cc63cc77e09e8464d242621bb53f8954fd57d38549174e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:00e1416db792cf76e14a902d39d2d086bbeb16be8e74772fb19707d9b6ed533b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.4 MB (148381505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3f951cb4ac6939fc728bc39257c39f5b30fd2f0390327e742fbfaf1ab113474`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:43:24 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 10 Jun 2020 02:43:41 GMT
ENV INFLUXDB_VERSION=1.7.10-c1.7.10
# Wed, 10 Jun 2020 02:43:50 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 10 Jun 2020 02:43:50 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 10 Jun 2020 02:43:50 GMT
EXPOSE 8086
# Wed, 10 Jun 2020 02:43:51 GMT
VOLUME [/var/lib/influxdb]
# Wed, 10 Jun 2020 02:43:51 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 10 Jun 2020 02:43:51 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 10 Jun 2020 02:43:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 02:43:51 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e4835694e137bd4973eca79a9bb485066fb4b944fe90b33abadbdf75863b4a`  
		Last Modified: Wed, 10 Jun 2020 02:45:11 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fbb8c51cb20946eda0076cea910f7eeba69a40f95ef161c819c0b143b0012b`  
		Last Modified: Wed, 10 Jun 2020 02:45:39 GMT  
		Size: 87.9 MB (87912253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f420755ed80c4ef6ae231d8aaebd37e7c89d10794e5fa2bc2f4a51828ce00974`  
		Last Modified: Wed, 10 Jun 2020 02:45:27 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1292dd9cb23d7c178207b0129ade5227c58cc5f1f7dee7e6dc09dfd85b5f25be`  
		Last Modified: Wed, 10 Jun 2020 02:45:26 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7719a17057cb669b11b55bb474ca2813599687e21c54d2424910113b1ab043da`  
		Last Modified: Wed, 10 Jun 2020 02:45:27 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.10-data-alpine`

```console
$ docker pull influxdb@sha256:6f250d7b1cc13d3b798789d480d82bdf0ffea2004e44d563619b0b397b088ec7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.10-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:70a708452c2a1ff2c4fe2cad36847aa83ca1b5d9b80a5ecc16579118e9b544a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92308348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bae5cbf4e52e5b3da9fbfdee13fcd1e5806ca3f8cfad3d19ef8ae5064ef6b69f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 15:28:09 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 15:28:26 GMT
ENV INFLUXDB_VERSION=1.7.10-c1.7.10
# Fri, 24 Apr 2020 15:28:38 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 15:28:38 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 24 Apr 2020 15:28:38 GMT
EXPOSE 8086
# Fri, 24 Apr 2020 15:28:39 GMT
VOLUME [/var/lib/influxdb]
# Fri, 24 Apr 2020 15:28:39 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 24 Apr 2020 15:28:39 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 24 Apr 2020 15:28:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 15:28:39 GMT
CMD ["influxd"]
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
	-	`sha256:c9984b0a697389d40ad58252364c9cbb4e4a5258602767230a8f149134746718`  
		Last Modified: Fri, 24 Apr 2020 15:30:04 GMT  
		Size: 1.9 MB (1863602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8edd32b853201f14ebc1936e706d17eb835091b987588bea9264a45758b1b81c`  
		Last Modified: Fri, 24 Apr 2020 15:30:32 GMT  
		Size: 87.7 MB (87669411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24b53788b2bbcd58690fc7ef76c7ea9c1eceff1796a093161fe8ed3de0530cd`  
		Last Modified: Fri, 24 Apr 2020 15:30:19 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232bedee238d45217ce15f43133f9f8cebe172f996e449793704111099486c52`  
		Last Modified: Fri, 24 Apr 2020 15:30:19 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06db629dfa54d5a6727c4f73b214d90437d3640cd6bde265a8b861edc687cda`  
		Last Modified: Fri, 24 Apr 2020 15:30:19 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.10-meta`

```console
$ docker pull influxdb@sha256:99410a403a49a5203bc75e8ab8b65cf5e8195d08c4a5cec35fbffeb16330e1fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:76f298db97df7bf063fdcb1aa7841f620f585574a4960c6039478e4dbe211d5a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.6 MB (83600689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a08599e6865f78b6689cc81200e9f5b39f66a0b7742d2e0675635f30ce4214a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:43:24 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 10 Jun 2020 02:43:41 GMT
ENV INFLUXDB_VERSION=1.7.10-c1.7.10
# Wed, 10 Jun 2020 02:44:05 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 10 Jun 2020 02:44:05 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 10 Jun 2020 02:44:05 GMT
EXPOSE 8091
# Wed, 10 Jun 2020 02:44:05 GMT
VOLUME [/var/lib/influxdb]
# Wed, 10 Jun 2020 02:44:05 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 10 Jun 2020 02:44:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 02:44:06 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e4835694e137bd4973eca79a9bb485066fb4b944fe90b33abadbdf75863b4a`  
		Last Modified: Wed, 10 Jun 2020 02:45:11 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559e270ef08b84c5740a2765401c83163833f141143e300fc73dba4c795aa267`  
		Last Modified: Wed, 10 Jun 2020 02:45:48 GMT  
		Size: 23.1 MB (23132641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef5caaff96d2a3f9214bb2d934b3b30b885d0ba226373bedacf3df99b2b869e`  
		Last Modified: Wed, 10 Jun 2020 02:45:45 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e4b5394efbed7f4da90eccc852bd818f0e4f3add12087a833be0281592360f`  
		Last Modified: Wed, 10 Jun 2020 02:45:45 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.10-meta-alpine`

```console
$ docker pull influxdb@sha256:a9cc22461d2f36bc3794b09dc6878f51b5d34d635475c89c9bce4b3582642642
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.10-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:83006300e441c3d613b679f74ceeaf2b858635500e894bfdabb0f4165e85c8e5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27703385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d488e358e094fb5a4b10c46a25792a62288d03a3912d8321d91f20fb5d9416a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 15:28:09 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 15:28:26 GMT
ENV INFLUXDB_VERSION=1.7.10-c1.7.10
# Fri, 24 Apr 2020 15:28:52 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 15:28:53 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 24 Apr 2020 15:28:53 GMT
EXPOSE 8091
# Fri, 24 Apr 2020 15:28:53 GMT
VOLUME [/var/lib/influxdb]
# Fri, 24 Apr 2020 15:28:53 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 24 Apr 2020 15:28:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 15:28:53 GMT
CMD ["influxd-meta"]
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
	-	`sha256:c9984b0a697389d40ad58252364c9cbb4e4a5258602767230a8f149134746718`  
		Last Modified: Fri, 24 Apr 2020 15:30:04 GMT  
		Size: 1.9 MB (1863602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ff89aa062bdb7a1a80129c8bcce60d7d6dd691a149c073e74c0876616ed43a`  
		Last Modified: Fri, 24 Apr 2020 15:30:39 GMT  
		Size: 23.1 MB (23065649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3663bb55eb8ab96716ac08e09fa1c7f6d3758caa9d115dca19be9a19c507859e`  
		Last Modified: Fri, 24 Apr 2020 15:30:36 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7a9206a9f14558d5470916b3124349a4575f6ecead7a899ca34c3fcb59ef0f`  
		Last Modified: Fri, 24 Apr 2020 15:30:36 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-alpine`

```console
$ docker pull influxdb@sha256:d8ea9d1d96dd69eb63d0c6f7c848604df8a3e5d3c193051e2b825d3856ba30fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:849cc2ab7ef9942f036c052f0f3d3bc4cd0695438655d0b9b5460bec52603d0a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68530277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e25540c816202585a6fae4637c76572d11fb7b5876158b668aaa6a104ac2cfb2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 15:28:09 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 15:28:09 GMT
ENV INFLUXDB_VERSION=1.7.10
# Fri, 24 Apr 2020 15:28:18 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 15:28:18 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 24 Apr 2020 15:28:18 GMT
EXPOSE 8086
# Fri, 24 Apr 2020 15:28:18 GMT
VOLUME [/var/lib/influxdb]
# Fri, 24 Apr 2020 15:28:19 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 24 Apr 2020 15:28:19 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 24 Apr 2020 15:28:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 15:28:19 GMT
CMD ["influxd"]
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
	-	`sha256:c9984b0a697389d40ad58252364c9cbb4e4a5258602767230a8f149134746718`  
		Last Modified: Fri, 24 Apr 2020 15:30:04 GMT  
		Size: 1.9 MB (1863602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3deadc9a03ce9d7f0df4d8daeb5c1c14bed2da992ea25959d92429347c3a7750`  
		Last Modified: Fri, 24 Apr 2020 15:30:13 GMT  
		Size: 63.9 MB (63891399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e03c842a2b43e7a3e90fc111f9a31b46a3c571602ff6c88d68f0cb83031487f`  
		Last Modified: Fri, 24 Apr 2020 15:30:03 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db77010b7e69bbb82798640c2a5592f7b3b061034f82ec952f5d40194306016`  
		Last Modified: Fri, 24 Apr 2020 15:30:04 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f9223aa73b313d67a35777833eb832c3207ee6b6f2331d8491abde40ebf22e`  
		Last Modified: Fri, 24 Apr 2020 15:30:04 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data`

```console
$ docker pull influxdb@sha256:077630b6d1af956d11cc63cc77e09e8464d242621bb53f8954fd57d38549174e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-data` - linux; amd64

```console
$ docker pull influxdb@sha256:00e1416db792cf76e14a902d39d2d086bbeb16be8e74772fb19707d9b6ed533b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.4 MB (148381505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3f951cb4ac6939fc728bc39257c39f5b30fd2f0390327e742fbfaf1ab113474`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:43:24 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 10 Jun 2020 02:43:41 GMT
ENV INFLUXDB_VERSION=1.7.10-c1.7.10
# Wed, 10 Jun 2020 02:43:50 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 10 Jun 2020 02:43:50 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 10 Jun 2020 02:43:50 GMT
EXPOSE 8086
# Wed, 10 Jun 2020 02:43:51 GMT
VOLUME [/var/lib/influxdb]
# Wed, 10 Jun 2020 02:43:51 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 10 Jun 2020 02:43:51 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 10 Jun 2020 02:43:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 02:43:51 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e4835694e137bd4973eca79a9bb485066fb4b944fe90b33abadbdf75863b4a`  
		Last Modified: Wed, 10 Jun 2020 02:45:11 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fbb8c51cb20946eda0076cea910f7eeba69a40f95ef161c819c0b143b0012b`  
		Last Modified: Wed, 10 Jun 2020 02:45:39 GMT  
		Size: 87.9 MB (87912253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f420755ed80c4ef6ae231d8aaebd37e7c89d10794e5fa2bc2f4a51828ce00974`  
		Last Modified: Wed, 10 Jun 2020 02:45:27 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1292dd9cb23d7c178207b0129ade5227c58cc5f1f7dee7e6dc09dfd85b5f25be`  
		Last Modified: Wed, 10 Jun 2020 02:45:26 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7719a17057cb669b11b55bb474ca2813599687e21c54d2424910113b1ab043da`  
		Last Modified: Wed, 10 Jun 2020 02:45:27 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data-alpine`

```console
$ docker pull influxdb@sha256:6f250d7b1cc13d3b798789d480d82bdf0ffea2004e44d563619b0b397b088ec7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:70a708452c2a1ff2c4fe2cad36847aa83ca1b5d9b80a5ecc16579118e9b544a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92308348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bae5cbf4e52e5b3da9fbfdee13fcd1e5806ca3f8cfad3d19ef8ae5064ef6b69f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 15:28:09 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 15:28:26 GMT
ENV INFLUXDB_VERSION=1.7.10-c1.7.10
# Fri, 24 Apr 2020 15:28:38 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 15:28:38 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 24 Apr 2020 15:28:38 GMT
EXPOSE 8086
# Fri, 24 Apr 2020 15:28:39 GMT
VOLUME [/var/lib/influxdb]
# Fri, 24 Apr 2020 15:28:39 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 24 Apr 2020 15:28:39 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 24 Apr 2020 15:28:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 15:28:39 GMT
CMD ["influxd"]
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
	-	`sha256:c9984b0a697389d40ad58252364c9cbb4e4a5258602767230a8f149134746718`  
		Last Modified: Fri, 24 Apr 2020 15:30:04 GMT  
		Size: 1.9 MB (1863602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8edd32b853201f14ebc1936e706d17eb835091b987588bea9264a45758b1b81c`  
		Last Modified: Fri, 24 Apr 2020 15:30:32 GMT  
		Size: 87.7 MB (87669411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24b53788b2bbcd58690fc7ef76c7ea9c1eceff1796a093161fe8ed3de0530cd`  
		Last Modified: Fri, 24 Apr 2020 15:30:19 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232bedee238d45217ce15f43133f9f8cebe172f996e449793704111099486c52`  
		Last Modified: Fri, 24 Apr 2020 15:30:19 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06db629dfa54d5a6727c4f73b214d90437d3640cd6bde265a8b861edc687cda`  
		Last Modified: Fri, 24 Apr 2020 15:30:19 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta`

```console
$ docker pull influxdb@sha256:99410a403a49a5203bc75e8ab8b65cf5e8195d08c4a5cec35fbffeb16330e1fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:76f298db97df7bf063fdcb1aa7841f620f585574a4960c6039478e4dbe211d5a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.6 MB (83600689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a08599e6865f78b6689cc81200e9f5b39f66a0b7742d2e0675635f30ce4214a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:43:24 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 10 Jun 2020 02:43:41 GMT
ENV INFLUXDB_VERSION=1.7.10-c1.7.10
# Wed, 10 Jun 2020 02:44:05 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 10 Jun 2020 02:44:05 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 10 Jun 2020 02:44:05 GMT
EXPOSE 8091
# Wed, 10 Jun 2020 02:44:05 GMT
VOLUME [/var/lib/influxdb]
# Wed, 10 Jun 2020 02:44:05 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 10 Jun 2020 02:44:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 02:44:06 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e4835694e137bd4973eca79a9bb485066fb4b944fe90b33abadbdf75863b4a`  
		Last Modified: Wed, 10 Jun 2020 02:45:11 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559e270ef08b84c5740a2765401c83163833f141143e300fc73dba4c795aa267`  
		Last Modified: Wed, 10 Jun 2020 02:45:48 GMT  
		Size: 23.1 MB (23132641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef5caaff96d2a3f9214bb2d934b3b30b885d0ba226373bedacf3df99b2b869e`  
		Last Modified: Wed, 10 Jun 2020 02:45:45 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e4b5394efbed7f4da90eccc852bd818f0e4f3add12087a833be0281592360f`  
		Last Modified: Wed, 10 Jun 2020 02:45:45 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta-alpine`

```console
$ docker pull influxdb@sha256:a9cc22461d2f36bc3794b09dc6878f51b5d34d635475c89c9bce4b3582642642
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:83006300e441c3d613b679f74ceeaf2b858635500e894bfdabb0f4165e85c8e5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27703385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d488e358e094fb5a4b10c46a25792a62288d03a3912d8321d91f20fb5d9416a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 15:28:09 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 15:28:26 GMT
ENV INFLUXDB_VERSION=1.7.10-c1.7.10
# Fri, 24 Apr 2020 15:28:52 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 15:28:53 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 24 Apr 2020 15:28:53 GMT
EXPOSE 8091
# Fri, 24 Apr 2020 15:28:53 GMT
VOLUME [/var/lib/influxdb]
# Fri, 24 Apr 2020 15:28:53 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 24 Apr 2020 15:28:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 15:28:53 GMT
CMD ["influxd-meta"]
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
	-	`sha256:c9984b0a697389d40ad58252364c9cbb4e4a5258602767230a8f149134746718`  
		Last Modified: Fri, 24 Apr 2020 15:30:04 GMT  
		Size: 1.9 MB (1863602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ff89aa062bdb7a1a80129c8bcce60d7d6dd691a149c073e74c0876616ed43a`  
		Last Modified: Fri, 24 Apr 2020 15:30:39 GMT  
		Size: 23.1 MB (23065649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3663bb55eb8ab96716ac08e09fa1c7f6d3758caa9d115dca19be9a19c507859e`  
		Last Modified: Fri, 24 Apr 2020 15:30:36 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7a9206a9f14558d5470916b3124349a4575f6ecead7a899ca34c3fcb59ef0f`  
		Last Modified: Fri, 24 Apr 2020 15:30:36 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8`

```console
$ docker pull influxdb@sha256:2c4ee7675963a8f5a388e7853f6e68a1fcabebd24ce386364356587ad374e047
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:9e7c9fd78802e882ac441b4a25ecf95437d27651888148a61cf646b1d57286e8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124427438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95750833bc56d19870063238f49dbd465a7ed51928963d43f8360005004be663`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:43:24 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 10 Jun 2020 02:44:13 GMT
ENV INFLUXDB_VERSION=1.8.0
# Wed, 10 Jun 2020 02:44:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 10 Jun 2020 02:44:20 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 10 Jun 2020 02:44:21 GMT
EXPOSE 8086
# Wed, 10 Jun 2020 02:44:22 GMT
VOLUME [/var/lib/influxdb]
# Wed, 10 Jun 2020 02:44:22 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 10 Jun 2020 02:44:22 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 10 Jun 2020 02:44:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 02:44:22 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e4835694e137bd4973eca79a9bb485066fb4b944fe90b33abadbdf75863b4a`  
		Last Modified: Wed, 10 Jun 2020 02:45:11 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05df09a184e99c772f1f2fb571d741cd42209bdf169fc84dd24a73836ea130e0`  
		Last Modified: Wed, 10 Jun 2020 02:46:01 GMT  
		Size: 64.0 MB (63958242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671fe28366cfee32412469096c3c784ee91255b10b42b71ec4c5909cfa2d40d5`  
		Last Modified: Wed, 10 Jun 2020 02:45:52 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36ec69a8c120ed9c7d731a9f9de448d6fd258eb42310646741ca9a1fb878aac`  
		Last Modified: Wed, 10 Jun 2020 02:45:52 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc93bd218ea315e4551227d83072e8a9e2ac29f86174b39331fa44f586956c14`  
		Last Modified: Wed, 10 Jun 2020 02:45:52 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:73f876e0c3bd02900f829d4884f53fdfffd7098dd572406ba549eed955bf821f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115627234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0866da0fd5bb684b2b9b13002956f1d9806bc8eac6d62a98bf1056d4268a25c6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:07 GMT
ADD file:c0b9ed1244ec0acfc9054c7cb80c768878e3da99740f981ba3a82bdd854305db in / 
# Tue, 09 Jun 2020 01:06:09 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:02:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:02:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 18:42:50 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Jun 2020 18:43:14 GMT
ENV INFLUXDB_VERSION=1.8.0
# Tue, 09 Jun 2020 18:43:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 09 Jun 2020 18:43:25 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 09 Jun 2020 18:43:25 GMT
EXPOSE 8086
# Tue, 09 Jun 2020 18:43:26 GMT
VOLUME [/var/lib/influxdb]
# Tue, 09 Jun 2020 18:43:26 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 09 Jun 2020 18:43:27 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 09 Jun 2020 18:43:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Jun 2020 18:43:28 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:2566ca784846d2d0d4f9105084d94d68d8ea1a82a06a76c5bcd991ce5a10cda1`  
		Last Modified: Tue, 09 Jun 2020 01:13:35 GMT  
		Size: 42.1 MB (42102504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f976b5a12722f5e6e115157695654d36452b713c7fa64a860f8c9e14859402`  
		Last Modified: Tue, 09 Jun 2020 02:15:15 GMT  
		Size: 9.4 MB (9443335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35142ef6ea6c722cd0397799ab151e5da354eabc784b3acef29def7fa34e9bc`  
		Last Modified: Tue, 09 Jun 2020 02:15:13 GMT  
		Size: 3.9 MB (3918433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c8981f961756294156fe1f662892a0a0ab88baf5d457700d5fade1752d133`  
		Last Modified: Tue, 09 Jun 2020 18:43:39 GMT  
		Size: 2.8 KB (2801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec55bded7406efadfff0ab33a4879caf23ae15b846b282906d334ef39738d46`  
		Last Modified: Tue, 09 Jun 2020 18:44:23 GMT  
		Size: 60.2 MB (60158443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141c96330a48e29f21c5bf016a2eefbb49c1ab532b9e48112ba09e7bd6f5aa35`  
		Last Modified: Tue, 09 Jun 2020 18:44:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2069b504090bf9237fe41f9a0fa5826e1a12d44f89666cdf049c67f1d05e890`  
		Last Modified: Tue, 09 Jun 2020 18:44:05 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a58495eec75a130d57287efc999b6160de975b9596cafb6566637b1400c18d`  
		Last Modified: Tue, 09 Jun 2020 18:44:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:b76b73b81676fd808da43bf72924ed0a203b63c630513eb62d01e662d8e0e05d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116698602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e7427c6dbaf4e4f4d83e539fbc62c43023b7b87b3c17556506949ec7996aba3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:22 GMT
ADD file:5cbf00485aed776e940988cadfad6853c640c13635ae54fb2b00aafccfe81a73 in / 
# Tue, 09 Jun 2020 01:54:25 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 21:50:27 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Jun 2020 21:51:07 GMT
ENV INFLUXDB_VERSION=1.8.0
# Tue, 09 Jun 2020 21:51:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 09 Jun 2020 21:51:22 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 09 Jun 2020 21:51:23 GMT
EXPOSE 8086
# Tue, 09 Jun 2020 21:51:24 GMT
VOLUME [/var/lib/influxdb]
# Tue, 09 Jun 2020 21:51:25 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 09 Jun 2020 21:51:26 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 09 Jun 2020 21:51:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Jun 2020 21:51:29 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:4c4f692ec920eecb1f30d9ef8e50125217decc872d7ada6eeccc36c6dcb49e4d`  
		Last Modified: Tue, 09 Jun 2020 02:00:09 GMT  
		Size: 43.2 MB (43160923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0990c417a21ef9e268cc0822cd23968c4b17cded8170cce0c4d8f7e020e6fd`  
		Last Modified: Tue, 09 Jun 2020 02:50:17 GMT  
		Size: 9.7 MB (9699635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6b83fd41426d182f67fdac882a6bfcd3aad22d7226a653ae58d3046bd46b5e`  
		Last Modified: Tue, 09 Jun 2020 02:50:15 GMT  
		Size: 4.1 MB (4094104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039c1b8b197fb87df9fbb2ea446d6a6608957e69c6af971e06bf2040595482aa`  
		Last Modified: Tue, 09 Jun 2020 21:51:40 GMT  
		Size: 2.8 KB (2803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17a5103f843cdcb7e5a48e3420715e57f3b5ace27e26a726a1689ccd5367977`  
		Last Modified: Tue, 09 Jun 2020 21:52:19 GMT  
		Size: 59.7 MB (59739422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea6790eec015a1b5f075918a4d382e9ecf0d7e834d62d5712a7f0559221b70b`  
		Last Modified: Tue, 09 Jun 2020 21:52:04 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3eb93df098898860f2953544bc8acab4219e4416d95c8a0941523f2fa822a6`  
		Last Modified: Tue, 09 Jun 2020 21:52:03 GMT  
		Size: 207.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bb5b48a0d21cb7b7654e5df0fcc8c90f1ac7f117ee103c4afcb9fe371a4101`  
		Last Modified: Tue, 09 Jun 2020 21:52:03 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.1`

**does not exist** (yet?)

## `influxdb:1.8.1-alpine`

**does not exist** (yet?)

## `influxdb:1.8.1-data`

**does not exist** (yet?)

## `influxdb:1.8.1-data-alpine`

**does not exist** (yet?)

## `influxdb:1.8.1-meta`

**does not exist** (yet?)

## `influxdb:1.8.1-meta-alpine`

**does not exist** (yet?)

## `influxdb:1.8-alpine`

```console
$ docker pull influxdb@sha256:5eca9dfe9930a3325323cef801827eb1b0940070465f8f215447b8e732c72b34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:345a5246d3845386bb78fc97fbef3595f584416cfa8e9615af94ffc62f9c9b51
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68382880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c94b99616e72bf86ef11331cab8206d09c526f728a772d49d95a2cad43acfc4b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 15:28:09 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 15:29:01 GMT
ENV INFLUXDB_VERSION=1.8.0
# Fri, 24 Apr 2020 15:29:10 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 15:29:10 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 24 Apr 2020 15:29:10 GMT
EXPOSE 8086
# Fri, 24 Apr 2020 15:29:11 GMT
VOLUME [/var/lib/influxdb]
# Fri, 24 Apr 2020 15:29:11 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 24 Apr 2020 15:29:11 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 24 Apr 2020 15:29:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 15:29:11 GMT
CMD ["influxd"]
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
	-	`sha256:c9984b0a697389d40ad58252364c9cbb4e4a5258602767230a8f149134746718`  
		Last Modified: Fri, 24 Apr 2020 15:30:04 GMT  
		Size: 1.9 MB (1863602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf06c5f43ad15e3ff59921dff0cdb34414350983ac9972bf65bfe08f778bad1`  
		Last Modified: Fri, 24 Apr 2020 15:30:54 GMT  
		Size: 63.7 MB (63744002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46d9ed31eb9ce49b62e87e5d6154a314bd76696665a53dc790509789f813ece`  
		Last Modified: Fri, 24 Apr 2020 15:30:44 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9ea8ee8599c6abae4947e8bd8d9cf0796c8b15e7706f34d08d51d300ca5459`  
		Last Modified: Fri, 24 Apr 2020 15:30:44 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f948c2bacdf11982dd859393720280262abd366419cff9fafca14cf7ae61b037`  
		Last Modified: Fri, 24 Apr 2020 15:30:44 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data`

```console
$ docker pull influxdb@sha256:7b01f4838eaf0352b0212c4a08f157112753b9114060cac7fb8395d7fbf9de07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:ba9df9791e9b6881419fc692e0ec0d88a808ce2e414b64f70644b89b1b669283
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126218217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8fe42538472945189a51af1cb25b2d17e5b747e43042937ca08a365e19654ba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:43:24 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 10 Jun 2020 02:44:31 GMT
ENV INFLUXDB_VERSION=1.8.0-c1.8.0
# Wed, 10 Jun 2020 02:44:39 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 10 Jun 2020 02:44:39 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 10 Jun 2020 02:44:39 GMT
EXPOSE 8086
# Wed, 10 Jun 2020 02:44:39 GMT
VOLUME [/var/lib/influxdb]
# Wed, 10 Jun 2020 02:44:39 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 10 Jun 2020 02:44:40 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 10 Jun 2020 02:44:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 02:44:40 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e4835694e137bd4973eca79a9bb485066fb4b944fe90b33abadbdf75863b4a`  
		Last Modified: Wed, 10 Jun 2020 02:45:11 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58b0452dc7ac60aa15f5255718faee231546e984f4a690cf59e0bd136a69e1b`  
		Last Modified: Wed, 10 Jun 2020 02:46:19 GMT  
		Size: 65.7 MB (65748964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740f473fdb7652625bc94a752cb20eab27e69c138028a5d7c29da577ab1997a2`  
		Last Modified: Wed, 10 Jun 2020 02:46:07 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4ec38347be67a447fb95f0f18687dd10c9bf18c84009de4f28a516263f3e66`  
		Last Modified: Wed, 10 Jun 2020 02:46:07 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2682689fd289ac8d6b67097d2a705dee393e73de2a4815e18baea6aef1fa5ebd`  
		Last Modified: Wed, 10 Jun 2020 02:46:08 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data-alpine`

```console
$ docker pull influxdb@sha256:f1c88ea48881ae18a6fac9f5813d41a890861b5d1db1f433261ee8aa0146b244
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:65ae942f979083e9108b5e9a7870e4de2885530f338c3c0b23f50522f665e0be
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70184572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3263a29ef68203d5819223d5377eb26b4bef27f2741105bf18a7863116b70dfa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 15:28:09 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 15:29:19 GMT
ENV INFLUXDB_VERSION=1.8.0-c1.8.0
# Fri, 24 Apr 2020 15:29:27 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 15:29:28 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 24 Apr 2020 15:29:28 GMT
EXPOSE 8086
# Fri, 24 Apr 2020 15:29:28 GMT
VOLUME [/var/lib/influxdb]
# Fri, 24 Apr 2020 15:29:28 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 24 Apr 2020 15:29:28 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 24 Apr 2020 15:29:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 15:29:29 GMT
CMD ["influxd"]
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
	-	`sha256:c9984b0a697389d40ad58252364c9cbb4e4a5258602767230a8f149134746718`  
		Last Modified: Fri, 24 Apr 2020 15:30:04 GMT  
		Size: 1.9 MB (1863602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843346bc3e53dc0279f66a2856caba81be908f294f98f589e37b94000d9d4f03`  
		Last Modified: Fri, 24 Apr 2020 15:31:09 GMT  
		Size: 65.5 MB (65545628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bd6b1e71d7f58518d1f9aecdcff6f9d755780990c41a69982c343f54eb60b5`  
		Last Modified: Fri, 24 Apr 2020 15:31:00 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7364616d5c55aef621c1a84ad6b835c04b05062d087513e0475701ef608614ed`  
		Last Modified: Fri, 24 Apr 2020 15:30:59 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c529298a52d6b2299ee8bb4d410063fa678d93b36540841ca8e4e417626b05d`  
		Last Modified: Fri, 24 Apr 2020 15:31:00 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta`

```console
$ docker pull influxdb@sha256:79a9564a285f23be9db62b827c8d0f54332dac0250e04f62507548acfeeaeba4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:5290c16beadce9967bb3d81f6d5bf30bec8798730768bd491084d14d332875f0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83400056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebdc9b3b60bc2aee3beced4302c88b33d5b8b0258183fcfa5c497d75a02ce4ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:43:24 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 10 Jun 2020 02:44:31 GMT
ENV INFLUXDB_VERSION=1.8.0-c1.8.0
# Wed, 10 Jun 2020 02:44:51 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 10 Jun 2020 02:44:51 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 10 Jun 2020 02:44:51 GMT
EXPOSE 8091
# Wed, 10 Jun 2020 02:44:52 GMT
VOLUME [/var/lib/influxdb]
# Wed, 10 Jun 2020 02:44:52 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 10 Jun 2020 02:44:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 02:44:53 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e4835694e137bd4973eca79a9bb485066fb4b944fe90b33abadbdf75863b4a`  
		Last Modified: Wed, 10 Jun 2020 02:45:11 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14793e88cf81476500da3764583ad37aedfac7b968810a282d3028575b5196de`  
		Last Modified: Wed, 10 Jun 2020 02:46:32 GMT  
		Size: 22.9 MB (22932009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecc98e2a16498d86b3903a2338c64f27efa68855c3f2ec5cc61b612b0d129c0`  
		Last Modified: Wed, 10 Jun 2020 02:46:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a51212ac59f382b8306f9c56430c3ce516561f392c7c822b24206e4d3a72dce`  
		Last Modified: Wed, 10 Jun 2020 02:46:27 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta-alpine`

```console
$ docker pull influxdb@sha256:0b305d29c9b741e41ddc4238844889df457fabe00adfefa7cd9f1aab62cc4942
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:8d52a1557dba68ce24f1160f909c6b8c0861a886c8d66feed9d46b3878efea9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27499835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4229b89d6f742112b1641eeb833852a43039638411ee836f2844d9a879972c8c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 15:28:09 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 15:29:19 GMT
ENV INFLUXDB_VERSION=1.8.0-c1.8.0
# Fri, 24 Apr 2020 15:29:39 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 15:29:40 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 24 Apr 2020 15:29:40 GMT
EXPOSE 8091
# Fri, 24 Apr 2020 15:29:41 GMT
VOLUME [/var/lib/influxdb]
# Fri, 24 Apr 2020 15:29:41 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 24 Apr 2020 15:29:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 15:29:41 GMT
CMD ["influxd-meta"]
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
	-	`sha256:c9984b0a697389d40ad58252364c9cbb4e4a5258602767230a8f149134746718`  
		Last Modified: Fri, 24 Apr 2020 15:30:04 GMT  
		Size: 1.9 MB (1863602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bca21c6e4e58d671040ae34b832f11c78c8fdf2f21ab87a467c4020e10004a`  
		Last Modified: Fri, 24 Apr 2020 15:31:18 GMT  
		Size: 22.9 MB (22862100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d324db747584584fcaee61408f9d6038d393e7377028f5031fd7db62b0e3ef0`  
		Last Modified: Fri, 24 Apr 2020 15:31:15 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be071ebf219263c79b41cf2ad2fa2367f5c531f9c263d75fb4aa021a0452dbff`  
		Last Modified: Fri, 24 Apr 2020 15:31:15 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:5eca9dfe9930a3325323cef801827eb1b0940070465f8f215447b8e732c72b34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:345a5246d3845386bb78fc97fbef3595f584416cfa8e9615af94ffc62f9c9b51
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68382880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c94b99616e72bf86ef11331cab8206d09c526f728a772d49d95a2cad43acfc4b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 15:28:09 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 15:29:01 GMT
ENV INFLUXDB_VERSION=1.8.0
# Fri, 24 Apr 2020 15:29:10 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 15:29:10 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 24 Apr 2020 15:29:10 GMT
EXPOSE 8086
# Fri, 24 Apr 2020 15:29:11 GMT
VOLUME [/var/lib/influxdb]
# Fri, 24 Apr 2020 15:29:11 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 24 Apr 2020 15:29:11 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 24 Apr 2020 15:29:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 15:29:11 GMT
CMD ["influxd"]
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
	-	`sha256:c9984b0a697389d40ad58252364c9cbb4e4a5258602767230a8f149134746718`  
		Last Modified: Fri, 24 Apr 2020 15:30:04 GMT  
		Size: 1.9 MB (1863602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf06c5f43ad15e3ff59921dff0cdb34414350983ac9972bf65bfe08f778bad1`  
		Last Modified: Fri, 24 Apr 2020 15:30:54 GMT  
		Size: 63.7 MB (63744002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46d9ed31eb9ce49b62e87e5d6154a314bd76696665a53dc790509789f813ece`  
		Last Modified: Fri, 24 Apr 2020 15:30:44 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9ea8ee8599c6abae4947e8bd8d9cf0796c8b15e7706f34d08d51d300ca5459`  
		Last Modified: Fri, 24 Apr 2020 15:30:44 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f948c2bacdf11982dd859393720280262abd366419cff9fafca14cf7ae61b037`  
		Last Modified: Fri, 24 Apr 2020 15:30:44 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data`

```console
$ docker pull influxdb@sha256:7b01f4838eaf0352b0212c4a08f157112753b9114060cac7fb8395d7fbf9de07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:ba9df9791e9b6881419fc692e0ec0d88a808ce2e414b64f70644b89b1b669283
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126218217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8fe42538472945189a51af1cb25b2d17e5b747e43042937ca08a365e19654ba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:43:24 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 10 Jun 2020 02:44:31 GMT
ENV INFLUXDB_VERSION=1.8.0-c1.8.0
# Wed, 10 Jun 2020 02:44:39 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 10 Jun 2020 02:44:39 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 10 Jun 2020 02:44:39 GMT
EXPOSE 8086
# Wed, 10 Jun 2020 02:44:39 GMT
VOLUME [/var/lib/influxdb]
# Wed, 10 Jun 2020 02:44:39 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 10 Jun 2020 02:44:40 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 10 Jun 2020 02:44:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 02:44:40 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e4835694e137bd4973eca79a9bb485066fb4b944fe90b33abadbdf75863b4a`  
		Last Modified: Wed, 10 Jun 2020 02:45:11 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58b0452dc7ac60aa15f5255718faee231546e984f4a690cf59e0bd136a69e1b`  
		Last Modified: Wed, 10 Jun 2020 02:46:19 GMT  
		Size: 65.7 MB (65748964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740f473fdb7652625bc94a752cb20eab27e69c138028a5d7c29da577ab1997a2`  
		Last Modified: Wed, 10 Jun 2020 02:46:07 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4ec38347be67a447fb95f0f18687dd10c9bf18c84009de4f28a516263f3e66`  
		Last Modified: Wed, 10 Jun 2020 02:46:07 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2682689fd289ac8d6b67097d2a705dee393e73de2a4815e18baea6aef1fa5ebd`  
		Last Modified: Wed, 10 Jun 2020 02:46:08 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data-alpine`

```console
$ docker pull influxdb@sha256:f1c88ea48881ae18a6fac9f5813d41a890861b5d1db1f433261ee8aa0146b244
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:65ae942f979083e9108b5e9a7870e4de2885530f338c3c0b23f50522f665e0be
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70184572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3263a29ef68203d5819223d5377eb26b4bef27f2741105bf18a7863116b70dfa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 15:28:09 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 15:29:19 GMT
ENV INFLUXDB_VERSION=1.8.0-c1.8.0
# Fri, 24 Apr 2020 15:29:27 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 15:29:28 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 24 Apr 2020 15:29:28 GMT
EXPOSE 8086
# Fri, 24 Apr 2020 15:29:28 GMT
VOLUME [/var/lib/influxdb]
# Fri, 24 Apr 2020 15:29:28 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 24 Apr 2020 15:29:28 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 24 Apr 2020 15:29:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 15:29:29 GMT
CMD ["influxd"]
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
	-	`sha256:c9984b0a697389d40ad58252364c9cbb4e4a5258602767230a8f149134746718`  
		Last Modified: Fri, 24 Apr 2020 15:30:04 GMT  
		Size: 1.9 MB (1863602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843346bc3e53dc0279f66a2856caba81be908f294f98f589e37b94000d9d4f03`  
		Last Modified: Fri, 24 Apr 2020 15:31:09 GMT  
		Size: 65.5 MB (65545628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bd6b1e71d7f58518d1f9aecdcff6f9d755780990c41a69982c343f54eb60b5`  
		Last Modified: Fri, 24 Apr 2020 15:31:00 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7364616d5c55aef621c1a84ad6b835c04b05062d087513e0475701ef608614ed`  
		Last Modified: Fri, 24 Apr 2020 15:30:59 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c529298a52d6b2299ee8bb4d410063fa678d93b36540841ca8e4e417626b05d`  
		Last Modified: Fri, 24 Apr 2020 15:31:00 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:latest`

```console
$ docker pull influxdb@sha256:2c4ee7675963a8f5a388e7853f6e68a1fcabebd24ce386364356587ad374e047
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:9e7c9fd78802e882ac441b4a25ecf95437d27651888148a61cf646b1d57286e8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124427438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95750833bc56d19870063238f49dbd465a7ed51928963d43f8360005004be663`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:43:24 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 10 Jun 2020 02:44:13 GMT
ENV INFLUXDB_VERSION=1.8.0
# Wed, 10 Jun 2020 02:44:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 10 Jun 2020 02:44:20 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 10 Jun 2020 02:44:21 GMT
EXPOSE 8086
# Wed, 10 Jun 2020 02:44:22 GMT
VOLUME [/var/lib/influxdb]
# Wed, 10 Jun 2020 02:44:22 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 10 Jun 2020 02:44:22 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 10 Jun 2020 02:44:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 02:44:22 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e4835694e137bd4973eca79a9bb485066fb4b944fe90b33abadbdf75863b4a`  
		Last Modified: Wed, 10 Jun 2020 02:45:11 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05df09a184e99c772f1f2fb571d741cd42209bdf169fc84dd24a73836ea130e0`  
		Last Modified: Wed, 10 Jun 2020 02:46:01 GMT  
		Size: 64.0 MB (63958242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671fe28366cfee32412469096c3c784ee91255b10b42b71ec4c5909cfa2d40d5`  
		Last Modified: Wed, 10 Jun 2020 02:45:52 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36ec69a8c120ed9c7d731a9f9de448d6fd258eb42310646741ca9a1fb878aac`  
		Last Modified: Wed, 10 Jun 2020 02:45:52 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc93bd218ea315e4551227d83072e8a9e2ac29f86174b39331fa44f586956c14`  
		Last Modified: Wed, 10 Jun 2020 02:45:52 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:73f876e0c3bd02900f829d4884f53fdfffd7098dd572406ba549eed955bf821f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115627234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0866da0fd5bb684b2b9b13002956f1d9806bc8eac6d62a98bf1056d4268a25c6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:07 GMT
ADD file:c0b9ed1244ec0acfc9054c7cb80c768878e3da99740f981ba3a82bdd854305db in / 
# Tue, 09 Jun 2020 01:06:09 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:02:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:02:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 18:42:50 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Jun 2020 18:43:14 GMT
ENV INFLUXDB_VERSION=1.8.0
# Tue, 09 Jun 2020 18:43:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 09 Jun 2020 18:43:25 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 09 Jun 2020 18:43:25 GMT
EXPOSE 8086
# Tue, 09 Jun 2020 18:43:26 GMT
VOLUME [/var/lib/influxdb]
# Tue, 09 Jun 2020 18:43:26 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 09 Jun 2020 18:43:27 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 09 Jun 2020 18:43:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Jun 2020 18:43:28 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:2566ca784846d2d0d4f9105084d94d68d8ea1a82a06a76c5bcd991ce5a10cda1`  
		Last Modified: Tue, 09 Jun 2020 01:13:35 GMT  
		Size: 42.1 MB (42102504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f976b5a12722f5e6e115157695654d36452b713c7fa64a860f8c9e14859402`  
		Last Modified: Tue, 09 Jun 2020 02:15:15 GMT  
		Size: 9.4 MB (9443335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35142ef6ea6c722cd0397799ab151e5da354eabc784b3acef29def7fa34e9bc`  
		Last Modified: Tue, 09 Jun 2020 02:15:13 GMT  
		Size: 3.9 MB (3918433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c8981f961756294156fe1f662892a0a0ab88baf5d457700d5fade1752d133`  
		Last Modified: Tue, 09 Jun 2020 18:43:39 GMT  
		Size: 2.8 KB (2801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec55bded7406efadfff0ab33a4879caf23ae15b846b282906d334ef39738d46`  
		Last Modified: Tue, 09 Jun 2020 18:44:23 GMT  
		Size: 60.2 MB (60158443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141c96330a48e29f21c5bf016a2eefbb49c1ab532b9e48112ba09e7bd6f5aa35`  
		Last Modified: Tue, 09 Jun 2020 18:44:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2069b504090bf9237fe41f9a0fa5826e1a12d44f89666cdf049c67f1d05e890`  
		Last Modified: Tue, 09 Jun 2020 18:44:05 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a58495eec75a130d57287efc999b6160de975b9596cafb6566637b1400c18d`  
		Last Modified: Tue, 09 Jun 2020 18:44:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:b76b73b81676fd808da43bf72924ed0a203b63c630513eb62d01e662d8e0e05d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116698602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e7427c6dbaf4e4f4d83e539fbc62c43023b7b87b3c17556506949ec7996aba3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:22 GMT
ADD file:5cbf00485aed776e940988cadfad6853c640c13635ae54fb2b00aafccfe81a73 in / 
# Tue, 09 Jun 2020 01:54:25 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 21:50:27 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Jun 2020 21:51:07 GMT
ENV INFLUXDB_VERSION=1.8.0
# Tue, 09 Jun 2020 21:51:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 09 Jun 2020 21:51:22 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 09 Jun 2020 21:51:23 GMT
EXPOSE 8086
# Tue, 09 Jun 2020 21:51:24 GMT
VOLUME [/var/lib/influxdb]
# Tue, 09 Jun 2020 21:51:25 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 09 Jun 2020 21:51:26 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 09 Jun 2020 21:51:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Jun 2020 21:51:29 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:4c4f692ec920eecb1f30d9ef8e50125217decc872d7ada6eeccc36c6dcb49e4d`  
		Last Modified: Tue, 09 Jun 2020 02:00:09 GMT  
		Size: 43.2 MB (43160923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0990c417a21ef9e268cc0822cd23968c4b17cded8170cce0c4d8f7e020e6fd`  
		Last Modified: Tue, 09 Jun 2020 02:50:17 GMT  
		Size: 9.7 MB (9699635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6b83fd41426d182f67fdac882a6bfcd3aad22d7226a653ae58d3046bd46b5e`  
		Last Modified: Tue, 09 Jun 2020 02:50:15 GMT  
		Size: 4.1 MB (4094104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039c1b8b197fb87df9fbb2ea446d6a6608957e69c6af971e06bf2040595482aa`  
		Last Modified: Tue, 09 Jun 2020 21:51:40 GMT  
		Size: 2.8 KB (2803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17a5103f843cdcb7e5a48e3420715e57f3b5ace27e26a726a1689ccd5367977`  
		Last Modified: Tue, 09 Jun 2020 21:52:19 GMT  
		Size: 59.7 MB (59739422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea6790eec015a1b5f075918a4d382e9ecf0d7e834d62d5712a7f0559221b70b`  
		Last Modified: Tue, 09 Jun 2020 21:52:04 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3eb93df098898860f2953544bc8acab4219e4416d95c8a0941523f2fa822a6`  
		Last Modified: Tue, 09 Jun 2020 21:52:03 GMT  
		Size: 207.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bb5b48a0d21cb7b7654e5df0fcc8c90f1ac7f117ee103c4afcb9fe371a4101`  
		Last Modified: Tue, 09 Jun 2020 21:52:03 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:79a9564a285f23be9db62b827c8d0f54332dac0250e04f62507548acfeeaeba4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:5290c16beadce9967bb3d81f6d5bf30bec8798730768bd491084d14d332875f0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83400056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebdc9b3b60bc2aee3beced4302c88b33d5b8b0258183fcfa5c497d75a02ce4ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:43:24 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 10 Jun 2020 02:44:31 GMT
ENV INFLUXDB_VERSION=1.8.0-c1.8.0
# Wed, 10 Jun 2020 02:44:51 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 10 Jun 2020 02:44:51 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 10 Jun 2020 02:44:51 GMT
EXPOSE 8091
# Wed, 10 Jun 2020 02:44:52 GMT
VOLUME [/var/lib/influxdb]
# Wed, 10 Jun 2020 02:44:52 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 10 Jun 2020 02:44:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 02:44:53 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e4835694e137bd4973eca79a9bb485066fb4b944fe90b33abadbdf75863b4a`  
		Last Modified: Wed, 10 Jun 2020 02:45:11 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14793e88cf81476500da3764583ad37aedfac7b968810a282d3028575b5196de`  
		Last Modified: Wed, 10 Jun 2020 02:46:32 GMT  
		Size: 22.9 MB (22932009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecc98e2a16498d86b3903a2338c64f27efa68855c3f2ec5cc61b612b0d129c0`  
		Last Modified: Wed, 10 Jun 2020 02:46:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a51212ac59f382b8306f9c56430c3ce516561f392c7c822b24206e4d3a72dce`  
		Last Modified: Wed, 10 Jun 2020 02:46:27 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta-alpine`

```console
$ docker pull influxdb@sha256:0b305d29c9b741e41ddc4238844889df457fabe00adfefa7cd9f1aab62cc4942
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:8d52a1557dba68ce24f1160f909c6b8c0861a886c8d66feed9d46b3878efea9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27499835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4229b89d6f742112b1641eeb833852a43039638411ee836f2844d9a879972c8c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 15:28:09 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 15:29:19 GMT
ENV INFLUXDB_VERSION=1.8.0-c1.8.0
# Fri, 24 Apr 2020 15:29:39 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 15:29:40 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 24 Apr 2020 15:29:40 GMT
EXPOSE 8091
# Fri, 24 Apr 2020 15:29:41 GMT
VOLUME [/var/lib/influxdb]
# Fri, 24 Apr 2020 15:29:41 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 24 Apr 2020 15:29:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 15:29:41 GMT
CMD ["influxd-meta"]
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
	-	`sha256:c9984b0a697389d40ad58252364c9cbb4e4a5258602767230a8f149134746718`  
		Last Modified: Fri, 24 Apr 2020 15:30:04 GMT  
		Size: 1.9 MB (1863602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bca21c6e4e58d671040ae34b832f11c78c8fdf2f21ab87a467c4020e10004a`  
		Last Modified: Fri, 24 Apr 2020 15:31:18 GMT  
		Size: 22.9 MB (22862100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d324db747584584fcaee61408f9d6038d393e7377028f5031fd7db62b0e3ef0`  
		Last Modified: Fri, 24 Apr 2020 15:31:15 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be071ebf219263c79b41cf2ad2fa2367f5c531f9c263d75fb4aa021a0452dbff`  
		Last Modified: Fri, 24 Apr 2020 15:31:15 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
