## `emqx:latest`

```console
$ docker pull emqx@sha256:5fd23424e47c38bbeda099da995af702ffd718b8d5bff67468976429a819f06a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:195b3c618454faa76d6f5029b0881bb36a7f9e2e8323db8cbdf95d125dfea4ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.1 MB (100081734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cedbe39026299ae846576795162dcfe1df7723be15fd45291faa0d0676d57ad8`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:04:14 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 15 Dec 2022 18:25:47 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 15 Dec 2022 18:25:47 GMT
ENV EMQX_VERSION=5.0.12
# Thu, 15 Dec 2022 18:25:47 GMT
ENV AMD64_SHA256=c137284b389c472f3c2563bc89c8016f5ce9bdb0acf820014afcbbb26a0e81e7
# Thu, 15 Dec 2022 18:25:47 GMT
ENV ARM64_SHA256=5925bb5462d6f163b829c2f1e6490dc5a46e445b5b15c268482bb7310a95f7c4
# Thu, 15 Dec 2022 18:25:47 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 15 Dec 2022 18:25:54 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 15 Dec 2022 18:25:54 GMT
WORKDIR /opt/emqx
# Thu, 15 Dec 2022 18:25:55 GMT
USER emqx
# Thu, 15 Dec 2022 18:25:55 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 15 Dec 2022 18:25:55 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 15 Dec 2022 18:25:55 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 15 Dec 2022 18:25:55 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 15 Dec 2022 18:25:55 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29e5e20fa16580fcb41964870e6c9d3d48072cc1abdbe98fe1645a15c65e9ec`  
		Last Modified: Tue, 06 Dec 2022 04:05:16 GMT  
		Size: 3.0 MB (2988935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca86891f342dfb918e69e1d9909f9489c716b4a0630d00eda5b7da3f0a6faa5`  
		Last Modified: Thu, 15 Dec 2022 18:26:14 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f6fe23c2dfc1f380e42d68c9d8b4d65d15c575ff56f417418c8026e5064b4d`  
		Last Modified: Thu, 15 Dec 2022 18:26:21 GMT  
		Size: 65.7 MB (65674930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c672a158b261dc7c7cccce4017aa3b1a59a62e8d94e72c5e1762340198a9a7`  
		Last Modified: Thu, 15 Dec 2022 18:26:14 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:ff42c1d34ff7bc2546e9533755afb5346971443964d2105bd0a412affb8e7c06
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.8 MB (147767024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0bf741af4a3cb7568ee0a2901b493ba51354c94de68beb92d06e3e6bc97e5a8`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 10:51:04 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 10:51:04 GMT
ENV EMQX_VERSION=5.0.11
# Tue, 06 Dec 2022 10:51:04 GMT
ENV AMD64_SHA256=68609fcc1d74be917f9c28c57c14daabccee22361af91b6e98812a35300a1c80
# Tue, 06 Dec 2022 10:51:04 GMT
ENV ARM64_SHA256=f7c7417951beb490ed3a7347b3879db8e9e80ea214c9ef942e777c7136681d31
# Tue, 06 Dec 2022 10:51:05 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 06 Dec 2022 10:51:09 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Tue, 06 Dec 2022 10:51:09 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 06 Dec 2022 10:51:09 GMT
WORKDIR /opt/emqx
# Tue, 06 Dec 2022 10:51:14 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 06 Dec 2022 10:51:14 GMT
USER emqx
# Tue, 06 Dec 2022 10:51:14 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 06 Dec 2022 10:51:15 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 06 Dec 2022 10:51:15 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 10:51:15 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0384cd65a949b2d9a9f07a689377a09c1c0180066afbebd1aec5b7a8ff60655d`  
		Last Modified: Tue, 06 Dec 2022 10:51:56 GMT  
		Size: 3.0 MB (3004192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9cc25503198e3e8751ac2fab811ff7ec5016530c3d0831de39629cd82a7883`  
		Last Modified: Tue, 06 Dec 2022 10:52:02 GMT  
		Size: 57.3 MB (57348552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4bcb2bff5ab040d41282cf08712f8ab3cf03d6802309182711c26ccc029a9b`  
		Last Modified: Tue, 06 Dec 2022 10:51:56 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36441e61b498fd1d2bab1938dbd755c69c1b8171dff2c56e831d9c472a5e3fc3`  
		Last Modified: Tue, 06 Dec 2022 10:52:02 GMT  
		Size: 57.4 MB (57353058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
