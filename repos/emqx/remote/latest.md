## `emqx:latest`

```console
$ docker pull emqx@sha256:2390698531e0b77819a2e3baaaab4685e62c71c0c477f12e6912ac08afe48c91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:1697b5f83de3d17e0e80cc0e3295d544b9b0f19b9984658041c09d272ff7dec2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110336604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b6dd453854b320728b40a0cfda36571c5b46ccb383c848439a1050553598a3`
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
# Tue, 23 May 2023 08:24:01 GMT
ENV EMQX_VERSION=5.0.24
# Tue, 23 May 2023 08:24:01 GMT
ENV AMD64_SHA256=d104bc3e1839447f5ceeaadbb3feb6c604c5f74b07ca33ab4c37baf2a9b33ae3
# Tue, 23 May 2023 08:24:01 GMT
ENV ARM64_SHA256=40d387b7d4dfc4aa7162ef628f25bcb33e8a3fc67740b3cdb5a6d843aa87c2ec
# Tue, 23 May 2023 08:24:01 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 23 May 2023 08:24:08 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 23 May 2023 08:24:09 GMT
WORKDIR /opt/emqx
# Tue, 23 May 2023 08:24:09 GMT
USER emqx
# Tue, 23 May 2023 08:24:09 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 23 May 2023 08:24:09 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 23 May 2023 08:24:09 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 23 May 2023 08:24:09 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 23 May 2023 08:24:09 GMT
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
	-	`sha256:53691f33c7296085eae018fe463c1a965bc73ca9698d36ec12091cea59fcd3aa`  
		Last Modified: Tue, 23 May 2023 08:24:43 GMT  
		Size: 75.9 MB (75940191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ebadc979bbb9d556755b9d7548864dcd109403eed90da383743546fc152574`  
		Last Modified: Tue, 23 May 2023 08:24:35 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:6e814162a881a076c095cd9780167b8742a18bd46afd2ecc0e3f0c019f194549
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.4 MB (101420925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39a249e8111403d80b28441f004ac7b3b9a576fcbe337c24b09595e9c3993d50`
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
# Tue, 23 May 2023 01:42:43 GMT
ENV EMQX_VERSION=5.0.24
# Tue, 23 May 2023 01:42:43 GMT
ENV AMD64_SHA256=d104bc3e1839447f5ceeaadbb3feb6c604c5f74b07ca33ab4c37baf2a9b33ae3
# Tue, 23 May 2023 01:42:43 GMT
ENV ARM64_SHA256=40d387b7d4dfc4aa7162ef628f25bcb33e8a3fc67740b3cdb5a6d843aa87c2ec
# Tue, 23 May 2023 01:42:43 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 23 May 2023 01:42:48 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 23 May 2023 01:42:49 GMT
WORKDIR /opt/emqx
# Tue, 23 May 2023 01:42:49 GMT
USER emqx
# Tue, 23 May 2023 01:42:49 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 23 May 2023 01:42:49 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 23 May 2023 01:42:49 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 23 May 2023 01:42:49 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 23 May 2023 01:42:50 GMT
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
	-	`sha256:3f3928ab53fc1ed36f55e43718a8e82fdc4b572ff52ec108e1cc737d144d1f63`  
		Last Modified: Tue, 23 May 2023 01:43:18 GMT  
		Size: 68.4 MB (68360170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7629c5a6040608e24f6cca4a4a2dd9e31e4baa54d425e39557dc3c38d6204758`  
		Last Modified: Tue, 23 May 2023 01:43:15 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
