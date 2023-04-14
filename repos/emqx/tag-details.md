<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.16`](#emqx4416)
-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.22`](#emqx5022)
-	[`emqx:latest`](#emqxlatest)

## `emqx:4`

```console
$ docker pull emqx@sha256:f4a5457940a950d30d1d4ff904ec3bbc37fc3f2c59d81fc1df7441870f372a29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:777be2ec320c0448e8d4c79dcade7501ae98cf53f256d973f4faa47150d748b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81279221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02879c1b8ec47f99da6f309c6b0b829c3256e60f997d0cb2905851085fde7047`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:42:35 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:42:35 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 12 Apr 2023 00:42:35 GMT
ENV EMQX_VERSION=4.4.16
# Wed, 12 Apr 2023 00:42:35 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 12 Apr 2023 00:42:40 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 12 Apr 2023 00:42:40 GMT
WORKDIR /opt/emqx
# Wed, 12 Apr 2023 00:42:41 GMT
USER emqx
# Wed, 12 Apr 2023 00:42:41 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 12 Apr 2023 00:42:41 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 12 Apr 2023 00:42:41 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 12 Apr 2023 00:42:41 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 00:42:41 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e901aaad2c36dc10a256fae9d94810d0bcd1d3732eb3e172f7d18eba970956df`  
		Last Modified: Wed, 12 Apr 2023 00:43:09 GMT  
		Size: 2.6 MB (2569627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f607aa293305bd4722109d3b17853a91b8de9754b42fe37d71be6cf3c9abb42`  
		Last Modified: Wed, 12 Apr 2023 00:43:08 GMT  
		Size: 4.1 KB (4105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d76c9e6de33b4e4930f490339f65388845be0f45ac8c927caa21f8284e91968`  
		Last Modified: Wed, 12 Apr 2023 00:43:13 GMT  
		Size: 47.3 MB (47286153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982eabc32ac02081fb30fb30af3b0b9098324072276786bfe38338b79409aa87`  
		Last Modified: Wed, 12 Apr 2023 00:43:08 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:e4f49a9bae3c3ad547148e517ad4451fbd4fba2d21f3b53a40a115bd9dbbd3d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72701529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23307f7422a0441a902d08c03d1f4c65e395e77b8190ff8032600e254a5b15a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:38:12 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:38:13 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 12 Apr 2023 01:38:13 GMT
ENV EMQX_VERSION=4.4.16
# Wed, 12 Apr 2023 01:38:13 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 12 Apr 2023 01:38:16 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 12 Apr 2023 01:38:17 GMT
WORKDIR /opt/emqx
# Wed, 12 Apr 2023 01:38:17 GMT
USER emqx
# Wed, 12 Apr 2023 01:38:17 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 12 Apr 2023 01:38:17 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 12 Apr 2023 01:38:17 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 12 Apr 2023 01:38:17 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 01:38:17 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4322e90f757b16a8adb2d40ade499d3006e85ca6d83f0eb96ea9691b6871dd`  
		Last Modified: Wed, 12 Apr 2023 01:38:39 GMT  
		Size: 2.6 MB (2559482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3071e2b66079e6214608516ff2e6a436738f7da65ae6bb2c5357edcfb8d54a78`  
		Last Modified: Wed, 12 Apr 2023 01:38:38 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f229fe6e12568f30110a7e32b64c2663347f777453d0221e3f69c94cbd0363e3`  
		Last Modified: Wed, 12 Apr 2023 01:38:42 GMT  
		Size: 40.1 MB (40072999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c781b0628ed08d53bc0110d452cdce09ec0e87def799a744c729d43350c58e2b`  
		Last Modified: Wed, 12 Apr 2023 01:38:38 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:f4a5457940a950d30d1d4ff904ec3bbc37fc3f2c59d81fc1df7441870f372a29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:777be2ec320c0448e8d4c79dcade7501ae98cf53f256d973f4faa47150d748b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81279221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02879c1b8ec47f99da6f309c6b0b829c3256e60f997d0cb2905851085fde7047`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:42:35 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:42:35 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 12 Apr 2023 00:42:35 GMT
ENV EMQX_VERSION=4.4.16
# Wed, 12 Apr 2023 00:42:35 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 12 Apr 2023 00:42:40 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 12 Apr 2023 00:42:40 GMT
WORKDIR /opt/emqx
# Wed, 12 Apr 2023 00:42:41 GMT
USER emqx
# Wed, 12 Apr 2023 00:42:41 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 12 Apr 2023 00:42:41 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 12 Apr 2023 00:42:41 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 12 Apr 2023 00:42:41 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 00:42:41 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e901aaad2c36dc10a256fae9d94810d0bcd1d3732eb3e172f7d18eba970956df`  
		Last Modified: Wed, 12 Apr 2023 00:43:09 GMT  
		Size: 2.6 MB (2569627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f607aa293305bd4722109d3b17853a91b8de9754b42fe37d71be6cf3c9abb42`  
		Last Modified: Wed, 12 Apr 2023 00:43:08 GMT  
		Size: 4.1 KB (4105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d76c9e6de33b4e4930f490339f65388845be0f45ac8c927caa21f8284e91968`  
		Last Modified: Wed, 12 Apr 2023 00:43:13 GMT  
		Size: 47.3 MB (47286153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982eabc32ac02081fb30fb30af3b0b9098324072276786bfe38338b79409aa87`  
		Last Modified: Wed, 12 Apr 2023 00:43:08 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:e4f49a9bae3c3ad547148e517ad4451fbd4fba2d21f3b53a40a115bd9dbbd3d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72701529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23307f7422a0441a902d08c03d1f4c65e395e77b8190ff8032600e254a5b15a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:38:12 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:38:13 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 12 Apr 2023 01:38:13 GMT
ENV EMQX_VERSION=4.4.16
# Wed, 12 Apr 2023 01:38:13 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 12 Apr 2023 01:38:16 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 12 Apr 2023 01:38:17 GMT
WORKDIR /opt/emqx
# Wed, 12 Apr 2023 01:38:17 GMT
USER emqx
# Wed, 12 Apr 2023 01:38:17 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 12 Apr 2023 01:38:17 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 12 Apr 2023 01:38:17 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 12 Apr 2023 01:38:17 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 01:38:17 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4322e90f757b16a8adb2d40ade499d3006e85ca6d83f0eb96ea9691b6871dd`  
		Last Modified: Wed, 12 Apr 2023 01:38:39 GMT  
		Size: 2.6 MB (2559482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3071e2b66079e6214608516ff2e6a436738f7da65ae6bb2c5357edcfb8d54a78`  
		Last Modified: Wed, 12 Apr 2023 01:38:38 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f229fe6e12568f30110a7e32b64c2663347f777453d0221e3f69c94cbd0363e3`  
		Last Modified: Wed, 12 Apr 2023 01:38:42 GMT  
		Size: 40.1 MB (40072999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c781b0628ed08d53bc0110d452cdce09ec0e87def799a744c729d43350c58e2b`  
		Last Modified: Wed, 12 Apr 2023 01:38:38 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.16`

```console
$ docker pull emqx@sha256:f4a5457940a950d30d1d4ff904ec3bbc37fc3f2c59d81fc1df7441870f372a29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.16` - linux; amd64

```console
$ docker pull emqx@sha256:777be2ec320c0448e8d4c79dcade7501ae98cf53f256d973f4faa47150d748b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81279221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02879c1b8ec47f99da6f309c6b0b829c3256e60f997d0cb2905851085fde7047`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:42:35 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:42:35 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 12 Apr 2023 00:42:35 GMT
ENV EMQX_VERSION=4.4.16
# Wed, 12 Apr 2023 00:42:35 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 12 Apr 2023 00:42:40 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 12 Apr 2023 00:42:40 GMT
WORKDIR /opt/emqx
# Wed, 12 Apr 2023 00:42:41 GMT
USER emqx
# Wed, 12 Apr 2023 00:42:41 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 12 Apr 2023 00:42:41 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 12 Apr 2023 00:42:41 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 12 Apr 2023 00:42:41 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 00:42:41 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e901aaad2c36dc10a256fae9d94810d0bcd1d3732eb3e172f7d18eba970956df`  
		Last Modified: Wed, 12 Apr 2023 00:43:09 GMT  
		Size: 2.6 MB (2569627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f607aa293305bd4722109d3b17853a91b8de9754b42fe37d71be6cf3c9abb42`  
		Last Modified: Wed, 12 Apr 2023 00:43:08 GMT  
		Size: 4.1 KB (4105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d76c9e6de33b4e4930f490339f65388845be0f45ac8c927caa21f8284e91968`  
		Last Modified: Wed, 12 Apr 2023 00:43:13 GMT  
		Size: 47.3 MB (47286153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982eabc32ac02081fb30fb30af3b0b9098324072276786bfe38338b79409aa87`  
		Last Modified: Wed, 12 Apr 2023 00:43:08 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.16` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:e4f49a9bae3c3ad547148e517ad4451fbd4fba2d21f3b53a40a115bd9dbbd3d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72701529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23307f7422a0441a902d08c03d1f4c65e395e77b8190ff8032600e254a5b15a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:38:12 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:38:13 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 12 Apr 2023 01:38:13 GMT
ENV EMQX_VERSION=4.4.16
# Wed, 12 Apr 2023 01:38:13 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 12 Apr 2023 01:38:16 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 12 Apr 2023 01:38:17 GMT
WORKDIR /opt/emqx
# Wed, 12 Apr 2023 01:38:17 GMT
USER emqx
# Wed, 12 Apr 2023 01:38:17 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 12 Apr 2023 01:38:17 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 12 Apr 2023 01:38:17 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 12 Apr 2023 01:38:17 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 01:38:17 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4322e90f757b16a8adb2d40ade499d3006e85ca6d83f0eb96ea9691b6871dd`  
		Last Modified: Wed, 12 Apr 2023 01:38:39 GMT  
		Size: 2.6 MB (2559482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3071e2b66079e6214608516ff2e6a436738f7da65ae6bb2c5357edcfb8d54a78`  
		Last Modified: Wed, 12 Apr 2023 01:38:38 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f229fe6e12568f30110a7e32b64c2663347f777453d0221e3f69c94cbd0363e3`  
		Last Modified: Wed, 12 Apr 2023 01:38:42 GMT  
		Size: 40.1 MB (40072999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c781b0628ed08d53bc0110d452cdce09ec0e87def799a744c729d43350c58e2b`  
		Last Modified: Wed, 12 Apr 2023 01:38:38 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5`

```console
$ docker pull emqx@sha256:35d0b6f888562d5ea32fdd5b163d7eb75ded34e726b8e891608a7fc9cc6923a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:f989e47367da5a656f82a7aeec894a50ecf5fd083a50b54e74118ab897033f1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.4 MB (101411977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b62de259a0237f960db47c17ace4181a9d0b4651786088aa8a49f8099353a64e`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:42:50 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:42:51 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 12 Apr 2023 00:42:51 GMT
ENV EMQX_VERSION=5.0.21
# Wed, 12 Apr 2023 00:42:51 GMT
ENV AMD64_SHA256=d83d435bfd49fc06cf9448de12ee76d383f9919fbb4d149545ccc246c903b78e
# Wed, 12 Apr 2023 00:42:51 GMT
ENV ARM64_SHA256=29dc8a470c9d43069dbc0f640e9493a991516fa18e028930726e8a6c7e60afc6
# Wed, 12 Apr 2023 00:42:51 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 12 Apr 2023 00:42:57 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 12 Apr 2023 00:42:58 GMT
WORKDIR /opt/emqx
# Wed, 12 Apr 2023 00:42:58 GMT
USER emqx
# Wed, 12 Apr 2023 00:42:58 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 12 Apr 2023 00:42:58 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 12 Apr 2023 00:42:58 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 12 Apr 2023 00:42:58 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 00:42:58 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f79c821cbd23fa1420033390e2828e0922b8efe06687c960eb7ff40edfbd0d6`  
		Last Modified: Wed, 12 Apr 2023 00:43:23 GMT  
		Size: 3.0 MB (2987825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048c1bdd86f15f4d429d049f898a2d3c0f0732c5b7e68a31b824acae055655d8`  
		Last Modified: Wed, 12 Apr 2023 00:43:22 GMT  
		Size: 4.1 KB (4105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4773c7908a53fe2a3cfd56039eb7c0a86af81933b57fb3b539d9f4994f5a4c`  
		Last Modified: Wed, 12 Apr 2023 00:43:30 GMT  
		Size: 67.0 MB (67000917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba19bb9c71ad2945f2eae572505c1e6047c345ec90c0a9283aba640bcca70e9c`  
		Last Modified: Wed, 12 Apr 2023 00:43:23 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:4768cca0bdd0c9d3220c04324dae4f23d4a0d173198389d53f94fd9a298900b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.5 MB (92499291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e18a3436e25d685512eaaa2535734c8393159049706f41427222cad25dbf636`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:38:23 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:38:24 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 12 Apr 2023 01:38:24 GMT
ENV EMQX_VERSION=5.0.21
# Wed, 12 Apr 2023 01:38:24 GMT
ENV AMD64_SHA256=d83d435bfd49fc06cf9448de12ee76d383f9919fbb4d149545ccc246c903b78e
# Wed, 12 Apr 2023 01:38:24 GMT
ENV ARM64_SHA256=29dc8a470c9d43069dbc0f640e9493a991516fa18e028930726e8a6c7e60afc6
# Wed, 12 Apr 2023 01:38:24 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 12 Apr 2023 01:38:29 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 12 Apr 2023 01:38:29 GMT
WORKDIR /opt/emqx
# Wed, 12 Apr 2023 01:38:29 GMT
USER emqx
# Wed, 12 Apr 2023 01:38:29 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 12 Apr 2023 01:38:30 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 12 Apr 2023 01:38:30 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 12 Apr 2023 01:38:30 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 01:38:30 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b64e3be9abc32d122bd4b9c6cbdc2adc75085b08f7644acbd1e9a963977cd48`  
		Last Modified: Wed, 12 Apr 2023 01:38:53 GMT  
		Size: 3.0 MB (3002944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b665badbe1ecc88ea2bdc4962042f6412551d166e4bc0bfbfcd3e00d159e605`  
		Last Modified: Wed, 12 Apr 2023 01:38:52 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f60cb43970fd9770be4b4842be70e9b0b29ca9b4ff9ab04589f944dc44b3b3`  
		Last Modified: Wed, 12 Apr 2023 01:38:58 GMT  
		Size: 59.4 MB (59427507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860a1f80f58c5f8171a12433e753695633645ebb760bb9604624694d5dfd5618`  
		Last Modified: Wed, 12 Apr 2023 01:38:52 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:35d0b6f888562d5ea32fdd5b163d7eb75ded34e726b8e891608a7fc9cc6923a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:f989e47367da5a656f82a7aeec894a50ecf5fd083a50b54e74118ab897033f1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.4 MB (101411977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b62de259a0237f960db47c17ace4181a9d0b4651786088aa8a49f8099353a64e`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:42:50 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:42:51 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 12 Apr 2023 00:42:51 GMT
ENV EMQX_VERSION=5.0.21
# Wed, 12 Apr 2023 00:42:51 GMT
ENV AMD64_SHA256=d83d435bfd49fc06cf9448de12ee76d383f9919fbb4d149545ccc246c903b78e
# Wed, 12 Apr 2023 00:42:51 GMT
ENV ARM64_SHA256=29dc8a470c9d43069dbc0f640e9493a991516fa18e028930726e8a6c7e60afc6
# Wed, 12 Apr 2023 00:42:51 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 12 Apr 2023 00:42:57 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 12 Apr 2023 00:42:58 GMT
WORKDIR /opt/emqx
# Wed, 12 Apr 2023 00:42:58 GMT
USER emqx
# Wed, 12 Apr 2023 00:42:58 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 12 Apr 2023 00:42:58 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 12 Apr 2023 00:42:58 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 12 Apr 2023 00:42:58 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 00:42:58 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f79c821cbd23fa1420033390e2828e0922b8efe06687c960eb7ff40edfbd0d6`  
		Last Modified: Wed, 12 Apr 2023 00:43:23 GMT  
		Size: 3.0 MB (2987825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048c1bdd86f15f4d429d049f898a2d3c0f0732c5b7e68a31b824acae055655d8`  
		Last Modified: Wed, 12 Apr 2023 00:43:22 GMT  
		Size: 4.1 KB (4105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4773c7908a53fe2a3cfd56039eb7c0a86af81933b57fb3b539d9f4994f5a4c`  
		Last Modified: Wed, 12 Apr 2023 00:43:30 GMT  
		Size: 67.0 MB (67000917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba19bb9c71ad2945f2eae572505c1e6047c345ec90c0a9283aba640bcca70e9c`  
		Last Modified: Wed, 12 Apr 2023 00:43:23 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:4768cca0bdd0c9d3220c04324dae4f23d4a0d173198389d53f94fd9a298900b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.5 MB (92499291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e18a3436e25d685512eaaa2535734c8393159049706f41427222cad25dbf636`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:38:23 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:38:24 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 12 Apr 2023 01:38:24 GMT
ENV EMQX_VERSION=5.0.21
# Wed, 12 Apr 2023 01:38:24 GMT
ENV AMD64_SHA256=d83d435bfd49fc06cf9448de12ee76d383f9919fbb4d149545ccc246c903b78e
# Wed, 12 Apr 2023 01:38:24 GMT
ENV ARM64_SHA256=29dc8a470c9d43069dbc0f640e9493a991516fa18e028930726e8a6c7e60afc6
# Wed, 12 Apr 2023 01:38:24 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 12 Apr 2023 01:38:29 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 12 Apr 2023 01:38:29 GMT
WORKDIR /opt/emqx
# Wed, 12 Apr 2023 01:38:29 GMT
USER emqx
# Wed, 12 Apr 2023 01:38:29 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 12 Apr 2023 01:38:30 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 12 Apr 2023 01:38:30 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 12 Apr 2023 01:38:30 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 01:38:30 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b64e3be9abc32d122bd4b9c6cbdc2adc75085b08f7644acbd1e9a963977cd48`  
		Last Modified: Wed, 12 Apr 2023 01:38:53 GMT  
		Size: 3.0 MB (3002944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b665badbe1ecc88ea2bdc4962042f6412551d166e4bc0bfbfcd3e00d159e605`  
		Last Modified: Wed, 12 Apr 2023 01:38:52 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f60cb43970fd9770be4b4842be70e9b0b29ca9b4ff9ab04589f944dc44b3b3`  
		Last Modified: Wed, 12 Apr 2023 01:38:58 GMT  
		Size: 59.4 MB (59427507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860a1f80f58c5f8171a12433e753695633645ebb760bb9604624694d5dfd5618`  
		Last Modified: Wed, 12 Apr 2023 01:38:52 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.22`

```console
$ docker pull emqx@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `emqx:latest`

```console
$ docker pull emqx@sha256:35d0b6f888562d5ea32fdd5b163d7eb75ded34e726b8e891608a7fc9cc6923a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:f989e47367da5a656f82a7aeec894a50ecf5fd083a50b54e74118ab897033f1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.4 MB (101411977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b62de259a0237f960db47c17ace4181a9d0b4651786088aa8a49f8099353a64e`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:42:50 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:42:51 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 12 Apr 2023 00:42:51 GMT
ENV EMQX_VERSION=5.0.21
# Wed, 12 Apr 2023 00:42:51 GMT
ENV AMD64_SHA256=d83d435bfd49fc06cf9448de12ee76d383f9919fbb4d149545ccc246c903b78e
# Wed, 12 Apr 2023 00:42:51 GMT
ENV ARM64_SHA256=29dc8a470c9d43069dbc0f640e9493a991516fa18e028930726e8a6c7e60afc6
# Wed, 12 Apr 2023 00:42:51 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 12 Apr 2023 00:42:57 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 12 Apr 2023 00:42:58 GMT
WORKDIR /opt/emqx
# Wed, 12 Apr 2023 00:42:58 GMT
USER emqx
# Wed, 12 Apr 2023 00:42:58 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 12 Apr 2023 00:42:58 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 12 Apr 2023 00:42:58 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 12 Apr 2023 00:42:58 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 00:42:58 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f79c821cbd23fa1420033390e2828e0922b8efe06687c960eb7ff40edfbd0d6`  
		Last Modified: Wed, 12 Apr 2023 00:43:23 GMT  
		Size: 3.0 MB (2987825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048c1bdd86f15f4d429d049f898a2d3c0f0732c5b7e68a31b824acae055655d8`  
		Last Modified: Wed, 12 Apr 2023 00:43:22 GMT  
		Size: 4.1 KB (4105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4773c7908a53fe2a3cfd56039eb7c0a86af81933b57fb3b539d9f4994f5a4c`  
		Last Modified: Wed, 12 Apr 2023 00:43:30 GMT  
		Size: 67.0 MB (67000917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba19bb9c71ad2945f2eae572505c1e6047c345ec90c0a9283aba640bcca70e9c`  
		Last Modified: Wed, 12 Apr 2023 00:43:23 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:4768cca0bdd0c9d3220c04324dae4f23d4a0d173198389d53f94fd9a298900b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.5 MB (92499291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e18a3436e25d685512eaaa2535734c8393159049706f41427222cad25dbf636`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:38:23 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:38:24 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 12 Apr 2023 01:38:24 GMT
ENV EMQX_VERSION=5.0.21
# Wed, 12 Apr 2023 01:38:24 GMT
ENV AMD64_SHA256=d83d435bfd49fc06cf9448de12ee76d383f9919fbb4d149545ccc246c903b78e
# Wed, 12 Apr 2023 01:38:24 GMT
ENV ARM64_SHA256=29dc8a470c9d43069dbc0f640e9493a991516fa18e028930726e8a6c7e60afc6
# Wed, 12 Apr 2023 01:38:24 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 12 Apr 2023 01:38:29 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 12 Apr 2023 01:38:29 GMT
WORKDIR /opt/emqx
# Wed, 12 Apr 2023 01:38:29 GMT
USER emqx
# Wed, 12 Apr 2023 01:38:29 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 12 Apr 2023 01:38:30 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 12 Apr 2023 01:38:30 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 12 Apr 2023 01:38:30 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 01:38:30 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b64e3be9abc32d122bd4b9c6cbdc2adc75085b08f7644acbd1e9a963977cd48`  
		Last Modified: Wed, 12 Apr 2023 01:38:53 GMT  
		Size: 3.0 MB (3002944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b665badbe1ecc88ea2bdc4962042f6412551d166e4bc0bfbfcd3e00d159e605`  
		Last Modified: Wed, 12 Apr 2023 01:38:52 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f60cb43970fd9770be4b4842be70e9b0b29ca9b4ff9ab04589f944dc44b3b3`  
		Last Modified: Wed, 12 Apr 2023 01:38:58 GMT  
		Size: 59.4 MB (59427507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860a1f80f58c5f8171a12433e753695633645ebb760bb9604624694d5dfd5618`  
		Last Modified: Wed, 12 Apr 2023 01:38:52 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
