## `julia:buster`

```console
$ docker pull julia@sha256:1b4cfb9be61b95d18758693314b4f5ef4d0bd170c9aa6db2a62119eb77762bae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:buster` - linux; amd64

```console
$ docker pull julia@sha256:0804a40f58a8d908c1f0b2ee458c11b53dd85fe7bebca1f400afd2999c34315a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.3 MB (153335915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f49a191a16e0261b614a2c17b5170e6b39469febd93a73605e7189473fd5b1b`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:09 GMT
ADD file:99db7cfe7952a1c7a7959cc3457af37c1d6facdd43a946bd72313d8b5ede0029 in / 
# Tue, 28 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:34:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:34:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 28 Sep 2021 01:34:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 01:34:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 28 Sep 2021 01:35:26 GMT
ENV JULIA_VERSION=1.6.3
# Tue, 28 Sep 2021 01:35:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='c7459c334cd7c3e4a297baf52535937c6bad640e60882f9201a73bab9394314b' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7cf08affbad206bd3c1ef8bc117bf0aa6ac95d1666bf4c06f9d530cff29b2067' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='df1a7e96f83b60fda54fd14713a373e37ac2d80fd11dbd708a77c8a22ab86e25' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='06e3d64813e4ba6019d8d79e918c48af4943700bd1eb689c481d82a64f8c280a' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='a3cb6f58ee93bbd3bd72ecd45b9f37bf5e16e9c0ef30ba17c809ec7cbb84ee96' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 28 Sep 2021 01:35:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:07aded7c29c6011dfdf02fc98e087c941d3c2661c4e73d134c6491e25231d16c`  
		Last Modified: Tue, 28 Sep 2021 01:29:45 GMT  
		Size: 27.1 MB (27145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1990a9d94e61fa96f2feaa2b28f45bb6702a59964c7aa1ab80001a7b071e76`  
		Last Modified: Tue, 28 Sep 2021 01:38:12 GMT  
		Size: 4.5 MB (4458605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea61129cb2444a1d34ec92f7a7bb7265677def0557392ef3ab2748e5b89146cd`  
		Last Modified: Tue, 28 Sep 2021 01:39:10 GMT  
		Size: 121.7 MB (121731316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:a7a15561071c7d4ee521daad39f99b83db76d72e57eb0cb00dfab0c993eec85d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.4 MB (139354356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0615ac2f8683aec67e9a25539a2c4fab65ef7e6306655dc7d0dc2e8eb3e7c5`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 30 Sep 2021 18:04:11 GMT
ADD file:e71f315aa894d483f75b32109fff32974c43ce2e684cd28eb6492bc6fc450931 in / 
# Thu, 30 Sep 2021 18:04:12 GMT
CMD ["bash"]
# Thu, 30 Sep 2021 19:28:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Sep 2021 19:28:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 30 Sep 2021 19:28:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Sep 2021 19:28:37 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 30 Sep 2021 19:29:43 GMT
ENV JULIA_VERSION=1.6.3
# Thu, 30 Sep 2021 19:30:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='c7459c334cd7c3e4a297baf52535937c6bad640e60882f9201a73bab9394314b' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7cf08affbad206bd3c1ef8bc117bf0aa6ac95d1666bf4c06f9d530cff29b2067' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='df1a7e96f83b60fda54fd14713a373e37ac2d80fd11dbd708a77c8a22ab86e25' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='06e3d64813e4ba6019d8d79e918c48af4943700bd1eb689c481d82a64f8c280a' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='a3cb6f58ee93bbd3bd72ecd45b9f37bf5e16e9c0ef30ba17c809ec7cbb84ee96' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 30 Sep 2021 19:30:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:421f17c521234da0c5b07d4f6e44314149dc3790ef12134e85e61741452c9f96`  
		Last Modified: Thu, 30 Sep 2021 18:20:50 GMT  
		Size: 22.7 MB (22746246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2d01f5e85cbd48bad3782ed159d479ae05722ff1bca567445a1181d50a6aad`  
		Last Modified: Thu, 30 Sep 2021 19:34:15 GMT  
		Size: 3.8 MB (3806075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7808dd5a2d6d88ef5999023fd3d9f5851ff9af94b965615480864b0b4c300301`  
		Last Modified: Thu, 30 Sep 2021 19:37:09 GMT  
		Size: 112.8 MB (112802035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:1a367453ec9cdc52cbf6fccb6da57d28a54065e21b7c65495b797119915b3fd9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.6 MB (145631208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:227640c44ed5fa2ce4bd22c9472687bda7c29ea757954b567fab60291062ab9d`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 28 Sep 2021 01:41:13 GMT
ADD file:3e2426765cfe2b896fc847bcb435624930753c72ac00b87d2c73f4a81c813fd4 in / 
# Tue, 28 Sep 2021 01:41:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:55:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:55:08 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 28 Sep 2021 01:55:08 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 01:55:08 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 28 Sep 2021 01:55:45 GMT
ENV JULIA_VERSION=1.6.3
# Tue, 28 Sep 2021 01:56:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='c7459c334cd7c3e4a297baf52535937c6bad640e60882f9201a73bab9394314b' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7cf08affbad206bd3c1ef8bc117bf0aa6ac95d1666bf4c06f9d530cff29b2067' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='df1a7e96f83b60fda54fd14713a373e37ac2d80fd11dbd708a77c8a22ab86e25' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='06e3d64813e4ba6019d8d79e918c48af4943700bd1eb689c481d82a64f8c280a' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='a3cb6f58ee93bbd3bd72ecd45b9f37bf5e16e9c0ef30ba17c809ec7cbb84ee96' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 28 Sep 2021 01:56:03 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:896f18f54b28590b15a0f3354b13e8ea2f88a05f13de4117720f88cef30206ee`  
		Last Modified: Tue, 28 Sep 2021 01:49:22 GMT  
		Size: 25.9 MB (25915039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9aec2f3d12f3dfd0a6d923c6d3ed24ba78d6c7606e60ce03f7459f05bcb3966`  
		Last Modified: Tue, 28 Sep 2021 01:57:44 GMT  
		Size: 4.3 MB (4339166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cc7145f9de9827e77f7818d8278494db7fefc3dc230b118322bfaec7cfe83e`  
		Last Modified: Tue, 28 Sep 2021 01:58:41 GMT  
		Size: 115.4 MB (115377003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:363f8804a80df74c9b084b406a297c5c49431ae2b7aa9e72bf90d19671310271
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.8 MB (151752068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55dedf0fa394003ec409255f321f667e87ba7d2d645fd9aed2717129b7429104`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:49 GMT
ADD file:c090abbb3afcfebf797e06e2ac4b778acb4e97d5dca79c29d1927f43cf14b23e in / 
# Tue, 28 Sep 2021 01:40:49 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:57:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:57:02 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 28 Sep 2021 01:57:02 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 01:57:03 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 28 Sep 2021 01:57:39 GMT
ENV JULIA_VERSION=1.6.3
# Tue, 28 Sep 2021 01:58:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='c7459c334cd7c3e4a297baf52535937c6bad640e60882f9201a73bab9394314b' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7cf08affbad206bd3c1ef8bc117bf0aa6ac95d1666bf4c06f9d530cff29b2067' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='df1a7e96f83b60fda54fd14713a373e37ac2d80fd11dbd708a77c8a22ab86e25' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='06e3d64813e4ba6019d8d79e918c48af4943700bd1eb689c481d82a64f8c280a' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='a3cb6f58ee93bbd3bd72ecd45b9f37bf5e16e9c0ef30ba17c809ec7cbb84ee96' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 28 Sep 2021 01:58:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:82f7c8b98609aee82696182c03cb09ae62ceab1b17f8eec1e233a68180876d41`  
		Last Modified: Tue, 28 Sep 2021 01:50:06 GMT  
		Size: 27.8 MB (27797629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c2d9b1881723c8a8ce6abb3476c2a2f8858da16a61adb71d9bcde200ddc0d`  
		Last Modified: Tue, 28 Sep 2021 02:00:03 GMT  
		Size: 4.6 MB (4611006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716e052a051021255e106d43083df9600a06d468c414d688f20247bbdc783f5c`  
		Last Modified: Tue, 28 Sep 2021 02:01:10 GMT  
		Size: 119.3 MB (119343433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; ppc64le

```console
$ docker pull julia@sha256:cce46284039293b46262a58b3ccb53edb538f22646b15dbe10f1b205f2c5f3e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.0 MB (142010578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af72e79428f27e1796ad6030c9cc0254e1832b2f9e8d20369be28d5243fca3ef`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 03 Sep 2021 01:24:33 GMT
ADD file:6c1662ddb92232ae8969a86a18dacab97b3b5792a1ecda49e6ac741a1a5c878c in / 
# Fri, 03 Sep 2021 01:24:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:16:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:16:38 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 03 Sep 2021 08:16:41 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:16:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Sep 2021 08:18:48 GMT
ENV JULIA_VERSION=1.6.2
# Fri, 03 Sep 2021 08:20:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 03 Sep 2021 08:20:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8258146296247df1f308a336d4abf286afae14e3375edefb87a091e80745e29f`  
		Last Modified: Fri, 03 Sep 2021 01:39:45 GMT  
		Size: 30.6 MB (30553675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a54f94c4773f149e324c9485ac146a921c9f496490b95eaf3f2ad044038c1f`  
		Last Modified: Fri, 03 Sep 2021 08:21:17 GMT  
		Size: 4.9 MB (4854342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc9792ae633ab78f340f708e1ae6819fea98048006ecb49bd43f61272b93a22`  
		Last Modified: Fri, 03 Sep 2021 08:22:16 GMT  
		Size: 106.6 MB (106602561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
