<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.3`](#emqx43)
-	[`emqx:4.3.22`](#emqx4322)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.11`](#emqx4411)
-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.13`](#emqx5013)
-	[`emqx:latest`](#emqxlatest)

## `emqx:4`

```console
$ docker pull emqx@sha256:38f86c76af0506dfcb38b534bfc9f28814514dbe593c4d99bed26187bdaf1871
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:2f8a6bd7a179a1c8938177b799450bb9279d1595e291fccc0174dc2853322bfe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127221348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bc68d4844f0af5cb3a28250e22f90b59abed0fbccc1960b485432343aeaa42`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:19:00 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:19:00 GMT
ENV EMQX_VERSION=4.4.11
# Wed, 21 Dec 2022 02:19:00 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 21 Dec 2022 02:19:05 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 21 Dec 2022 02:19:11 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 21 Dec 2022 02:19:11 GMT
WORKDIR /opt/emqx
# Wed, 21 Dec 2022 02:19:11 GMT
USER emqx
# Wed, 21 Dec 2022 02:19:11 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 21 Dec 2022 02:19:12 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 21 Dec 2022 02:19:12 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 21 Dec 2022 02:19:12 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 02:19:12 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51bc532c35fbcc15da7a7847c0ae8e4ccf0896b1f4a79e8d44d0ee557da66d5`  
		Last Modified: Wed, 21 Dec 2022 02:19:56 GMT  
		Size: 2.6 MB (2569551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c5156f480d8640f01b600e9b336ab38aa15c3b737c5e73c1c5d29be106fe4f`  
		Last Modified: Wed, 21 Dec 2022 02:20:01 GMT  
		Size: 46.6 MB (46617924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc30cedb682ef867160fe3bce54d111696ce3a73dbab3283af8562408df3145`  
		Last Modified: Wed, 21 Dec 2022 02:20:01 GMT  
		Size: 46.6 MB (46635822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68279017f9aafa2157e88c860f91c4221e854516c610a87b3190d343e4aacf51`  
		Last Modified: Wed, 21 Dec 2022 02:19:56 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:7dd73709b94fa0ef33a02bf7a0218d323d3ed9d16638aa6ace75784c30c8357c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111417879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b813fe567331d7d68c23ca54201ff7de9b2a7c0faf40a4e409cb6ed3ee0a45f0`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:37:34 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:37:35 GMT
ENV EMQX_VERSION=4.4.11
# Wed, 21 Dec 2022 02:37:35 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 21 Dec 2022 02:37:38 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 21 Dec 2022 02:37:42 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 21 Dec 2022 02:37:42 GMT
WORKDIR /opt/emqx
# Wed, 21 Dec 2022 02:37:42 GMT
USER emqx
# Wed, 21 Dec 2022 02:37:42 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 21 Dec 2022 02:37:43 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 21 Dec 2022 02:37:43 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 21 Dec 2022 02:37:43 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 02:37:43 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f54b227d051db3a5adf4052f23f9f04079b36c5ee7325bc0bb89de5a0c01431`  
		Last Modified: Wed, 21 Dec 2022 02:38:23 GMT  
		Size: 2.6 MB (2559277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6294bd6555bd8ecb18f540f500f4c59148623e99e95097727bf3f066d0e5e7`  
		Last Modified: Wed, 21 Dec 2022 02:38:26 GMT  
		Size: 39.4 MB (39403616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28334a224641a108af0414ab663b2c97afdb9b7d3ca87b7e628b50444deef003`  
		Last Modified: Wed, 21 Dec 2022 02:38:26 GMT  
		Size: 39.4 MB (39409106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd76f1db199d5827e580d508673f871505dcd0788aae5af91b3138f18700dc5`  
		Last Modified: Wed, 21 Dec 2022 02:38:22 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3`

```console
$ docker pull emqx@sha256:9bfee4254e1839fd4fd568ede64cd1673fd60673fc68d2a62bb9dd938cb58f7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3` - linux; amd64

```console
$ docker pull emqx@sha256:a20e751c3d21100a4920feec920c7624d7cefede32be951b40a29aedd28e577a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.8 MB (104828519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca3993829218abf48294e8b86277778397977077242765bf5a77cee263ee19d5`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:52 GMT
ADD file:660e0093a3da49e4ca41260d09d585754ccb1eff8974c4b0dd4456b76ddbbc9a in / 
# Wed, 21 Dec 2022 01:20:52 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:18:41 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:18:42 GMT
ENV EMQX_VERSION=4.3.22
# Wed, 21 Dec 2022 02:18:46 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 21 Dec 2022 02:18:51 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 21 Dec 2022 02:18:52 GMT
WORKDIR /opt/emqx
# Wed, 21 Dec 2022 02:18:52 GMT
USER emqx
# Wed, 21 Dec 2022 02:18:52 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 21 Dec 2022 02:18:52 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 21 Dec 2022 02:18:52 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Wed, 21 Dec 2022 02:18:52 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 02:18:52 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:b52ebda398ed2c4602ea06056f78d45a59474ee4e2a020967251ba082424e7e2`  
		Last Modified: Wed, 21 Dec 2022 01:25:17 GMT  
		Size: 27.1 MB (27140331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7ded23573403c36aa1c6351ef9873e7155a90fdb0fa126adb6013e5dce9f33`  
		Last Modified: Wed, 21 Dec 2022 02:19:43 GMT  
		Size: 4.6 MB (4612551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a104cdeb4fe1d1a34c7d78d659c38a9e90ae41ff826a0f8bf937fc1896e40716`  
		Last Modified: Wed, 21 Dec 2022 02:19:47 GMT  
		Size: 36.5 MB (36537214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838b486d86bfe4dc5bfa977c59dfba5e389fdd4f4a0728ffdd2de86ddee1361c`  
		Last Modified: Wed, 21 Dec 2022 02:19:47 GMT  
		Size: 36.5 MB (36537381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36564107aa0a1782ba18b2fcdee3ae34e402cf304576afbdaed70daee1423d29`  
		Last Modified: Wed, 21 Dec 2022 02:19:42 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:9803d13f2887e3f9e287ab35fe5d3bf83f5a7404baf0ace6157c6409bb46ca0d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102846198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a7717370b6f52a08cfa7b77daa9075c62a16e4d93fae6baa119fd6dde41882`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:40:02 GMT
ADD file:51788132818f0e1cbed57cd022358b0564ec0d9cab6d33e5ef53902645d53c98 in / 
# Wed, 21 Dec 2022 01:40:02 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:37:19 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:37:19 GMT
ENV EMQX_VERSION=4.3.22
# Wed, 21 Dec 2022 02:37:23 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 21 Dec 2022 02:37:27 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 21 Dec 2022 02:37:28 GMT
WORKDIR /opt/emqx
# Wed, 21 Dec 2022 02:37:28 GMT
USER emqx
# Wed, 21 Dec 2022 02:37:28 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 21 Dec 2022 02:37:28 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 21 Dec 2022 02:37:28 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Wed, 21 Dec 2022 02:37:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 02:37:28 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:eb4ce5bba15e4b6fd353d7fc222fbe9c71d6881cefe1e10384c6c358d4b4eb90`  
		Last Modified: Wed, 21 Dec 2022 01:43:52 GMT  
		Size: 25.9 MB (25914906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd6c73c4f5079d9f33c5b9fd8a0070a9ac92fa0e44194ab2c9a2e58ba5e661b`  
		Last Modified: Wed, 21 Dec 2022 02:38:11 GMT  
		Size: 4.5 MB (4490402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe70d99423f90fb9b757a52e857f7feb92cb724c5dd4d4fbe83a2431772a449f`  
		Last Modified: Wed, 21 Dec 2022 02:38:14 GMT  
		Size: 36.2 MB (36216040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ad5dd0deaa2677941018aaed289fa57c7106cb0bd14a4cf665fd8ec0314f18`  
		Last Modified: Wed, 21 Dec 2022 02:38:14 GMT  
		Size: 36.2 MB (36223809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b046a5dab4938961f37eabebcd6f35c6180a2bff6280a6cb11275120f588e5a5`  
		Last Modified: Wed, 21 Dec 2022 02:38:11 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3.22`

```console
$ docker pull emqx@sha256:9bfee4254e1839fd4fd568ede64cd1673fd60673fc68d2a62bb9dd938cb58f7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3.22` - linux; amd64

```console
$ docker pull emqx@sha256:a20e751c3d21100a4920feec920c7624d7cefede32be951b40a29aedd28e577a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.8 MB (104828519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca3993829218abf48294e8b86277778397977077242765bf5a77cee263ee19d5`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:52 GMT
ADD file:660e0093a3da49e4ca41260d09d585754ccb1eff8974c4b0dd4456b76ddbbc9a in / 
# Wed, 21 Dec 2022 01:20:52 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:18:41 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:18:42 GMT
ENV EMQX_VERSION=4.3.22
# Wed, 21 Dec 2022 02:18:46 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 21 Dec 2022 02:18:51 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 21 Dec 2022 02:18:52 GMT
WORKDIR /opt/emqx
# Wed, 21 Dec 2022 02:18:52 GMT
USER emqx
# Wed, 21 Dec 2022 02:18:52 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 21 Dec 2022 02:18:52 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 21 Dec 2022 02:18:52 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Wed, 21 Dec 2022 02:18:52 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 02:18:52 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:b52ebda398ed2c4602ea06056f78d45a59474ee4e2a020967251ba082424e7e2`  
		Last Modified: Wed, 21 Dec 2022 01:25:17 GMT  
		Size: 27.1 MB (27140331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7ded23573403c36aa1c6351ef9873e7155a90fdb0fa126adb6013e5dce9f33`  
		Last Modified: Wed, 21 Dec 2022 02:19:43 GMT  
		Size: 4.6 MB (4612551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a104cdeb4fe1d1a34c7d78d659c38a9e90ae41ff826a0f8bf937fc1896e40716`  
		Last Modified: Wed, 21 Dec 2022 02:19:47 GMT  
		Size: 36.5 MB (36537214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838b486d86bfe4dc5bfa977c59dfba5e389fdd4f4a0728ffdd2de86ddee1361c`  
		Last Modified: Wed, 21 Dec 2022 02:19:47 GMT  
		Size: 36.5 MB (36537381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36564107aa0a1782ba18b2fcdee3ae34e402cf304576afbdaed70daee1423d29`  
		Last Modified: Wed, 21 Dec 2022 02:19:42 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3.22` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:9803d13f2887e3f9e287ab35fe5d3bf83f5a7404baf0ace6157c6409bb46ca0d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102846198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a7717370b6f52a08cfa7b77daa9075c62a16e4d93fae6baa119fd6dde41882`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:40:02 GMT
ADD file:51788132818f0e1cbed57cd022358b0564ec0d9cab6d33e5ef53902645d53c98 in / 
# Wed, 21 Dec 2022 01:40:02 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:37:19 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:37:19 GMT
ENV EMQX_VERSION=4.3.22
# Wed, 21 Dec 2022 02:37:23 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 21 Dec 2022 02:37:27 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 21 Dec 2022 02:37:28 GMT
WORKDIR /opt/emqx
# Wed, 21 Dec 2022 02:37:28 GMT
USER emqx
# Wed, 21 Dec 2022 02:37:28 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 21 Dec 2022 02:37:28 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 21 Dec 2022 02:37:28 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Wed, 21 Dec 2022 02:37:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 02:37:28 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:eb4ce5bba15e4b6fd353d7fc222fbe9c71d6881cefe1e10384c6c358d4b4eb90`  
		Last Modified: Wed, 21 Dec 2022 01:43:52 GMT  
		Size: 25.9 MB (25914906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd6c73c4f5079d9f33c5b9fd8a0070a9ac92fa0e44194ab2c9a2e58ba5e661b`  
		Last Modified: Wed, 21 Dec 2022 02:38:11 GMT  
		Size: 4.5 MB (4490402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe70d99423f90fb9b757a52e857f7feb92cb724c5dd4d4fbe83a2431772a449f`  
		Last Modified: Wed, 21 Dec 2022 02:38:14 GMT  
		Size: 36.2 MB (36216040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ad5dd0deaa2677941018aaed289fa57c7106cb0bd14a4cf665fd8ec0314f18`  
		Last Modified: Wed, 21 Dec 2022 02:38:14 GMT  
		Size: 36.2 MB (36223809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b046a5dab4938961f37eabebcd6f35c6180a2bff6280a6cb11275120f588e5a5`  
		Last Modified: Wed, 21 Dec 2022 02:38:11 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:38f86c76af0506dfcb38b534bfc9f28814514dbe593c4d99bed26187bdaf1871
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:2f8a6bd7a179a1c8938177b799450bb9279d1595e291fccc0174dc2853322bfe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127221348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bc68d4844f0af5cb3a28250e22f90b59abed0fbccc1960b485432343aeaa42`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:19:00 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:19:00 GMT
ENV EMQX_VERSION=4.4.11
# Wed, 21 Dec 2022 02:19:00 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 21 Dec 2022 02:19:05 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 21 Dec 2022 02:19:11 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 21 Dec 2022 02:19:11 GMT
WORKDIR /opt/emqx
# Wed, 21 Dec 2022 02:19:11 GMT
USER emqx
# Wed, 21 Dec 2022 02:19:11 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 21 Dec 2022 02:19:12 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 21 Dec 2022 02:19:12 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 21 Dec 2022 02:19:12 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 02:19:12 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51bc532c35fbcc15da7a7847c0ae8e4ccf0896b1f4a79e8d44d0ee557da66d5`  
		Last Modified: Wed, 21 Dec 2022 02:19:56 GMT  
		Size: 2.6 MB (2569551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c5156f480d8640f01b600e9b336ab38aa15c3b737c5e73c1c5d29be106fe4f`  
		Last Modified: Wed, 21 Dec 2022 02:20:01 GMT  
		Size: 46.6 MB (46617924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc30cedb682ef867160fe3bce54d111696ce3a73dbab3283af8562408df3145`  
		Last Modified: Wed, 21 Dec 2022 02:20:01 GMT  
		Size: 46.6 MB (46635822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68279017f9aafa2157e88c860f91c4221e854516c610a87b3190d343e4aacf51`  
		Last Modified: Wed, 21 Dec 2022 02:19:56 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:7dd73709b94fa0ef33a02bf7a0218d323d3ed9d16638aa6ace75784c30c8357c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111417879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b813fe567331d7d68c23ca54201ff7de9b2a7c0faf40a4e409cb6ed3ee0a45f0`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:37:34 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:37:35 GMT
ENV EMQX_VERSION=4.4.11
# Wed, 21 Dec 2022 02:37:35 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 21 Dec 2022 02:37:38 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 21 Dec 2022 02:37:42 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 21 Dec 2022 02:37:42 GMT
WORKDIR /opt/emqx
# Wed, 21 Dec 2022 02:37:42 GMT
USER emqx
# Wed, 21 Dec 2022 02:37:42 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 21 Dec 2022 02:37:43 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 21 Dec 2022 02:37:43 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 21 Dec 2022 02:37:43 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 02:37:43 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f54b227d051db3a5adf4052f23f9f04079b36c5ee7325bc0bb89de5a0c01431`  
		Last Modified: Wed, 21 Dec 2022 02:38:23 GMT  
		Size: 2.6 MB (2559277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6294bd6555bd8ecb18f540f500f4c59148623e99e95097727bf3f066d0e5e7`  
		Last Modified: Wed, 21 Dec 2022 02:38:26 GMT  
		Size: 39.4 MB (39403616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28334a224641a108af0414ab663b2c97afdb9b7d3ca87b7e628b50444deef003`  
		Last Modified: Wed, 21 Dec 2022 02:38:26 GMT  
		Size: 39.4 MB (39409106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd76f1db199d5827e580d508673f871505dcd0788aae5af91b3138f18700dc5`  
		Last Modified: Wed, 21 Dec 2022 02:38:22 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.11`

```console
$ docker pull emqx@sha256:38f86c76af0506dfcb38b534bfc9f28814514dbe593c4d99bed26187bdaf1871
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.11` - linux; amd64

```console
$ docker pull emqx@sha256:2f8a6bd7a179a1c8938177b799450bb9279d1595e291fccc0174dc2853322bfe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127221348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bc68d4844f0af5cb3a28250e22f90b59abed0fbccc1960b485432343aeaa42`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:19:00 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:19:00 GMT
ENV EMQX_VERSION=4.4.11
# Wed, 21 Dec 2022 02:19:00 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 21 Dec 2022 02:19:05 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 21 Dec 2022 02:19:11 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 21 Dec 2022 02:19:11 GMT
WORKDIR /opt/emqx
# Wed, 21 Dec 2022 02:19:11 GMT
USER emqx
# Wed, 21 Dec 2022 02:19:11 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 21 Dec 2022 02:19:12 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 21 Dec 2022 02:19:12 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 21 Dec 2022 02:19:12 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 02:19:12 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51bc532c35fbcc15da7a7847c0ae8e4ccf0896b1f4a79e8d44d0ee557da66d5`  
		Last Modified: Wed, 21 Dec 2022 02:19:56 GMT  
		Size: 2.6 MB (2569551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c5156f480d8640f01b600e9b336ab38aa15c3b737c5e73c1c5d29be106fe4f`  
		Last Modified: Wed, 21 Dec 2022 02:20:01 GMT  
		Size: 46.6 MB (46617924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc30cedb682ef867160fe3bce54d111696ce3a73dbab3283af8562408df3145`  
		Last Modified: Wed, 21 Dec 2022 02:20:01 GMT  
		Size: 46.6 MB (46635822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68279017f9aafa2157e88c860f91c4221e854516c610a87b3190d343e4aacf51`  
		Last Modified: Wed, 21 Dec 2022 02:19:56 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.11` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:7dd73709b94fa0ef33a02bf7a0218d323d3ed9d16638aa6ace75784c30c8357c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111417879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b813fe567331d7d68c23ca54201ff7de9b2a7c0faf40a4e409cb6ed3ee0a45f0`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:37:34 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:37:35 GMT
ENV EMQX_VERSION=4.4.11
# Wed, 21 Dec 2022 02:37:35 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 21 Dec 2022 02:37:38 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 21 Dec 2022 02:37:42 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 21 Dec 2022 02:37:42 GMT
WORKDIR /opt/emqx
# Wed, 21 Dec 2022 02:37:42 GMT
USER emqx
# Wed, 21 Dec 2022 02:37:42 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 21 Dec 2022 02:37:43 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 21 Dec 2022 02:37:43 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 21 Dec 2022 02:37:43 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 02:37:43 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f54b227d051db3a5adf4052f23f9f04079b36c5ee7325bc0bb89de5a0c01431`  
		Last Modified: Wed, 21 Dec 2022 02:38:23 GMT  
		Size: 2.6 MB (2559277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6294bd6555bd8ecb18f540f500f4c59148623e99e95097727bf3f066d0e5e7`  
		Last Modified: Wed, 21 Dec 2022 02:38:26 GMT  
		Size: 39.4 MB (39403616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28334a224641a108af0414ab663b2c97afdb9b7d3ca87b7e628b50444deef003`  
		Last Modified: Wed, 21 Dec 2022 02:38:26 GMT  
		Size: 39.4 MB (39409106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd76f1db199d5827e580d508673f871505dcd0788aae5af91b3138f18700dc5`  
		Last Modified: Wed, 21 Dec 2022 02:38:22 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5`

```console
$ docker pull emqx@sha256:d8880991cde5cbf558acc2d8a457a4756ad0ec5668599543c29223d6057b7968
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:9933b20f02a8ade4ec30561fe2640009e77aa896c25c4e3e2f7c2421c9c3e503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.1 MB (100064626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2fbe86d097c26a4f2379168faebb025010d12e5326996a05e0ec47e28833a08`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:19:20 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:19:21 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 21 Dec 2022 02:19:21 GMT
ENV EMQX_VERSION=5.0.12
# Wed, 21 Dec 2022 02:19:21 GMT
ENV AMD64_SHA256=c137284b389c472f3c2563bc89c8016f5ce9bdb0acf820014afcbbb26a0e81e7
# Wed, 21 Dec 2022 02:19:21 GMT
ENV ARM64_SHA256=5925bb5462d6f163b829c2f1e6490dc5a46e445b5b15c268482bb7310a95f7c4
# Wed, 21 Dec 2022 02:19:21 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 21 Dec 2022 02:19:27 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 21 Dec 2022 02:19:28 GMT
WORKDIR /opt/emqx
# Wed, 21 Dec 2022 02:19:28 GMT
USER emqx
# Wed, 21 Dec 2022 02:19:28 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 21 Dec 2022 02:19:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 21 Dec 2022 02:19:28 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 21 Dec 2022 02:19:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 02:19:29 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d6b5917519f53c840e4677b597bc306543191257c0df7d4744506bb47a4f48`  
		Last Modified: Wed, 21 Dec 2022 02:20:13 GMT  
		Size: 3.0 MB (2987709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a734e6aa155d70825e937e49fab5c55eb61d32a118b6f8ca5d7a9cbf2cdcd72e`  
		Last Modified: Wed, 21 Dec 2022 02:20:13 GMT  
		Size: 4.1 KB (4107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2e55394b6ad877d2b88cba106ac78e8addef68f3d084d9d9bf62f8b6cc0a05`  
		Last Modified: Wed, 21 Dec 2022 02:20:21 GMT  
		Size: 65.7 MB (65674964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c97e31115a8760995b9b155752db32a52e4115b7fb69851f33a7bd419113586`  
		Last Modified: Wed, 21 Dec 2022 02:20:13 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:573150915935bd0d7b58d3867a6cb73521d9950d34735236f1a40aa85ede120d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91158508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4b387edc565c81c05f7c8e200cd3c392b58fce9af8ba84d39781613f5300c85`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:37:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:37:51 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 21 Dec 2022 02:37:51 GMT
ENV EMQX_VERSION=5.0.12
# Wed, 21 Dec 2022 02:37:51 GMT
ENV AMD64_SHA256=c137284b389c472f3c2563bc89c8016f5ce9bdb0acf820014afcbbb26a0e81e7
# Wed, 21 Dec 2022 02:37:51 GMT
ENV ARM64_SHA256=5925bb5462d6f163b829c2f1e6490dc5a46e445b5b15c268482bb7310a95f7c4
# Wed, 21 Dec 2022 02:37:52 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 21 Dec 2022 02:37:56 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 21 Dec 2022 02:37:56 GMT
WORKDIR /opt/emqx
# Wed, 21 Dec 2022 02:37:56 GMT
USER emqx
# Wed, 21 Dec 2022 02:37:56 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 21 Dec 2022 02:37:56 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 21 Dec 2022 02:37:56 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 21 Dec 2022 02:37:56 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 02:37:57 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00bfb98ad2c7fcd02eb0e70fa6f4c91eeb687fc3062f5a249a46bd6e29124a8`  
		Last Modified: Wed, 21 Dec 2022 02:38:37 GMT  
		Size: 3.0 MB (3002677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32322aa000b6d18c777989890f9d396f187818464d2d0eb2b436bddbffda647f`  
		Last Modified: Wed, 21 Dec 2022 02:38:37 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefda07967ac3dd4c6dd8fc909b47143f4235e0c26633688d5a8177ef5c85799`  
		Last Modified: Wed, 21 Dec 2022 02:38:42 GMT  
		Size: 58.1 MB (58106041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ea0d2ead94d77e756f5c7ec56ee3deea581986e3c8a5f956c12edd5555c648`  
		Last Modified: Wed, 21 Dec 2022 02:38:37 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:d8880991cde5cbf558acc2d8a457a4756ad0ec5668599543c29223d6057b7968
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:9933b20f02a8ade4ec30561fe2640009e77aa896c25c4e3e2f7c2421c9c3e503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.1 MB (100064626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2fbe86d097c26a4f2379168faebb025010d12e5326996a05e0ec47e28833a08`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:19:20 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:19:21 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 21 Dec 2022 02:19:21 GMT
ENV EMQX_VERSION=5.0.12
# Wed, 21 Dec 2022 02:19:21 GMT
ENV AMD64_SHA256=c137284b389c472f3c2563bc89c8016f5ce9bdb0acf820014afcbbb26a0e81e7
# Wed, 21 Dec 2022 02:19:21 GMT
ENV ARM64_SHA256=5925bb5462d6f163b829c2f1e6490dc5a46e445b5b15c268482bb7310a95f7c4
# Wed, 21 Dec 2022 02:19:21 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 21 Dec 2022 02:19:27 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 21 Dec 2022 02:19:28 GMT
WORKDIR /opt/emqx
# Wed, 21 Dec 2022 02:19:28 GMT
USER emqx
# Wed, 21 Dec 2022 02:19:28 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 21 Dec 2022 02:19:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 21 Dec 2022 02:19:28 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 21 Dec 2022 02:19:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 02:19:29 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d6b5917519f53c840e4677b597bc306543191257c0df7d4744506bb47a4f48`  
		Last Modified: Wed, 21 Dec 2022 02:20:13 GMT  
		Size: 3.0 MB (2987709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a734e6aa155d70825e937e49fab5c55eb61d32a118b6f8ca5d7a9cbf2cdcd72e`  
		Last Modified: Wed, 21 Dec 2022 02:20:13 GMT  
		Size: 4.1 KB (4107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2e55394b6ad877d2b88cba106ac78e8addef68f3d084d9d9bf62f8b6cc0a05`  
		Last Modified: Wed, 21 Dec 2022 02:20:21 GMT  
		Size: 65.7 MB (65674964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c97e31115a8760995b9b155752db32a52e4115b7fb69851f33a7bd419113586`  
		Last Modified: Wed, 21 Dec 2022 02:20:13 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:573150915935bd0d7b58d3867a6cb73521d9950d34735236f1a40aa85ede120d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91158508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4b387edc565c81c05f7c8e200cd3c392b58fce9af8ba84d39781613f5300c85`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:37:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:37:51 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 21 Dec 2022 02:37:51 GMT
ENV EMQX_VERSION=5.0.12
# Wed, 21 Dec 2022 02:37:51 GMT
ENV AMD64_SHA256=c137284b389c472f3c2563bc89c8016f5ce9bdb0acf820014afcbbb26a0e81e7
# Wed, 21 Dec 2022 02:37:51 GMT
ENV ARM64_SHA256=5925bb5462d6f163b829c2f1e6490dc5a46e445b5b15c268482bb7310a95f7c4
# Wed, 21 Dec 2022 02:37:52 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 21 Dec 2022 02:37:56 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 21 Dec 2022 02:37:56 GMT
WORKDIR /opt/emqx
# Wed, 21 Dec 2022 02:37:56 GMT
USER emqx
# Wed, 21 Dec 2022 02:37:56 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 21 Dec 2022 02:37:56 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 21 Dec 2022 02:37:56 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 21 Dec 2022 02:37:56 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 02:37:57 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00bfb98ad2c7fcd02eb0e70fa6f4c91eeb687fc3062f5a249a46bd6e29124a8`  
		Last Modified: Wed, 21 Dec 2022 02:38:37 GMT  
		Size: 3.0 MB (3002677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32322aa000b6d18c777989890f9d396f187818464d2d0eb2b436bddbffda647f`  
		Last Modified: Wed, 21 Dec 2022 02:38:37 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefda07967ac3dd4c6dd8fc909b47143f4235e0c26633688d5a8177ef5c85799`  
		Last Modified: Wed, 21 Dec 2022 02:38:42 GMT  
		Size: 58.1 MB (58106041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ea0d2ead94d77e756f5c7ec56ee3deea581986e3c8a5f956c12edd5555c648`  
		Last Modified: Wed, 21 Dec 2022 02:38:37 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.13`

**does not exist** (yet?)

## `emqx:latest`

```console
$ docker pull emqx@sha256:d8880991cde5cbf558acc2d8a457a4756ad0ec5668599543c29223d6057b7968
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:9933b20f02a8ade4ec30561fe2640009e77aa896c25c4e3e2f7c2421c9c3e503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.1 MB (100064626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2fbe86d097c26a4f2379168faebb025010d12e5326996a05e0ec47e28833a08`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:19:20 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:19:21 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 21 Dec 2022 02:19:21 GMT
ENV EMQX_VERSION=5.0.12
# Wed, 21 Dec 2022 02:19:21 GMT
ENV AMD64_SHA256=c137284b389c472f3c2563bc89c8016f5ce9bdb0acf820014afcbbb26a0e81e7
# Wed, 21 Dec 2022 02:19:21 GMT
ENV ARM64_SHA256=5925bb5462d6f163b829c2f1e6490dc5a46e445b5b15c268482bb7310a95f7c4
# Wed, 21 Dec 2022 02:19:21 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 21 Dec 2022 02:19:27 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 21 Dec 2022 02:19:28 GMT
WORKDIR /opt/emqx
# Wed, 21 Dec 2022 02:19:28 GMT
USER emqx
# Wed, 21 Dec 2022 02:19:28 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 21 Dec 2022 02:19:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 21 Dec 2022 02:19:28 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 21 Dec 2022 02:19:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 02:19:29 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d6b5917519f53c840e4677b597bc306543191257c0df7d4744506bb47a4f48`  
		Last Modified: Wed, 21 Dec 2022 02:20:13 GMT  
		Size: 3.0 MB (2987709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a734e6aa155d70825e937e49fab5c55eb61d32a118b6f8ca5d7a9cbf2cdcd72e`  
		Last Modified: Wed, 21 Dec 2022 02:20:13 GMT  
		Size: 4.1 KB (4107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2e55394b6ad877d2b88cba106ac78e8addef68f3d084d9d9bf62f8b6cc0a05`  
		Last Modified: Wed, 21 Dec 2022 02:20:21 GMT  
		Size: 65.7 MB (65674964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c97e31115a8760995b9b155752db32a52e4115b7fb69851f33a7bd419113586`  
		Last Modified: Wed, 21 Dec 2022 02:20:13 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:573150915935bd0d7b58d3867a6cb73521d9950d34735236f1a40aa85ede120d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91158508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4b387edc565c81c05f7c8e200cd3c392b58fce9af8ba84d39781613f5300c85`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:37:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:37:51 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 21 Dec 2022 02:37:51 GMT
ENV EMQX_VERSION=5.0.12
# Wed, 21 Dec 2022 02:37:51 GMT
ENV AMD64_SHA256=c137284b389c472f3c2563bc89c8016f5ce9bdb0acf820014afcbbb26a0e81e7
# Wed, 21 Dec 2022 02:37:51 GMT
ENV ARM64_SHA256=5925bb5462d6f163b829c2f1e6490dc5a46e445b5b15c268482bb7310a95f7c4
# Wed, 21 Dec 2022 02:37:52 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 21 Dec 2022 02:37:56 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 21 Dec 2022 02:37:56 GMT
WORKDIR /opt/emqx
# Wed, 21 Dec 2022 02:37:56 GMT
USER emqx
# Wed, 21 Dec 2022 02:37:56 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 21 Dec 2022 02:37:56 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 21 Dec 2022 02:37:56 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 21 Dec 2022 02:37:56 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 02:37:57 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00bfb98ad2c7fcd02eb0e70fa6f4c91eeb687fc3062f5a249a46bd6e29124a8`  
		Last Modified: Wed, 21 Dec 2022 02:38:37 GMT  
		Size: 3.0 MB (3002677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32322aa000b6d18c777989890f9d396f187818464d2d0eb2b436bddbffda647f`  
		Last Modified: Wed, 21 Dec 2022 02:38:37 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefda07967ac3dd4c6dd8fc909b47143f4235e0c26633688d5a8177ef5c85799`  
		Last Modified: Wed, 21 Dec 2022 02:38:42 GMT  
		Size: 58.1 MB (58106041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ea0d2ead94d77e756f5c7ec56ee3deea581986e3c8a5f956c12edd5555c648`  
		Last Modified: Wed, 21 Dec 2022 02:38:37 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
