## `julia:latest`

```console
$ docker pull julia@sha256:1078363d6c94949b3f2f154e42d9638b2fe48cf122f3e12ac0edc8e17a2fb321
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `julia:latest` - linux; amd64

```console
$ docker pull julia@sha256:03e22170ea4b2718eb9bec848f6caa15884a1412ea64c599866e4f14cb0df7c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.8 MB (152841908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cda5aca429fade4df2bb051049435045771ceaae10a0f7ce43a0228c4c4bd104`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:36:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:36:01 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 09:36:02 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 09:36:02 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 09:36:02 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 09:36:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 09:36:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebe3e6f4fecd87b5a88384d7073cd2980427460d97df199c3902070ceff0910`  
		Last Modified: Thu, 22 Jul 2021 09:37:52 GMT  
		Size: 4.5 MB (4457986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c675740a024e5b0c74789b01d2456b355c4ae4f8894e39f328c5e036d5d63c84`  
		Last Modified: Thu, 22 Jul 2021 09:38:10 GMT  
		Size: 121.2 MB (121238127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm variant v7

```console
$ docker pull julia@sha256:8227526b538f3c5722c33b95347831e594dc786e092d2da4e4f0301f458931cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138995918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6a92fd63ee0ccae5b2580375b577fde954069fbb13aefc7aaf2271847d34c0`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 08:11:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 08:11:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 08:11:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 08:12:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 08:12:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6baaf097f768b56fe00e83538f3de53e4e8d0daa34ad79793afcf7d6ceeded`  
		Last Modified: Thu, 22 Jul 2021 08:15:43 GMT  
		Size: 3.8 MB (3805430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441056932b57179a6f22c0b15f1612f326bc0f2caaf4f408d4ecd47eccdfc26c`  
		Last Modified: Thu, 22 Jul 2021 08:16:54 GMT  
		Size: 112.4 MB (112444514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:548dcfa0b48b7b37a5f582b6096a3a102ee63448250d97d658110b9ffaaa6b82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145411960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bfe9672c96d8ea53549a03238ea074429efcd491aed1c85bc45bab9380bc7c4`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 00:40:14 GMT
ADD file:074ffc2065bab83c9a5c596576656b04d271dd78406aadad160b68e38f38269f in / 
# Thu, 22 Jul 2021 00:40:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:28:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:28:38 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 04:28:39 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 04:28:39 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 04:28:39 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 04:28:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 04:28:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:513c6babab2b9079da61a69300c0e26d1037ca98910376098e9ae87baeb112c0`  
		Last Modified: Thu, 22 Jul 2021 00:45:53 GMT  
		Size: 25.9 MB (25914794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09296bbfedc59f17c58a9aa067b3d4371902684d16ff4510f187b1860488e3db`  
		Last Modified: Thu, 22 Jul 2021 04:30:24 GMT  
		Size: 4.3 MB (4338346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230ab68bb3b77b3e4bd9a427bc499f3146486ab22aaed7641f93f29965d69c2a`  
		Last Modified: Thu, 22 Jul 2021 04:30:43 GMT  
		Size: 115.2 MB (115158820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; 386

```console
$ docker pull julia@sha256:f7b72f1e98f0617f8f6710d959589d4c884d4c025cccff7e9d8fae3d1596c564
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151312202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2225b9d9faf2617000f9ff94c710bffe475dec18423045d0fd323f9912445fdf`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:50 GMT
ADD file:cb657a3d01f25bf815677ce223e8802d054f11aeb95f85b160982277916637bd in / 
# Thu, 22 Jul 2021 00:39:51 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:41:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:41:22 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 04:41:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 04:41:23 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 04:41:23 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 04:41:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 04:41:48 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fa9d06db5f4195bd51665a89e08e2e7db25636ac28ab162fe876ae0a53093fe5`  
		Last Modified: Thu, 22 Jul 2021 00:46:36 GMT  
		Size: 27.8 MB (27797459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28aa900f4cb082e6763ff6d40b40f1bc86ed2d4ce8f54134098751a57139d3e`  
		Last Modified: Thu, 22 Jul 2021 04:43:38 GMT  
		Size: 4.6 MB (4610589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c267b1e72763f73a861051d5607c2e69aca5bab3721853edf4c67eb8ce9ecab0`  
		Last Modified: Thu, 22 Jul 2021 04:44:15 GMT  
		Size: 118.9 MB (118904154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; ppc64le

```console
$ docker pull julia@sha256:0a4bbd735273e267514717a187cca1475366ddc6c930df4f7fecdadca9f0fc69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.0 MB (142009834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dbceb35c27bc3d1bff37fc2825c6182e91c37dcd483a6ea53d391694269c65b`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 07:55:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 07:55:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 07:56:03 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 07:56:05 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 07:56:11 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 07:57:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 07:57:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7030c44b136c8de83d74ae09b565174756f2f3ff2dee55885b458f3319d805`  
		Last Modified: Thu, 22 Jul 2021 07:58:32 GMT  
		Size: 4.9 MB (4853473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15b7a7b1631f7a8a140572b774d44aa1929a8d0b6ea4d2d49848acd0da77230`  
		Last Modified: Thu, 22 Jul 2021 07:58:50 GMT  
		Size: 106.6 MB (106602652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.17763.2114; amd64

```console
$ docker pull julia@sha256:4864ef25c972c714afbc5d30293956a403639e17d278bcd8209a3d46944d48e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2819461834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c15e4cf688eccdbea4a0c8ad51488f19e2e288357238008067f7ab93af8b10`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:31:53 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:31:56 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:34:08 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:34:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c078c711fb6c8ce9576f8dd2c9a5bc7b27c4028c2cc4ecf73fa51496dfddb37`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd3f3a64fffd4a6b075410687ff920992b8d532eee734f01a23c8b4acd6eeee`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf511001abbb952897431c950e3ce3c8767038aa724abbc790a05b468dcfbb4`  
		Last Modified: Wed, 11 Aug 2021 16:43:52 GMT  
		Size: 133.5 MB (133458221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d79499293ab2e6910164de236be148ac8a632bf1a159adc08f9c30dedfcb80`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.14393.4583; amd64

```console
$ docker pull julia@sha256:44f4d3bfb9ba8c20d0f791831e0317e698bddf73b22c54bc48951ac0bf399fe8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6408877306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9866121315e46465b3db7d8253e9835d6b32ff8810ee9b62e6c8f2f40a9165a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:34:22 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:34:26 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:37:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:37:16 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf4d37a068724cf088d64b143f952d057279607a5ea96202c171ccc235e0d10`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7527903790dab1fed6f1b33403b2f51147576eba5f0e57003265456f301d580e`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beab471f1cddf276909b1df5e600fcf90f396cf1992ce340206ac53a217204dc`  
		Last Modified: Wed, 11 Aug 2021 16:46:54 GMT  
		Size: 137.9 MB (137905576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347992b07a31f90c28cc76bdb461185c0c4b6788d9531dc59d27d832312174f5`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
