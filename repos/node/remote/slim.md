## `node:slim`

```console
$ docker pull node@sha256:20117eab1fb1f820eb4d38d929815e8b58054f04372625574993cfc60eebaf85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `node:slim` - linux; amd64

```console
$ docker pull node@sha256:2be0b0ff8fdf14453b43f8f10234d05c718fd7b6947e080982f5e57ed4c595f0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.6 MB (60604830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc1b29d4496210600024df0a3964faa9f9eff0557f3bfef565bc84195d754884`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:37 GMT
ADD file:83fbd2352bbac612c7a954e19abd295607cea4482c556c225308e0241b58e2bf in / 
# Thu, 10 Sep 2020 00:30:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 12:37:34 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 10 Sep 2020 12:37:34 GMT
ENV NODE_VERSION=14.10.0
# Thu, 10 Sep 2020 12:37:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Thu, 10 Sep 2020 12:37:56 GMT
ENV YARN_VERSION=1.22.5
# Thu, 10 Sep 2020 12:38:12 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Thu, 10 Sep 2020 12:38:12 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 10 Sep 2020 12:38:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 12:38:13 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:abb454610128b028301ee40af387d31111a1e699e4ea424fd53186ff77067402`  
		Last Modified: Thu, 10 Sep 2020 00:37:40 GMT  
		Size: 22.5 MB (22522274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfc5a66c51721369399f016ae7a7b2953e8c467c752653645d8eb19d0a1c973`  
		Last Modified: Thu, 10 Sep 2020 12:46:14 GMT  
		Size: 4.2 KB (4150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08dd7de0782059e5339adba1e62cb208f0e3cdac1ff200ff632f19cfada8bb`  
		Last Modified: Thu, 10 Sep 2020 12:46:24 GMT  
		Size: 35.3 MB (35269802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a81eb0495044c167aac2623de3d4f96d60188f774ed26f7242695ddddbe4c59`  
		Last Modified: Thu, 10 Sep 2020 12:46:14 GMT  
		Size: 2.8 MB (2808309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e97427c2180930024a16a152fa3362ece9bb541c8a98554f8baca573593e1cd`  
		Last Modified: Thu, 10 Sep 2020 12:46:14 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:slim` - linux; arm variant v7

```console
$ docker pull node@sha256:68ee20dfda068cd1af29e87bc21cdb5d584764dc7c641a0dfb905f7884c60a38
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.6 MB (55605961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16645363ac50fe1f22265a9a84fe88e6afc909a857314af8564de4638bead26d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 10 Sep 2020 00:13:48 GMT
ADD file:01ae1c10181763bd674d028f8ce4e5e3bf24c400e60a76fa6bfb43dfba07a0c6 in / 
# Thu, 10 Sep 2020 00:13:49 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 07:55:01 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 11 Sep 2020 00:18:01 GMT
ENV NODE_VERSION=14.10.1
# Fri, 11 Sep 2020 00:18:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 11 Sep 2020 00:18:52 GMT
ENV YARN_VERSION=1.22.5
# Fri, 11 Sep 2020 00:19:30 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 11 Sep 2020 00:19:31 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Fri, 11 Sep 2020 00:19:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 00:19:32 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:a1f2bf709796106dda8cc033b6c173e05f0838e1cf4fca653453e2999db8ba3d`  
		Last Modified: Thu, 10 Sep 2020 00:21:34 GMT  
		Size: 19.3 MB (19304627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9657a5f1f4320deae62d0d231ad4076caf965973b6896bd0fbcb087c6928e0`  
		Last Modified: Thu, 10 Sep 2020 08:19:19 GMT  
		Size: 4.2 KB (4162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9168a1ca8c111ddf8fdc0a996c9a96206a8855f9f70ca1615961760a572e84f5`  
		Last Modified: Fri, 11 Sep 2020 00:40:59 GMT  
		Size: 33.5 MB (33497657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46da7e2efe2b1c6a8998f35a576eb494223786fe9db09a8459752717c0142195`  
		Last Modified: Fri, 11 Sep 2020 00:40:48 GMT  
		Size: 2.8 MB (2799220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ac9ff0ccd60da71982b7f09201fee14ee44f8e304afd8186b889ef6f181551`  
		Last Modified: Fri, 11 Sep 2020 00:40:47 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:slim` - linux; arm64 variant v8

```console
$ docker pull node@sha256:a82e59f3065c1bf947a9af574db8130d7a56bac19c09fab42edda83e4a153ce5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58561442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:166ce902db643aa4c96db6f298bc598b38d4498f093f4851957b862439ae8d43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Wed, 09 Sep 2020 23:54:57 GMT
ADD file:fe3fc1ceb78e0b280e8429ba94710b765701de58e9958d27e9bcb8af97084f1b in / 
# Wed, 09 Sep 2020 23:55:02 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 10:14:58 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 11 Sep 2020 01:33:39 GMT
ENV NODE_VERSION=14.10.1
# Fri, 11 Sep 2020 01:34:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 11 Sep 2020 01:34:22 GMT
ENV YARN_VERSION=1.22.5
# Fri, 11 Sep 2020 01:34:54 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 11 Sep 2020 01:34:55 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Fri, 11 Sep 2020 01:34:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 01:34:56 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:852f38eca5e441cf6f4d6130ee167637bc8117d57f8f0156f5e489e8c3dd8f17`  
		Last Modified: Thu, 10 Sep 2020 00:01:56 GMT  
		Size: 20.4 MB (20377071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0119cf1f40e652dfc73cf37b05629a55bd0d1a2f1801374de0bc53d0eba2917f`  
		Last Modified: Thu, 10 Sep 2020 10:32:36 GMT  
		Size: 4.2 KB (4175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7d0ee488bc123d87193919e2469ee4ca36bd42984ec44894adafbd1ab6f2f2`  
		Last Modified: Fri, 11 Sep 2020 02:00:45 GMT  
		Size: 35.4 MB (35371494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aff65d15d7afc132772b4d93f8c777db2d214950570c49d280e7704df6d1ffe`  
		Last Modified: Fri, 11 Sep 2020 02:00:29 GMT  
		Size: 2.8 MB (2808410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1ab968b1796eb4f3839ed694a8461a99757e6e38701aaa5ab995a82acbc40`  
		Last Modified: Fri, 11 Sep 2020 02:00:28 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
