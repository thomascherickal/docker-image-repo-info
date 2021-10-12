## `node:buster-slim`

```console
$ docker pull node@sha256:4ae67f37a12b4df492ac1e621e73fc3bbda785f6038356e6afeb77360831c1ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `node:buster-slim` - linux; amd64

```console
$ docker pull node@sha256:937fdf1037246e0cb7f13a42b28581a1522572a47905b699e20e0de3a3501f0a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63680165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:851628d5d6aeb83c42ec791738167c173a4a2a71591c09f930bfe3be06941f74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:09 GMT
ADD file:99db7cfe7952a1c7a7959cc3457af37c1d6facdd43a946bd72313d8b5ede0029 in / 
# Tue, 28 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 08:32:26 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Mon, 11 Oct 2021 18:26:27 GMT
ENV NODE_VERSION=16.11.0
# Mon, 11 Oct 2021 18:26:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Mon, 11 Oct 2021 18:26:54 GMT
ENV YARN_VERSION=1.22.15
# Mon, 11 Oct 2021 18:27:07 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Mon, 11 Oct 2021 18:27:07 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Mon, 11 Oct 2021 18:27:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Oct 2021 18:27:07 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:07aded7c29c6011dfdf02fc98e087c941d3c2661c4e73d134c6491e25231d16c`  
		Last Modified: Tue, 28 Sep 2021 01:29:45 GMT  
		Size: 27.1 MB (27145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92706508d1249e823cd5d903a9da8786ffaf61a06f5ed56f0342c218ba62bdef`  
		Last Modified: Tue, 28 Sep 2021 08:49:53 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a81539d1cb25c674ca37a7776875852eea8fed2c201534fd3ba8af7f7fb9db`  
		Last Modified: Mon, 11 Oct 2021 18:35:32 GMT  
		Size: 33.8 MB (33806649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28bd1a75002abe791085859e2aa46aa36226d4ef805139dc5fa6c932469bcfc`  
		Last Modified: Mon, 11 Oct 2021 18:35:28 GMT  
		Size: 2.7 MB (2723061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd832ff78650356a2cb5f08475dd3e620f5b0dc6af22dc84467b41fd6b09f6a5`  
		Last Modified: Mon, 11 Oct 2021 18:35:26 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:buster-slim` - linux; arm variant v7

```console
$ docker pull node@sha256:c4822308e952a647d7613abc65c3e3736ea74f89b1da6a061eda8cac4b80dc17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56579899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a205ef05cd987ae528af16fccac66e1eaa2b66e6c27d7259cf155023de7495ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 30 Sep 2021 18:04:11 GMT
ADD file:e71f315aa894d483f75b32109fff32974c43ce2e684cd28eb6492bc6fc450931 in / 
# Thu, 30 Sep 2021 18:04:12 GMT
CMD ["bash"]
# Thu, 30 Sep 2021 19:55:23 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Mon, 11 Oct 2021 21:17:02 GMT
ENV NODE_VERSION=16.11.0
# Mon, 11 Oct 2021 21:17:51 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Mon, 11 Oct 2021 21:17:52 GMT
ENV YARN_VERSION=1.22.15
# Mon, 11 Oct 2021 21:18:26 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Mon, 11 Oct 2021 21:18:26 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Mon, 11 Oct 2021 21:18:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Oct 2021 21:18:27 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:421f17c521234da0c5b07d4f6e44314149dc3790ef12134e85e61741452c9f96`  
		Last Modified: Thu, 30 Sep 2021 18:20:50 GMT  
		Size: 22.7 MB (22746246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d844eefe717b59be08bf7457feed9d8921807b827ff4f31519d7e60d620d476e`  
		Last Modified: Thu, 30 Sep 2021 21:20:10 GMT  
		Size: 4.2 KB (4173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab305ea3939fb8272f53914d0eca3a27a3947005e2ffca384fb41b432155665`  
		Last Modified: Mon, 11 Oct 2021 21:45:15 GMT  
		Size: 31.1 MB (31114564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96a8bbb02c1c8d2ae6752de0fdae76372b93642c2c474d3eb77e476c253a800`  
		Last Modified: Mon, 11 Oct 2021 21:44:56 GMT  
		Size: 2.7 MB (2714631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd82fc6020b376e6406beb6faeb0b9dafa7539eba1b47c668b175ca3dbd1dd1b`  
		Last Modified: Mon, 11 Oct 2021 21:44:54 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:buster-slim` - linux; arm64 variant v8

```console
$ docker pull node@sha256:68fc0beee4af58edfae4141245767fe16d15b2e63e7165824097ad18338ea9d1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.6 MB (62580687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75be32448c7acf8acbb0db16a8ad05bdd506b2ca63f8d2f6bc35847a866f06a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Tue, 28 Sep 2021 01:41:13 GMT
ADD file:3e2426765cfe2b896fc847bcb435624930753c72ac00b87d2c73f4a81c813fd4 in / 
# Tue, 28 Sep 2021 01:41:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 05:05:12 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Mon, 11 Oct 2021 22:31:16 GMT
ENV NODE_VERSION=16.11.0
# Mon, 11 Oct 2021 22:31:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Mon, 11 Oct 2021 22:31:42 GMT
ENV YARN_VERSION=1.22.15
# Mon, 11 Oct 2021 22:32:09 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Mon, 11 Oct 2021 22:32:09 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Mon, 11 Oct 2021 22:32:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Oct 2021 22:32:10 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:896f18f54b28590b15a0f3354b13e8ea2f88a05f13de4117720f88cef30206ee`  
		Last Modified: Tue, 28 Sep 2021 01:49:22 GMT  
		Size: 25.9 MB (25915039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf7549406a447b98d58dffe56bc13d20bd0aaf29fa6cc2eb07c847e166b5bed`  
		Last Modified: Tue, 28 Sep 2021 05:26:55 GMT  
		Size: 4.2 KB (4187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b9b78950c3730554fe4f83142ac12545733112a3ea48d5e8b1052d98bd25d6`  
		Last Modified: Mon, 11 Oct 2021 22:46:05 GMT  
		Size: 33.9 MB (33938288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077a2a109ba7b2ba7ac0617ee6c86d1dceda2522333547f88abf5f75ff1af292`  
		Last Modified: Mon, 11 Oct 2021 22:46:00 GMT  
		Size: 2.7 MB (2722889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd53eb791868c9711891a4bfcf1d9d3309da171fc8590b4318210a4fc0dc8896`  
		Last Modified: Mon, 11 Oct 2021 22:45:59 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:buster-slim` - linux; ppc64le

```console
$ docker pull node@sha256:4d68819187e9775eadd84ee8f6e59be6e0483fbb471f8d6763498b3a2970fd54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69140495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:593cf72d0656e360acbff0e9fba5eb62c5f2e3b1769db88168d5ca2e46bb946c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Mon, 04 Oct 2021 17:56:14 GMT
ADD file:0b55ec14c2e9aa78512985a5bff3881b6fabf6794ce4406bb874b173d5a60799 in / 
# Mon, 04 Oct 2021 17:56:20 GMT
CMD ["bash"]
# Mon, 04 Oct 2021 23:28:26 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Mon, 11 Oct 2021 21:02:58 GMT
ENV NODE_VERSION=16.11.0
# Mon, 11 Oct 2021 21:06:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Mon, 11 Oct 2021 21:06:06 GMT
ENV YARN_VERSION=1.22.15
# Mon, 11 Oct 2021 21:08:56 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Mon, 11 Oct 2021 21:08:58 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Mon, 11 Oct 2021 21:09:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Oct 2021 21:09:02 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:5736db2c6d2424206be3309412da520d7fe1fe4933cc2cc72641b311dd7d9099`  
		Last Modified: Mon, 04 Oct 2021 18:08:33 GMT  
		Size: 30.6 MB (30553728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98abbf42dd7c7c93dc5d9dfd733e7067ea7b44657263b1632d24aa2faecb3f5f`  
		Last Modified: Tue, 05 Oct 2021 01:38:07 GMT  
		Size: 4.2 KB (4204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51719cded12b450d0f33c5c63fb8ad92b931feddf298e1cab4237df400e300a5`  
		Last Modified: Mon, 11 Oct 2021 21:19:54 GMT  
		Size: 35.9 MB (35858487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412e48cfae1128a5ed87fe7f58a1a00c9f049a38f8e6f6387a82e8e66c8c5921`  
		Last Modified: Mon, 11 Oct 2021 21:19:48 GMT  
		Size: 2.7 MB (2723792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a856c2b1ac2455c4cdd6c7bfef93084aabfe0f742dc0c49f7d288484ead72321`  
		Last Modified: Mon, 11 Oct 2021 21:19:47 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:buster-slim` - linux; s390x

```console
$ docker pull node@sha256:cd70ec4e80fb6424259d6cba5ca99d720d39192d2fd2d720a2560ce88ba234db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62206940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e2bc4aa4a6318d7d523a88fa48786ef42a49316b4a32feedbadc227bf71d51a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:29 GMT
ADD file:118e7a596407435b5e2ff0aae6bb9bff3b66000c91ca37bfe1eeb98c23d99d49 in / 
# Tue, 28 Sep 2021 01:43:30 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 05:14:27 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Mon, 11 Oct 2021 20:00:47 GMT
ENV NODE_VERSION=16.11.0
# Mon, 11 Oct 2021 20:01:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Mon, 11 Oct 2021 20:01:07 GMT
ENV YARN_VERSION=1.22.15
# Mon, 11 Oct 2021 20:01:30 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Mon, 11 Oct 2021 20:01:31 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Mon, 11 Oct 2021 20:01:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Oct 2021 20:01:31 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:7cfe208f95c1b63305981b069795676fa149e7115b9044c241ee45ef4aaf0bb3`  
		Last Modified: Tue, 28 Sep 2021 01:49:36 GMT  
		Size: 25.8 MB (25760871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc8f513e2378c32155456e2b5f5cd717741fa5f22b537652f3f2981b247879f`  
		Last Modified: Tue, 28 Sep 2021 05:26:10 GMT  
		Size: 4.2 KB (4186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2514ace54f69b719b9a977f0b11946c38a4597849bd5e8fbb64532147d22c6`  
		Last Modified: Mon, 11 Oct 2021 20:09:59 GMT  
		Size: 33.7 MB (33717580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ced7a84135ece8edf64e76fcb3d867aaf26d1c3e84072a67a432f4dff5ea19`  
		Last Modified: Mon, 11 Oct 2021 20:09:55 GMT  
		Size: 2.7 MB (2724017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc902a2774b67973831254663c4a7d858cb775d34db2ad69e37602f01d308c50`  
		Last Modified: Mon, 11 Oct 2021 20:09:55 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
