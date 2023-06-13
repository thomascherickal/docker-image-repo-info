## `node:16-bullseye-slim`

```console
$ docker pull node@sha256:723a03a5ef3d277f34e72772bc22602a98385c4e85abdfefff3992342a1df26f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `node:16-bullseye-slim` - linux; amd64

```console
$ docker pull node@sha256:cea90a193e60027b8bddaf36d87814b8395e3ab7e69a1808604884208eda1c11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69450801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb7bf6ac9d805883cc12a781a15a43c52b90b45b3aeb8806f5f599bd5477dcc1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 02:50:24 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 13 Jun 2023 02:55:41 GMT
ENV NODE_VERSION=16.20.0
# Tue, 13 Jun 2023 02:56:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 13 Jun 2023 02:56:03 GMT
ENV YARN_VERSION=1.22.19
# Tue, 13 Jun 2023 02:56:14 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 13 Jun 2023 02:56:14 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 13 Jun 2023 02:56:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 02:56:14 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243faaa2ae94245b39540c27001ea8088e6e8f5dd481b8c40218ad474884944b`  
		Last Modified: Tue, 13 Jun 2023 02:59:04 GMT  
		Size: 4.2 KB (4177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c6b00e5ff0eb7be982b369758cc9c6fd1ff282a29a2b9c545b54f7e4f63bca`  
		Last Modified: Tue, 13 Jun 2023 03:02:28 GMT  
		Size: 35.3 MB (35270353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228000056c879b74be6f60317ec32d16a6a7aa07d4c383d3836fb7d85db02dd0`  
		Last Modified: Tue, 13 Jun 2023 03:02:24 GMT  
		Size: 2.8 MB (2758409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be8d64e0b24b999f868dd54a558bf185f078b6763ffbd41886d20345c104ddd`  
		Last Modified: Tue, 13 Jun 2023 03:02:23 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:16-bullseye-slim` - linux; arm variant v7

```console
$ docker pull node@sha256:5b6b0339b90cea4a97feb720b03bc04d02c9f95e571a578f004f0f70344049a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.8 MB (61835763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:096136fc61b35535dceb3c2cdda6ff1025cececac7717ef999049f513b3699e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:47 GMT
ADD file:319a24b7e30fc548f9dcf48ad6cee469e8bf7e89c67901cf3851e41e75693489 in / 
# Mon, 12 Jun 2023 23:58:47 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:37:12 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 13 Jun 2023 04:45:01 GMT
ENV NODE_VERSION=16.20.0
# Tue, 13 Jun 2023 04:45:24 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 13 Jun 2023 04:45:24 GMT
ENV YARN_VERSION=1.22.19
# Tue, 13 Jun 2023 04:45:35 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 13 Jun 2023 04:45:35 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:45:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:45:36 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:b7c295cb849275e211d18b720d2349cc84c0038be1a362aca4765ceb3342043c`  
		Last Modified: Tue, 13 Jun 2023 00:04:24 GMT  
		Size: 26.6 MB (26578690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5e892ed23eecb842c00284e7a04e5de47eb82f73bc1fecd3878a9bd53e9f4d`  
		Last Modified: Tue, 13 Jun 2023 04:47:53 GMT  
		Size: 4.2 KB (4164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8752c8a2eb04273ea0f53682077e50039a4df65917ac6b92e79b151cb849a367`  
		Last Modified: Tue, 13 Jun 2023 04:50:05 GMT  
		Size: 32.5 MB (32500536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a8f02accf89bc0d3eb0857267164138c1f1dddedc948c67f093b0c69827f16`  
		Last Modified: Tue, 13 Jun 2023 04:50:00 GMT  
		Size: 2.8 MB (2751926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fa1b4e9e16231ed16709aee68c88542a09f12393927eb45967080069a99314`  
		Last Modified: Tue, 13 Jun 2023 04:49:59 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:16-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull node@sha256:4268879b9b49efd9f5c1133aa9f5e14ec73540a4654a3e911bef6cd2b234bb42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68336432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:402ae5ac2f7af6a02e37e1096e8381f5acf3b3b5d8d7f7cd73d3dea5721c38ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 02:21:38 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 13 Jun 2023 02:26:28 GMT
ENV NODE_VERSION=16.20.0
# Tue, 13 Jun 2023 02:26:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 13 Jun 2023 02:26:48 GMT
ENV YARN_VERSION=1.22.19
# Tue, 13 Jun 2023 02:26:58 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 13 Jun 2023 02:26:58 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 13 Jun 2023 02:26:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 02:26:59 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92921b604517eeaa1513a6254b16dc0feed3962e727248f3603d0b08090bfade`  
		Last Modified: Tue, 13 Jun 2023 02:29:45 GMT  
		Size: 4.2 KB (4182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8919b51ce1bdc1984994ada0a26a7aa0cbeac3009b2f7c0be24eb53afae6a8cd`  
		Last Modified: Tue, 13 Jun 2023 02:33:00 GMT  
		Size: 35.5 MB (35510657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916c2a8ab368a0e5c333b6f6b30a4b317a27d575addd25a57fb6a83d64635c1c`  
		Last Modified: Tue, 13 Jun 2023 02:32:56 GMT  
		Size: 2.8 MB (2758309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d951263081425e46f5a4e01d67488be1eb217ec8dbcae7bfdc2b1d8ad62fa7c2`  
		Last Modified: Tue, 13 Jun 2023 02:32:56 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:16-bullseye-slim` - linux; ppc64le

```console
$ docker pull node@sha256:8ac79fbad53f196c0f4a66b1e58ce51dfd076e45ac6a9a3052a86c8e54d0275f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75387155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1839868a50aa54737eeab2c15e8e9ac885a4a37ada5712da5c2b14f0243b574`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Mon, 12 Jun 2023 23:18:20 GMT
ADD file:b17eabe509462fa1a2e4c5421e877e3e4149085e3da07a421a66c7b06566c457 in / 
# Mon, 12 Jun 2023 23:18:22 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:10:24 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 13 Jun 2023 04:17:18 GMT
ENV NODE_VERSION=16.20.0
# Tue, 13 Jun 2023 04:17:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 13 Jun 2023 04:18:01 GMT
ENV YARN_VERSION=1.22.19
# Tue, 13 Jun 2023 04:18:27 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 13 Jun 2023 04:18:28 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:18:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:18:28 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:2973ac0be4a80a6cecbb73370e92810a6f67a98e12e61b3044aa63a322dab03a`  
		Last Modified: Mon, 12 Jun 2023 23:25:03 GMT  
		Size: 35.3 MB (35290790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc74312e7fb333204e7451638a9c14b9f4803a89d2b8558c2878b32011c0d25`  
		Last Modified: Tue, 13 Jun 2023 04:20:59 GMT  
		Size: 4.2 KB (4179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c477eea49d8d3dd3471931dc2c3ad12f7ac32245ffddbc9edfe15c72fc80eaa6`  
		Last Modified: Tue, 13 Jun 2023 04:24:23 GMT  
		Size: 37.3 MB (37333204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aebe52f874f016f1d0f79c38f418f942ddec7923067b6af951d1774ea77fccf`  
		Last Modified: Tue, 13 Jun 2023 04:24:15 GMT  
		Size: 2.8 MB (2758532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:900dc4dc636c139aaa44cb032a4132e62d023e6ba800acf13e1a6ca2c92b2a4a`  
		Last Modified: Tue, 13 Jun 2023 04:24:14 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:16-bullseye-slim` - linux; s390x

```console
$ docker pull node@sha256:09603a6cba65d81d9205581fe03a4f3900dca6af2c9216970536efaafba3cd33
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67583086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a980a2ab13bedc47906c530557f519699a988b7d93c663991ba4402fcaa9e56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Tue, 23 May 2023 00:42:52 GMT
ADD file:23b1e12559302529556a94a1d4098dbdb454e263265258b940c2b2d23a97c121 in / 
# Tue, 23 May 2023 00:42:54 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:01:54 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 May 2023 04:05:31 GMT
ENV NODE_VERSION=16.20.0
# Tue, 23 May 2023 04:05:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 May 2023 04:05:50 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 May 2023 04:05:59 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 May 2023 04:05:59 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 May 2023 04:05:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 04:05:59 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:9c24ec455bdb6a9ad0d033c7cce8e71dd5bdbbe53a86d5feeb8d4cb7804fb8e5`  
		Last Modified: Tue, 23 May 2023 00:45:47 GMT  
		Size: 29.6 MB (29642170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7a128a505b034f99ebeb10ea96a7f73c08a572d155b9680af148a96658d711`  
		Last Modified: Tue, 23 May 2023 04:07:17 GMT  
		Size: 4.2 KB (4188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce96315d38120c624071d2c9d8cb269d644a411ca8ba8bd99151a61f45859ce`  
		Last Modified: Tue, 23 May 2023 04:09:13 GMT  
		Size: 35.2 MB (35175665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c932afb8d6f16c494cedf7e54eef2d555a31131dc592210981bfeddd7eeb3483`  
		Last Modified: Tue, 23 May 2023 04:09:09 GMT  
		Size: 2.8 MB (2760613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fd679d19b99a50bb64673b1056e640d58d9c843c488c8fa80b3ce89c94a905`  
		Last Modified: Tue, 23 May 2023 04:09:08 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
