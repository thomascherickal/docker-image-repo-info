## `emqx:latest`

```console
$ docker pull emqx@sha256:601c82ac0495ad758003d337c90c4f2cf408c4e85c995e611344b081c09c02c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:7d87307488a966746ab49e68e98eb65517db733af54cf209a6d927cb7648d941
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100346619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56505e666d708b81be558f0c7e2ed02b77138943b147fa9eb226ce895ec0151`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:08:45 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:08:46 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 09 Feb 2023 10:08:46 GMT
ENV EMQX_VERSION=5.0.16
# Thu, 09 Feb 2023 10:08:46 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Thu, 09 Feb 2023 10:08:46 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Thu, 09 Feb 2023 10:08:46 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 09 Feb 2023 10:08:58 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 09 Feb 2023 10:08:58 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 10:08:58 GMT
USER emqx
# Thu, 09 Feb 2023 10:08:59 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 10:08:59 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 09 Feb 2023 10:08:59 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 09 Feb 2023 10:08:59 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 10:08:59 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc09b4c23409fc6e30f1f0933f0f2c6bd9d7a6566ed0054cb6583015adff6a07`  
		Last Modified: Thu, 09 Feb 2023 10:09:44 GMT  
		Size: 3.0 MB (2987646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5690e645d1f946b924e8d76142ecfdece6e52665554c1a7e613091d6885878`  
		Last Modified: Thu, 09 Feb 2023 10:09:43 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8d953ea948855c1f2fb3f57b7d7c23e9736c453bad99369844efe4dc499ffd`  
		Last Modified: Thu, 09 Feb 2023 10:09:51 GMT  
		Size: 65.9 MB (65942145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5687a1533ec033755e06b7c820a08146f8677a51fee7416c28de93a5f31ae6d5`  
		Last Modified: Thu, 09 Feb 2023 10:09:43 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:34ca0ce3077d1e2d1d46e231a442ea68b8f8b695a08f3278c39538fe54ea25c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91443872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dbae1937e6637a793bdc65e2d083cd920472c28c6e242b811a8921b05d6d108`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:41:00 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:41:01 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 09 Feb 2023 09:41:01 GMT
ENV EMQX_VERSION=5.0.16
# Thu, 09 Feb 2023 09:41:01 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Thu, 09 Feb 2023 09:41:01 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Thu, 09 Feb 2023 09:41:01 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 09 Feb 2023 09:41:06 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 09 Feb 2023 09:41:07 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 09:41:07 GMT
USER emqx
# Thu, 09 Feb 2023 09:41:07 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 09:41:07 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 09 Feb 2023 09:41:07 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 09 Feb 2023 09:41:07 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:41:07 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5394f2f4b016df4b79fc515dbf7cd492b3dbe93b959baf39817d26676ae083`  
		Last Modified: Thu, 09 Feb 2023 09:41:48 GMT  
		Size: 3.0 MB (3002749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def267c4d834a0cd84dd88a877e1c746c0a38d9d4b39043b22f599b1a6b9e6b9`  
		Last Modified: Thu, 09 Feb 2023 09:41:47 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f45e39fe16597c4cd113c4c6390cec4adadb72279e5937cfd5ebf925d3f50d`  
		Last Modified: Thu, 09 Feb 2023 09:41:55 GMT  
		Size: 58.4 MB (58373594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0b8c7e3854a4c45110a7bac48de29bb922a8660f7d4ed1855ce44364cdff81`  
		Last Modified: Thu, 09 Feb 2023 09:41:47 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
