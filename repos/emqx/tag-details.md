<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.3`](#emqx43)
-	[`emqx:4.3.22`](#emqx4322)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.11`](#emqx4411)
-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.11`](#emqx5011)
-	[`emqx:latest`](#emqxlatest)

## `emqx:4`

```console
$ docker pull emqx@sha256:2ea151261023a455801417d07d80fc1d0b70eae47fbf6f592cf1f7aeccbdcec7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:8be37672002da71c09afcc272ac307e4017b680f7069ca619a3e5c798e446598
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127238513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d038dd794eb77dd150206b76261930d4bdb8a979f7f800f3423b4ffad95d8eb3`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:14:37 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:19:46 GMT
ENV EMQX_VERSION=4.4.11
# Wed, 30 Nov 2022 01:19:46 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 30 Nov 2022 01:19:51 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 30 Nov 2022 01:19:57 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:19:57 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:19:57 GMT
USER emqx
# Wed, 30 Nov 2022 01:19:57 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:19:57 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 30 Nov 2022 01:19:58 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 30 Nov 2022 01:19:58 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:19:58 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9361f46d474c278613330bf20b7b1264c2eec81c3e1f05e78b21aa201437a7`  
		Last Modified: Tue, 15 Nov 2022 12:15:15 GMT  
		Size: 2.6 MB (2571046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:917f457968ac8d4dd2b98c2362bcd2f2d57806420a2c15db36c5b27fb402ca96`  
		Last Modified: Wed, 30 Nov 2022 01:20:57 GMT  
		Size: 46.6 MB (46617905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f804b6655a180b64b4c49e2e503f1441582fcca8bda19d8ece2cbdde09d3bc27`  
		Last Modified: Wed, 30 Nov 2022 01:20:57 GMT  
		Size: 46.6 MB (46635825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf229b4b0d2cf79a784b6a734f6111f323a96d984922ced75fbae0a1138e225`  
		Last Modified: Wed, 30 Nov 2022 01:20:52 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:db311e07a1dbe868f478f416210c3d80ae36f1698ef35144df93452fdb3e18ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111435225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c9545e78c631045922aeb537864f74d52e56f4ee9aed57257e02471cc1c43c4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:13:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:52:42 GMT
ENV EMQX_VERSION=4.4.11
# Wed, 30 Nov 2022 01:52:42 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 30 Nov 2022 01:52:45 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 30 Nov 2022 01:52:50 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:52:50 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:52:50 GMT
USER emqx
# Wed, 30 Nov 2022 01:52:50 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:52:50 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 30 Nov 2022 01:52:50 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 30 Nov 2022 01:52:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:52:50 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad108ef5d5673e32622aa158fbc152df7e8c340c7f4e79efffecd4c5d6c2a7be`  
		Last Modified: Tue, 15 Nov 2022 06:14:09 GMT  
		Size: 2.6 MB (2560816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78386a1c510620cb84f856900798687f1ea67c708915c4a9a2e60b8f5df15857`  
		Last Modified: Wed, 30 Nov 2022 01:53:43 GMT  
		Size: 39.4 MB (39403596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a6da069cff1af881684d95753d55911ca54eeea95ffa2cee0f9d2a3b3ec7ae`  
		Last Modified: Wed, 30 Nov 2022 01:53:43 GMT  
		Size: 39.4 MB (39409100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28aad18ab154243a8cbc713b374f429ba44b49ef016ca56878375a604e29b74`  
		Last Modified: Wed, 30 Nov 2022 01:53:40 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3`

```console
$ docker pull emqx@sha256:641ea48162d6d581fef4135780cf7c4c97d9621f58e3dcbac85901bde473dae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3` - linux; amd64

```console
$ docker pull emqx@sha256:7d039128a163912d6f42a83834cd8d2b1488c765be83fdb2828d219e8ed10c05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.8 MB (104828352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8db4537e49f74f633a3bdabea8e83f735658f5e3bf29f46ecd003de81f2c6ae`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:14 GMT
ADD file:9461639b945ced6fb6164491a7e0131261a1b7d69264cce516e75c71e4df22d2 in / 
# Tue, 15 Nov 2022 04:05:14 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:14:14 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:19:32 GMT
ENV EMQX_VERSION=4.3.22
# Wed, 30 Nov 2022 01:19:37 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 30 Nov 2022 01:19:42 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:19:43 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:19:43 GMT
USER emqx
# Wed, 30 Nov 2022 01:19:43 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:19:43 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 30 Nov 2022 01:19:43 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Wed, 30 Nov 2022 01:19:43 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:19:43 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:32820e52a00eb22dc76d70d992be7082cd24b636cfb597ff3951d29a821b46b9`  
		Last Modified: Tue, 15 Nov 2022 04:09:26 GMT  
		Size: 27.1 MB (27140332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a034d47f6faf5df0c00edec91ebcd75cc95132acb38b2ee8646b151d04075a52`  
		Last Modified: Tue, 15 Nov 2022 12:15:02 GMT  
		Size: 4.6 MB (4612387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a174a85c34809b141834814841742dce5e829f8ab51321f2d4af41cff6f1d77e`  
		Last Modified: Wed, 30 Nov 2022 01:20:44 GMT  
		Size: 36.5 MB (36537213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab32b8bb90d6c5c8639d88e17285f5d0c9a728b3a88ac50f3bcce1ba3bf9c50`  
		Last Modified: Wed, 30 Nov 2022 01:20:44 GMT  
		Size: 36.5 MB (36537379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4b109a43f1ce49e353eea72f00eb14993a28d2f09f4a0b98e257d981e65483`  
		Last Modified: Wed, 30 Nov 2022 01:20:40 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:cc61dcf2073c3c0e7c48c3426df5b07fe18c21a19b0fe5f6cbdbc0c643d75fd1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102846275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e2fc6c8ffa36a6976b6c936af65033e160f87365205ace2e212305da0c50d3`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:34 GMT
ADD file:aaead8e4dd08d41c8d1692bbe76b673119289836428e1f713ca550c2468711ac in / 
# Tue, 15 Nov 2022 01:41:34 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:13:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:52:30 GMT
ENV EMQX_VERSION=4.3.22
# Wed, 30 Nov 2022 01:52:34 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 30 Nov 2022 01:52:38 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:52:39 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:52:39 GMT
USER emqx
# Wed, 30 Nov 2022 01:52:39 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:52:39 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 30 Nov 2022 01:52:39 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Wed, 30 Nov 2022 01:52:39 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:52:39 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:cc457132e077d684a6cecad3331c35341d814c5d364f3cf24d698a6d8e76d0e7`  
		Last Modified: Tue, 15 Nov 2022 01:45:13 GMT  
		Size: 25.9 MB (25914924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d027abecdd5af35e9a16c44518f0617af3a9b80b03d0fac7e90d16f1de3c6100`  
		Last Modified: Tue, 15 Nov 2022 06:13:52 GMT  
		Size: 4.5 MB (4490492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd156f83df550b9c60e06e429f96308123f16fa687c477cde4fb6cd8a7a6ef99`  
		Last Modified: Wed, 30 Nov 2022 01:53:29 GMT  
		Size: 36.2 MB (36216026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abc81371049c42b020f56e5e771f9ad18237fe536d1bd104145b732303cf727`  
		Last Modified: Wed, 30 Nov 2022 01:53:29 GMT  
		Size: 36.2 MB (36223793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5b18e968368274267af0a7369ddcaf359cb15cfd80aade6e5238b4de183f74`  
		Last Modified: Wed, 30 Nov 2022 01:53:26 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3.22`

```console
$ docker pull emqx@sha256:641ea48162d6d581fef4135780cf7c4c97d9621f58e3dcbac85901bde473dae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3.22` - linux; amd64

```console
$ docker pull emqx@sha256:7d039128a163912d6f42a83834cd8d2b1488c765be83fdb2828d219e8ed10c05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.8 MB (104828352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8db4537e49f74f633a3bdabea8e83f735658f5e3bf29f46ecd003de81f2c6ae`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:14 GMT
ADD file:9461639b945ced6fb6164491a7e0131261a1b7d69264cce516e75c71e4df22d2 in / 
# Tue, 15 Nov 2022 04:05:14 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:14:14 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:19:32 GMT
ENV EMQX_VERSION=4.3.22
# Wed, 30 Nov 2022 01:19:37 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 30 Nov 2022 01:19:42 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:19:43 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:19:43 GMT
USER emqx
# Wed, 30 Nov 2022 01:19:43 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:19:43 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 30 Nov 2022 01:19:43 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Wed, 30 Nov 2022 01:19:43 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:19:43 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:32820e52a00eb22dc76d70d992be7082cd24b636cfb597ff3951d29a821b46b9`  
		Last Modified: Tue, 15 Nov 2022 04:09:26 GMT  
		Size: 27.1 MB (27140332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a034d47f6faf5df0c00edec91ebcd75cc95132acb38b2ee8646b151d04075a52`  
		Last Modified: Tue, 15 Nov 2022 12:15:02 GMT  
		Size: 4.6 MB (4612387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a174a85c34809b141834814841742dce5e829f8ab51321f2d4af41cff6f1d77e`  
		Last Modified: Wed, 30 Nov 2022 01:20:44 GMT  
		Size: 36.5 MB (36537213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab32b8bb90d6c5c8639d88e17285f5d0c9a728b3a88ac50f3bcce1ba3bf9c50`  
		Last Modified: Wed, 30 Nov 2022 01:20:44 GMT  
		Size: 36.5 MB (36537379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4b109a43f1ce49e353eea72f00eb14993a28d2f09f4a0b98e257d981e65483`  
		Last Modified: Wed, 30 Nov 2022 01:20:40 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3.22` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:cc61dcf2073c3c0e7c48c3426df5b07fe18c21a19b0fe5f6cbdbc0c643d75fd1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102846275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e2fc6c8ffa36a6976b6c936af65033e160f87365205ace2e212305da0c50d3`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:34 GMT
ADD file:aaead8e4dd08d41c8d1692bbe76b673119289836428e1f713ca550c2468711ac in / 
# Tue, 15 Nov 2022 01:41:34 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:13:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:52:30 GMT
ENV EMQX_VERSION=4.3.22
# Wed, 30 Nov 2022 01:52:34 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 30 Nov 2022 01:52:38 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:52:39 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:52:39 GMT
USER emqx
# Wed, 30 Nov 2022 01:52:39 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:52:39 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 30 Nov 2022 01:52:39 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Wed, 30 Nov 2022 01:52:39 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:52:39 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:cc457132e077d684a6cecad3331c35341d814c5d364f3cf24d698a6d8e76d0e7`  
		Last Modified: Tue, 15 Nov 2022 01:45:13 GMT  
		Size: 25.9 MB (25914924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d027abecdd5af35e9a16c44518f0617af3a9b80b03d0fac7e90d16f1de3c6100`  
		Last Modified: Tue, 15 Nov 2022 06:13:52 GMT  
		Size: 4.5 MB (4490492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd156f83df550b9c60e06e429f96308123f16fa687c477cde4fb6cd8a7a6ef99`  
		Last Modified: Wed, 30 Nov 2022 01:53:29 GMT  
		Size: 36.2 MB (36216026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abc81371049c42b020f56e5e771f9ad18237fe536d1bd104145b732303cf727`  
		Last Modified: Wed, 30 Nov 2022 01:53:29 GMT  
		Size: 36.2 MB (36223793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5b18e968368274267af0a7369ddcaf359cb15cfd80aade6e5238b4de183f74`  
		Last Modified: Wed, 30 Nov 2022 01:53:26 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:2ea151261023a455801417d07d80fc1d0b70eae47fbf6f592cf1f7aeccbdcec7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:8be37672002da71c09afcc272ac307e4017b680f7069ca619a3e5c798e446598
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127238513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d038dd794eb77dd150206b76261930d4bdb8a979f7f800f3423b4ffad95d8eb3`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:14:37 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:19:46 GMT
ENV EMQX_VERSION=4.4.11
# Wed, 30 Nov 2022 01:19:46 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 30 Nov 2022 01:19:51 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 30 Nov 2022 01:19:57 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:19:57 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:19:57 GMT
USER emqx
# Wed, 30 Nov 2022 01:19:57 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:19:57 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 30 Nov 2022 01:19:58 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 30 Nov 2022 01:19:58 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:19:58 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9361f46d474c278613330bf20b7b1264c2eec81c3e1f05e78b21aa201437a7`  
		Last Modified: Tue, 15 Nov 2022 12:15:15 GMT  
		Size: 2.6 MB (2571046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:917f457968ac8d4dd2b98c2362bcd2f2d57806420a2c15db36c5b27fb402ca96`  
		Last Modified: Wed, 30 Nov 2022 01:20:57 GMT  
		Size: 46.6 MB (46617905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f804b6655a180b64b4c49e2e503f1441582fcca8bda19d8ece2cbdde09d3bc27`  
		Last Modified: Wed, 30 Nov 2022 01:20:57 GMT  
		Size: 46.6 MB (46635825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf229b4b0d2cf79a784b6a734f6111f323a96d984922ced75fbae0a1138e225`  
		Last Modified: Wed, 30 Nov 2022 01:20:52 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:db311e07a1dbe868f478f416210c3d80ae36f1698ef35144df93452fdb3e18ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111435225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c9545e78c631045922aeb537864f74d52e56f4ee9aed57257e02471cc1c43c4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:13:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:52:42 GMT
ENV EMQX_VERSION=4.4.11
# Wed, 30 Nov 2022 01:52:42 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 30 Nov 2022 01:52:45 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 30 Nov 2022 01:52:50 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:52:50 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:52:50 GMT
USER emqx
# Wed, 30 Nov 2022 01:52:50 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:52:50 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 30 Nov 2022 01:52:50 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 30 Nov 2022 01:52:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:52:50 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad108ef5d5673e32622aa158fbc152df7e8c340c7f4e79efffecd4c5d6c2a7be`  
		Last Modified: Tue, 15 Nov 2022 06:14:09 GMT  
		Size: 2.6 MB (2560816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78386a1c510620cb84f856900798687f1ea67c708915c4a9a2e60b8f5df15857`  
		Last Modified: Wed, 30 Nov 2022 01:53:43 GMT  
		Size: 39.4 MB (39403596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a6da069cff1af881684d95753d55911ca54eeea95ffa2cee0f9d2a3b3ec7ae`  
		Last Modified: Wed, 30 Nov 2022 01:53:43 GMT  
		Size: 39.4 MB (39409100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28aad18ab154243a8cbc713b374f429ba44b49ef016ca56878375a604e29b74`  
		Last Modified: Wed, 30 Nov 2022 01:53:40 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.11`

```console
$ docker pull emqx@sha256:2ea151261023a455801417d07d80fc1d0b70eae47fbf6f592cf1f7aeccbdcec7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.11` - linux; amd64

```console
$ docker pull emqx@sha256:8be37672002da71c09afcc272ac307e4017b680f7069ca619a3e5c798e446598
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127238513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d038dd794eb77dd150206b76261930d4bdb8a979f7f800f3423b4ffad95d8eb3`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:14:37 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:19:46 GMT
ENV EMQX_VERSION=4.4.11
# Wed, 30 Nov 2022 01:19:46 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 30 Nov 2022 01:19:51 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 30 Nov 2022 01:19:57 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:19:57 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:19:57 GMT
USER emqx
# Wed, 30 Nov 2022 01:19:57 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:19:57 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 30 Nov 2022 01:19:58 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 30 Nov 2022 01:19:58 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:19:58 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9361f46d474c278613330bf20b7b1264c2eec81c3e1f05e78b21aa201437a7`  
		Last Modified: Tue, 15 Nov 2022 12:15:15 GMT  
		Size: 2.6 MB (2571046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:917f457968ac8d4dd2b98c2362bcd2f2d57806420a2c15db36c5b27fb402ca96`  
		Last Modified: Wed, 30 Nov 2022 01:20:57 GMT  
		Size: 46.6 MB (46617905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f804b6655a180b64b4c49e2e503f1441582fcca8bda19d8ece2cbdde09d3bc27`  
		Last Modified: Wed, 30 Nov 2022 01:20:57 GMT  
		Size: 46.6 MB (46635825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf229b4b0d2cf79a784b6a734f6111f323a96d984922ced75fbae0a1138e225`  
		Last Modified: Wed, 30 Nov 2022 01:20:52 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.11` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:db311e07a1dbe868f478f416210c3d80ae36f1698ef35144df93452fdb3e18ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111435225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c9545e78c631045922aeb537864f74d52e56f4ee9aed57257e02471cc1c43c4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:13:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:52:42 GMT
ENV EMQX_VERSION=4.4.11
# Wed, 30 Nov 2022 01:52:42 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 30 Nov 2022 01:52:45 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="652fb25a2a5c9d4e9fc029a4094d39c5bd824c78ad77361fb5fee09a940209a6"; fi;     if [ ${arch} = "arm64" ]; then sha256="6532a0f93fe8ce419633142b376107f3d7a2a79df24ce95551026b9e144a77b8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 30 Nov 2022 01:52:50 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:52:50 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:52:50 GMT
USER emqx
# Wed, 30 Nov 2022 01:52:50 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:52:50 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 30 Nov 2022 01:52:50 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 30 Nov 2022 01:52:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:52:50 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad108ef5d5673e32622aa158fbc152df7e8c340c7f4e79efffecd4c5d6c2a7be`  
		Last Modified: Tue, 15 Nov 2022 06:14:09 GMT  
		Size: 2.6 MB (2560816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78386a1c510620cb84f856900798687f1ea67c708915c4a9a2e60b8f5df15857`  
		Last Modified: Wed, 30 Nov 2022 01:53:43 GMT  
		Size: 39.4 MB (39403596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a6da069cff1af881684d95753d55911ca54eeea95ffa2cee0f9d2a3b3ec7ae`  
		Last Modified: Wed, 30 Nov 2022 01:53:43 GMT  
		Size: 39.4 MB (39409100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28aad18ab154243a8cbc713b374f429ba44b49ef016ca56878375a604e29b74`  
		Last Modified: Wed, 30 Nov 2022 01:53:40 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5`

```console
$ docker pull emqx@sha256:26198574fa106dcd1642e32cec98c84d2dc14875df000ebb8bf83befbb304f32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:b47ae65c73f7ed27c52fd09fafed3fe5dbe9a2d787f4f4d69a0e0cdfd394fd0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.2 MB (164249511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23be81c1865939e9c6ee7e29985a73c7ff5e44409e39bc6763a81af7e1e61006`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Wed, 30 Nov 2022 01:20:07 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:20:07 GMT
ENV EMQX_VERSION=5.0.11
# Wed, 30 Nov 2022 01:20:08 GMT
ENV AMD64_SHA256=68609fcc1d74be917f9c28c57c14daabccee22361af91b6e98812a35300a1c80
# Wed, 30 Nov 2022 01:20:08 GMT
ENV ARM64_SHA256=f7c7417951beb490ed3a7347b3879db8e9e80ea214c9ef942e777c7136681d31
# Wed, 30 Nov 2022 01:20:08 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 30 Nov 2022 01:20:14 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 30 Nov 2022 01:20:15 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 30 Nov 2022 01:20:15 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:20:21 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:20:22 GMT
USER emqx
# Wed, 30 Nov 2022 01:20:22 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:20:22 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 30 Nov 2022 01:20:22 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:20:22 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253a3a37dc22afc619ff390ed7558f8f578fd9d8ef057da70abd02564ba3294a`  
		Last Modified: Wed, 30 Nov 2022 01:21:09 GMT  
		Size: 3.0 MB (2988983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e9fd38a69851f358ff810c2ecda7d0f8a987fe04c00addd4df8eb223aadc78`  
		Last Modified: Wed, 30 Nov 2022 01:21:16 GMT  
		Size: 64.9 MB (64920980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5afacf135bcc58ec9fa6a66f2d3cdd10bf3c3872be5736c92ba283cf0cccb9`  
		Last Modified: Wed, 30 Nov 2022 01:21:08 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5be75c6f2b43f65b17a0aea0eb8dd8cb56229af18065076017f57ad4cc0402`  
		Last Modified: Wed, 30 Nov 2022 01:21:16 GMT  
		Size: 64.9 MB (64926017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:36847cbc801d37eafe836c7486f7069e618b168054494a17e6b9108a02c80d06
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.8 MB (147767210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88d2c84148e688bdd6a324207d0535c831a0a169d9ac580388ab9659e4f6df89`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Wed, 30 Nov 2022 01:52:58 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:52:58 GMT
ENV EMQX_VERSION=5.0.11
# Wed, 30 Nov 2022 01:52:58 GMT
ENV AMD64_SHA256=68609fcc1d74be917f9c28c57c14daabccee22361af91b6e98812a35300a1c80
# Wed, 30 Nov 2022 01:52:58 GMT
ENV ARM64_SHA256=f7c7417951beb490ed3a7347b3879db8e9e80ea214c9ef942e777c7136681d31
# Wed, 30 Nov 2022 01:52:58 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 30 Nov 2022 01:53:02 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 30 Nov 2022 01:53:03 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 30 Nov 2022 01:53:03 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:53:08 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:53:08 GMT
USER emqx
# Wed, 30 Nov 2022 01:53:08 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:53:08 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 30 Nov 2022 01:53:08 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:53:08 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779afb6670c886761cbd92232fabbfb5460051f084cda020112fd649fd64c9e9`  
		Last Modified: Wed, 30 Nov 2022 01:53:54 GMT  
		Size: 3.0 MB (3004113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950c27ff169ec58514bc5b2f6c9432b3c603c0f3c9d900e0f87cf167e7e8216e`  
		Last Modified: Wed, 30 Nov 2022 01:53:59 GMT  
		Size: 57.3 MB (57348503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554dd3630b90df5cd7b76d935f8ca60310032deeb91f91555ace233382d57c09`  
		Last Modified: Wed, 30 Nov 2022 01:53:53 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d390a44da3d80a16d371b5d4fa0e9de4b35bc149a4fcb8c8c13309aa6c6cee`  
		Last Modified: Wed, 30 Nov 2022 01:53:59 GMT  
		Size: 57.4 MB (57353085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:26198574fa106dcd1642e32cec98c84d2dc14875df000ebb8bf83befbb304f32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:b47ae65c73f7ed27c52fd09fafed3fe5dbe9a2d787f4f4d69a0e0cdfd394fd0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.2 MB (164249511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23be81c1865939e9c6ee7e29985a73c7ff5e44409e39bc6763a81af7e1e61006`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Wed, 30 Nov 2022 01:20:07 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:20:07 GMT
ENV EMQX_VERSION=5.0.11
# Wed, 30 Nov 2022 01:20:08 GMT
ENV AMD64_SHA256=68609fcc1d74be917f9c28c57c14daabccee22361af91b6e98812a35300a1c80
# Wed, 30 Nov 2022 01:20:08 GMT
ENV ARM64_SHA256=f7c7417951beb490ed3a7347b3879db8e9e80ea214c9ef942e777c7136681d31
# Wed, 30 Nov 2022 01:20:08 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 30 Nov 2022 01:20:14 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 30 Nov 2022 01:20:15 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 30 Nov 2022 01:20:15 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:20:21 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:20:22 GMT
USER emqx
# Wed, 30 Nov 2022 01:20:22 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:20:22 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 30 Nov 2022 01:20:22 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:20:22 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253a3a37dc22afc619ff390ed7558f8f578fd9d8ef057da70abd02564ba3294a`  
		Last Modified: Wed, 30 Nov 2022 01:21:09 GMT  
		Size: 3.0 MB (2988983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e9fd38a69851f358ff810c2ecda7d0f8a987fe04c00addd4df8eb223aadc78`  
		Last Modified: Wed, 30 Nov 2022 01:21:16 GMT  
		Size: 64.9 MB (64920980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5afacf135bcc58ec9fa6a66f2d3cdd10bf3c3872be5736c92ba283cf0cccb9`  
		Last Modified: Wed, 30 Nov 2022 01:21:08 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5be75c6f2b43f65b17a0aea0eb8dd8cb56229af18065076017f57ad4cc0402`  
		Last Modified: Wed, 30 Nov 2022 01:21:16 GMT  
		Size: 64.9 MB (64926017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:36847cbc801d37eafe836c7486f7069e618b168054494a17e6b9108a02c80d06
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.8 MB (147767210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88d2c84148e688bdd6a324207d0535c831a0a169d9ac580388ab9659e4f6df89`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Wed, 30 Nov 2022 01:52:58 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:52:58 GMT
ENV EMQX_VERSION=5.0.11
# Wed, 30 Nov 2022 01:52:58 GMT
ENV AMD64_SHA256=68609fcc1d74be917f9c28c57c14daabccee22361af91b6e98812a35300a1c80
# Wed, 30 Nov 2022 01:52:58 GMT
ENV ARM64_SHA256=f7c7417951beb490ed3a7347b3879db8e9e80ea214c9ef942e777c7136681d31
# Wed, 30 Nov 2022 01:52:58 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 30 Nov 2022 01:53:02 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 30 Nov 2022 01:53:03 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 30 Nov 2022 01:53:03 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:53:08 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:53:08 GMT
USER emqx
# Wed, 30 Nov 2022 01:53:08 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:53:08 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 30 Nov 2022 01:53:08 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:53:08 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779afb6670c886761cbd92232fabbfb5460051f084cda020112fd649fd64c9e9`  
		Last Modified: Wed, 30 Nov 2022 01:53:54 GMT  
		Size: 3.0 MB (3004113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950c27ff169ec58514bc5b2f6c9432b3c603c0f3c9d900e0f87cf167e7e8216e`  
		Last Modified: Wed, 30 Nov 2022 01:53:59 GMT  
		Size: 57.3 MB (57348503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554dd3630b90df5cd7b76d935f8ca60310032deeb91f91555ace233382d57c09`  
		Last Modified: Wed, 30 Nov 2022 01:53:53 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d390a44da3d80a16d371b5d4fa0e9de4b35bc149a4fcb8c8c13309aa6c6cee`  
		Last Modified: Wed, 30 Nov 2022 01:53:59 GMT  
		Size: 57.4 MB (57353085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.11`

```console
$ docker pull emqx@sha256:26198574fa106dcd1642e32cec98c84d2dc14875df000ebb8bf83befbb304f32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0.11` - linux; amd64

```console
$ docker pull emqx@sha256:b47ae65c73f7ed27c52fd09fafed3fe5dbe9a2d787f4f4d69a0e0cdfd394fd0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.2 MB (164249511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23be81c1865939e9c6ee7e29985a73c7ff5e44409e39bc6763a81af7e1e61006`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Wed, 30 Nov 2022 01:20:07 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:20:07 GMT
ENV EMQX_VERSION=5.0.11
# Wed, 30 Nov 2022 01:20:08 GMT
ENV AMD64_SHA256=68609fcc1d74be917f9c28c57c14daabccee22361af91b6e98812a35300a1c80
# Wed, 30 Nov 2022 01:20:08 GMT
ENV ARM64_SHA256=f7c7417951beb490ed3a7347b3879db8e9e80ea214c9ef942e777c7136681d31
# Wed, 30 Nov 2022 01:20:08 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 30 Nov 2022 01:20:14 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 30 Nov 2022 01:20:15 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 30 Nov 2022 01:20:15 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:20:21 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:20:22 GMT
USER emqx
# Wed, 30 Nov 2022 01:20:22 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:20:22 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 30 Nov 2022 01:20:22 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:20:22 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253a3a37dc22afc619ff390ed7558f8f578fd9d8ef057da70abd02564ba3294a`  
		Last Modified: Wed, 30 Nov 2022 01:21:09 GMT  
		Size: 3.0 MB (2988983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e9fd38a69851f358ff810c2ecda7d0f8a987fe04c00addd4df8eb223aadc78`  
		Last Modified: Wed, 30 Nov 2022 01:21:16 GMT  
		Size: 64.9 MB (64920980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5afacf135bcc58ec9fa6a66f2d3cdd10bf3c3872be5736c92ba283cf0cccb9`  
		Last Modified: Wed, 30 Nov 2022 01:21:08 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5be75c6f2b43f65b17a0aea0eb8dd8cb56229af18065076017f57ad4cc0402`  
		Last Modified: Wed, 30 Nov 2022 01:21:16 GMT  
		Size: 64.9 MB (64926017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0.11` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:36847cbc801d37eafe836c7486f7069e618b168054494a17e6b9108a02c80d06
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.8 MB (147767210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88d2c84148e688bdd6a324207d0535c831a0a169d9ac580388ab9659e4f6df89`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Wed, 30 Nov 2022 01:52:58 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:52:58 GMT
ENV EMQX_VERSION=5.0.11
# Wed, 30 Nov 2022 01:52:58 GMT
ENV AMD64_SHA256=68609fcc1d74be917f9c28c57c14daabccee22361af91b6e98812a35300a1c80
# Wed, 30 Nov 2022 01:52:58 GMT
ENV ARM64_SHA256=f7c7417951beb490ed3a7347b3879db8e9e80ea214c9ef942e777c7136681d31
# Wed, 30 Nov 2022 01:52:58 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 30 Nov 2022 01:53:02 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 30 Nov 2022 01:53:03 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 30 Nov 2022 01:53:03 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:53:08 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:53:08 GMT
USER emqx
# Wed, 30 Nov 2022 01:53:08 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:53:08 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 30 Nov 2022 01:53:08 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:53:08 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779afb6670c886761cbd92232fabbfb5460051f084cda020112fd649fd64c9e9`  
		Last Modified: Wed, 30 Nov 2022 01:53:54 GMT  
		Size: 3.0 MB (3004113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950c27ff169ec58514bc5b2f6c9432b3c603c0f3c9d900e0f87cf167e7e8216e`  
		Last Modified: Wed, 30 Nov 2022 01:53:59 GMT  
		Size: 57.3 MB (57348503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554dd3630b90df5cd7b76d935f8ca60310032deeb91f91555ace233382d57c09`  
		Last Modified: Wed, 30 Nov 2022 01:53:53 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d390a44da3d80a16d371b5d4fa0e9de4b35bc149a4fcb8c8c13309aa6c6cee`  
		Last Modified: Wed, 30 Nov 2022 01:53:59 GMT  
		Size: 57.4 MB (57353085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:26198574fa106dcd1642e32cec98c84d2dc14875df000ebb8bf83befbb304f32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:b47ae65c73f7ed27c52fd09fafed3fe5dbe9a2d787f4f4d69a0e0cdfd394fd0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.2 MB (164249511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23be81c1865939e9c6ee7e29985a73c7ff5e44409e39bc6763a81af7e1e61006`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Wed, 30 Nov 2022 01:20:07 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:20:07 GMT
ENV EMQX_VERSION=5.0.11
# Wed, 30 Nov 2022 01:20:08 GMT
ENV AMD64_SHA256=68609fcc1d74be917f9c28c57c14daabccee22361af91b6e98812a35300a1c80
# Wed, 30 Nov 2022 01:20:08 GMT
ENV ARM64_SHA256=f7c7417951beb490ed3a7347b3879db8e9e80ea214c9ef942e777c7136681d31
# Wed, 30 Nov 2022 01:20:08 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 30 Nov 2022 01:20:14 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 30 Nov 2022 01:20:15 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 30 Nov 2022 01:20:15 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:20:21 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:20:22 GMT
USER emqx
# Wed, 30 Nov 2022 01:20:22 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:20:22 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 30 Nov 2022 01:20:22 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:20:22 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253a3a37dc22afc619ff390ed7558f8f578fd9d8ef057da70abd02564ba3294a`  
		Last Modified: Wed, 30 Nov 2022 01:21:09 GMT  
		Size: 3.0 MB (2988983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e9fd38a69851f358ff810c2ecda7d0f8a987fe04c00addd4df8eb223aadc78`  
		Last Modified: Wed, 30 Nov 2022 01:21:16 GMT  
		Size: 64.9 MB (64920980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5afacf135bcc58ec9fa6a66f2d3cdd10bf3c3872be5736c92ba283cf0cccb9`  
		Last Modified: Wed, 30 Nov 2022 01:21:08 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5be75c6f2b43f65b17a0aea0eb8dd8cb56229af18065076017f57ad4cc0402`  
		Last Modified: Wed, 30 Nov 2022 01:21:16 GMT  
		Size: 64.9 MB (64926017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:36847cbc801d37eafe836c7486f7069e618b168054494a17e6b9108a02c80d06
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.8 MB (147767210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88d2c84148e688bdd6a324207d0535c831a0a169d9ac580388ab9659e4f6df89`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Wed, 30 Nov 2022 01:52:58 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Nov 2022 01:52:58 GMT
ENV EMQX_VERSION=5.0.11
# Wed, 30 Nov 2022 01:52:58 GMT
ENV AMD64_SHA256=68609fcc1d74be917f9c28c57c14daabccee22361af91b6e98812a35300a1c80
# Wed, 30 Nov 2022 01:52:58 GMT
ENV ARM64_SHA256=f7c7417951beb490ed3a7347b3879db8e9e80ea214c9ef942e777c7136681d31
# Wed, 30 Nov 2022 01:52:58 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 30 Nov 2022 01:53:02 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 30 Nov 2022 01:53:03 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 30 Nov 2022 01:53:03 GMT
WORKDIR /opt/emqx
# Wed, 30 Nov 2022 01:53:08 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Wed, 30 Nov 2022 01:53:08 GMT
USER emqx
# Wed, 30 Nov 2022 01:53:08 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 30 Nov 2022 01:53:08 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 30 Nov 2022 01:53:08 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 30 Nov 2022 01:53:08 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779afb6670c886761cbd92232fabbfb5460051f084cda020112fd649fd64c9e9`  
		Last Modified: Wed, 30 Nov 2022 01:53:54 GMT  
		Size: 3.0 MB (3004113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950c27ff169ec58514bc5b2f6c9432b3c603c0f3c9d900e0f87cf167e7e8216e`  
		Last Modified: Wed, 30 Nov 2022 01:53:59 GMT  
		Size: 57.3 MB (57348503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554dd3630b90df5cd7b76d935f8ca60310032deeb91f91555ace233382d57c09`  
		Last Modified: Wed, 30 Nov 2022 01:53:53 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d390a44da3d80a16d371b5d4fa0e9de4b35bc149a4fcb8c8c13309aa6c6cee`  
		Last Modified: Wed, 30 Nov 2022 01:53:59 GMT  
		Size: 57.4 MB (57353085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
