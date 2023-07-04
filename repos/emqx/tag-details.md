<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.18`](#emqx4418)
-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.26`](#emqx5026)
-	[`emqx:5.1`](#emqx51)
-	[`emqx:5.1.0`](#emqx510)
-	[`emqx:latest`](#emqxlatest)

## `emqx:4`

```console
$ docker pull emqx@sha256:ec2c136fb5831a5619b45e3ef70ed8727c7e8d65227339b31596525851b73934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:59814c0cd7e916de55642b6534fd578b0a6e57eb699663d010dc069dcda222b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81290390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:369b89a4a859e567c7417697198a5de2189165cab88dfdaca3ad6276ea00b827`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:20:58 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:20:58 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 04 Jul 2023 04:20:58 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 04 Jul 2023 04:20:58 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 04 Jul 2023 04:21:03 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 04 Jul 2023 04:21:03 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 04:21:03 GMT
USER emqx
# Tue, 04 Jul 2023 04:21:04 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 04:21:04 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 04 Jul 2023 04:21:04 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 04 Jul 2023 04:21:04 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 04:21:04 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ef462373a136b96c0a554f87fe5b08b7c8461aba1e112745b996eaa7b98a7d`  
		Last Modified: Tue, 04 Jul 2023 04:21:43 GMT  
		Size: 2.6 MB (2569640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ad23a7d23aef4b144a14d30ac52f4568fb6adbc5c43bebc8041add65f9d8bd`  
		Last Modified: Tue, 04 Jul 2023 04:21:42 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7aaf596f0066ac6b1036ee6901f889790109e0307a7769061cc46db57b37e0e`  
		Last Modified: Tue, 04 Jul 2023 04:21:47 GMT  
		Size: 47.3 MB (47298154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe0eabbe33e4b55892b3f2a3a28715c0da29545d619854b113633ec7d92e25e`  
		Last Modified: Tue, 04 Jul 2023 04:21:43 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:2d08ee2bc416b6f69851a687377881c076764d6010794177a34c576f405d0eea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72707473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99ef632180b6d12a52f16c392ec17886bc0626d84ec46d8a7d1f71cea9b85a0d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:08 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:08 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 04 Jul 2023 03:03:08 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 04 Jul 2023 03:03:09 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 04 Jul 2023 03:03:12 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 04 Jul 2023 03:03:13 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 03:03:13 GMT
USER emqx
# Tue, 04 Jul 2023 03:03:13 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 03:03:13 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 04 Jul 2023 03:03:13 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 04 Jul 2023 03:03:13 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:03:13 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a1428b80937a0eb55c8466779cec4bcf7e31bdcc4fc66b763448cf9d131563`  
		Last Modified: Tue, 04 Jul 2023 03:03:50 GMT  
		Size: 2.6 MB (2559426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa00861c721843ae490a68a90f1db04218b5131cb6b2d6d39618973618f3da3`  
		Last Modified: Tue, 04 Jul 2023 03:03:49 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3e06c4413e69400a792d7a95cad6d643afdbcdc2f28fdd90e603e2f22e33a7`  
		Last Modified: Tue, 04 Jul 2023 03:03:53 GMT  
		Size: 40.1 MB (40079874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ab794d03683cd2393608f40731e4c588dbc7661668e884227ec782c7011921`  
		Last Modified: Tue, 04 Jul 2023 03:03:49 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:ec2c136fb5831a5619b45e3ef70ed8727c7e8d65227339b31596525851b73934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:59814c0cd7e916de55642b6534fd578b0a6e57eb699663d010dc069dcda222b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81290390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:369b89a4a859e567c7417697198a5de2189165cab88dfdaca3ad6276ea00b827`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:20:58 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:20:58 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 04 Jul 2023 04:20:58 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 04 Jul 2023 04:20:58 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 04 Jul 2023 04:21:03 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 04 Jul 2023 04:21:03 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 04:21:03 GMT
USER emqx
# Tue, 04 Jul 2023 04:21:04 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 04:21:04 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 04 Jul 2023 04:21:04 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 04 Jul 2023 04:21:04 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 04:21:04 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ef462373a136b96c0a554f87fe5b08b7c8461aba1e112745b996eaa7b98a7d`  
		Last Modified: Tue, 04 Jul 2023 04:21:43 GMT  
		Size: 2.6 MB (2569640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ad23a7d23aef4b144a14d30ac52f4568fb6adbc5c43bebc8041add65f9d8bd`  
		Last Modified: Tue, 04 Jul 2023 04:21:42 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7aaf596f0066ac6b1036ee6901f889790109e0307a7769061cc46db57b37e0e`  
		Last Modified: Tue, 04 Jul 2023 04:21:47 GMT  
		Size: 47.3 MB (47298154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe0eabbe33e4b55892b3f2a3a28715c0da29545d619854b113633ec7d92e25e`  
		Last Modified: Tue, 04 Jul 2023 04:21:43 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:2d08ee2bc416b6f69851a687377881c076764d6010794177a34c576f405d0eea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72707473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99ef632180b6d12a52f16c392ec17886bc0626d84ec46d8a7d1f71cea9b85a0d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:08 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:08 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 04 Jul 2023 03:03:08 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 04 Jul 2023 03:03:09 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 04 Jul 2023 03:03:12 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 04 Jul 2023 03:03:13 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 03:03:13 GMT
USER emqx
# Tue, 04 Jul 2023 03:03:13 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 03:03:13 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 04 Jul 2023 03:03:13 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 04 Jul 2023 03:03:13 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:03:13 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a1428b80937a0eb55c8466779cec4bcf7e31bdcc4fc66b763448cf9d131563`  
		Last Modified: Tue, 04 Jul 2023 03:03:50 GMT  
		Size: 2.6 MB (2559426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa00861c721843ae490a68a90f1db04218b5131cb6b2d6d39618973618f3da3`  
		Last Modified: Tue, 04 Jul 2023 03:03:49 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3e06c4413e69400a792d7a95cad6d643afdbcdc2f28fdd90e603e2f22e33a7`  
		Last Modified: Tue, 04 Jul 2023 03:03:53 GMT  
		Size: 40.1 MB (40079874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ab794d03683cd2393608f40731e4c588dbc7661668e884227ec782c7011921`  
		Last Modified: Tue, 04 Jul 2023 03:03:49 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.18`

```console
$ docker pull emqx@sha256:ec2c136fb5831a5619b45e3ef70ed8727c7e8d65227339b31596525851b73934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.18` - linux; amd64

```console
$ docker pull emqx@sha256:59814c0cd7e916de55642b6534fd578b0a6e57eb699663d010dc069dcda222b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81290390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:369b89a4a859e567c7417697198a5de2189165cab88dfdaca3ad6276ea00b827`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:20:58 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:20:58 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 04 Jul 2023 04:20:58 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 04 Jul 2023 04:20:58 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 04 Jul 2023 04:21:03 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 04 Jul 2023 04:21:03 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 04:21:03 GMT
USER emqx
# Tue, 04 Jul 2023 04:21:04 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 04:21:04 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 04 Jul 2023 04:21:04 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 04 Jul 2023 04:21:04 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 04:21:04 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ef462373a136b96c0a554f87fe5b08b7c8461aba1e112745b996eaa7b98a7d`  
		Last Modified: Tue, 04 Jul 2023 04:21:43 GMT  
		Size: 2.6 MB (2569640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ad23a7d23aef4b144a14d30ac52f4568fb6adbc5c43bebc8041add65f9d8bd`  
		Last Modified: Tue, 04 Jul 2023 04:21:42 GMT  
		Size: 4.1 KB (4103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7aaf596f0066ac6b1036ee6901f889790109e0307a7769061cc46db57b37e0e`  
		Last Modified: Tue, 04 Jul 2023 04:21:47 GMT  
		Size: 47.3 MB (47298154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe0eabbe33e4b55892b3f2a3a28715c0da29545d619854b113633ec7d92e25e`  
		Last Modified: Tue, 04 Jul 2023 04:21:43 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.18` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:2d08ee2bc416b6f69851a687377881c076764d6010794177a34c576f405d0eea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72707473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99ef632180b6d12a52f16c392ec17886bc0626d84ec46d8a7d1f71cea9b85a0d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:08 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:08 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 04 Jul 2023 03:03:08 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 04 Jul 2023 03:03:09 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 04 Jul 2023 03:03:12 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 04 Jul 2023 03:03:13 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 03:03:13 GMT
USER emqx
# Tue, 04 Jul 2023 03:03:13 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 03:03:13 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 04 Jul 2023 03:03:13 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 04 Jul 2023 03:03:13 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:03:13 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a1428b80937a0eb55c8466779cec4bcf7e31bdcc4fc66b763448cf9d131563`  
		Last Modified: Tue, 04 Jul 2023 03:03:50 GMT  
		Size: 2.6 MB (2559426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa00861c721843ae490a68a90f1db04218b5131cb6b2d6d39618973618f3da3`  
		Last Modified: Tue, 04 Jul 2023 03:03:49 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3e06c4413e69400a792d7a95cad6d643afdbcdc2f28fdd90e603e2f22e33a7`  
		Last Modified: Tue, 04 Jul 2023 03:03:53 GMT  
		Size: 40.1 MB (40079874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ab794d03683cd2393608f40731e4c588dbc7661668e884227ec782c7011921`  
		Last Modified: Tue, 04 Jul 2023 03:03:49 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5`

```console
$ docker pull emqx@sha256:2b27eb151be02ab9c31e866f0e84c7008c5c6592b4de773dcb45670ccf07d97a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:150a0ad4f76f422b65943de7e08dc19ee02c398d0545397d3dbdde1be18b00dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.5 MB (103466209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b3ee6a61133741d0c25cfe49d0b11a64e7e45515f864604521562069ea92bd2`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:14 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 04 Jul 2023 04:21:24 GMT
ENV EMQX_VERSION=5.1.0
# Tue, 04 Jul 2023 04:21:24 GMT
ENV AMD64_SHA256=946d8a047c8863afa318abf41be4c265c205d86aa8e6401a39282f02eecbe481
# Tue, 04 Jul 2023 04:21:24 GMT
ENV ARM64_SHA256=9f9ffa019960a6d4a6d60ec0b0f7a45513e326df7667a166aef827d248054940
# Tue, 04 Jul 2023 04:21:24 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 04 Jul 2023 04:21:31 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 04 Jul 2023 04:21:31 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 04:21:31 GMT
USER emqx
# Tue, 04 Jul 2023 04:21:31 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 04:21:31 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 04 Jul 2023 04:21:31 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 04 Jul 2023 04:21:31 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 04:21:31 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a63034914a435ac7d89264c48bbfd001cc80603c14d21f4eb9895099fa4e31a`  
		Last Modified: Tue, 04 Jul 2023 04:21:58 GMT  
		Size: 3.0 MB (2987794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27d1c79ae1ac7fb241e52deb948fc9ef459a4cc65b366dcc7911393421f4d4`  
		Last Modified: Tue, 04 Jul 2023 04:21:57 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563ee21ab39dfb4552324632ac896591a823b5c34e63cc4eb6935e977af4e788`  
		Last Modified: Tue, 04 Jul 2023 04:22:22 GMT  
		Size: 69.1 MB (69056021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636eaab88751694b736e6218485a16c06e98f18c14cbea0faf34af8c941a584b`  
		Last Modified: Tue, 04 Jul 2023 04:22:14 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:4148afe49e12dc03200209413840898e99aa03b8f5f5bfec85cf44019656642a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.8 MB (93775506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deb850920403a69a76452c79aa52766dcb4dbc5c7a8940c2ce4a284a346d2e8b`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:21 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:22 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 04 Jul 2023 03:03:33 GMT
ENV EMQX_VERSION=5.1.0
# Tue, 04 Jul 2023 03:03:33 GMT
ENV AMD64_SHA256=946d8a047c8863afa318abf41be4c265c205d86aa8e6401a39282f02eecbe481
# Tue, 04 Jul 2023 03:03:33 GMT
ENV ARM64_SHA256=9f9ffa019960a6d4a6d60ec0b0f7a45513e326df7667a166aef827d248054940
# Tue, 04 Jul 2023 03:03:33 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 04 Jul 2023 03:03:38 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 04 Jul 2023 03:03:39 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 03:03:39 GMT
USER emqx
# Tue, 04 Jul 2023 03:03:39 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 03:03:39 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 04 Jul 2023 03:03:39 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 04 Jul 2023 03:03:39 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:03:39 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc212c7c7d61e498e2041ef1be251acbca34483d513266fc40c2b0d41721f61`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 3.0 MB (3003072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94aca2cf657bb3bfb3bf3c6675087076999f1bd3e64ffbe99a129c8475d7795`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb0ee34f24505f117510ea59fbcce761b0774efa37d970225c044ea801563ef`  
		Last Modified: Tue, 04 Jul 2023 03:04:21 GMT  
		Size: 60.7 MB (60704464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f314df5ec7d54820af1b65139f593fc8c59095734ef557f9116c1a8b42d5ba60`  
		Last Modified: Tue, 04 Jul 2023 03:04:16 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:ed48aca55fd8df1845e9f6b8bab7a234667f82ee54ae3c883e7a390be9fec1b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:af206b512e1993e2ec001139a2f953cd371d9384fdc405b8119a6ebbac8540cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101982049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef0cfed032bdaa77c77d68bbd4278426f4ed54fedc2ac0f37bc22f2e87ca2219`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:14 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 04 Jul 2023 04:21:14 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 04 Jul 2023 04:21:14 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 04 Jul 2023 04:21:14 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 04 Jul 2023 04:21:14 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 04 Jul 2023 04:21:20 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 04 Jul 2023 04:21:21 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 04:21:21 GMT
USER emqx
# Tue, 04 Jul 2023 04:21:21 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 04:21:21 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 04 Jul 2023 04:21:21 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 04 Jul 2023 04:21:21 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 04:21:21 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a63034914a435ac7d89264c48bbfd001cc80603c14d21f4eb9895099fa4e31a`  
		Last Modified: Tue, 04 Jul 2023 04:21:58 GMT  
		Size: 3.0 MB (2987794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27d1c79ae1ac7fb241e52deb948fc9ef459a4cc65b366dcc7911393421f4d4`  
		Last Modified: Tue, 04 Jul 2023 04:21:57 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62baa3e39a567ab3fb2ef18688452d5a8e863961248234dc567d41b0d6bd798a`  
		Last Modified: Tue, 04 Jul 2023 04:22:05 GMT  
		Size: 67.6 MB (67571860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8c5ab9c1f57c1002a6b3251c5f524eb0c22290720ea5fe523cc649471a1084`  
		Last Modified: Tue, 04 Jul 2023 04:21:57 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:0abdd21e8a6b3206455cb733eca21c22695b7dc06a98d3a4de5eb999537b0195
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93060437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db90f1f3fab83ce999d6472a64971ca463afb82097d6b4cdb5da98a3c2f28c0d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:21 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:22 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 04 Jul 2023 03:03:22 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 04 Jul 2023 03:03:22 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 04 Jul 2023 03:03:22 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 04 Jul 2023 03:03:22 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 04 Jul 2023 03:03:28 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 04 Jul 2023 03:03:28 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 03:03:28 GMT
USER emqx
# Tue, 04 Jul 2023 03:03:28 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 03:03:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 04 Jul 2023 03:03:29 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 04 Jul 2023 03:03:29 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:03:29 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc212c7c7d61e498e2041ef1be251acbca34483d513266fc40c2b0d41721f61`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 3.0 MB (3003072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94aca2cf657bb3bfb3bf3c6675087076999f1bd3e64ffbe99a129c8475d7795`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf20fcfbb7660480c1e5425d2d670e3fc48e00264da9d9a5b0eb282e2472df6`  
		Last Modified: Tue, 04 Jul 2023 03:04:08 GMT  
		Size: 60.0 MB (59989394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03deeecf9242891f89e9ebbde2e0197c04be91ee39569bfcd63a6a3336b20801`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.26`

```console
$ docker pull emqx@sha256:ed48aca55fd8df1845e9f6b8bab7a234667f82ee54ae3c883e7a390be9fec1b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0.26` - linux; amd64

```console
$ docker pull emqx@sha256:af206b512e1993e2ec001139a2f953cd371d9384fdc405b8119a6ebbac8540cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101982049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef0cfed032bdaa77c77d68bbd4278426f4ed54fedc2ac0f37bc22f2e87ca2219`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:14 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 04 Jul 2023 04:21:14 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 04 Jul 2023 04:21:14 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 04 Jul 2023 04:21:14 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 04 Jul 2023 04:21:14 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 04 Jul 2023 04:21:20 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 04 Jul 2023 04:21:21 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 04:21:21 GMT
USER emqx
# Tue, 04 Jul 2023 04:21:21 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 04:21:21 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 04 Jul 2023 04:21:21 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 04 Jul 2023 04:21:21 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 04:21:21 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a63034914a435ac7d89264c48bbfd001cc80603c14d21f4eb9895099fa4e31a`  
		Last Modified: Tue, 04 Jul 2023 04:21:58 GMT  
		Size: 3.0 MB (2987794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27d1c79ae1ac7fb241e52deb948fc9ef459a4cc65b366dcc7911393421f4d4`  
		Last Modified: Tue, 04 Jul 2023 04:21:57 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62baa3e39a567ab3fb2ef18688452d5a8e863961248234dc567d41b0d6bd798a`  
		Last Modified: Tue, 04 Jul 2023 04:22:05 GMT  
		Size: 67.6 MB (67571860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8c5ab9c1f57c1002a6b3251c5f524eb0c22290720ea5fe523cc649471a1084`  
		Last Modified: Tue, 04 Jul 2023 04:21:57 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0.26` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:0abdd21e8a6b3206455cb733eca21c22695b7dc06a98d3a4de5eb999537b0195
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93060437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db90f1f3fab83ce999d6472a64971ca463afb82097d6b4cdb5da98a3c2f28c0d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:21 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:22 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 04 Jul 2023 03:03:22 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 04 Jul 2023 03:03:22 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 04 Jul 2023 03:03:22 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 04 Jul 2023 03:03:22 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 04 Jul 2023 03:03:28 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 04 Jul 2023 03:03:28 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 03:03:28 GMT
USER emqx
# Tue, 04 Jul 2023 03:03:28 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 03:03:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 04 Jul 2023 03:03:29 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 04 Jul 2023 03:03:29 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:03:29 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc212c7c7d61e498e2041ef1be251acbca34483d513266fc40c2b0d41721f61`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 3.0 MB (3003072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94aca2cf657bb3bfb3bf3c6675087076999f1bd3e64ffbe99a129c8475d7795`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf20fcfbb7660480c1e5425d2d670e3fc48e00264da9d9a5b0eb282e2472df6`  
		Last Modified: Tue, 04 Jul 2023 03:04:08 GMT  
		Size: 60.0 MB (59989394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03deeecf9242891f89e9ebbde2e0197c04be91ee39569bfcd63a6a3336b20801`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.1`

```console
$ docker pull emqx@sha256:2b27eb151be02ab9c31e866f0e84c7008c5c6592b4de773dcb45670ccf07d97a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.1` - linux; amd64

```console
$ docker pull emqx@sha256:150a0ad4f76f422b65943de7e08dc19ee02c398d0545397d3dbdde1be18b00dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.5 MB (103466209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b3ee6a61133741d0c25cfe49d0b11a64e7e45515f864604521562069ea92bd2`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:14 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 04 Jul 2023 04:21:24 GMT
ENV EMQX_VERSION=5.1.0
# Tue, 04 Jul 2023 04:21:24 GMT
ENV AMD64_SHA256=946d8a047c8863afa318abf41be4c265c205d86aa8e6401a39282f02eecbe481
# Tue, 04 Jul 2023 04:21:24 GMT
ENV ARM64_SHA256=9f9ffa019960a6d4a6d60ec0b0f7a45513e326df7667a166aef827d248054940
# Tue, 04 Jul 2023 04:21:24 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 04 Jul 2023 04:21:31 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 04 Jul 2023 04:21:31 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 04:21:31 GMT
USER emqx
# Tue, 04 Jul 2023 04:21:31 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 04:21:31 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 04 Jul 2023 04:21:31 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 04 Jul 2023 04:21:31 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 04:21:31 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a63034914a435ac7d89264c48bbfd001cc80603c14d21f4eb9895099fa4e31a`  
		Last Modified: Tue, 04 Jul 2023 04:21:58 GMT  
		Size: 3.0 MB (2987794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27d1c79ae1ac7fb241e52deb948fc9ef459a4cc65b366dcc7911393421f4d4`  
		Last Modified: Tue, 04 Jul 2023 04:21:57 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563ee21ab39dfb4552324632ac896591a823b5c34e63cc4eb6935e977af4e788`  
		Last Modified: Tue, 04 Jul 2023 04:22:22 GMT  
		Size: 69.1 MB (69056021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636eaab88751694b736e6218485a16c06e98f18c14cbea0faf34af8c941a584b`  
		Last Modified: Tue, 04 Jul 2023 04:22:14 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.1` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:4148afe49e12dc03200209413840898e99aa03b8f5f5bfec85cf44019656642a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.8 MB (93775506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deb850920403a69a76452c79aa52766dcb4dbc5c7a8940c2ce4a284a346d2e8b`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:21 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:22 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 04 Jul 2023 03:03:33 GMT
ENV EMQX_VERSION=5.1.0
# Tue, 04 Jul 2023 03:03:33 GMT
ENV AMD64_SHA256=946d8a047c8863afa318abf41be4c265c205d86aa8e6401a39282f02eecbe481
# Tue, 04 Jul 2023 03:03:33 GMT
ENV ARM64_SHA256=9f9ffa019960a6d4a6d60ec0b0f7a45513e326df7667a166aef827d248054940
# Tue, 04 Jul 2023 03:03:33 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 04 Jul 2023 03:03:38 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 04 Jul 2023 03:03:39 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 03:03:39 GMT
USER emqx
# Tue, 04 Jul 2023 03:03:39 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 03:03:39 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 04 Jul 2023 03:03:39 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 04 Jul 2023 03:03:39 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:03:39 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc212c7c7d61e498e2041ef1be251acbca34483d513266fc40c2b0d41721f61`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 3.0 MB (3003072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94aca2cf657bb3bfb3bf3c6675087076999f1bd3e64ffbe99a129c8475d7795`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb0ee34f24505f117510ea59fbcce761b0774efa37d970225c044ea801563ef`  
		Last Modified: Tue, 04 Jul 2023 03:04:21 GMT  
		Size: 60.7 MB (60704464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f314df5ec7d54820af1b65139f593fc8c59095734ef557f9116c1a8b42d5ba60`  
		Last Modified: Tue, 04 Jul 2023 03:04:16 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.1.0`

```console
$ docker pull emqx@sha256:2b27eb151be02ab9c31e866f0e84c7008c5c6592b4de773dcb45670ccf07d97a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.1.0` - linux; amd64

```console
$ docker pull emqx@sha256:150a0ad4f76f422b65943de7e08dc19ee02c398d0545397d3dbdde1be18b00dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.5 MB (103466209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b3ee6a61133741d0c25cfe49d0b11a64e7e45515f864604521562069ea92bd2`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:14 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 04 Jul 2023 04:21:24 GMT
ENV EMQX_VERSION=5.1.0
# Tue, 04 Jul 2023 04:21:24 GMT
ENV AMD64_SHA256=946d8a047c8863afa318abf41be4c265c205d86aa8e6401a39282f02eecbe481
# Tue, 04 Jul 2023 04:21:24 GMT
ENV ARM64_SHA256=9f9ffa019960a6d4a6d60ec0b0f7a45513e326df7667a166aef827d248054940
# Tue, 04 Jul 2023 04:21:24 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 04 Jul 2023 04:21:31 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 04 Jul 2023 04:21:31 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 04:21:31 GMT
USER emqx
# Tue, 04 Jul 2023 04:21:31 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 04:21:31 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 04 Jul 2023 04:21:31 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 04 Jul 2023 04:21:31 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 04:21:31 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a63034914a435ac7d89264c48bbfd001cc80603c14d21f4eb9895099fa4e31a`  
		Last Modified: Tue, 04 Jul 2023 04:21:58 GMT  
		Size: 3.0 MB (2987794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27d1c79ae1ac7fb241e52deb948fc9ef459a4cc65b366dcc7911393421f4d4`  
		Last Modified: Tue, 04 Jul 2023 04:21:57 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563ee21ab39dfb4552324632ac896591a823b5c34e63cc4eb6935e977af4e788`  
		Last Modified: Tue, 04 Jul 2023 04:22:22 GMT  
		Size: 69.1 MB (69056021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636eaab88751694b736e6218485a16c06e98f18c14cbea0faf34af8c941a584b`  
		Last Modified: Tue, 04 Jul 2023 04:22:14 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.1.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:4148afe49e12dc03200209413840898e99aa03b8f5f5bfec85cf44019656642a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.8 MB (93775506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deb850920403a69a76452c79aa52766dcb4dbc5c7a8940c2ce4a284a346d2e8b`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:21 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:22 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 04 Jul 2023 03:03:33 GMT
ENV EMQX_VERSION=5.1.0
# Tue, 04 Jul 2023 03:03:33 GMT
ENV AMD64_SHA256=946d8a047c8863afa318abf41be4c265c205d86aa8e6401a39282f02eecbe481
# Tue, 04 Jul 2023 03:03:33 GMT
ENV ARM64_SHA256=9f9ffa019960a6d4a6d60ec0b0f7a45513e326df7667a166aef827d248054940
# Tue, 04 Jul 2023 03:03:33 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 04 Jul 2023 03:03:38 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 04 Jul 2023 03:03:39 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 03:03:39 GMT
USER emqx
# Tue, 04 Jul 2023 03:03:39 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 03:03:39 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 04 Jul 2023 03:03:39 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 04 Jul 2023 03:03:39 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:03:39 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc212c7c7d61e498e2041ef1be251acbca34483d513266fc40c2b0d41721f61`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 3.0 MB (3003072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94aca2cf657bb3bfb3bf3c6675087076999f1bd3e64ffbe99a129c8475d7795`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb0ee34f24505f117510ea59fbcce761b0774efa37d970225c044ea801563ef`  
		Last Modified: Tue, 04 Jul 2023 03:04:21 GMT  
		Size: 60.7 MB (60704464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f314df5ec7d54820af1b65139f593fc8c59095734ef557f9116c1a8b42d5ba60`  
		Last Modified: Tue, 04 Jul 2023 03:04:16 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:2b27eb151be02ab9c31e866f0e84c7008c5c6592b4de773dcb45670ccf07d97a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:150a0ad4f76f422b65943de7e08dc19ee02c398d0545397d3dbdde1be18b00dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.5 MB (103466209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b3ee6a61133741d0c25cfe49d0b11a64e7e45515f864604521562069ea92bd2`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:14 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 04 Jul 2023 04:21:24 GMT
ENV EMQX_VERSION=5.1.0
# Tue, 04 Jul 2023 04:21:24 GMT
ENV AMD64_SHA256=946d8a047c8863afa318abf41be4c265c205d86aa8e6401a39282f02eecbe481
# Tue, 04 Jul 2023 04:21:24 GMT
ENV ARM64_SHA256=9f9ffa019960a6d4a6d60ec0b0f7a45513e326df7667a166aef827d248054940
# Tue, 04 Jul 2023 04:21:24 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 04 Jul 2023 04:21:31 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 04 Jul 2023 04:21:31 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 04:21:31 GMT
USER emqx
# Tue, 04 Jul 2023 04:21:31 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 04:21:31 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 04 Jul 2023 04:21:31 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 04 Jul 2023 04:21:31 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 04:21:31 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a63034914a435ac7d89264c48bbfd001cc80603c14d21f4eb9895099fa4e31a`  
		Last Modified: Tue, 04 Jul 2023 04:21:58 GMT  
		Size: 3.0 MB (2987794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27d1c79ae1ac7fb241e52deb948fc9ef459a4cc65b366dcc7911393421f4d4`  
		Last Modified: Tue, 04 Jul 2023 04:21:57 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563ee21ab39dfb4552324632ac896591a823b5c34e63cc4eb6935e977af4e788`  
		Last Modified: Tue, 04 Jul 2023 04:22:22 GMT  
		Size: 69.1 MB (69056021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636eaab88751694b736e6218485a16c06e98f18c14cbea0faf34af8c941a584b`  
		Last Modified: Tue, 04 Jul 2023 04:22:14 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:4148afe49e12dc03200209413840898e99aa03b8f5f5bfec85cf44019656642a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.8 MB (93775506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deb850920403a69a76452c79aa52766dcb4dbc5c7a8940c2ce4a284a346d2e8b`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:03:21 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:03:22 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 04 Jul 2023 03:03:33 GMT
ENV EMQX_VERSION=5.1.0
# Tue, 04 Jul 2023 03:03:33 GMT
ENV AMD64_SHA256=946d8a047c8863afa318abf41be4c265c205d86aa8e6401a39282f02eecbe481
# Tue, 04 Jul 2023 03:03:33 GMT
ENV ARM64_SHA256=9f9ffa019960a6d4a6d60ec0b0f7a45513e326df7667a166aef827d248054940
# Tue, 04 Jul 2023 03:03:33 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 04 Jul 2023 03:03:38 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 04 Jul 2023 03:03:39 GMT
WORKDIR /opt/emqx
# Tue, 04 Jul 2023 03:03:39 GMT
USER emqx
# Tue, 04 Jul 2023 03:03:39 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 04 Jul 2023 03:03:39 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 04 Jul 2023 03:03:39 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 04 Jul 2023 03:03:39 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:03:39 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc212c7c7d61e498e2041ef1be251acbca34483d513266fc40c2b0d41721f61`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 3.0 MB (3003072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94aca2cf657bb3bfb3bf3c6675087076999f1bd3e64ffbe99a129c8475d7795`  
		Last Modified: Tue, 04 Jul 2023 03:04:03 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb0ee34f24505f117510ea59fbcce761b0774efa37d970225c044ea801563ef`  
		Last Modified: Tue, 04 Jul 2023 03:04:21 GMT  
		Size: 60.7 MB (60704464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f314df5ec7d54820af1b65139f593fc8c59095734ef557f9116c1a8b42d5ba60`  
		Last Modified: Tue, 04 Jul 2023 03:04:16 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
