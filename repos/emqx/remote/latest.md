## `emqx:latest`

```console
$ docker pull emqx@sha256:249d45407c52d762189247784d8b978f58e047a9467f90a193428fb70fcbed76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:e47766659078d916ccc036677b18c4e8b7925282879f3bcfa15bc2f53bfd6c9a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.1 MB (100088218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07b7938e576e8da7f925339ae7b75d040acfff5f138dcd233dd32ecdf7740ba8`
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
# Thu, 29 Dec 2022 16:19:38 GMT
ENV EMQX_VERSION=5.0.13
# Thu, 29 Dec 2022 16:19:38 GMT
ENV AMD64_SHA256=d52ea9a5c07cb31106f3bb7ac541a269ce205a6d1c9d847d7fe01ad39da0b1a4
# Thu, 29 Dec 2022 16:19:38 GMT
ENV ARM64_SHA256=5f02e38b6fbd07c23455890a59b041f8d91fcceeeaedaec090435f913927538e
# Thu, 29 Dec 2022 16:19:38 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 29 Dec 2022 16:19:44 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 29 Dec 2022 16:19:45 GMT
WORKDIR /opt/emqx
# Thu, 29 Dec 2022 16:19:45 GMT
USER emqx
# Thu, 29 Dec 2022 16:19:45 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 29 Dec 2022 16:19:45 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 29 Dec 2022 16:19:45 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 29 Dec 2022 16:19:45 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 29 Dec 2022 16:19:45 GMT
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
	-	`sha256:271a21361cb43bd987ad50a1b867da6430318c1e32c6a7e8e68bdc4d7ad85696`  
		Last Modified: Thu, 29 Dec 2022 16:20:11 GMT  
		Size: 65.7 MB (65698558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f988f1e34dde69c964f23379fcf8c423d25e5b0cb0ba5357397ddf83755930`  
		Last Modified: Thu, 29 Dec 2022 16:20:03 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:125987045f6ce0032de67377df4526dfd98fd952f4cf7d6acf74c40cde2d5cbf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91182859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cb848811cfcb263f6b942d143b5b29676b99cf6c3b5f507d547e69d5665cd08`
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
# Thu, 29 Dec 2022 16:47:27 GMT
ENV EMQX_VERSION=5.0.13
# Thu, 29 Dec 2022 16:47:28 GMT
ENV AMD64_SHA256=d52ea9a5c07cb31106f3bb7ac541a269ce205a6d1c9d847d7fe01ad39da0b1a4
# Thu, 29 Dec 2022 16:47:28 GMT
ENV ARM64_SHA256=5f02e38b6fbd07c23455890a59b041f8d91fcceeeaedaec090435f913927538e
# Thu, 29 Dec 2022 16:47:28 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 29 Dec 2022 16:47:32 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 29 Dec 2022 16:47:33 GMT
WORKDIR /opt/emqx
# Thu, 29 Dec 2022 16:47:33 GMT
USER emqx
# Thu, 29 Dec 2022 16:47:33 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 29 Dec 2022 16:47:33 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 29 Dec 2022 16:47:33 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 29 Dec 2022 16:47:33 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 29 Dec 2022 16:47:33 GMT
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
	-	`sha256:25c10bc5c21d8d6d12621e7d39ce31f1962f258ddcafa714ac13754b5a741476`  
		Last Modified: Thu, 29 Dec 2022 16:47:57 GMT  
		Size: 58.1 MB (58130393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd957cd7da661a6bf4d762dac3c8ad42c3a7467d98d94c5582e8476e652195a`  
		Last Modified: Thu, 29 Dec 2022 16:47:51 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
