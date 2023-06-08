<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.18`](#emqx4418)
-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.26`](#emqx5026)
-	[`emqx:latest`](#emqxlatest)

## `emqx:4`

```console
$ docker pull emqx@sha256:107753cba90c6d21cf672fb273cbdb4e4f62a194cdf0ddc60380ac8625927a41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:6d5f00b0c9200c3505a8ce271800663529f113cd2706fd4b4e08d126c5052cb6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81276666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6700291e3b693c5c27f00ad9ee0dbcd6afda2b5943b242e99287cb7909baaa84`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 08:23:46 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 08:23:47 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 23 May 2023 08:23:47 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 23 May 2023 08:23:47 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 23 May 2023 08:23:52 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 23 May 2023 08:23:52 GMT
WORKDIR /opt/emqx
# Tue, 23 May 2023 08:23:53 GMT
USER emqx
# Tue, 23 May 2023 08:23:53 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 23 May 2023 08:23:53 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 23 May 2023 08:23:53 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 23 May 2023 08:23:53 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 23 May 2023 08:23:53 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c357982b906825c7f27d5a15ef8411492d88de11e38de5b4561e8b5fcdd1cc`  
		Last Modified: Tue, 23 May 2023 08:24:20 GMT  
		Size: 2.6 MB (2569661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e6c170ad4c04e1fd54f5c1b87c0d4ad727619673e741a0e359f8e17c513c9e`  
		Last Modified: Tue, 23 May 2023 08:24:20 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694f3ca204fc6911a5d9e9408aac5556c11eb8ee1b606e5b01fe1f9066fff5b0`  
		Last Modified: Tue, 23 May 2023 08:24:24 GMT  
		Size: 47.3 MB (47298202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1117a08a7689b94086f3459bbf4c632a65f8dca0507cc34ed421be7824c5d7e5`  
		Last Modified: Tue, 23 May 2023 08:24:20 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:7688768a72b7fa9010de1fe1700217548815af988a17de2b9bd65a60a454e067
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72697315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa151f551c374dd3d4e17e89a56c17041e9bfb540a498c24aa000dd2426bd8d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:42:31 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:42:32 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 23 May 2023 01:42:32 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 23 May 2023 01:42:32 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 23 May 2023 01:42:36 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 23 May 2023 01:42:36 GMT
WORKDIR /opt/emqx
# Tue, 23 May 2023 01:42:36 GMT
USER emqx
# Tue, 23 May 2023 01:42:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 23 May 2023 01:42:36 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 23 May 2023 01:42:36 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 23 May 2023 01:42:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 23 May 2023 01:42:36 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e3be4db2d4e51135129c236fbac8797820630823c20cc285003c52204383a9`  
		Last Modified: Tue, 23 May 2023 01:42:59 GMT  
		Size: 2.6 MB (2559465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fea7a7747eda949c0b01b8782f9bce294e4d252d81ad86e697b761fa378ee86`  
		Last Modified: Tue, 23 May 2023 01:42:58 GMT  
		Size: 4.1 KB (4115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762dea4f4f570daf68e5a15a784874befa9af9aade89f064f7aa6c95956eb8af`  
		Last Modified: Tue, 23 May 2023 01:43:02 GMT  
		Size: 40.1 MB (40079880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a354585a72ccdf88f7dbe22e0f7173467f9273217904a5f411184836f4b2487d`  
		Last Modified: Tue, 23 May 2023 01:42:59 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:107753cba90c6d21cf672fb273cbdb4e4f62a194cdf0ddc60380ac8625927a41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:6d5f00b0c9200c3505a8ce271800663529f113cd2706fd4b4e08d126c5052cb6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81276666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6700291e3b693c5c27f00ad9ee0dbcd6afda2b5943b242e99287cb7909baaa84`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 08:23:46 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 08:23:47 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 23 May 2023 08:23:47 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 23 May 2023 08:23:47 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 23 May 2023 08:23:52 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 23 May 2023 08:23:52 GMT
WORKDIR /opt/emqx
# Tue, 23 May 2023 08:23:53 GMT
USER emqx
# Tue, 23 May 2023 08:23:53 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 23 May 2023 08:23:53 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 23 May 2023 08:23:53 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 23 May 2023 08:23:53 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 23 May 2023 08:23:53 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c357982b906825c7f27d5a15ef8411492d88de11e38de5b4561e8b5fcdd1cc`  
		Last Modified: Tue, 23 May 2023 08:24:20 GMT  
		Size: 2.6 MB (2569661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e6c170ad4c04e1fd54f5c1b87c0d4ad727619673e741a0e359f8e17c513c9e`  
		Last Modified: Tue, 23 May 2023 08:24:20 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694f3ca204fc6911a5d9e9408aac5556c11eb8ee1b606e5b01fe1f9066fff5b0`  
		Last Modified: Tue, 23 May 2023 08:24:24 GMT  
		Size: 47.3 MB (47298202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1117a08a7689b94086f3459bbf4c632a65f8dca0507cc34ed421be7824c5d7e5`  
		Last Modified: Tue, 23 May 2023 08:24:20 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:7688768a72b7fa9010de1fe1700217548815af988a17de2b9bd65a60a454e067
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72697315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa151f551c374dd3d4e17e89a56c17041e9bfb540a498c24aa000dd2426bd8d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:42:31 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:42:32 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 23 May 2023 01:42:32 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 23 May 2023 01:42:32 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 23 May 2023 01:42:36 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 23 May 2023 01:42:36 GMT
WORKDIR /opt/emqx
# Tue, 23 May 2023 01:42:36 GMT
USER emqx
# Tue, 23 May 2023 01:42:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 23 May 2023 01:42:36 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 23 May 2023 01:42:36 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 23 May 2023 01:42:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 23 May 2023 01:42:36 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e3be4db2d4e51135129c236fbac8797820630823c20cc285003c52204383a9`  
		Last Modified: Tue, 23 May 2023 01:42:59 GMT  
		Size: 2.6 MB (2559465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fea7a7747eda949c0b01b8782f9bce294e4d252d81ad86e697b761fa378ee86`  
		Last Modified: Tue, 23 May 2023 01:42:58 GMT  
		Size: 4.1 KB (4115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762dea4f4f570daf68e5a15a784874befa9af9aade89f064f7aa6c95956eb8af`  
		Last Modified: Tue, 23 May 2023 01:43:02 GMT  
		Size: 40.1 MB (40079880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a354585a72ccdf88f7dbe22e0f7173467f9273217904a5f411184836f4b2487d`  
		Last Modified: Tue, 23 May 2023 01:42:59 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.18`

```console
$ docker pull emqx@sha256:107753cba90c6d21cf672fb273cbdb4e4f62a194cdf0ddc60380ac8625927a41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.18` - linux; amd64

```console
$ docker pull emqx@sha256:6d5f00b0c9200c3505a8ce271800663529f113cd2706fd4b4e08d126c5052cb6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81276666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6700291e3b693c5c27f00ad9ee0dbcd6afda2b5943b242e99287cb7909baaa84`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 08:23:46 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 08:23:47 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 23 May 2023 08:23:47 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 23 May 2023 08:23:47 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 23 May 2023 08:23:52 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 23 May 2023 08:23:52 GMT
WORKDIR /opt/emqx
# Tue, 23 May 2023 08:23:53 GMT
USER emqx
# Tue, 23 May 2023 08:23:53 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 23 May 2023 08:23:53 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 23 May 2023 08:23:53 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 23 May 2023 08:23:53 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 23 May 2023 08:23:53 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c357982b906825c7f27d5a15ef8411492d88de11e38de5b4561e8b5fcdd1cc`  
		Last Modified: Tue, 23 May 2023 08:24:20 GMT  
		Size: 2.6 MB (2569661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e6c170ad4c04e1fd54f5c1b87c0d4ad727619673e741a0e359f8e17c513c9e`  
		Last Modified: Tue, 23 May 2023 08:24:20 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694f3ca204fc6911a5d9e9408aac5556c11eb8ee1b606e5b01fe1f9066fff5b0`  
		Last Modified: Tue, 23 May 2023 08:24:24 GMT  
		Size: 47.3 MB (47298202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1117a08a7689b94086f3459bbf4c632a65f8dca0507cc34ed421be7824c5d7e5`  
		Last Modified: Tue, 23 May 2023 08:24:20 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.18` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:7688768a72b7fa9010de1fe1700217548815af988a17de2b9bd65a60a454e067
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72697315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa151f551c374dd3d4e17e89a56c17041e9bfb540a498c24aa000dd2426bd8d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:42:31 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:42:32 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Tue, 23 May 2023 01:42:32 GMT
ENV EMQX_VERSION=4.4.18
# Tue, 23 May 2023 01:42:32 GMT
ENV OTP=otp24.3.4.2-1
# Tue, 23 May 2023 01:42:36 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="53712834a3cf209e488b97842ed9d6bae887e6e79ebaae3a0887018aab59b05b"; fi;     if [ ${arch} = "arm64" ]; then sha256="5fe04b2a10fc5e43ee582b38ecd526480a44ae277f5e6aa68ccd85f45e76baad"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 23 May 2023 01:42:36 GMT
WORKDIR /opt/emqx
# Tue, 23 May 2023 01:42:36 GMT
USER emqx
# Tue, 23 May 2023 01:42:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 23 May 2023 01:42:36 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 23 May 2023 01:42:36 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 23 May 2023 01:42:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 23 May 2023 01:42:36 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e3be4db2d4e51135129c236fbac8797820630823c20cc285003c52204383a9`  
		Last Modified: Tue, 23 May 2023 01:42:59 GMT  
		Size: 2.6 MB (2559465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fea7a7747eda949c0b01b8782f9bce294e4d252d81ad86e697b761fa378ee86`  
		Last Modified: Tue, 23 May 2023 01:42:58 GMT  
		Size: 4.1 KB (4115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762dea4f4f570daf68e5a15a784874befa9af9aade89f064f7aa6c95956eb8af`  
		Last Modified: Tue, 23 May 2023 01:43:02 GMT  
		Size: 40.1 MB (40079880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a354585a72ccdf88f7dbe22e0f7173467f9273217904a5f411184836f4b2487d`  
		Last Modified: Tue, 23 May 2023 01:42:59 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5`

```console
$ docker pull emqx@sha256:b0fe72a44d77f7c0528aad08ca4a6d2aa125229308ab92bd9c627faa9ff4464e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:4d19a6cb422675146d37e55ea865dd48ed7f11f06ab01ac687cb8782372a470d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101968277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95a19311e1c3f696622ca62e69ddf194dd3609e7ad5a93054f23551d385dc8ff`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 08:24:00 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 08:24:01 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 08 Jun 2023 16:19:39 GMT
ENV EMQX_VERSION=5.0.26
# Thu, 08 Jun 2023 16:19:39 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Thu, 08 Jun 2023 16:19:39 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Thu, 08 Jun 2023 16:19:40 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 08 Jun 2023 16:19:46 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 08 Jun 2023 16:19:47 GMT
WORKDIR /opt/emqx
# Thu, 08 Jun 2023 16:19:47 GMT
USER emqx
# Thu, 08 Jun 2023 16:19:47 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 08 Jun 2023 16:19:47 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 08 Jun 2023 16:19:47 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 08 Jun 2023 16:19:47 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 08 Jun 2023 16:19:47 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ce7ad79b255e788cff6cef738579e0bbf7797cb46293052c0dac256ec5cce9`  
		Last Modified: Tue, 23 May 2023 08:24:36 GMT  
		Size: 3.0 MB (2987806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7beaac16821c81034b9f18e03825f60acf03fbd723d44a9650179d3059bc25`  
		Last Modified: Tue, 23 May 2023 08:24:35 GMT  
		Size: 4.1 KB (4119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575f38e8e71d018e527d06b05a4425cf58acc4265e53f203cb15f7643d99791e`  
		Last Modified: Thu, 08 Jun 2023 16:20:05 GMT  
		Size: 67.6 MB (67571863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801d24f1c64e8ff688cf56f07e65e590a3411a4319de2413f5295128016e2e81`  
		Last Modified: Thu, 08 Jun 2023 16:19:58 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:14be62d2d889fda33654710ce8dc7f83a3f62d0d62b91f4439d6ce99ffa8791a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93050144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d49baedc236d4d7d75401808848130f850c4788b9f9f03167ccd8682ea73188`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:42:42 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:42:43 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 08 Jun 2023 16:39:24 GMT
ENV EMQX_VERSION=5.0.26
# Thu, 08 Jun 2023 16:39:24 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Thu, 08 Jun 2023 16:39:24 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Thu, 08 Jun 2023 16:39:24 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 08 Jun 2023 16:39:30 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 08 Jun 2023 16:39:30 GMT
WORKDIR /opt/emqx
# Thu, 08 Jun 2023 16:39:30 GMT
USER emqx
# Thu, 08 Jun 2023 16:39:30 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 08 Jun 2023 16:39:31 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 08 Jun 2023 16:39:31 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 08 Jun 2023 16:39:31 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 08 Jun 2023 16:39:31 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8345ceedc06f3b0ae12a8eb9f0f0e7dd52b3ae9800880811d86f7c26b0651446`  
		Last Modified: Tue, 23 May 2023 01:43:12 GMT  
		Size: 3.0 MB (3002990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b78e6c4890d65e6f6f17dbd7faa9d396eaad9d65dd2bbeb2e49aee524b18b1e`  
		Last Modified: Tue, 23 May 2023 01:43:11 GMT  
		Size: 4.1 KB (4115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0747c7d95e3a29e9a42c032ab9e7fd7a2f9a83887751923d8a1ba76ece60e0f6`  
		Last Modified: Thu, 08 Jun 2023 16:39:46 GMT  
		Size: 60.0 MB (59989387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5504f0bc88e3943acea76d78680ec89b99149c73ec33633ac1d1b47ac6c555f5`  
		Last Modified: Thu, 08 Jun 2023 16:39:40 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:b0fe72a44d77f7c0528aad08ca4a6d2aa125229308ab92bd9c627faa9ff4464e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:4d19a6cb422675146d37e55ea865dd48ed7f11f06ab01ac687cb8782372a470d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101968277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95a19311e1c3f696622ca62e69ddf194dd3609e7ad5a93054f23551d385dc8ff`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 08:24:00 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 08:24:01 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 08 Jun 2023 16:19:39 GMT
ENV EMQX_VERSION=5.0.26
# Thu, 08 Jun 2023 16:19:39 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Thu, 08 Jun 2023 16:19:39 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Thu, 08 Jun 2023 16:19:40 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 08 Jun 2023 16:19:46 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 08 Jun 2023 16:19:47 GMT
WORKDIR /opt/emqx
# Thu, 08 Jun 2023 16:19:47 GMT
USER emqx
# Thu, 08 Jun 2023 16:19:47 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 08 Jun 2023 16:19:47 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 08 Jun 2023 16:19:47 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 08 Jun 2023 16:19:47 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 08 Jun 2023 16:19:47 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ce7ad79b255e788cff6cef738579e0bbf7797cb46293052c0dac256ec5cce9`  
		Last Modified: Tue, 23 May 2023 08:24:36 GMT  
		Size: 3.0 MB (2987806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7beaac16821c81034b9f18e03825f60acf03fbd723d44a9650179d3059bc25`  
		Last Modified: Tue, 23 May 2023 08:24:35 GMT  
		Size: 4.1 KB (4119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575f38e8e71d018e527d06b05a4425cf58acc4265e53f203cb15f7643d99791e`  
		Last Modified: Thu, 08 Jun 2023 16:20:05 GMT  
		Size: 67.6 MB (67571863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801d24f1c64e8ff688cf56f07e65e590a3411a4319de2413f5295128016e2e81`  
		Last Modified: Thu, 08 Jun 2023 16:19:58 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:14be62d2d889fda33654710ce8dc7f83a3f62d0d62b91f4439d6ce99ffa8791a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93050144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d49baedc236d4d7d75401808848130f850c4788b9f9f03167ccd8682ea73188`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:42:42 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:42:43 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 08 Jun 2023 16:39:24 GMT
ENV EMQX_VERSION=5.0.26
# Thu, 08 Jun 2023 16:39:24 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Thu, 08 Jun 2023 16:39:24 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Thu, 08 Jun 2023 16:39:24 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 08 Jun 2023 16:39:30 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 08 Jun 2023 16:39:30 GMT
WORKDIR /opt/emqx
# Thu, 08 Jun 2023 16:39:30 GMT
USER emqx
# Thu, 08 Jun 2023 16:39:30 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 08 Jun 2023 16:39:31 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 08 Jun 2023 16:39:31 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 08 Jun 2023 16:39:31 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 08 Jun 2023 16:39:31 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8345ceedc06f3b0ae12a8eb9f0f0e7dd52b3ae9800880811d86f7c26b0651446`  
		Last Modified: Tue, 23 May 2023 01:43:12 GMT  
		Size: 3.0 MB (3002990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b78e6c4890d65e6f6f17dbd7faa9d396eaad9d65dd2bbeb2e49aee524b18b1e`  
		Last Modified: Tue, 23 May 2023 01:43:11 GMT  
		Size: 4.1 KB (4115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0747c7d95e3a29e9a42c032ab9e7fd7a2f9a83887751923d8a1ba76ece60e0f6`  
		Last Modified: Thu, 08 Jun 2023 16:39:46 GMT  
		Size: 60.0 MB (59989387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5504f0bc88e3943acea76d78680ec89b99149c73ec33633ac1d1b47ac6c555f5`  
		Last Modified: Thu, 08 Jun 2023 16:39:40 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.26`

```console
$ docker pull emqx@sha256:b0fe72a44d77f7c0528aad08ca4a6d2aa125229308ab92bd9c627faa9ff4464e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0.26` - linux; amd64

```console
$ docker pull emqx@sha256:4d19a6cb422675146d37e55ea865dd48ed7f11f06ab01ac687cb8782372a470d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101968277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95a19311e1c3f696622ca62e69ddf194dd3609e7ad5a93054f23551d385dc8ff`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 08:24:00 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 08:24:01 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 08 Jun 2023 16:19:39 GMT
ENV EMQX_VERSION=5.0.26
# Thu, 08 Jun 2023 16:19:39 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Thu, 08 Jun 2023 16:19:39 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Thu, 08 Jun 2023 16:19:40 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 08 Jun 2023 16:19:46 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 08 Jun 2023 16:19:47 GMT
WORKDIR /opt/emqx
# Thu, 08 Jun 2023 16:19:47 GMT
USER emqx
# Thu, 08 Jun 2023 16:19:47 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 08 Jun 2023 16:19:47 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 08 Jun 2023 16:19:47 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 08 Jun 2023 16:19:47 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 08 Jun 2023 16:19:47 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ce7ad79b255e788cff6cef738579e0bbf7797cb46293052c0dac256ec5cce9`  
		Last Modified: Tue, 23 May 2023 08:24:36 GMT  
		Size: 3.0 MB (2987806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7beaac16821c81034b9f18e03825f60acf03fbd723d44a9650179d3059bc25`  
		Last Modified: Tue, 23 May 2023 08:24:35 GMT  
		Size: 4.1 KB (4119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575f38e8e71d018e527d06b05a4425cf58acc4265e53f203cb15f7643d99791e`  
		Last Modified: Thu, 08 Jun 2023 16:20:05 GMT  
		Size: 67.6 MB (67571863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801d24f1c64e8ff688cf56f07e65e590a3411a4319de2413f5295128016e2e81`  
		Last Modified: Thu, 08 Jun 2023 16:19:58 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0.26` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:14be62d2d889fda33654710ce8dc7f83a3f62d0d62b91f4439d6ce99ffa8791a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93050144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d49baedc236d4d7d75401808848130f850c4788b9f9f03167ccd8682ea73188`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:42:42 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:42:43 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 08 Jun 2023 16:39:24 GMT
ENV EMQX_VERSION=5.0.26
# Thu, 08 Jun 2023 16:39:24 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Thu, 08 Jun 2023 16:39:24 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Thu, 08 Jun 2023 16:39:24 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 08 Jun 2023 16:39:30 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 08 Jun 2023 16:39:30 GMT
WORKDIR /opt/emqx
# Thu, 08 Jun 2023 16:39:30 GMT
USER emqx
# Thu, 08 Jun 2023 16:39:30 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 08 Jun 2023 16:39:31 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 08 Jun 2023 16:39:31 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 08 Jun 2023 16:39:31 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 08 Jun 2023 16:39:31 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8345ceedc06f3b0ae12a8eb9f0f0e7dd52b3ae9800880811d86f7c26b0651446`  
		Last Modified: Tue, 23 May 2023 01:43:12 GMT  
		Size: 3.0 MB (3002990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b78e6c4890d65e6f6f17dbd7faa9d396eaad9d65dd2bbeb2e49aee524b18b1e`  
		Last Modified: Tue, 23 May 2023 01:43:11 GMT  
		Size: 4.1 KB (4115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0747c7d95e3a29e9a42c032ab9e7fd7a2f9a83887751923d8a1ba76ece60e0f6`  
		Last Modified: Thu, 08 Jun 2023 16:39:46 GMT  
		Size: 60.0 MB (59989387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5504f0bc88e3943acea76d78680ec89b99149c73ec33633ac1d1b47ac6c555f5`  
		Last Modified: Thu, 08 Jun 2023 16:39:40 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:b0fe72a44d77f7c0528aad08ca4a6d2aa125229308ab92bd9c627faa9ff4464e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:4d19a6cb422675146d37e55ea865dd48ed7f11f06ab01ac687cb8782372a470d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101968277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95a19311e1c3f696622ca62e69ddf194dd3609e7ad5a93054f23551d385dc8ff`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 08:24:00 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 08:24:01 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 08 Jun 2023 16:19:39 GMT
ENV EMQX_VERSION=5.0.26
# Thu, 08 Jun 2023 16:19:39 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Thu, 08 Jun 2023 16:19:39 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Thu, 08 Jun 2023 16:19:40 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 08 Jun 2023 16:19:46 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 08 Jun 2023 16:19:47 GMT
WORKDIR /opt/emqx
# Thu, 08 Jun 2023 16:19:47 GMT
USER emqx
# Thu, 08 Jun 2023 16:19:47 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 08 Jun 2023 16:19:47 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 08 Jun 2023 16:19:47 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 08 Jun 2023 16:19:47 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 08 Jun 2023 16:19:47 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ce7ad79b255e788cff6cef738579e0bbf7797cb46293052c0dac256ec5cce9`  
		Last Modified: Tue, 23 May 2023 08:24:36 GMT  
		Size: 3.0 MB (2987806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7beaac16821c81034b9f18e03825f60acf03fbd723d44a9650179d3059bc25`  
		Last Modified: Tue, 23 May 2023 08:24:35 GMT  
		Size: 4.1 KB (4119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575f38e8e71d018e527d06b05a4425cf58acc4265e53f203cb15f7643d99791e`  
		Last Modified: Thu, 08 Jun 2023 16:20:05 GMT  
		Size: 67.6 MB (67571863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801d24f1c64e8ff688cf56f07e65e590a3411a4319de2413f5295128016e2e81`  
		Last Modified: Thu, 08 Jun 2023 16:19:58 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:14be62d2d889fda33654710ce8dc7f83a3f62d0d62b91f4439d6ce99ffa8791a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93050144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d49baedc236d4d7d75401808848130f850c4788b9f9f03167ccd8682ea73188`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:42:42 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:42:43 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 08 Jun 2023 16:39:24 GMT
ENV EMQX_VERSION=5.0.26
# Thu, 08 Jun 2023 16:39:24 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Thu, 08 Jun 2023 16:39:24 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Thu, 08 Jun 2023 16:39:24 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 08 Jun 2023 16:39:30 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 08 Jun 2023 16:39:30 GMT
WORKDIR /opt/emqx
# Thu, 08 Jun 2023 16:39:30 GMT
USER emqx
# Thu, 08 Jun 2023 16:39:30 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 08 Jun 2023 16:39:31 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 08 Jun 2023 16:39:31 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 08 Jun 2023 16:39:31 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 08 Jun 2023 16:39:31 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8345ceedc06f3b0ae12a8eb9f0f0e7dd52b3ae9800880811d86f7c26b0651446`  
		Last Modified: Tue, 23 May 2023 01:43:12 GMT  
		Size: 3.0 MB (3002990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b78e6c4890d65e6f6f17dbd7faa9d396eaad9d65dd2bbeb2e49aee524b18b1e`  
		Last Modified: Tue, 23 May 2023 01:43:11 GMT  
		Size: 4.1 KB (4115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0747c7d95e3a29e9a42c032ab9e7fd7a2f9a83887751923d8a1ba76ece60e0f6`  
		Last Modified: Thu, 08 Jun 2023 16:39:46 GMT  
		Size: 60.0 MB (59989387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5504f0bc88e3943acea76d78680ec89b99149c73ec33633ac1d1b47ac6c555f5`  
		Last Modified: Thu, 08 Jun 2023 16:39:40 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
