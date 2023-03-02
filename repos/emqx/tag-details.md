<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.3`](#emqx43)
-	[`emqx:4.3.22`](#emqx4322)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.14`](#emqx4414)
-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.19`](#emqx5019)
-	[`emqx:latest`](#emqxlatest)

## `emqx:4`

```console
$ docker pull emqx@sha256:f5c19a42b900c15fec735697d073a7eb891ad2fea64686ee51366f462f92e977
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:9925947130abf045695cca3dea026930762a4c66414242f139e42438a424adee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81177936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44662d454ecfb614f83cac143bf823dde93c77534999091c719372192bec1ac7`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:03:11 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:03:11 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 01 Mar 2023 05:03:11 GMT
ENV EMQX_VERSION=4.4.14
# Wed, 01 Mar 2023 05:03:11 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 01 Mar 2023 05:03:16 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 01 Mar 2023 05:03:16 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 05:03:17 GMT
USER emqx
# Wed, 01 Mar 2023 05:03:17 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 05:03:17 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 01 Mar 2023 05:03:17 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 01 Mar 2023 05:03:17 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 05:03:17 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396ee3d6a271f9fce1d0b1fd4fc0bd3a54cd9c9139a819de5351b130046fea9d`  
		Last Modified: Wed, 01 Mar 2023 05:04:03 GMT  
		Size: 2.6 MB (2569541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79aa88ad721c3aad2bd0e2aaccdbb555263a96f1e69f9f9e7e2e698cbd61acf`  
		Last Modified: Wed, 01 Mar 2023 05:04:02 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b421161b99172f6c3dabd83eae35c1489da7480d66860300f0b6b4025aec422`  
		Last Modified: Wed, 01 Mar 2023 05:04:08 GMT  
		Size: 47.2 MB (47191775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade1f522c63517d3db149447ad0de1fae150bd0ff001332ce58d3fec3140d039`  
		Last Modified: Wed, 01 Mar 2023 05:04:02 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:ae8f840eb106d5d18af9e4487d3a3819c28a3542c5d10c43e61d9ceff411e5b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72603155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f38f6b8bf7be6fc7d357641e49d09960febef32976b22b9f71f593796a393906`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:03 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:03 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 01 Mar 2023 03:21:03 GMT
ENV EMQX_VERSION=4.4.14
# Wed, 01 Mar 2023 03:21:03 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 01 Mar 2023 03:21:07 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 01 Mar 2023 03:21:07 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 03:21:07 GMT
USER emqx
# Wed, 01 Mar 2023 03:21:07 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 03:21:07 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 01 Mar 2023 03:21:07 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 01 Mar 2023 03:21:07 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 03:21:08 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ea117f9b26bad2c79fea1dafb19b2ccbfb0e0744061d7743a5aea0c0e38af7`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 2.6 MB (2559230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fde159950f1c178189d5f614a5405bd1df5caabc1ebd2bfc1e35376f9bd0e19`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d42366bbef4db720a85360a1e5ec058db9bd96b35006fbc973a5cf9ecbf48b`  
		Last Modified: Wed, 01 Mar 2023 03:21:53 GMT  
		Size: 40.0 MB (39975889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019c9ee157601eb624484538f97008c28085e534e6a64105956cf6e213907f0f`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3`

```console
$ docker pull emqx@sha256:44be32a81a37ad37bdfa5ffeb79489cca276e1f979b944ce021e4314192f8624
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3` - linux; amd64

```console
$ docker pull emqx@sha256:b56ab632dd6a1a200e4df0256cfbe5e0ff61d78dd2a813fd31890fa98830d423
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68297666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65bb5db22a5b3c692b92f3c76acdf93e71a1d550b3a9bf10ca721490b806df8d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:22 GMT
ADD file:2254e48bf53907be7a0b1744bc4fcd7805a627672793cf5f86a01ac751a1b24d in / 
# Wed, 01 Mar 2023 04:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:02:55 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:02:56 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 01 Mar 2023 05:02:56 GMT
ENV EMQX_VERSION=4.3.22
# Wed, 01 Mar 2023 05:03:00 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 01 Mar 2023 05:03:00 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 05:03:00 GMT
USER emqx
# Wed, 01 Mar 2023 05:03:00 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 05:03:00 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 01 Mar 2023 05:03:01 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Wed, 01 Mar 2023 05:03:01 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 05:03:01 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:8fd419aca81cfd3987d61550e700546537628562693bc01acc9f85468f483706`  
		Last Modified: Wed, 01 Mar 2023 04:15:04 GMT  
		Size: 27.1 MB (27139882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67076c499bc9b87ea800a1a15f827f09ec02243971bc50429ede922233b306e`  
		Last Modified: Wed, 01 Mar 2023 05:03:50 GMT  
		Size: 4.6 MB (4613913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea322942ca5ca8724f4e0402fd4535d9c4ce5727ce02b43967aaf45df5b6f11`  
		Last Modified: Wed, 01 Mar 2023 05:03:49 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25300f2d707eb52cf44cbc8158d804eb20aec49de67ba58fa1eb90084591c74a`  
		Last Modified: Wed, 01 Mar 2023 05:03:53 GMT  
		Size: 36.5 MB (36538719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f365602634a44efd06fbfafc0c932fe8fa49092192415548e9f38f1256f72526`  
		Last Modified: Wed, 01 Mar 2023 05:03:49 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:89ad756cddacc9a8e7d657437fef22d6a04a63552fd523dd810ff5a3527d445a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66639578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be9948dc18d32a4562583e65e5455a098e0e8eea0f5c378b5560ae8eaf12749b`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:56 GMT
ADD file:ab0ca1f1ee3db357c8de06fd63e3d5f0132541162438c121e99f29e6af190bfa in / 
# Wed, 01 Mar 2023 02:20:56 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:20:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:20:51 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 01 Mar 2023 03:20:51 GMT
ENV EMQX_VERSION=4.3.22
# Wed, 01 Mar 2023 03:20:55 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 01 Mar 2023 03:20:55 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 03:20:55 GMT
USER emqx
# Wed, 01 Mar 2023 03:20:56 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 03:20:56 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 01 Mar 2023 03:20:56 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Wed, 01 Mar 2023 03:20:56 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 03:20:56 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:ed22f951ea44cd39f81544a2f0bf196ad60d13c1428cea537535186be61818f7`  
		Last Modified: Wed, 01 Mar 2023 02:24:56 GMT  
		Size: 25.9 MB (25922699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7346bcd4662575fe5f0ea4143c451c7843a2927e5d0af2c294e7c7b589e9d3e0`  
		Last Modified: Wed, 01 Mar 2023 03:21:38 GMT  
		Size: 4.5 MB (4493853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ef18dcd45f52a315de3b9e5a1b3bc82ce7266e4c0a09c1c54ee9e64042d3d3`  
		Last Modified: Wed, 01 Mar 2023 03:21:37 GMT  
		Size: 4.1 KB (4110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff6e06a2ade1d5dfdb81d43c239729701492a224e96c96b6c9c754206dcad4a`  
		Last Modified: Wed, 01 Mar 2023 03:21:41 GMT  
		Size: 36.2 MB (36217876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050b237224db3aa1ad2c03c13cefb9af92d7c7610660dd90e017c2605cadf57b`  
		Last Modified: Wed, 01 Mar 2023 03:21:37 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3.22`

```console
$ docker pull emqx@sha256:44be32a81a37ad37bdfa5ffeb79489cca276e1f979b944ce021e4314192f8624
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3.22` - linux; amd64

```console
$ docker pull emqx@sha256:b56ab632dd6a1a200e4df0256cfbe5e0ff61d78dd2a813fd31890fa98830d423
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68297666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65bb5db22a5b3c692b92f3c76acdf93e71a1d550b3a9bf10ca721490b806df8d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:22 GMT
ADD file:2254e48bf53907be7a0b1744bc4fcd7805a627672793cf5f86a01ac751a1b24d in / 
# Wed, 01 Mar 2023 04:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:02:55 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:02:56 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 01 Mar 2023 05:02:56 GMT
ENV EMQX_VERSION=4.3.22
# Wed, 01 Mar 2023 05:03:00 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 01 Mar 2023 05:03:00 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 05:03:00 GMT
USER emqx
# Wed, 01 Mar 2023 05:03:00 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 05:03:00 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 01 Mar 2023 05:03:01 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Wed, 01 Mar 2023 05:03:01 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 05:03:01 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:8fd419aca81cfd3987d61550e700546537628562693bc01acc9f85468f483706`  
		Last Modified: Wed, 01 Mar 2023 04:15:04 GMT  
		Size: 27.1 MB (27139882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67076c499bc9b87ea800a1a15f827f09ec02243971bc50429ede922233b306e`  
		Last Modified: Wed, 01 Mar 2023 05:03:50 GMT  
		Size: 4.6 MB (4613913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea322942ca5ca8724f4e0402fd4535d9c4ce5727ce02b43967aaf45df5b6f11`  
		Last Modified: Wed, 01 Mar 2023 05:03:49 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25300f2d707eb52cf44cbc8158d804eb20aec49de67ba58fa1eb90084591c74a`  
		Last Modified: Wed, 01 Mar 2023 05:03:53 GMT  
		Size: 36.5 MB (36538719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f365602634a44efd06fbfafc0c932fe8fa49092192415548e9f38f1256f72526`  
		Last Modified: Wed, 01 Mar 2023 05:03:49 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3.22` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:89ad756cddacc9a8e7d657437fef22d6a04a63552fd523dd810ff5a3527d445a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66639578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be9948dc18d32a4562583e65e5455a098e0e8eea0f5c378b5560ae8eaf12749b`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:56 GMT
ADD file:ab0ca1f1ee3db357c8de06fd63e3d5f0132541162438c121e99f29e6af190bfa in / 
# Wed, 01 Mar 2023 02:20:56 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:20:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:20:51 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 01 Mar 2023 03:20:51 GMT
ENV EMQX_VERSION=4.3.22
# Wed, 01 Mar 2023 03:20:55 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 01 Mar 2023 03:20:55 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 03:20:55 GMT
USER emqx
# Wed, 01 Mar 2023 03:20:56 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 03:20:56 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 01 Mar 2023 03:20:56 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Wed, 01 Mar 2023 03:20:56 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 03:20:56 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:ed22f951ea44cd39f81544a2f0bf196ad60d13c1428cea537535186be61818f7`  
		Last Modified: Wed, 01 Mar 2023 02:24:56 GMT  
		Size: 25.9 MB (25922699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7346bcd4662575fe5f0ea4143c451c7843a2927e5d0af2c294e7c7b589e9d3e0`  
		Last Modified: Wed, 01 Mar 2023 03:21:38 GMT  
		Size: 4.5 MB (4493853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ef18dcd45f52a315de3b9e5a1b3bc82ce7266e4c0a09c1c54ee9e64042d3d3`  
		Last Modified: Wed, 01 Mar 2023 03:21:37 GMT  
		Size: 4.1 KB (4110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff6e06a2ade1d5dfdb81d43c239729701492a224e96c96b6c9c754206dcad4a`  
		Last Modified: Wed, 01 Mar 2023 03:21:41 GMT  
		Size: 36.2 MB (36217876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050b237224db3aa1ad2c03c13cefb9af92d7c7610660dd90e017c2605cadf57b`  
		Last Modified: Wed, 01 Mar 2023 03:21:37 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:f5c19a42b900c15fec735697d073a7eb891ad2fea64686ee51366f462f92e977
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:9925947130abf045695cca3dea026930762a4c66414242f139e42438a424adee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81177936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44662d454ecfb614f83cac143bf823dde93c77534999091c719372192bec1ac7`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:03:11 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:03:11 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 01 Mar 2023 05:03:11 GMT
ENV EMQX_VERSION=4.4.14
# Wed, 01 Mar 2023 05:03:11 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 01 Mar 2023 05:03:16 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 01 Mar 2023 05:03:16 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 05:03:17 GMT
USER emqx
# Wed, 01 Mar 2023 05:03:17 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 05:03:17 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 01 Mar 2023 05:03:17 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 01 Mar 2023 05:03:17 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 05:03:17 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396ee3d6a271f9fce1d0b1fd4fc0bd3a54cd9c9139a819de5351b130046fea9d`  
		Last Modified: Wed, 01 Mar 2023 05:04:03 GMT  
		Size: 2.6 MB (2569541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79aa88ad721c3aad2bd0e2aaccdbb555263a96f1e69f9f9e7e2e698cbd61acf`  
		Last Modified: Wed, 01 Mar 2023 05:04:02 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b421161b99172f6c3dabd83eae35c1489da7480d66860300f0b6b4025aec422`  
		Last Modified: Wed, 01 Mar 2023 05:04:08 GMT  
		Size: 47.2 MB (47191775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade1f522c63517d3db149447ad0de1fae150bd0ff001332ce58d3fec3140d039`  
		Last Modified: Wed, 01 Mar 2023 05:04:02 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:ae8f840eb106d5d18af9e4487d3a3819c28a3542c5d10c43e61d9ceff411e5b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72603155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f38f6b8bf7be6fc7d357641e49d09960febef32976b22b9f71f593796a393906`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:03 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:03 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 01 Mar 2023 03:21:03 GMT
ENV EMQX_VERSION=4.4.14
# Wed, 01 Mar 2023 03:21:03 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 01 Mar 2023 03:21:07 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 01 Mar 2023 03:21:07 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 03:21:07 GMT
USER emqx
# Wed, 01 Mar 2023 03:21:07 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 03:21:07 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 01 Mar 2023 03:21:07 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 01 Mar 2023 03:21:07 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 03:21:08 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ea117f9b26bad2c79fea1dafb19b2ccbfb0e0744061d7743a5aea0c0e38af7`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 2.6 MB (2559230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fde159950f1c178189d5f614a5405bd1df5caabc1ebd2bfc1e35376f9bd0e19`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d42366bbef4db720a85360a1e5ec058db9bd96b35006fbc973a5cf9ecbf48b`  
		Last Modified: Wed, 01 Mar 2023 03:21:53 GMT  
		Size: 40.0 MB (39975889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019c9ee157601eb624484538f97008c28085e534e6a64105956cf6e213907f0f`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.14`

```console
$ docker pull emqx@sha256:f5c19a42b900c15fec735697d073a7eb891ad2fea64686ee51366f462f92e977
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.14` - linux; amd64

```console
$ docker pull emqx@sha256:9925947130abf045695cca3dea026930762a4c66414242f139e42438a424adee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81177936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44662d454ecfb614f83cac143bf823dde93c77534999091c719372192bec1ac7`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:03:11 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:03:11 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 01 Mar 2023 05:03:11 GMT
ENV EMQX_VERSION=4.4.14
# Wed, 01 Mar 2023 05:03:11 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 01 Mar 2023 05:03:16 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 01 Mar 2023 05:03:16 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 05:03:17 GMT
USER emqx
# Wed, 01 Mar 2023 05:03:17 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 05:03:17 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 01 Mar 2023 05:03:17 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 01 Mar 2023 05:03:17 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 05:03:17 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396ee3d6a271f9fce1d0b1fd4fc0bd3a54cd9c9139a819de5351b130046fea9d`  
		Last Modified: Wed, 01 Mar 2023 05:04:03 GMT  
		Size: 2.6 MB (2569541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79aa88ad721c3aad2bd0e2aaccdbb555263a96f1e69f9f9e7e2e698cbd61acf`  
		Last Modified: Wed, 01 Mar 2023 05:04:02 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b421161b99172f6c3dabd83eae35c1489da7480d66860300f0b6b4025aec422`  
		Last Modified: Wed, 01 Mar 2023 05:04:08 GMT  
		Size: 47.2 MB (47191775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade1f522c63517d3db149447ad0de1fae150bd0ff001332ce58d3fec3140d039`  
		Last Modified: Wed, 01 Mar 2023 05:04:02 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.14` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:ae8f840eb106d5d18af9e4487d3a3819c28a3542c5d10c43e61d9ceff411e5b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72603155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f38f6b8bf7be6fc7d357641e49d09960febef32976b22b9f71f593796a393906`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:03 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:03 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 01 Mar 2023 03:21:03 GMT
ENV EMQX_VERSION=4.4.14
# Wed, 01 Mar 2023 03:21:03 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 01 Mar 2023 03:21:07 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 01 Mar 2023 03:21:07 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 03:21:07 GMT
USER emqx
# Wed, 01 Mar 2023 03:21:07 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 03:21:07 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 01 Mar 2023 03:21:07 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 01 Mar 2023 03:21:07 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 03:21:08 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ea117f9b26bad2c79fea1dafb19b2ccbfb0e0744061d7743a5aea0c0e38af7`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 2.6 MB (2559230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fde159950f1c178189d5f614a5405bd1df5caabc1ebd2bfc1e35376f9bd0e19`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d42366bbef4db720a85360a1e5ec058db9bd96b35006fbc973a5cf9ecbf48b`  
		Last Modified: Wed, 01 Mar 2023 03:21:53 GMT  
		Size: 40.0 MB (39975889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019c9ee157601eb624484538f97008c28085e534e6a64105956cf6e213907f0f`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5`

```console
$ docker pull emqx@sha256:ac5b5c0abe4fca5c7021deba6626955b6f73a3d3729708a139f5cfbc70a43f33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:7b5f07c9a2de5626df4bcf9b120676522ff379c3b20d7060470fb67cbcf66d40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100382719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a13c680478644672ceb0b19237bd2936f3b50df800a5b541fba5af6b777bb7a0`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:03:25 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:03:26 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Mar 2023 05:03:26 GMT
ENV EMQX_VERSION=5.0.17
# Wed, 01 Mar 2023 05:03:26 GMT
ENV AMD64_SHA256=baed949959990ac18c12f35776a8ddf3b0bc4db3f7a855997e127b1fd1e7f1a7
# Wed, 01 Mar 2023 05:03:26 GMT
ENV ARM64_SHA256=1a2c40a71d55814e99207537616e4fec1c401fea77b53612c6d24dc7d55fe13d
# Wed, 01 Mar 2023 05:03:26 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Mar 2023 05:03:32 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 01 Mar 2023 05:03:32 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 05:03:32 GMT
USER emqx
# Wed, 01 Mar 2023 05:03:33 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 05:03:33 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Mar 2023 05:03:33 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Mar 2023 05:03:33 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 05:03:33 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a35a595ef04513102e76624112833df5aee4f5e7a95b61fa5eddc304211ab3`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 3.0 MB (2987679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e798ac719c7147c6c2faada408a48221abe27042dbc139527a475289fd20c98a`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90082bdef278a00e8f0f402c5d1d0d16842f414d5c26f1026e94c85a09e8c01`  
		Last Modified: Wed, 01 Mar 2023 05:04:27 GMT  
		Size: 66.0 MB (65978625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3520531f1aedaeb8f6657b0038a7910aadfbc1ac68d967315920e63f1d64e6f7`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:d222de7e3082562495e7489361785d9afff79946b6f7cf539cdb413c925cd1e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91481252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e07131b1bf1a6771f2062969c0e108ec4a223c65b61d57d8f5eaccc2b04af83e`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:17 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Mar 2023 03:21:17 GMT
ENV EMQX_VERSION=5.0.17
# Wed, 01 Mar 2023 03:21:17 GMT
ENV AMD64_SHA256=baed949959990ac18c12f35776a8ddf3b0bc4db3f7a855997e127b1fd1e7f1a7
# Wed, 01 Mar 2023 03:21:17 GMT
ENV ARM64_SHA256=1a2c40a71d55814e99207537616e4fec1c401fea77b53612c6d24dc7d55fe13d
# Wed, 01 Mar 2023 03:21:17 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Mar 2023 03:21:22 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 01 Mar 2023 03:21:23 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 03:21:23 GMT
USER emqx
# Wed, 01 Mar 2023 03:21:23 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 03:21:23 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Mar 2023 03:21:23 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Mar 2023 03:21:23 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 03:21:23 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38086ab7a191a5da95fb6158c384014d022c21f7e3615ad8b0cdd460c25f9035`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 3.0 MB (3002759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54eeac58f385f878614093545595a71c10cb909203557c85c1b5ef5defba64d`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5876ed859c2399e42063251e048eb01628d191474154ee3e2692e01707e8c5`  
		Last Modified: Wed, 01 Mar 2023 03:22:10 GMT  
		Size: 58.4 MB (58410663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7ba419171d628ef2af2a2a9c4f4970ebc699c278af40d2d4fa9f8b097c7426`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:ac5b5c0abe4fca5c7021deba6626955b6f73a3d3729708a139f5cfbc70a43f33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:7b5f07c9a2de5626df4bcf9b120676522ff379c3b20d7060470fb67cbcf66d40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100382719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a13c680478644672ceb0b19237bd2936f3b50df800a5b541fba5af6b777bb7a0`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:03:25 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:03:26 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Mar 2023 05:03:26 GMT
ENV EMQX_VERSION=5.0.17
# Wed, 01 Mar 2023 05:03:26 GMT
ENV AMD64_SHA256=baed949959990ac18c12f35776a8ddf3b0bc4db3f7a855997e127b1fd1e7f1a7
# Wed, 01 Mar 2023 05:03:26 GMT
ENV ARM64_SHA256=1a2c40a71d55814e99207537616e4fec1c401fea77b53612c6d24dc7d55fe13d
# Wed, 01 Mar 2023 05:03:26 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Mar 2023 05:03:32 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 01 Mar 2023 05:03:32 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 05:03:32 GMT
USER emqx
# Wed, 01 Mar 2023 05:03:33 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 05:03:33 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Mar 2023 05:03:33 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Mar 2023 05:03:33 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 05:03:33 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a35a595ef04513102e76624112833df5aee4f5e7a95b61fa5eddc304211ab3`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 3.0 MB (2987679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e798ac719c7147c6c2faada408a48221abe27042dbc139527a475289fd20c98a`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90082bdef278a00e8f0f402c5d1d0d16842f414d5c26f1026e94c85a09e8c01`  
		Last Modified: Wed, 01 Mar 2023 05:04:27 GMT  
		Size: 66.0 MB (65978625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3520531f1aedaeb8f6657b0038a7910aadfbc1ac68d967315920e63f1d64e6f7`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:d222de7e3082562495e7489361785d9afff79946b6f7cf539cdb413c925cd1e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91481252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e07131b1bf1a6771f2062969c0e108ec4a223c65b61d57d8f5eaccc2b04af83e`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:17 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Mar 2023 03:21:17 GMT
ENV EMQX_VERSION=5.0.17
# Wed, 01 Mar 2023 03:21:17 GMT
ENV AMD64_SHA256=baed949959990ac18c12f35776a8ddf3b0bc4db3f7a855997e127b1fd1e7f1a7
# Wed, 01 Mar 2023 03:21:17 GMT
ENV ARM64_SHA256=1a2c40a71d55814e99207537616e4fec1c401fea77b53612c6d24dc7d55fe13d
# Wed, 01 Mar 2023 03:21:17 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Mar 2023 03:21:22 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 01 Mar 2023 03:21:23 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 03:21:23 GMT
USER emqx
# Wed, 01 Mar 2023 03:21:23 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 03:21:23 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Mar 2023 03:21:23 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Mar 2023 03:21:23 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 03:21:23 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38086ab7a191a5da95fb6158c384014d022c21f7e3615ad8b0cdd460c25f9035`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 3.0 MB (3002759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54eeac58f385f878614093545595a71c10cb909203557c85c1b5ef5defba64d`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5876ed859c2399e42063251e048eb01628d191474154ee3e2692e01707e8c5`  
		Last Modified: Wed, 01 Mar 2023 03:22:10 GMT  
		Size: 58.4 MB (58410663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7ba419171d628ef2af2a2a9c4f4970ebc699c278af40d2d4fa9f8b097c7426`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.19`

**does not exist** (yet?)

## `emqx:latest`

```console
$ docker pull emqx@sha256:ac5b5c0abe4fca5c7021deba6626955b6f73a3d3729708a139f5cfbc70a43f33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:7b5f07c9a2de5626df4bcf9b120676522ff379c3b20d7060470fb67cbcf66d40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100382719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a13c680478644672ceb0b19237bd2936f3b50df800a5b541fba5af6b777bb7a0`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:03:25 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:03:26 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Mar 2023 05:03:26 GMT
ENV EMQX_VERSION=5.0.17
# Wed, 01 Mar 2023 05:03:26 GMT
ENV AMD64_SHA256=baed949959990ac18c12f35776a8ddf3b0bc4db3f7a855997e127b1fd1e7f1a7
# Wed, 01 Mar 2023 05:03:26 GMT
ENV ARM64_SHA256=1a2c40a71d55814e99207537616e4fec1c401fea77b53612c6d24dc7d55fe13d
# Wed, 01 Mar 2023 05:03:26 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Mar 2023 05:03:32 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 01 Mar 2023 05:03:32 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 05:03:32 GMT
USER emqx
# Wed, 01 Mar 2023 05:03:33 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 05:03:33 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Mar 2023 05:03:33 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Mar 2023 05:03:33 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 05:03:33 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a35a595ef04513102e76624112833df5aee4f5e7a95b61fa5eddc304211ab3`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 3.0 MB (2987679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e798ac719c7147c6c2faada408a48221abe27042dbc139527a475289fd20c98a`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90082bdef278a00e8f0f402c5d1d0d16842f414d5c26f1026e94c85a09e8c01`  
		Last Modified: Wed, 01 Mar 2023 05:04:27 GMT  
		Size: 66.0 MB (65978625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3520531f1aedaeb8f6657b0038a7910aadfbc1ac68d967315920e63f1d64e6f7`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:d222de7e3082562495e7489361785d9afff79946b6f7cf539cdb413c925cd1e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91481252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e07131b1bf1a6771f2062969c0e108ec4a223c65b61d57d8f5eaccc2b04af83e`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:17 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Mar 2023 03:21:17 GMT
ENV EMQX_VERSION=5.0.17
# Wed, 01 Mar 2023 03:21:17 GMT
ENV AMD64_SHA256=baed949959990ac18c12f35776a8ddf3b0bc4db3f7a855997e127b1fd1e7f1a7
# Wed, 01 Mar 2023 03:21:17 GMT
ENV ARM64_SHA256=1a2c40a71d55814e99207537616e4fec1c401fea77b53612c6d24dc7d55fe13d
# Wed, 01 Mar 2023 03:21:17 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Mar 2023 03:21:22 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 01 Mar 2023 03:21:23 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 03:21:23 GMT
USER emqx
# Wed, 01 Mar 2023 03:21:23 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 03:21:23 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Mar 2023 03:21:23 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Mar 2023 03:21:23 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 03:21:23 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38086ab7a191a5da95fb6158c384014d022c21f7e3615ad8b0cdd460c25f9035`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 3.0 MB (3002759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54eeac58f385f878614093545595a71c10cb909203557c85c1b5ef5defba64d`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5876ed859c2399e42063251e048eb01628d191474154ee3e2692e01707e8c5`  
		Last Modified: Wed, 01 Mar 2023 03:22:10 GMT  
		Size: 58.4 MB (58410663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7ba419171d628ef2af2a2a9c4f4970ebc699c278af40d2d4fa9f8b097c7426`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
