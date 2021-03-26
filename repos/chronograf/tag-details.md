<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `chronograf`

-	[`chronograf:1.6`](#chronograf16)
-	[`chronograf:1.6-alpine`](#chronograf16-alpine)
-	[`chronograf:1.6.2`](#chronograf162)
-	[`chronograf:1.6.2-alpine`](#chronograf162-alpine)
-	[`chronograf:1.7`](#chronograf17)
-	[`chronograf:1.7-alpine`](#chronograf17-alpine)
-	[`chronograf:1.7.17`](#chronograf1717)
-	[`chronograf:1.7.17-alpine`](#chronograf1717-alpine)
-	[`chronograf:1.8`](#chronograf18)
-	[`chronograf:1.8-alpine`](#chronograf18-alpine)
-	[`chronograf:1.8.8`](#chronograf188)
-	[`chronograf:1.8.8-alpine`](#chronograf188-alpine)
-	[`chronograf:alpine`](#chronografalpine)
-	[`chronograf:latest`](#chronograflatest)

## `chronograf:1.6`

```console
$ docker pull chronograf@sha256:ee7523be0cdb135662d73cfa6c5f804a73d096a3259cf367cf29b67200957997
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6` - linux; amd64

```console
$ docker pull chronograf@sha256:eabc55bd7ec9958d7ae26b40f8e9dad2ba8daec0c937e91ae1c79cae54c1b7c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49341970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53431b64749f0083c5aace2dfc6f6208cae94d4877c61c262a05ceb79f030a2d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 02:22:47 GMT
ADD file:1d706af4169332956a23f3faa02754cb503003812cc1d43ad9b2448f7c26f431 in / 
# Fri, 12 Mar 2021 02:22:48 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:37:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 03:37:28 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 12 Mar 2021 03:37:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 03:37:41 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 03:37:42 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 03:37:42 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 03:37:43 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 03:37:43 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 03:37:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 03:37:44 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a4feded82f54dd43cb68930d190cb6715378fa2aca3ecce0bcac959359f58d2f`  
		Last Modified: Fri, 12 Mar 2021 02:30:28 GMT  
		Size: 22.5 MB (22528907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5784273a6633bf2240f20b7dcdae41732461704080ea64a01135f933f93c0592`  
		Last Modified: Fri, 12 Mar 2021 03:39:37 GMT  
		Size: 6.7 MB (6744499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8bc994eb7d6154adec48f567d04a7d350afa400f59df2edeb73dfb371bac70`  
		Last Modified: Fri, 12 Mar 2021 03:39:39 GMT  
		Size: 20.0 MB (20044170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0e7ed5a15b6d69feb48f9eb1d8677b594a7e5ed2b631a02eb5f1f851aa6bba`  
		Last Modified: Fri, 12 Mar 2021 03:39:34 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd1887c3d4b1c3c79df03dd513d5f44307f2ec19aa123ed2da3837b97a676ca`  
		Last Modified: Fri, 12 Mar 2021 03:39:34 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11381fd679f02ead0309d69239f246b93124a92b47c4635bcd48c121ff45d3a`  
		Last Modified: Fri, 12 Mar 2021 03:39:35 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:65b7a97dcfba62127d49e5806868e09f8964730905b39b13377dcdea789bfbb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43922670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6961fbccd59945162dde68cb4439d5b8d30db9b7404b1cf140d207c98ecd02f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 02:05:43 GMT
ADD file:37f1c27246cb6d0d42be6f807f54c620cc083043d7395656a56178df89e5d6d9 in / 
# Fri, 12 Mar 2021 02:05:45 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:23:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 03:23:32 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 12 Mar 2021 03:23:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 03:23:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 03:23:51 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 03:23:52 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 03:23:53 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 03:23:54 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 03:23:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 03:23:55 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:61211de2ba721a5e516c346a68bf2ae409d80525a872c3ad47ccefce648dc07c`  
		Last Modified: Fri, 12 Mar 2021 02:14:31 GMT  
		Size: 19.3 MB (19316567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81289d47720c1e0503331a7afcf4b884bc489014ea7cae2bba6244f9a10882bd`  
		Last Modified: Fri, 12 Mar 2021 03:25:57 GMT  
		Size: 5.8 MB (5765215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f825f16688fdb957d14042a54cec28c5cf84095b8a9d1005186dddfc202847b6`  
		Last Modified: Fri, 12 Mar 2021 03:26:03 GMT  
		Size: 18.8 MB (18816490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f322a521fb80ed3850fb7679caa7f57a287b485f826e82cb59952cd3e358682`  
		Last Modified: Fri, 12 Mar 2021 03:25:56 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b956a35d2432ef8641b5589e2f4cb59b5ccce1917ad56056872cc38df22150`  
		Last Modified: Fri, 12 Mar 2021 03:25:56 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a9687662fed4cfd77c48c2140537d64b00554781e5cb3bae625d5495598633`  
		Last Modified: Fri, 12 Mar 2021 03:25:55 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:98ee086dee6cf597158569cc06d0a2d1eafc277bd682c33096fa0063f10c6d85
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45400632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fff277fd1ab6c12f5d6cc64358d9077d0cd02d365ac905fb38828951508ac9f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 01:57:19 GMT
ADD file:cd70de3ff9dab2f20378f87a36ca54171a79fde726291a9c5c7eae7b5435cfa2 in / 
# Fri, 12 Mar 2021 01:57:20 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:48:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 02:48:31 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 12 Mar 2021 02:48:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 02:48:46 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 02:48:47 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 02:48:48 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 02:48:49 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 02:48:49 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 02:48:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 02:48:51 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9cb8532b12b699d7151babb99e22315d94bfbf317f3c1db01c532a61fc38a748`  
		Last Modified: Fri, 12 Mar 2021 02:04:16 GMT  
		Size: 20.4 MB (20389391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b0ca74c9f3b67abeb6c8251b912c45335d11e252375188570d0ee2db5777cbc`  
		Last Modified: Fri, 12 Mar 2021 02:50:36 GMT  
		Size: 6.0 MB (6028358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ba11827fdb86a1b7aedd951449e87b4fd2ce9208a39408356f6ace2d205287`  
		Last Modified: Fri, 12 Mar 2021 02:50:40 GMT  
		Size: 19.0 MB (18958484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31538cf8ddfaf6b03217987e1f1420015b5890c9e811c20404b60731934c116f`  
		Last Modified: Fri, 12 Mar 2021 02:50:35 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6594e175e8dd7c7894b582e5ca28950207a902aa85e6d6e59b96738b334b3cd8`  
		Last Modified: Fri, 12 Mar 2021 02:50:35 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419f123a4abfacf79bbc19a1a4248d6d716d33c3e1b09b5dc18756f2a351a087`  
		Last Modified: Fri, 12 Mar 2021 02:50:35 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6-alpine`

```console
$ docker pull chronograf@sha256:865641b1f7a0ec7d2eacdd0431132ce8d4a96e648d5981193f3ae8f31b337a90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.6-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:f0aebf3a16b9438a5aeed9c108b0af42564477cee319bc062a088273af6076cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14841963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eedf76ed9ed86a8f5aaefa50c855fd386b31bd9b6f4b6451237a49024e863d4f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 02:40:44 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 02:40:45 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 26 Mar 2021 02:40:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 02:40:52 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 02:40:53 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 02:40:53 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 02:40:53 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 02:40:54 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 26 Mar 2021 02:40:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 02:40:55 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21f4fdff4d2de3741ff5301f2ca4d71dfb5041fbd5f4aa01cfd6823ac6693f9`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 280.9 KB (280877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db12e5ff56de26f4ed0958fb375c07c902515fdc8665f4a11b472c4b867bd856`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 11.7 MB (11736751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b555b8110c844c0e86847b84adf1bb0a942dfc22cbafc4eb9d3639170bb85e`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 12.3 KB (12277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f12381a23b90f4eeeaf431a6749c00bdd2b74ebf9af28c63c666f66980dbab`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554f1bb27bd5414c71fb0835174d5e9edf0cf37d1ec243753f036ec89833d9de`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2`

```console
$ docker pull chronograf@sha256:ee7523be0cdb135662d73cfa6c5f804a73d096a3259cf367cf29b67200957997
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.6.2` - linux; amd64

```console
$ docker pull chronograf@sha256:eabc55bd7ec9958d7ae26b40f8e9dad2ba8daec0c937e91ae1c79cae54c1b7c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49341970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53431b64749f0083c5aace2dfc6f6208cae94d4877c61c262a05ceb79f030a2d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 02:22:47 GMT
ADD file:1d706af4169332956a23f3faa02754cb503003812cc1d43ad9b2448f7c26f431 in / 
# Fri, 12 Mar 2021 02:22:48 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:37:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 03:37:28 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 12 Mar 2021 03:37:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 03:37:41 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 03:37:42 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 03:37:42 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 03:37:43 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 03:37:43 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 03:37:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 03:37:44 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a4feded82f54dd43cb68930d190cb6715378fa2aca3ecce0bcac959359f58d2f`  
		Last Modified: Fri, 12 Mar 2021 02:30:28 GMT  
		Size: 22.5 MB (22528907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5784273a6633bf2240f20b7dcdae41732461704080ea64a01135f933f93c0592`  
		Last Modified: Fri, 12 Mar 2021 03:39:37 GMT  
		Size: 6.7 MB (6744499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8bc994eb7d6154adec48f567d04a7d350afa400f59df2edeb73dfb371bac70`  
		Last Modified: Fri, 12 Mar 2021 03:39:39 GMT  
		Size: 20.0 MB (20044170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0e7ed5a15b6d69feb48f9eb1d8677b594a7e5ed2b631a02eb5f1f851aa6bba`  
		Last Modified: Fri, 12 Mar 2021 03:39:34 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd1887c3d4b1c3c79df03dd513d5f44307f2ec19aa123ed2da3837b97a676ca`  
		Last Modified: Fri, 12 Mar 2021 03:39:34 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11381fd679f02ead0309d69239f246b93124a92b47c4635bcd48c121ff45d3a`  
		Last Modified: Fri, 12 Mar 2021 03:39:35 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:65b7a97dcfba62127d49e5806868e09f8964730905b39b13377dcdea789bfbb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43922670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6961fbccd59945162dde68cb4439d5b8d30db9b7404b1cf140d207c98ecd02f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 02:05:43 GMT
ADD file:37f1c27246cb6d0d42be6f807f54c620cc083043d7395656a56178df89e5d6d9 in / 
# Fri, 12 Mar 2021 02:05:45 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:23:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 03:23:32 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 12 Mar 2021 03:23:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 03:23:51 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 03:23:51 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 03:23:52 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 03:23:53 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 03:23:54 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 03:23:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 03:23:55 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:61211de2ba721a5e516c346a68bf2ae409d80525a872c3ad47ccefce648dc07c`  
		Last Modified: Fri, 12 Mar 2021 02:14:31 GMT  
		Size: 19.3 MB (19316567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81289d47720c1e0503331a7afcf4b884bc489014ea7cae2bba6244f9a10882bd`  
		Last Modified: Fri, 12 Mar 2021 03:25:57 GMT  
		Size: 5.8 MB (5765215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f825f16688fdb957d14042a54cec28c5cf84095b8a9d1005186dddfc202847b6`  
		Last Modified: Fri, 12 Mar 2021 03:26:03 GMT  
		Size: 18.8 MB (18816490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f322a521fb80ed3850fb7679caa7f57a287b485f826e82cb59952cd3e358682`  
		Last Modified: Fri, 12 Mar 2021 03:25:56 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b956a35d2432ef8641b5589e2f4cb59b5ccce1917ad56056872cc38df22150`  
		Last Modified: Fri, 12 Mar 2021 03:25:56 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a9687662fed4cfd77c48c2140537d64b00554781e5cb3bae625d5495598633`  
		Last Modified: Fri, 12 Mar 2021 03:25:55 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.6.2` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:98ee086dee6cf597158569cc06d0a2d1eafc277bd682c33096fa0063f10c6d85
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45400632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fff277fd1ab6c12f5d6cc64358d9077d0cd02d365ac905fb38828951508ac9f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 01:57:19 GMT
ADD file:cd70de3ff9dab2f20378f87a36ca54171a79fde726291a9c5c7eae7b5435cfa2 in / 
# Fri, 12 Mar 2021 01:57:20 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:48:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 02:48:31 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 12 Mar 2021 02:48:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 02:48:46 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 02:48:47 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 02:48:48 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 02:48:49 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 02:48:49 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 02:48:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 02:48:51 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9cb8532b12b699d7151babb99e22315d94bfbf317f3c1db01c532a61fc38a748`  
		Last Modified: Fri, 12 Mar 2021 02:04:16 GMT  
		Size: 20.4 MB (20389391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b0ca74c9f3b67abeb6c8251b912c45335d11e252375188570d0ee2db5777cbc`  
		Last Modified: Fri, 12 Mar 2021 02:50:36 GMT  
		Size: 6.0 MB (6028358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ba11827fdb86a1b7aedd951449e87b4fd2ce9208a39408356f6ace2d205287`  
		Last Modified: Fri, 12 Mar 2021 02:50:40 GMT  
		Size: 19.0 MB (18958484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31538cf8ddfaf6b03217987e1f1420015b5890c9e811c20404b60731934c116f`  
		Last Modified: Fri, 12 Mar 2021 02:50:35 GMT  
		Size: 12.2 KB (12250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6594e175e8dd7c7894b582e5ca28950207a902aa85e6d6e59b96738b334b3cd8`  
		Last Modified: Fri, 12 Mar 2021 02:50:35 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419f123a4abfacf79bbc19a1a4248d6d716d33c3e1b09b5dc18756f2a351a087`  
		Last Modified: Fri, 12 Mar 2021 02:50:35 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.6.2-alpine`

```console
$ docker pull chronograf@sha256:865641b1f7a0ec7d2eacdd0431132ce8d4a96e648d5981193f3ae8f31b337a90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.6.2-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:f0aebf3a16b9438a5aeed9c108b0af42564477cee319bc062a088273af6076cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14841963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eedf76ed9ed86a8f5aaefa50c855fd386b31bd9b6f4b6451237a49024e863d4f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 02:40:44 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 02:40:45 GMT
ENV CHRONOGRAF_VERSION=1.6.2
# Fri, 26 Mar 2021 02:40:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 02:40:52 GMT
COPY file:aa4a9d01295c7013d89da92a943af071556aea6dbe6269affd4664fdd86969b8 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 02:40:53 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 02:40:53 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 02:40:53 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 02:40:54 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 26 Mar 2021 02:40:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 02:40:55 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21f4fdff4d2de3741ff5301f2ca4d71dfb5041fbd5f4aa01cfd6823ac6693f9`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 280.9 KB (280877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db12e5ff56de26f4ed0958fb375c07c902515fdc8665f4a11b472c4b867bd856`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 11.7 MB (11736751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b555b8110c844c0e86847b84adf1bb0a942dfc22cbafc4eb9d3639170bb85e`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 12.3 KB (12277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f12381a23b90f4eeeaf431a6749c00bdd2b74ebf9af28c63c666f66980dbab`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554f1bb27bd5414c71fb0835174d5e9edf0cf37d1ec243753f036ec89833d9de`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7`

```console
$ docker pull chronograf@sha256:c3e37e8a897ed426e797388a194024ada4aab55db4d82997c1a40d87e6cb81a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:d595764740ccb7c53f8928f462fc3cf09f033e3fc58ff0f647cabc8f4b9601de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65368772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38545687ea3290ba7d656dce6cbb18f86826a999e210d99e6ccf9e46307249b6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 02:22:47 GMT
ADD file:1d706af4169332956a23f3faa02754cb503003812cc1d43ad9b2448f7c26f431 in / 
# Fri, 12 Mar 2021 02:22:48 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:38:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 03:38:23 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 12 Mar 2021 03:38:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 03:38:35 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 03:38:35 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 03:38:35 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 03:38:36 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 03:38:36 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 03:38:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 03:38:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a4feded82f54dd43cb68930d190cb6715378fa2aca3ecce0bcac959359f58d2f`  
		Last Modified: Fri, 12 Mar 2021 02:30:28 GMT  
		Size: 22.5 MB (22528907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300e081e277c9b74f28933c9a25ef113d8fb6e64bc8ff01027f6fe8114193946`  
		Last Modified: Fri, 12 Mar 2021 03:40:03 GMT  
		Size: 4.5 MB (4505986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ae5a453be44e8af2583fa6462892e5318713cb14a5df5ad8a483db45411874`  
		Last Modified: Fri, 12 Mar 2021 03:40:10 GMT  
		Size: 38.3 MB (38309483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d5e43238a2f09ddb901ceb5be44de5428fc938af7aad2fe913a17d27a8fc0e`  
		Last Modified: Fri, 12 Mar 2021 03:40:01 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dee968df248c79ced4959479788e32928f9c2e417472a86c4ca3e2abeaf6643`  
		Last Modified: Fri, 12 Mar 2021 03:40:01 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad0b3fc52924062cd05cfef494f5db496e344d4c3dc219f9c2e3a21b451f388`  
		Last Modified: Fri, 12 Mar 2021 03:40:02 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:710ea877485e350a1d0028c63150f6090487f1f87b1a0852f7741756bea56c3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58973297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b75d4dcd6962de2a3af8aeec8d58cf9c60da4bf6c5cab4a61232a8655513af1a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 02:05:43 GMT
ADD file:37f1c27246cb6d0d42be6f807f54c620cc083043d7395656a56178df89e5d6d9 in / 
# Fri, 12 Mar 2021 02:05:45 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:24:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 03:24:23 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 12 Mar 2021 03:24:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 03:24:49 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 03:24:50 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 03:24:51 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 03:24:51 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 03:24:52 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 03:24:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 03:24:54 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:61211de2ba721a5e516c346a68bf2ae409d80525a872c3ad47ccefce648dc07c`  
		Last Modified: Fri, 12 Mar 2021 02:14:31 GMT  
		Size: 19.3 MB (19316567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717a1a0e3726ef8b17b1953bd044deeacec6d40f61da08e7d546439ffc9943e1`  
		Last Modified: Fri, 12 Mar 2021 03:26:12 GMT  
		Size: 3.9 MB (3879559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0639c578888126a369925d939d8ba98e637b41b69eea3068fd0049288a1a13`  
		Last Modified: Fri, 12 Mar 2021 03:26:23 GMT  
		Size: 35.8 MB (35752776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b48f00b7bfe2ffadc644672228562db0522fe3a278043ba0e047f3ea500ecc`  
		Last Modified: Fri, 12 Mar 2021 03:26:11 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d0a8cd1d649b6b9cea453bc69a1dcd875a95b9825447785f47dca99a2443b9`  
		Last Modified: Fri, 12 Mar 2021 03:26:11 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097a346b641ceea35a0ad717c9f7eadf1bbaa84e3f59fcabdca702624ba4dfd6`  
		Last Modified: Fri, 12 Mar 2021 03:26:11 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:ecec0a0db43695bb3a0909fb499e2f3fde1469f08796b94eebe3d4a5a02fe71f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60457937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96a67b2669aff68657bc32e23724ccb35593f23537ead878cb836cde2fcd3627`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 01:57:19 GMT
ADD file:cd70de3ff9dab2f20378f87a36ca54171a79fde726291a9c5c7eae7b5435cfa2 in / 
# Fri, 12 Mar 2021 01:57:20 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 02:49:16 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 12 Mar 2021 02:49:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 02:49:35 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 02:49:36 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 02:49:37 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 02:49:38 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 02:49:39 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 02:49:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 02:49:41 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9cb8532b12b699d7151babb99e22315d94bfbf317f3c1db01c532a61fc38a748`  
		Last Modified: Fri, 12 Mar 2021 02:04:16 GMT  
		Size: 20.4 MB (20389391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6b6f75f20b090ca56dcaef6e6f4b335808d763a90a94acf9877b64c6eb9b5`  
		Last Modified: Fri, 12 Mar 2021 02:50:48 GMT  
		Size: 4.1 MB (4082268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62dd44e9da376da6bac659b3d6d3429128b334db76917ea9a2d1dad9391c481f`  
		Last Modified: Fri, 12 Mar 2021 02:50:54 GMT  
		Size: 36.0 MB (35961890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6db7eb08ab5c88ff4c9cacb8ddaf7ce61de57b84c5b51887715131601974291`  
		Last Modified: Fri, 12 Mar 2021 02:50:46 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2820942f8e49016bd6b2b42213dd80c154b62ac4b54be9d8c7ab90607ed6b316`  
		Last Modified: Fri, 12 Mar 2021 02:50:46 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433571f7e633a08e44103b592c6d9fa1b875604f92704beb74f4da50e0919832`  
		Last Modified: Fri, 12 Mar 2021 02:50:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:2c763ee4efeabcda89d91708e177111bb459c3c4e2174ad697c671d780eec2f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.7-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:428e98a9f624def380648c24e4ab802f136b56e81459119580b83855902bf989
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22660462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7abe0632a70257e96d02ebf9c0f8f779291d0eaae40a5d32bbffb313658b2119`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 02:40:44 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 02:41:04 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 26 Mar 2021 02:41:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 02:41:12 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 02:41:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 02:41:13 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 02:41:14 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 02:41:14 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 26 Mar 2021 02:41:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 02:41:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21f4fdff4d2de3741ff5301f2ca4d71dfb5041fbd5f4aa01cfd6823ac6693f9`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 280.9 KB (280877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8347978863206fd815b2a3bb0be789f20244679d01952c7cf99a2b62f26e50`  
		Last Modified: Fri, 26 Mar 2021 02:42:27 GMT  
		Size: 19.6 MB (19555255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83be8e29182aea4959f986a45df5392775825ead1857be98fec722452d59eb7`  
		Last Modified: Fri, 26 Mar 2021 02:42:23 GMT  
		Size: 12.3 KB (12272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bba321eed11d28f7c89bf86c98104bfe62a8bdb233953efb77cda61c4b0304`  
		Last Modified: Fri, 26 Mar 2021 02:42:22 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7060062a0a29d0380f03a272669a9230258bab2dfa7df2d7d90bce2c3f60d60d`  
		Last Modified: Fri, 26 Mar 2021 02:42:22 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17`

```console
$ docker pull chronograf@sha256:c3e37e8a897ed426e797388a194024ada4aab55db4d82997c1a40d87e6cb81a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:d595764740ccb7c53f8928f462fc3cf09f033e3fc58ff0f647cabc8f4b9601de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65368772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38545687ea3290ba7d656dce6cbb18f86826a999e210d99e6ccf9e46307249b6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 02:22:47 GMT
ADD file:1d706af4169332956a23f3faa02754cb503003812cc1d43ad9b2448f7c26f431 in / 
# Fri, 12 Mar 2021 02:22:48 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:38:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 03:38:23 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 12 Mar 2021 03:38:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 03:38:35 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 03:38:35 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 03:38:35 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 03:38:36 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 03:38:36 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 03:38:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 03:38:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a4feded82f54dd43cb68930d190cb6715378fa2aca3ecce0bcac959359f58d2f`  
		Last Modified: Fri, 12 Mar 2021 02:30:28 GMT  
		Size: 22.5 MB (22528907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300e081e277c9b74f28933c9a25ef113d8fb6e64bc8ff01027f6fe8114193946`  
		Last Modified: Fri, 12 Mar 2021 03:40:03 GMT  
		Size: 4.5 MB (4505986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ae5a453be44e8af2583fa6462892e5318713cb14a5df5ad8a483db45411874`  
		Last Modified: Fri, 12 Mar 2021 03:40:10 GMT  
		Size: 38.3 MB (38309483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d5e43238a2f09ddb901ceb5be44de5428fc938af7aad2fe913a17d27a8fc0e`  
		Last Modified: Fri, 12 Mar 2021 03:40:01 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dee968df248c79ced4959479788e32928f9c2e417472a86c4ca3e2abeaf6643`  
		Last Modified: Fri, 12 Mar 2021 03:40:01 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad0b3fc52924062cd05cfef494f5db496e344d4c3dc219f9c2e3a21b451f388`  
		Last Modified: Fri, 12 Mar 2021 03:40:02 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:710ea877485e350a1d0028c63150f6090487f1f87b1a0852f7741756bea56c3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58973297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b75d4dcd6962de2a3af8aeec8d58cf9c60da4bf6c5cab4a61232a8655513af1a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 02:05:43 GMT
ADD file:37f1c27246cb6d0d42be6f807f54c620cc083043d7395656a56178df89e5d6d9 in / 
# Fri, 12 Mar 2021 02:05:45 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:24:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 03:24:23 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 12 Mar 2021 03:24:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 03:24:49 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 03:24:50 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 03:24:51 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 03:24:51 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 03:24:52 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 03:24:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 03:24:54 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:61211de2ba721a5e516c346a68bf2ae409d80525a872c3ad47ccefce648dc07c`  
		Last Modified: Fri, 12 Mar 2021 02:14:31 GMT  
		Size: 19.3 MB (19316567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717a1a0e3726ef8b17b1953bd044deeacec6d40f61da08e7d546439ffc9943e1`  
		Last Modified: Fri, 12 Mar 2021 03:26:12 GMT  
		Size: 3.9 MB (3879559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0639c578888126a369925d939d8ba98e637b41b69eea3068fd0049288a1a13`  
		Last Modified: Fri, 12 Mar 2021 03:26:23 GMT  
		Size: 35.8 MB (35752776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b48f00b7bfe2ffadc644672228562db0522fe3a278043ba0e047f3ea500ecc`  
		Last Modified: Fri, 12 Mar 2021 03:26:11 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d0a8cd1d649b6b9cea453bc69a1dcd875a95b9825447785f47dca99a2443b9`  
		Last Modified: Fri, 12 Mar 2021 03:26:11 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097a346b641ceea35a0ad717c9f7eadf1bbaa84e3f59fcabdca702624ba4dfd6`  
		Last Modified: Fri, 12 Mar 2021 03:26:11 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:ecec0a0db43695bb3a0909fb499e2f3fde1469f08796b94eebe3d4a5a02fe71f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60457937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96a67b2669aff68657bc32e23724ccb35593f23537ead878cb836cde2fcd3627`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 01:57:19 GMT
ADD file:cd70de3ff9dab2f20378f87a36ca54171a79fde726291a9c5c7eae7b5435cfa2 in / 
# Fri, 12 Mar 2021 01:57:20 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 02:49:16 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 12 Mar 2021 02:49:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 02:49:35 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 02:49:36 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 02:49:37 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 02:49:38 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 02:49:39 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 02:49:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 02:49:41 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9cb8532b12b699d7151babb99e22315d94bfbf317f3c1db01c532a61fc38a748`  
		Last Modified: Fri, 12 Mar 2021 02:04:16 GMT  
		Size: 20.4 MB (20389391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6b6f75f20b090ca56dcaef6e6f4b335808d763a90a94acf9877b64c6eb9b5`  
		Last Modified: Fri, 12 Mar 2021 02:50:48 GMT  
		Size: 4.1 MB (4082268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62dd44e9da376da6bac659b3d6d3429128b334db76917ea9a2d1dad9391c481f`  
		Last Modified: Fri, 12 Mar 2021 02:50:54 GMT  
		Size: 36.0 MB (35961890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6db7eb08ab5c88ff4c9cacb8ddaf7ce61de57b84c5b51887715131601974291`  
		Last Modified: Fri, 12 Mar 2021 02:50:46 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2820942f8e49016bd6b2b42213dd80c154b62ac4b54be9d8c7ab90607ed6b316`  
		Last Modified: Fri, 12 Mar 2021 02:50:46 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433571f7e633a08e44103b592c6d9fa1b875604f92704beb74f4da50e0919832`  
		Last Modified: Fri, 12 Mar 2021 02:50:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17-alpine`

```console
$ docker pull chronograf@sha256:2c763ee4efeabcda89d91708e177111bb459c3c4e2174ad697c671d780eec2f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.7.17-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:428e98a9f624def380648c24e4ab802f136b56e81459119580b83855902bf989
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22660462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7abe0632a70257e96d02ebf9c0f8f779291d0eaae40a5d32bbffb313658b2119`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 02:40:44 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 02:41:04 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Fri, 26 Mar 2021 02:41:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 02:41:12 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 02:41:13 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 02:41:13 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 02:41:14 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 02:41:14 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 26 Mar 2021 02:41:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 02:41:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21f4fdff4d2de3741ff5301f2ca4d71dfb5041fbd5f4aa01cfd6823ac6693f9`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 280.9 KB (280877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8347978863206fd815b2a3bb0be789f20244679d01952c7cf99a2b62f26e50`  
		Last Modified: Fri, 26 Mar 2021 02:42:27 GMT  
		Size: 19.6 MB (19555255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83be8e29182aea4959f986a45df5392775825ead1857be98fec722452d59eb7`  
		Last Modified: Fri, 26 Mar 2021 02:42:23 GMT  
		Size: 12.3 KB (12272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bba321eed11d28f7c89bf86c98104bfe62a8bdb233953efb77cda61c4b0304`  
		Last Modified: Fri, 26 Mar 2021 02:42:22 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7060062a0a29d0380f03a272669a9230258bab2dfa7df2d7d90bce2c3f60d60d`  
		Last Modified: Fri, 26 Mar 2021 02:42:22 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8`

```console
$ docker pull chronograf@sha256:1dfc5289bdf7a00336c82bedbbb4bbb3f142d14766d3d1deb89a5d0247715e82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:a81ea833bc10b5d811d4ee54c1b8bfd6827324d25d829b93c5e6877f064aeccf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70427234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:425d563cc73d034fe084131ff89bb9bc0d18a7ee91a95d5d531a5e743fb0e7b8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 02:22:47 GMT
ADD file:1d706af4169332956a23f3faa02754cb503003812cc1d43ad9b2448f7c26f431 in / 
# Fri, 12 Mar 2021 02:22:48 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:37:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 03:38:51 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 12 Mar 2021 03:39:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 03:39:00 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 03:39:00 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 03:39:01 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 03:39:01 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 03:39:01 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 03:39:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 03:39:02 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a4feded82f54dd43cb68930d190cb6715378fa2aca3ecce0bcac959359f58d2f`  
		Last Modified: Fri, 12 Mar 2021 02:30:28 GMT  
		Size: 22.5 MB (22528907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5784273a6633bf2240f20b7dcdae41732461704080ea64a01135f933f93c0592`  
		Last Modified: Fri, 12 Mar 2021 03:39:37 GMT  
		Size: 6.7 MB (6744499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825c29972746aa6e9e7cca1fe2627d9c736f1695d57c405f37cd3c6bab135f44`  
		Last Modified: Fri, 12 Mar 2021 03:40:42 GMT  
		Size: 41.1 MB (41129444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7e09adb4f2ed2370f597ec7f7242c5d7f744007644efaaf1ce7fbc64227e06`  
		Last Modified: Fri, 12 Mar 2021 03:40:36 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6359e70aaa9a2a16f8d15a4cc115e8cd244075055fe84f3e4e4cf2e4009b100`  
		Last Modified: Fri, 12 Mar 2021 03:40:35 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61b8d22982634f7562a23b27b6d2b8d132688553391c070923b7523f4f14e28`  
		Last Modified: Fri, 12 Mar 2021 03:40:36 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:79befa0e6e75914cf190ad3e7e4a71e947f940bd4f6abaf257c722fa446f4cda
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63840619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16092a2e42246c75eb67669079719481fb3a957cfee2fafa88d453a97b6d8978`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 02:05:43 GMT
ADD file:37f1c27246cb6d0d42be6f807f54c620cc083043d7395656a56178df89e5d6d9 in / 
# Fri, 12 Mar 2021 02:05:45 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:23:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 03:25:04 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 12 Mar 2021 03:25:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 03:25:27 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 03:25:28 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 03:25:29 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 03:25:30 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 03:25:31 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 03:25:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 03:25:34 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:61211de2ba721a5e516c346a68bf2ae409d80525a872c3ad47ccefce648dc07c`  
		Last Modified: Fri, 12 Mar 2021 02:14:31 GMT  
		Size: 19.3 MB (19316567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81289d47720c1e0503331a7afcf4b884bc489014ea7cae2bba6244f9a10882bd`  
		Last Modified: Fri, 12 Mar 2021 03:25:57 GMT  
		Size: 5.8 MB (5765215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4853807ac514864f5c6b6cc3978fd508bdb4f82c0f136998a63efef5a95914`  
		Last Modified: Fri, 12 Mar 2021 03:26:42 GMT  
		Size: 38.7 MB (38734449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f107072d4174946de1993ccd086d1840963d358f9a2f72bd0281aedc8575718`  
		Last Modified: Fri, 12 Mar 2021 03:26:31 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e32e563d96287a4fd623a2fb2ba282ea0801885b518e25bc015c9c38f5d47a3`  
		Last Modified: Fri, 12 Mar 2021 03:26:31 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d846bc6d46126ac08164d645fd22a96ecba62f2a6647f31f993502e5b151cb`  
		Last Modified: Fri, 12 Mar 2021 03:26:31 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:17898fbbde81e59b3c267641c0cab98f9aefc0afd6b71b55bd004a170ad7421a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64944638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966420e366f48a2d43cfd2763f47897bb6e1819773d7c3e85cfa1a51eed05e1f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 01:57:19 GMT
ADD file:cd70de3ff9dab2f20378f87a36ca54171a79fde726291a9c5c7eae7b5435cfa2 in / 
# Fri, 12 Mar 2021 01:57:20 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:48:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 02:49:50 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 12 Mar 2021 02:50:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 02:50:08 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 02:50:09 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 02:50:10 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 02:50:12 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 02:50:13 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 02:50:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 02:50:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9cb8532b12b699d7151babb99e22315d94bfbf317f3c1db01c532a61fc38a748`  
		Last Modified: Fri, 12 Mar 2021 02:04:16 GMT  
		Size: 20.4 MB (20389391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b0ca74c9f3b67abeb6c8251b912c45335d11e252375188570d0ee2db5777cbc`  
		Last Modified: Fri, 12 Mar 2021 02:50:36 GMT  
		Size: 6.0 MB (6028358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864df4124808745adf1a72ee3b43a19d7e9253d4d61489007577c0cce3f3cb8a`  
		Last Modified: Fri, 12 Mar 2021 02:51:09 GMT  
		Size: 38.5 MB (38502492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fb31ac7661675523447543e13180a8c6d4efce5b4d84e298a51a569b40f6f3`  
		Last Modified: Fri, 12 Mar 2021 02:51:00 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1d2115958092d6287660ecd6041bb41a7beac7a65a9ea82a66694d1e977fd9`  
		Last Modified: Fri, 12 Mar 2021 02:51:00 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d829fedd4d87993ef3ce9f39d13753b284afafb3907e1aab874812bd0522de12`  
		Last Modified: Fri, 12 Mar 2021 02:51:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8-alpine`

```console
$ docker pull chronograf@sha256:a87fd88259cc60d61da8fff38020b963d19af5ea27c8f09757edfc24d953b028
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:35f56635443cbc2b6314a7d6dad1fda8da5cb7a5a53de06199347ba321462f17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25350823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:447efb090623dd2a4debcb55d502b1d63f07119bb035175f7427ea6ee66c167d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 02:40:44 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 02:41:24 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 26 Mar 2021 02:41:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 02:41:33 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 02:41:34 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 02:41:34 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 02:41:34 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 02:41:35 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 26 Mar 2021 02:41:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 02:41:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21f4fdff4d2de3741ff5301f2ca4d71dfb5041fbd5f4aa01cfd6823ac6693f9`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 280.9 KB (280877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626ff74e170b55875e086419d1b1fab6da9bd91914ce28f6d78f0919580d3728`  
		Last Modified: Fri, 26 Mar 2021 02:42:46 GMT  
		Size: 22.2 MB (22245618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cd6cfbfce23179378201909b27dacc83a9232f2633d46cc380081da99cbec3`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 12.3 KB (12271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f1cd12ac723ee5be2cd86b964ab44bf03189ae72429366be423b5779de815f`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88601fd00ca59819a15064c6a971a4ae47287533ab5f3beece5ea7a7b93da57`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.8`

```console
$ docker pull chronograf@sha256:1dfc5289bdf7a00336c82bedbbb4bbb3f142d14766d3d1deb89a5d0247715e82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8.8` - linux; amd64

```console
$ docker pull chronograf@sha256:a81ea833bc10b5d811d4ee54c1b8bfd6827324d25d829b93c5e6877f064aeccf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70427234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:425d563cc73d034fe084131ff89bb9bc0d18a7ee91a95d5d531a5e743fb0e7b8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 02:22:47 GMT
ADD file:1d706af4169332956a23f3faa02754cb503003812cc1d43ad9b2448f7c26f431 in / 
# Fri, 12 Mar 2021 02:22:48 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:37:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 03:38:51 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 12 Mar 2021 03:39:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 03:39:00 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 03:39:00 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 03:39:01 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 03:39:01 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 03:39:01 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 03:39:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 03:39:02 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a4feded82f54dd43cb68930d190cb6715378fa2aca3ecce0bcac959359f58d2f`  
		Last Modified: Fri, 12 Mar 2021 02:30:28 GMT  
		Size: 22.5 MB (22528907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5784273a6633bf2240f20b7dcdae41732461704080ea64a01135f933f93c0592`  
		Last Modified: Fri, 12 Mar 2021 03:39:37 GMT  
		Size: 6.7 MB (6744499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825c29972746aa6e9e7cca1fe2627d9c736f1695d57c405f37cd3c6bab135f44`  
		Last Modified: Fri, 12 Mar 2021 03:40:42 GMT  
		Size: 41.1 MB (41129444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7e09adb4f2ed2370f597ec7f7242c5d7f744007644efaaf1ce7fbc64227e06`  
		Last Modified: Fri, 12 Mar 2021 03:40:36 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6359e70aaa9a2a16f8d15a4cc115e8cd244075055fe84f3e4e4cf2e4009b100`  
		Last Modified: Fri, 12 Mar 2021 03:40:35 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61b8d22982634f7562a23b27b6d2b8d132688553391c070923b7523f4f14e28`  
		Last Modified: Fri, 12 Mar 2021 03:40:36 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:79befa0e6e75914cf190ad3e7e4a71e947f940bd4f6abaf257c722fa446f4cda
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63840619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16092a2e42246c75eb67669079719481fb3a957cfee2fafa88d453a97b6d8978`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 02:05:43 GMT
ADD file:37f1c27246cb6d0d42be6f807f54c620cc083043d7395656a56178df89e5d6d9 in / 
# Fri, 12 Mar 2021 02:05:45 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:23:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 03:25:04 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 12 Mar 2021 03:25:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 03:25:27 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 03:25:28 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 03:25:29 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 03:25:30 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 03:25:31 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 03:25:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 03:25:34 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:61211de2ba721a5e516c346a68bf2ae409d80525a872c3ad47ccefce648dc07c`  
		Last Modified: Fri, 12 Mar 2021 02:14:31 GMT  
		Size: 19.3 MB (19316567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81289d47720c1e0503331a7afcf4b884bc489014ea7cae2bba6244f9a10882bd`  
		Last Modified: Fri, 12 Mar 2021 03:25:57 GMT  
		Size: 5.8 MB (5765215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4853807ac514864f5c6b6cc3978fd508bdb4f82c0f136998a63efef5a95914`  
		Last Modified: Fri, 12 Mar 2021 03:26:42 GMT  
		Size: 38.7 MB (38734449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f107072d4174946de1993ccd086d1840963d358f9a2f72bd0281aedc8575718`  
		Last Modified: Fri, 12 Mar 2021 03:26:31 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e32e563d96287a4fd623a2fb2ba282ea0801885b518e25bc015c9c38f5d47a3`  
		Last Modified: Fri, 12 Mar 2021 03:26:31 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d846bc6d46126ac08164d645fd22a96ecba62f2a6647f31f993502e5b151cb`  
		Last Modified: Fri, 12 Mar 2021 03:26:31 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:17898fbbde81e59b3c267641c0cab98f9aefc0afd6b71b55bd004a170ad7421a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64944638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966420e366f48a2d43cfd2763f47897bb6e1819773d7c3e85cfa1a51eed05e1f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 01:57:19 GMT
ADD file:cd70de3ff9dab2f20378f87a36ca54171a79fde726291a9c5c7eae7b5435cfa2 in / 
# Fri, 12 Mar 2021 01:57:20 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:48:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 02:49:50 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 12 Mar 2021 02:50:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 02:50:08 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 02:50:09 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 02:50:10 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 02:50:12 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 02:50:13 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 02:50:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 02:50:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9cb8532b12b699d7151babb99e22315d94bfbf317f3c1db01c532a61fc38a748`  
		Last Modified: Fri, 12 Mar 2021 02:04:16 GMT  
		Size: 20.4 MB (20389391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b0ca74c9f3b67abeb6c8251b912c45335d11e252375188570d0ee2db5777cbc`  
		Last Modified: Fri, 12 Mar 2021 02:50:36 GMT  
		Size: 6.0 MB (6028358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864df4124808745adf1a72ee3b43a19d7e9253d4d61489007577c0cce3f3cb8a`  
		Last Modified: Fri, 12 Mar 2021 02:51:09 GMT  
		Size: 38.5 MB (38502492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fb31ac7661675523447543e13180a8c6d4efce5b4d84e298a51a569b40f6f3`  
		Last Modified: Fri, 12 Mar 2021 02:51:00 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1d2115958092d6287660ecd6041bb41a7beac7a65a9ea82a66694d1e977fd9`  
		Last Modified: Fri, 12 Mar 2021 02:51:00 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d829fedd4d87993ef3ce9f39d13753b284afafb3907e1aab874812bd0522de12`  
		Last Modified: Fri, 12 Mar 2021 02:51:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.8-alpine`

```console
$ docker pull chronograf@sha256:a87fd88259cc60d61da8fff38020b963d19af5ea27c8f09757edfc24d953b028
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:1.8.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:35f56635443cbc2b6314a7d6dad1fda8da5cb7a5a53de06199347ba321462f17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25350823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:447efb090623dd2a4debcb55d502b1d63f07119bb035175f7427ea6ee66c167d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 02:40:44 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 02:41:24 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 26 Mar 2021 02:41:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 02:41:33 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 02:41:34 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 02:41:34 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 02:41:34 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 02:41:35 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 26 Mar 2021 02:41:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 02:41:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21f4fdff4d2de3741ff5301f2ca4d71dfb5041fbd5f4aa01cfd6823ac6693f9`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 280.9 KB (280877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626ff74e170b55875e086419d1b1fab6da9bd91914ce28f6d78f0919580d3728`  
		Last Modified: Fri, 26 Mar 2021 02:42:46 GMT  
		Size: 22.2 MB (22245618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cd6cfbfce23179378201909b27dacc83a9232f2633d46cc380081da99cbec3`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 12.3 KB (12271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f1cd12ac723ee5be2cd86b964ab44bf03189ae72429366be423b5779de815f`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88601fd00ca59819a15064c6a971a4ae47287533ab5f3beece5ea7a7b93da57`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:a87fd88259cc60d61da8fff38020b963d19af5ea27c8f09757edfc24d953b028
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:35f56635443cbc2b6314a7d6dad1fda8da5cb7a5a53de06199347ba321462f17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25350823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:447efb090623dd2a4debcb55d502b1d63f07119bb035175f7427ea6ee66c167d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 02:40:44 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 02:41:24 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 26 Mar 2021 02:41:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 02:41:33 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 26 Mar 2021 02:41:34 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 26 Mar 2021 02:41:34 GMT
EXPOSE 8888
# Fri, 26 Mar 2021 02:41:34 GMT
VOLUME [/var/lib/chronograf]
# Fri, 26 Mar 2021 02:41:35 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Fri, 26 Mar 2021 02:41:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 02:41:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21f4fdff4d2de3741ff5301f2ca4d71dfb5041fbd5f4aa01cfd6823ac6693f9`  
		Last Modified: Fri, 26 Mar 2021 02:42:07 GMT  
		Size: 280.9 KB (280877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626ff74e170b55875e086419d1b1fab6da9bd91914ce28f6d78f0919580d3728`  
		Last Modified: Fri, 26 Mar 2021 02:42:46 GMT  
		Size: 22.2 MB (22245618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cd6cfbfce23179378201909b27dacc83a9232f2633d46cc380081da99cbec3`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 12.3 KB (12271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f1cd12ac723ee5be2cd86b964ab44bf03189ae72429366be423b5779de815f`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88601fd00ca59819a15064c6a971a4ae47287533ab5f3beece5ea7a7b93da57`  
		Last Modified: Fri, 26 Mar 2021 02:42:40 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:latest`

```console
$ docker pull chronograf@sha256:1dfc5289bdf7a00336c82bedbbb4bbb3f142d14766d3d1deb89a5d0247715e82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:a81ea833bc10b5d811d4ee54c1b8bfd6827324d25d829b93c5e6877f064aeccf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70427234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:425d563cc73d034fe084131ff89bb9bc0d18a7ee91a95d5d531a5e743fb0e7b8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 02:22:47 GMT
ADD file:1d706af4169332956a23f3faa02754cb503003812cc1d43ad9b2448f7c26f431 in / 
# Fri, 12 Mar 2021 02:22:48 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:37:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 03:38:51 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 12 Mar 2021 03:39:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 03:39:00 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 03:39:00 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 03:39:01 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 03:39:01 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 03:39:01 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 03:39:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 03:39:02 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a4feded82f54dd43cb68930d190cb6715378fa2aca3ecce0bcac959359f58d2f`  
		Last Modified: Fri, 12 Mar 2021 02:30:28 GMT  
		Size: 22.5 MB (22528907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5784273a6633bf2240f20b7dcdae41732461704080ea64a01135f933f93c0592`  
		Last Modified: Fri, 12 Mar 2021 03:39:37 GMT  
		Size: 6.7 MB (6744499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825c29972746aa6e9e7cca1fe2627d9c736f1695d57c405f37cd3c6bab135f44`  
		Last Modified: Fri, 12 Mar 2021 03:40:42 GMT  
		Size: 41.1 MB (41129444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7e09adb4f2ed2370f597ec7f7242c5d7f744007644efaaf1ce7fbc64227e06`  
		Last Modified: Fri, 12 Mar 2021 03:40:36 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6359e70aaa9a2a16f8d15a4cc115e8cd244075055fe84f3e4e4cf2e4009b100`  
		Last Modified: Fri, 12 Mar 2021 03:40:35 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61b8d22982634f7562a23b27b6d2b8d132688553391c070923b7523f4f14e28`  
		Last Modified: Fri, 12 Mar 2021 03:40:36 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:79befa0e6e75914cf190ad3e7e4a71e947f940bd4f6abaf257c722fa446f4cda
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63840619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16092a2e42246c75eb67669079719481fb3a957cfee2fafa88d453a97b6d8978`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 02:05:43 GMT
ADD file:37f1c27246cb6d0d42be6f807f54c620cc083043d7395656a56178df89e5d6d9 in / 
# Fri, 12 Mar 2021 02:05:45 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:23:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 03:25:04 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 12 Mar 2021 03:25:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 03:25:27 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 03:25:28 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 03:25:29 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 03:25:30 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 03:25:31 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 03:25:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 03:25:34 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:61211de2ba721a5e516c346a68bf2ae409d80525a872c3ad47ccefce648dc07c`  
		Last Modified: Fri, 12 Mar 2021 02:14:31 GMT  
		Size: 19.3 MB (19316567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81289d47720c1e0503331a7afcf4b884bc489014ea7cae2bba6244f9a10882bd`  
		Last Modified: Fri, 12 Mar 2021 03:25:57 GMT  
		Size: 5.8 MB (5765215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4853807ac514864f5c6b6cc3978fd508bdb4f82c0f136998a63efef5a95914`  
		Last Modified: Fri, 12 Mar 2021 03:26:42 GMT  
		Size: 38.7 MB (38734449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f107072d4174946de1993ccd086d1840963d358f9a2f72bd0281aedc8575718`  
		Last Modified: Fri, 12 Mar 2021 03:26:31 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e32e563d96287a4fd623a2fb2ba282ea0801885b518e25bc015c9c38f5d47a3`  
		Last Modified: Fri, 12 Mar 2021 03:26:31 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d846bc6d46126ac08164d645fd22a96ecba62f2a6647f31f993502e5b151cb`  
		Last Modified: Fri, 12 Mar 2021 03:26:31 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:17898fbbde81e59b3c267641c0cab98f9aefc0afd6b71b55bd004a170ad7421a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64944638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966420e366f48a2d43cfd2763f47897bb6e1819773d7c3e85cfa1a51eed05e1f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Fri, 12 Mar 2021 01:57:19 GMT
ADD file:cd70de3ff9dab2f20378f87a36ca54171a79fde726291a9c5c7eae7b5435cfa2 in / 
# Fri, 12 Mar 2021 01:57:20 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:48:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 12 Mar 2021 02:49:50 GMT
ENV CHRONOGRAF_VERSION=1.8.8
# Fri, 12 Mar 2021 02:50:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 02:50:08 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 12 Mar 2021 02:50:09 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 12 Mar 2021 02:50:10 GMT
EXPOSE 8888
# Fri, 12 Mar 2021 02:50:12 GMT
VOLUME [/var/lib/chronograf]
# Fri, 12 Mar 2021 02:50:13 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 12 Mar 2021 02:50:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Mar 2021 02:50:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:9cb8532b12b699d7151babb99e22315d94bfbf317f3c1db01c532a61fc38a748`  
		Last Modified: Fri, 12 Mar 2021 02:04:16 GMT  
		Size: 20.4 MB (20389391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b0ca74c9f3b67abeb6c8251b912c45335d11e252375188570d0ee2db5777cbc`  
		Last Modified: Fri, 12 Mar 2021 02:50:36 GMT  
		Size: 6.0 MB (6028358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864df4124808745adf1a72ee3b43a19d7e9253d4d61489007577c0cce3f3cb8a`  
		Last Modified: Fri, 12 Mar 2021 02:51:09 GMT  
		Size: 38.5 MB (38502492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fb31ac7661675523447543e13180a8c6d4efce5b4d84e298a51a569b40f6f3`  
		Last Modified: Fri, 12 Mar 2021 02:51:00 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1d2115958092d6287660ecd6041bb41a7beac7a65a9ea82a66694d1e977fd9`  
		Last Modified: Fri, 12 Mar 2021 02:51:00 GMT  
		Size: 11.9 KB (11910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d829fedd4d87993ef3ce9f39d13753b284afafb3907e1aab874812bd0522de12`  
		Last Modified: Fri, 12 Mar 2021 02:51:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
