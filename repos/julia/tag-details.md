<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `julia`

-	[`julia:1`](#julia1)
-	[`julia:1.0`](#julia10)
-	[`julia:1.0.5`](#julia105)
-	[`julia:1.0.5-buster`](#julia105-buster)
-	[`julia:1.0.5-stretch`](#julia105-stretch)
-	[`julia:1.0.5-windowsservercore-1809`](#julia105-windowsservercore-1809)
-	[`julia:1.0.5-windowsservercore-ltsc2016`](#julia105-windowsservercore-ltsc2016)
-	[`julia:1.0-buster`](#julia10-buster)
-	[`julia:1.0-stretch`](#julia10-stretch)
-	[`julia:1.0-windowsservercore-1809`](#julia10-windowsservercore-1809)
-	[`julia:1.0-windowsservercore-ltsc2016`](#julia10-windowsservercore-ltsc2016)
-	[`julia:1.3`](#julia13)
-	[`julia:1.3.1`](#julia131)
-	[`julia:1.3.1-buster`](#julia131-buster)
-	[`julia:1.3.1-stretch`](#julia131-stretch)
-	[`julia:1.3.1-windowsservercore-1809`](#julia131-windowsservercore-1809)
-	[`julia:1.3.1-windowsservercore-ltsc2016`](#julia131-windowsservercore-ltsc2016)
-	[`julia:1.3-buster`](#julia13-buster)
-	[`julia:1.3-stretch`](#julia13-stretch)
-	[`julia:1.3-windowsservercore-1809`](#julia13-windowsservercore-1809)
-	[`julia:1.3-windowsservercore-ltsc2016`](#julia13-windowsservercore-ltsc2016)
-	[`julia:1.4`](#julia14)
-	[`julia:1.4.0`](#julia140)
-	[`julia:1.4.0-buster`](#julia140-buster)
-	[`julia:1.4.0-rc1`](#julia140-rc1)
-	[`julia:1.4.0-rc1-buster`](#julia140-rc1-buster)
-	[`julia:1.4.0-rc1-windowsservercore-1809`](#julia140-rc1-windowsservercore-1809)
-	[`julia:1.4.0-rc1-windowsservercore-ltsc2016`](#julia140-rc1-windowsservercore-ltsc2016)
-	[`julia:1.4.0-windowsservercore-1809`](#julia140-windowsservercore-1809)
-	[`julia:1.4.0-windowsservercore-ltsc2016`](#julia140-windowsservercore-ltsc2016)
-	[`julia:1.4-buster`](#julia14-buster)
-	[`julia:1.4-rc`](#julia14-rc)
-	[`julia:1.4-rc-buster`](#julia14-rc-buster)
-	[`julia:1.4-rc-windowsservercore-1809`](#julia14-rc-windowsservercore-1809)
-	[`julia:1.4-rc-windowsservercore-ltsc2016`](#julia14-rc-windowsservercore-ltsc2016)
-	[`julia:1.4-windowsservercore-1809`](#julia14-windowsservercore-1809)
-	[`julia:1.4-windowsservercore-ltsc2016`](#julia14-windowsservercore-ltsc2016)
-	[`julia:1-buster`](#julia1-buster)
-	[`julia:1-stretch`](#julia1-stretch)
-	[`julia:1-windowsservercore-1809`](#julia1-windowsservercore-1809)
-	[`julia:1-windowsservercore-ltsc2016`](#julia1-windowsservercore-ltsc2016)
-	[`julia:buster`](#juliabuster)
-	[`julia:latest`](#julialatest)
-	[`julia:rc`](#juliarc)
-	[`julia:rc-buster`](#juliarc-buster)
-	[`julia:rc-windowsservercore-1809`](#juliarc-windowsservercore-1809)
-	[`julia:rc-windowsservercore-ltsc2016`](#juliarc-windowsservercore-ltsc2016)
-	[`julia:stretch`](#juliastretch)
-	[`julia:windowsservercore-1809`](#juliawindowsservercore-1809)
-	[`julia:windowsservercore-ltsc2016`](#juliawindowsservercore-ltsc2016)

## `julia:1`

```console
$ docker pull julia@sha256:85176141b17a747a2ab6450f68cba5c8b93a53dc041ad98c63619c7683d3d35e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3443; amd64
	-	windows version 10.0.17763.973; amd64

### `julia:1` - linux; amd64

```console
$ docker pull julia@sha256:2f5edda11e40572230ad37cd4b2923b827b155c4542a6312caec61adb179584b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.9 MB (134893337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f13978756f05b96ca25ea4d71c6589914a77ddf2e349a3761d0367eb55fa0b9`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Jan 2020 01:23:44 GMT
ENV JULIA_VERSION=1.3.1
# Tue, 07 Jan 2020 23:22:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Jan 2020 23:22:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ff93c6b9676e267b87b0701ae8a4a1fd15469fb6cb775bfe0482c05895c54a`  
		Last Modified: Tue, 07 Jan 2020 23:23:13 GMT  
		Size: 103.4 MB (103364524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm variant v7

```console
$ docker pull julia@sha256:1bfe9380ebd44f7fd18c3290a71e25f6278faa39c77562e1b18d3e9b119c7732
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120290287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4595b8f6040b4ad375efa056027ac9e606ee0ae623de6a3c7a706ca5e5898da4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:34:09 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 18:34:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:34:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc33c18856b9c29ce25a2e310ac0179b18efac98365c421059a8fa3a5dac678c`  
		Last Modified: Sat, 01 Feb 2020 18:39:18 GMT  
		Size: 93.8 MB (93807611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:1a4c0eb118408134679edff728394cbe99b4c4212746134bf8f04f0e2b6a2160
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116459413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a110dfa96e9ee5fa149a28e84c761cf44dd66e0f917a088d76555c083730b1a9`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:08:31 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 20:08:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:09:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99145e615c9c0a7c5aeafdd370a317ac277725ebc627ebb11d0a1c8f52a0c59`  
		Last Modified: Sat, 01 Feb 2020 20:13:29 GMT  
		Size: 86.3 MB (86293332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; 386

```console
$ docker pull julia@sha256:15adafbd1bfc00363d5b663c28446058a374b89be8e9fca338aa3c8cdcab0fa7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131608207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a30e007a155af8717d6b257bc5496c6212ad47689fda6e7f4ec0d02094817f19`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:48:00 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 17:48:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:48:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0d35c9e0909ce80f8e46e986854da5cd06baece621bb8529d4ab7cd66e6c2b`  
		Last Modified: Sat, 01 Feb 2020 17:51:28 GMT  
		Size: 99.3 MB (99274918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:30236875171e7c6d54f8d55583330862e9a5db937ab63e55693d8ac33d574dea
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5853668011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a85a381283d750122455d795be2c7ea0996113ffdcd598f2faf84234f380bebb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 17:20:16 GMT
ENV JULIA_VERSION=1.3.1
# Wed, 15 Jan 2020 17:20:18 GMT
ENV JULIA_SHA256=8350ca66f80484c5ca6f7341ffbdb9d5182f8d4231762d585e229567b227ef7f
# Thu, 30 Jan 2020 03:12:43 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:12:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453d305ccea93f036fe51fd37293fd5aee64f8fe68c1096ce6591cf82c005f76`  
		Last Modified: Wed, 15 Jan 2020 17:28:28 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0318d1ad0420adf48ddb3a4911d306b810a69a68a75f1889bd72e2732e98f7d`  
		Last Modified: Wed, 15 Jan 2020 17:28:28 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bbb3d35fcc68e71a0cb1c0f23d09c911dddf22f436026370aad50a8cd14bf3`  
		Last Modified: Thu, 30 Jan 2020 03:26:55 GMT  
		Size: 129.1 MB (129063927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc05b01cfc9f41d5736018505f631cbd708ac93d6ea62c81857f67926cc0645`  
		Last Modified: Thu, 30 Jan 2020 03:26:18 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:ed1ddd20b9e1503e39766f617a3422dfed5cf242e396b7f036e15fd934c74800
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2341155050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97fec4e1fe1475c22c92fdf8fdf98346ba2396bc7ca1e0acba21fe0e0ece4632`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Jan 2020 19:15:23 GMT
ENV JULIA_VERSION=1.3.1
# Wed, 29 Jan 2020 19:15:25 GMT
ENV JULIA_SHA256=8350ca66f80484c5ca6f7341ffbdb9d5182f8d4231762d585e229567b227ef7f
# Thu, 30 Jan 2020 03:15:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:15:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7726a80f05eaa520d72fca444791156a10b3834f6597ac83b61cb27fb3200101`  
		Last Modified: Wed, 29 Jan 2020 19:21:59 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20f6546d9098b8dba4542af815fe5cae976db3c5a520a5579778229dc6b173e`  
		Last Modified: Wed, 29 Jan 2020 19:21:59 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669caefcaa1628658892b7d2bed49af0e63f523b8ece9f911791d36e5b66b366`  
		Last Modified: Thu, 30 Jan 2020 03:28:24 GMT  
		Size: 123.7 MB (123739167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab655bda7afc3539a1ddf6e38766e8e7e09bf4f25c113148bc7bfc595387b2e3`  
		Last Modified: Thu, 30 Jan 2020 03:27:52 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0`

```console
$ docker pull julia@sha256:a59616778bb0e3970fbfcf48b28ae8b0124654f2af43fbf3f545776338c79307
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3443; amd64
	-	windows version 10.0.17763.973; amd64

### `julia:1.0` - linux; amd64

```console
$ docker pull julia@sha256:0903f7748e66ae06621af5530fc9bbff244badf9fbf8da39562e58f81829304e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127091926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d31eb9013cd1c52672b800fb5d1dc2aa27afb4bf65306b51a7584c1b72d267b2`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 28 Dec 2019 13:55:04 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 28 Dec 2019 13:55:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 28 Dec 2019 13:55:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b3fd2bf03c171a7415db8f8a5112169cf164939df4397cc6972c6e59ddcad1`  
		Last Modified: Sat, 28 Dec 2019 13:57:59 GMT  
		Size: 95.6 MB (95563113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; arm variant v7

```console
$ docker pull julia@sha256:cbc7614d5a92feb0ca4404ad482167d63379f25aaf56d92f9bc5900f40002e76
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113611428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1dd8319f47f3697802fc53c9e3d1bad2a14bc63e82a4816f51765ecceda7cf2`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:35:54 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 01 Feb 2020 18:36:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:36:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bbbd51a5a2ebc2fe01a4f1ed00d0b4bb0e95927722b6b5c0378276c301a88a`  
		Last Modified: Sat, 01 Feb 2020 18:40:30 GMT  
		Size: 87.1 MB (87128752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:c6aaf1128ddc27c437d550808c7c3b3b87a81e9267505c75cb3e7136b7ed99c7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110057135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfd240cbfaf9f377646a9d4dfec90a2874dab9c00a3b7942dec00c231e1fa02c`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:33:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:33:08 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 08:33:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 08:33:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 28 Dec 2019 08:35:01 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 28 Dec 2019 08:35:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 28 Dec 2019 08:35:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275ebee11ff289a50b8ad0a89e3b8a53746994a46b7e0be7d83e85dbea7a1fe8`  
		Last Modified: Sat, 28 Dec 2019 08:37:04 GMT  
		Size: 4.3 MB (4315474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5194f2bd41d2c54fc58a02e2a92f396a1da55fb8e6bde4edafca92617b5ff74`  
		Last Modified: Sat, 28 Dec 2019 08:38:41 GMT  
		Size: 79.9 MB (79890959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; 386

```console
$ docker pull julia@sha256:211507853c43982a89cf6b67722e7cebfda737f0fefee0c743701d123ff0f92a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124831683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7b9c3b83ca57d995decdc0cea980a5860c1de8e76bdf0647d5da27540d2fd7d`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:49:09 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 01 Feb 2020 17:49:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:49:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b7071c057fb0734e5ad480624c6bba061b176061abb89754f0cd811971e939`  
		Last Modified: Sat, 01 Feb 2020 17:52:33 GMT  
		Size: 92.5 MB (92498394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:ccdfb37d98512c82f2d2abc0e3875a91b710c8a3420e170dcad15647cbc77398
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5832444225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac9ce3d12a3c30b776d1887af69ceaf45e72144c1b74082a9b9cc5fcb7a48222`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 17:24:24 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 15 Jan 2020 17:24:25 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Thu, 30 Jan 2020 03:19:42 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:19:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8a4a80056f3326f47898fc429fd7d157d7757091d7c6e5d242fa87bb3d41f3`  
		Last Modified: Wed, 15 Jan 2020 17:29:46 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cafad9f455c3b56b24d9e8a2580f0a172e9ed52de90d57d49fd4c7f3f176ad`  
		Last Modified: Wed, 15 Jan 2020 17:29:46 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ffe789a407f09cb8b1033a761cc021467224b782296b6c7e0dd8e8e1818b29`  
		Last Modified: Thu, 30 Jan 2020 03:29:30 GMT  
		Size: 107.8 MB (107840203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db4c02c8159ed13e44e6f80443605dbd87c7c4a79e63ea5e880921195fbc867`  
		Last Modified: Thu, 30 Jan 2020 03:29:02 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:c69c3a3b8efb3e266e6d3069a322841d5c1cc23dafe91edad749cdfd6d5cb961
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2319921779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:084bfbb223d8c30406c42acad54d4391e34b36a99628fc983da9e31fc9d728c1`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Jan 2020 19:18:51 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 29 Jan 2020 19:18:52 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Thu, 30 Jan 2020 03:22:34 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:22:36 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8488bef27ea0ec90f7f3743d554cfda97940db0e2576e6b668cc4e577ed881a6`  
		Last Modified: Wed, 29 Jan 2020 19:23:13 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0f4e994ca995912529537339b41a85203612b2059e42123c1794774b68b4f8`  
		Last Modified: Wed, 29 Jan 2020 19:23:13 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbd74ef4834ea9585d4ba82856bd04d97ede459ef8f504d359eadbfb7a496fb`  
		Last Modified: Thu, 30 Jan 2020 03:30:26 GMT  
		Size: 102.5 MB (102505803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b081b7b79f3af7379059e39852d1542acf81f62ea26d4e6740f4cd48e5357f`  
		Last Modified: Thu, 30 Jan 2020 03:29:51 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5`

```console
$ docker pull julia@sha256:a59616778bb0e3970fbfcf48b28ae8b0124654f2af43fbf3f545776338c79307
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3443; amd64
	-	windows version 10.0.17763.973; amd64

### `julia:1.0.5` - linux; amd64

```console
$ docker pull julia@sha256:0903f7748e66ae06621af5530fc9bbff244badf9fbf8da39562e58f81829304e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127091926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d31eb9013cd1c52672b800fb5d1dc2aa27afb4bf65306b51a7584c1b72d267b2`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 28 Dec 2019 13:55:04 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 28 Dec 2019 13:55:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 28 Dec 2019 13:55:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b3fd2bf03c171a7415db8f8a5112169cf164939df4397cc6972c6e59ddcad1`  
		Last Modified: Sat, 28 Dec 2019 13:57:59 GMT  
		Size: 95.6 MB (95563113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; arm variant v7

```console
$ docker pull julia@sha256:cbc7614d5a92feb0ca4404ad482167d63379f25aaf56d92f9bc5900f40002e76
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113611428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1dd8319f47f3697802fc53c9e3d1bad2a14bc63e82a4816f51765ecceda7cf2`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:35:54 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 01 Feb 2020 18:36:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:36:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bbbd51a5a2ebc2fe01a4f1ed00d0b4bb0e95927722b6b5c0378276c301a88a`  
		Last Modified: Sat, 01 Feb 2020 18:40:30 GMT  
		Size: 87.1 MB (87128752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:c6aaf1128ddc27c437d550808c7c3b3b87a81e9267505c75cb3e7136b7ed99c7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110057135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfd240cbfaf9f377646a9d4dfec90a2874dab9c00a3b7942dec00c231e1fa02c`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:33:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:33:08 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 08:33:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 08:33:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 28 Dec 2019 08:35:01 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 28 Dec 2019 08:35:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 28 Dec 2019 08:35:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275ebee11ff289a50b8ad0a89e3b8a53746994a46b7e0be7d83e85dbea7a1fe8`  
		Last Modified: Sat, 28 Dec 2019 08:37:04 GMT  
		Size: 4.3 MB (4315474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5194f2bd41d2c54fc58a02e2a92f396a1da55fb8e6bde4edafca92617b5ff74`  
		Last Modified: Sat, 28 Dec 2019 08:38:41 GMT  
		Size: 79.9 MB (79890959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; 386

```console
$ docker pull julia@sha256:211507853c43982a89cf6b67722e7cebfda737f0fefee0c743701d123ff0f92a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124831683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7b9c3b83ca57d995decdc0cea980a5860c1de8e76bdf0647d5da27540d2fd7d`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:49:09 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 01 Feb 2020 17:49:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:49:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b7071c057fb0734e5ad480624c6bba061b176061abb89754f0cd811971e939`  
		Last Modified: Sat, 01 Feb 2020 17:52:33 GMT  
		Size: 92.5 MB (92498394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:ccdfb37d98512c82f2d2abc0e3875a91b710c8a3420e170dcad15647cbc77398
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5832444225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac9ce3d12a3c30b776d1887af69ceaf45e72144c1b74082a9b9cc5fcb7a48222`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 17:24:24 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 15 Jan 2020 17:24:25 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Thu, 30 Jan 2020 03:19:42 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:19:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8a4a80056f3326f47898fc429fd7d157d7757091d7c6e5d242fa87bb3d41f3`  
		Last Modified: Wed, 15 Jan 2020 17:29:46 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cafad9f455c3b56b24d9e8a2580f0a172e9ed52de90d57d49fd4c7f3f176ad`  
		Last Modified: Wed, 15 Jan 2020 17:29:46 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ffe789a407f09cb8b1033a761cc021467224b782296b6c7e0dd8e8e1818b29`  
		Last Modified: Thu, 30 Jan 2020 03:29:30 GMT  
		Size: 107.8 MB (107840203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db4c02c8159ed13e44e6f80443605dbd87c7c4a79e63ea5e880921195fbc867`  
		Last Modified: Thu, 30 Jan 2020 03:29:02 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:c69c3a3b8efb3e266e6d3069a322841d5c1cc23dafe91edad749cdfd6d5cb961
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2319921779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:084bfbb223d8c30406c42acad54d4391e34b36a99628fc983da9e31fc9d728c1`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Jan 2020 19:18:51 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 29 Jan 2020 19:18:52 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Thu, 30 Jan 2020 03:22:34 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:22:36 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8488bef27ea0ec90f7f3743d554cfda97940db0e2576e6b668cc4e577ed881a6`  
		Last Modified: Wed, 29 Jan 2020 19:23:13 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0f4e994ca995912529537339b41a85203612b2059e42123c1794774b68b4f8`  
		Last Modified: Wed, 29 Jan 2020 19:23:13 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbd74ef4834ea9585d4ba82856bd04d97ede459ef8f504d359eadbfb7a496fb`  
		Last Modified: Thu, 30 Jan 2020 03:30:26 GMT  
		Size: 102.5 MB (102505803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b081b7b79f3af7379059e39852d1542acf81f62ea26d4e6740f4cd48e5357f`  
		Last Modified: Thu, 30 Jan 2020 03:29:51 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-buster`

```console
$ docker pull julia@sha256:733d2ff31337f05f5c97296bae318ec71beb4a5af8df5070908a1d96f4996696
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0.5-buster` - linux; amd64

```console
$ docker pull julia@sha256:0903f7748e66ae06621af5530fc9bbff244badf9fbf8da39562e58f81829304e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127091926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d31eb9013cd1c52672b800fb5d1dc2aa27afb4bf65306b51a7584c1b72d267b2`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 28 Dec 2019 13:55:04 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 28 Dec 2019 13:55:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 28 Dec 2019 13:55:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b3fd2bf03c171a7415db8f8a5112169cf164939df4397cc6972c6e59ddcad1`  
		Last Modified: Sat, 28 Dec 2019 13:57:59 GMT  
		Size: 95.6 MB (95563113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:cbc7614d5a92feb0ca4404ad482167d63379f25aaf56d92f9bc5900f40002e76
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113611428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1dd8319f47f3697802fc53c9e3d1bad2a14bc63e82a4816f51765ecceda7cf2`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:35:54 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 01 Feb 2020 18:36:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:36:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bbbd51a5a2ebc2fe01a4f1ed00d0b4bb0e95927722b6b5c0378276c301a88a`  
		Last Modified: Sat, 01 Feb 2020 18:40:30 GMT  
		Size: 87.1 MB (87128752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:c88458c32aea22bbf944e4fbd774ef30e934df5225f5a9b8a7b036279893e5e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110057009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c76cc8d06e8c2c4a38a74b448327a23429671230faadea71c3438e05d784dfd4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:10:16 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 01 Feb 2020 20:10:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:10:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76231643fbb3822d5e886715e6205676d9f7e22072252b5725323ccb15d69e96`  
		Last Modified: Sat, 01 Feb 2020 20:14:39 GMT  
		Size: 79.9 MB (79890928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; 386

```console
$ docker pull julia@sha256:211507853c43982a89cf6b67722e7cebfda737f0fefee0c743701d123ff0f92a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124831683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7b9c3b83ca57d995decdc0cea980a5860c1de8e76bdf0647d5da27540d2fd7d`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:49:09 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 01 Feb 2020 17:49:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:49:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b7071c057fb0734e5ad480624c6bba061b176061abb89754f0cd811971e939`  
		Last Modified: Sat, 01 Feb 2020 17:52:33 GMT  
		Size: 92.5 MB (92498394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-stretch`

```console
$ docker pull julia@sha256:64efc6cdd06b27f27b55f1b5fbcc315a8d57f07e4e59e77b63f637b826508a9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0.5-stretch` - linux; amd64

```console
$ docker pull julia@sha256:ea6af6649ef3bf3c5d9e8b56cdd672683cef57126259910d869b6272f09ba916
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.5 MB (150467034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93ce5641227c4f171c28326ec33e362b3874f14ad3793b01ba4905a35b068fe8`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:55:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:55:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:55:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:55:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 28 Dec 2019 13:55:46 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 28 Dec 2019 13:56:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 28 Dec 2019 13:56:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9704d36ceb7fd72ca1242ac84e38edaadd23a07f53fe5435e181d13425e4f644`  
		Last Modified: Sat, 28 Dec 2019 13:58:06 GMT  
		Size: 9.5 MB (9512341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67ba1b49505edc0525dc42ded454e0f208572b9eca39bcae96f8f3807abe7e6`  
		Last Modified: Sat, 28 Dec 2019 13:58:30 GMT  
		Size: 95.6 MB (95573949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:71098ca432cbf235081b6b2b28dd81a8ab291ad7581a53e75f5dcab6cadf9ec8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137482565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba9c39311b41b7800a637fea918bf627ff27a92c65d19def105c4d52c32f6d8c`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:08 GMT
ADD file:b7fc54d004d962f2cfb469a1aaa9e689e46dfa2554e0cf44c33981d688adc31b in / 
# Sat, 01 Feb 2020 17:04:09 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:37:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:37:03 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:37:05 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:37:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:37:08 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 01 Feb 2020 18:37:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:37:43 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:cc3b08e804cce7e88d9df954b76be506569775afe9cf36316f2fa6c5c9bf3d5c`  
		Last Modified: Sat, 01 Feb 2020 17:11:13 GMT  
		Size: 42.1 MB (42108370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576c1224aa4096f88b3b19b00b02659f34701b6307343c1668a0a3eb5f71982e`  
		Last Modified: Sat, 01 Feb 2020 18:40:39 GMT  
		Size: 8.2 MB (8236247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb7a0bc53c5dff92996e98a635c27cfe3d578ffa15a3411e651b705d3f813d1`  
		Last Modified: Sat, 01 Feb 2020 18:41:04 GMT  
		Size: 87.1 MB (87137948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:d4d6a34eaa7c1e929aca7f82d05adc3b901b74591ac1af327fcc8cfd33099729
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131551490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d51182b4e67f7a9d5e6071bc489d4b86bc509bbd537397e3364ffdf0618fa6e`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:01 GMT
ADD file:1618e6474dbe6462a610ce7eed99f0bfd087ea37ddfc287bbd69def5c24ede47 in / 
# Sat, 01 Feb 2020 16:43:02 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:11:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:11:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:11:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:11:27 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:11:28 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 01 Feb 2020 20:11:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:11:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:df3de44c7096ba135556a1e7044f9e1feee3ef713ab96f0416f71fe78422cbf6`  
		Last Modified: Sat, 01 Feb 2020 16:48:40 GMT  
		Size: 43.2 MB (43166749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c633eb114289121582d77468c8246620ba135de63e03089f87aee7188bacc6`  
		Last Modified: Sat, 01 Feb 2020 20:14:47 GMT  
		Size: 8.5 MB (8475437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf7ef3a8898dce65ae29b14fdb35ec80f77c203e16afa6705a1152d3a4e7817`  
		Last Modified: Sat, 01 Feb 2020 20:15:12 GMT  
		Size: 79.9 MB (79909304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; 386

```console
$ docker pull julia@sha256:095ecede6f4e0cd029534f1de48d19a29c31f63ab994d255b168469d3fdad03c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148120226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93518e41492f768c7cb431ce56a77c2bd3a7f824078511092dce0b4e1182ee33`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:53 GMT
ADD file:bae1646c4e3069e717d1ee4f6c312c249e96a21d795a639cdfaf338d645c8be9 in / 
# Sat, 01 Feb 2020 16:41:53 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:49:50 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:49:50 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:49:51 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:49:51 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 01 Feb 2020 17:50:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:50:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97067fdacc0601fe58a5f782cd09d3c58a214c43b8629a2d92bd7025f46fd265`  
		Last Modified: Sat, 01 Feb 2020 16:47:15 GMT  
		Size: 46.1 MB (46100017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7c630539a70bdcfe1e0f106527e7be5b6c3cd7e3deb8efe8d043e7a0722274`  
		Last Modified: Sat, 01 Feb 2020 17:52:40 GMT  
		Size: 9.5 MB (9518348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77fd11d9dccdde2b5d0a67fdfd1416e0e5298483a7572ad2deec55fea264400d`  
		Last Modified: Sat, 01 Feb 2020 17:53:02 GMT  
		Size: 92.5 MB (92501861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-windowsservercore-1809`

```console
$ docker pull julia@sha256:1f54c987b077be41d10f73ba9c905a647b74a885940157ae7b03f000d099e936
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `julia:1.0.5-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:c69c3a3b8efb3e266e6d3069a322841d5c1cc23dafe91edad749cdfd6d5cb961
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2319921779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:084bfbb223d8c30406c42acad54d4391e34b36a99628fc983da9e31fc9d728c1`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Jan 2020 19:18:51 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 29 Jan 2020 19:18:52 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Thu, 30 Jan 2020 03:22:34 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:22:36 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8488bef27ea0ec90f7f3743d554cfda97940db0e2576e6b668cc4e577ed881a6`  
		Last Modified: Wed, 29 Jan 2020 19:23:13 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0f4e994ca995912529537339b41a85203612b2059e42123c1794774b68b4f8`  
		Last Modified: Wed, 29 Jan 2020 19:23:13 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbd74ef4834ea9585d4ba82856bd04d97ede459ef8f504d359eadbfb7a496fb`  
		Last Modified: Thu, 30 Jan 2020 03:30:26 GMT  
		Size: 102.5 MB (102505803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b081b7b79f3af7379059e39852d1542acf81f62ea26d4e6740f4cd48e5357f`  
		Last Modified: Thu, 30 Jan 2020 03:29:51 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:94ac30ae9e6bd52c93a4b9e1a403428e30e5dbf6cfa8132b46c3b3868be54540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `julia:1.0.5-windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:ccdfb37d98512c82f2d2abc0e3875a91b710c8a3420e170dcad15647cbc77398
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5832444225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac9ce3d12a3c30b776d1887af69ceaf45e72144c1b74082a9b9cc5fcb7a48222`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 17:24:24 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 15 Jan 2020 17:24:25 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Thu, 30 Jan 2020 03:19:42 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:19:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8a4a80056f3326f47898fc429fd7d157d7757091d7c6e5d242fa87bb3d41f3`  
		Last Modified: Wed, 15 Jan 2020 17:29:46 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cafad9f455c3b56b24d9e8a2580f0a172e9ed52de90d57d49fd4c7f3f176ad`  
		Last Modified: Wed, 15 Jan 2020 17:29:46 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ffe789a407f09cb8b1033a761cc021467224b782296b6c7e0dd8e8e1818b29`  
		Last Modified: Thu, 30 Jan 2020 03:29:30 GMT  
		Size: 107.8 MB (107840203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db4c02c8159ed13e44e6f80443605dbd87c7c4a79e63ea5e880921195fbc867`  
		Last Modified: Thu, 30 Jan 2020 03:29:02 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-buster`

```console
$ docker pull julia@sha256:733d2ff31337f05f5c97296bae318ec71beb4a5af8df5070908a1d96f4996696
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0-buster` - linux; amd64

```console
$ docker pull julia@sha256:0903f7748e66ae06621af5530fc9bbff244badf9fbf8da39562e58f81829304e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127091926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d31eb9013cd1c52672b800fb5d1dc2aa27afb4bf65306b51a7584c1b72d267b2`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 28 Dec 2019 13:55:04 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 28 Dec 2019 13:55:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 28 Dec 2019 13:55:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b3fd2bf03c171a7415db8f8a5112169cf164939df4397cc6972c6e59ddcad1`  
		Last Modified: Sat, 28 Dec 2019 13:57:59 GMT  
		Size: 95.6 MB (95563113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:cbc7614d5a92feb0ca4404ad482167d63379f25aaf56d92f9bc5900f40002e76
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113611428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1dd8319f47f3697802fc53c9e3d1bad2a14bc63e82a4816f51765ecceda7cf2`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:35:54 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 01 Feb 2020 18:36:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:36:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bbbd51a5a2ebc2fe01a4f1ed00d0b4bb0e95927722b6b5c0378276c301a88a`  
		Last Modified: Sat, 01 Feb 2020 18:40:30 GMT  
		Size: 87.1 MB (87128752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:c88458c32aea22bbf944e4fbd774ef30e934df5225f5a9b8a7b036279893e5e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110057009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c76cc8d06e8c2c4a38a74b448327a23429671230faadea71c3438e05d784dfd4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:10:16 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 01 Feb 2020 20:10:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:10:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76231643fbb3822d5e886715e6205676d9f7e22072252b5725323ccb15d69e96`  
		Last Modified: Sat, 01 Feb 2020 20:14:39 GMT  
		Size: 79.9 MB (79890928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; 386

```console
$ docker pull julia@sha256:211507853c43982a89cf6b67722e7cebfda737f0fefee0c743701d123ff0f92a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124831683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7b9c3b83ca57d995decdc0cea980a5860c1de8e76bdf0647d5da27540d2fd7d`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:49:09 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 01 Feb 2020 17:49:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:49:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b7071c057fb0734e5ad480624c6bba061b176061abb89754f0cd811971e939`  
		Last Modified: Sat, 01 Feb 2020 17:52:33 GMT  
		Size: 92.5 MB (92498394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-stretch`

```console
$ docker pull julia@sha256:64efc6cdd06b27f27b55f1b5fbcc315a8d57f07e4e59e77b63f637b826508a9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0-stretch` - linux; amd64

```console
$ docker pull julia@sha256:ea6af6649ef3bf3c5d9e8b56cdd672683cef57126259910d869b6272f09ba916
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.5 MB (150467034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93ce5641227c4f171c28326ec33e362b3874f14ad3793b01ba4905a35b068fe8`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:55:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:55:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:55:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:55:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 28 Dec 2019 13:55:46 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 28 Dec 2019 13:56:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 28 Dec 2019 13:56:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9704d36ceb7fd72ca1242ac84e38edaadd23a07f53fe5435e181d13425e4f644`  
		Last Modified: Sat, 28 Dec 2019 13:58:06 GMT  
		Size: 9.5 MB (9512341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67ba1b49505edc0525dc42ded454e0f208572b9eca39bcae96f8f3807abe7e6`  
		Last Modified: Sat, 28 Dec 2019 13:58:30 GMT  
		Size: 95.6 MB (95573949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:71098ca432cbf235081b6b2b28dd81a8ab291ad7581a53e75f5dcab6cadf9ec8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137482565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba9c39311b41b7800a637fea918bf627ff27a92c65d19def105c4d52c32f6d8c`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:08 GMT
ADD file:b7fc54d004d962f2cfb469a1aaa9e689e46dfa2554e0cf44c33981d688adc31b in / 
# Sat, 01 Feb 2020 17:04:09 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:37:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:37:03 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:37:05 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:37:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:37:08 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 01 Feb 2020 18:37:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:37:43 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:cc3b08e804cce7e88d9df954b76be506569775afe9cf36316f2fa6c5c9bf3d5c`  
		Last Modified: Sat, 01 Feb 2020 17:11:13 GMT  
		Size: 42.1 MB (42108370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576c1224aa4096f88b3b19b00b02659f34701b6307343c1668a0a3eb5f71982e`  
		Last Modified: Sat, 01 Feb 2020 18:40:39 GMT  
		Size: 8.2 MB (8236247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb7a0bc53c5dff92996e98a635c27cfe3d578ffa15a3411e651b705d3f813d1`  
		Last Modified: Sat, 01 Feb 2020 18:41:04 GMT  
		Size: 87.1 MB (87137948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:d4d6a34eaa7c1e929aca7f82d05adc3b901b74591ac1af327fcc8cfd33099729
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131551490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d51182b4e67f7a9d5e6071bc489d4b86bc509bbd537397e3364ffdf0618fa6e`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:01 GMT
ADD file:1618e6474dbe6462a610ce7eed99f0bfd087ea37ddfc287bbd69def5c24ede47 in / 
# Sat, 01 Feb 2020 16:43:02 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:11:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:11:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:11:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:11:27 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:11:28 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 01 Feb 2020 20:11:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:11:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:df3de44c7096ba135556a1e7044f9e1feee3ef713ab96f0416f71fe78422cbf6`  
		Last Modified: Sat, 01 Feb 2020 16:48:40 GMT  
		Size: 43.2 MB (43166749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c633eb114289121582d77468c8246620ba135de63e03089f87aee7188bacc6`  
		Last Modified: Sat, 01 Feb 2020 20:14:47 GMT  
		Size: 8.5 MB (8475437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf7ef3a8898dce65ae29b14fdb35ec80f77c203e16afa6705a1152d3a4e7817`  
		Last Modified: Sat, 01 Feb 2020 20:15:12 GMT  
		Size: 79.9 MB (79909304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; 386

```console
$ docker pull julia@sha256:095ecede6f4e0cd029534f1de48d19a29c31f63ab994d255b168469d3fdad03c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148120226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93518e41492f768c7cb431ce56a77c2bd3a7f824078511092dce0b4e1182ee33`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:53 GMT
ADD file:bae1646c4e3069e717d1ee4f6c312c249e96a21d795a639cdfaf338d645c8be9 in / 
# Sat, 01 Feb 2020 16:41:53 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:49:50 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:49:50 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:49:51 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:49:51 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 01 Feb 2020 17:50:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:50:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97067fdacc0601fe58a5f782cd09d3c58a214c43b8629a2d92bd7025f46fd265`  
		Last Modified: Sat, 01 Feb 2020 16:47:15 GMT  
		Size: 46.1 MB (46100017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7c630539a70bdcfe1e0f106527e7be5b6c3cd7e3deb8efe8d043e7a0722274`  
		Last Modified: Sat, 01 Feb 2020 17:52:40 GMT  
		Size: 9.5 MB (9518348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77fd11d9dccdde2b5d0a67fdfd1416e0e5298483a7572ad2deec55fea264400d`  
		Last Modified: Sat, 01 Feb 2020 17:53:02 GMT  
		Size: 92.5 MB (92501861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-windowsservercore-1809`

```console
$ docker pull julia@sha256:1f54c987b077be41d10f73ba9c905a647b74a885940157ae7b03f000d099e936
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `julia:1.0-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:c69c3a3b8efb3e266e6d3069a322841d5c1cc23dafe91edad749cdfd6d5cb961
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2319921779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:084bfbb223d8c30406c42acad54d4391e34b36a99628fc983da9e31fc9d728c1`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Jan 2020 19:18:51 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 29 Jan 2020 19:18:52 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Thu, 30 Jan 2020 03:22:34 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:22:36 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8488bef27ea0ec90f7f3743d554cfda97940db0e2576e6b668cc4e577ed881a6`  
		Last Modified: Wed, 29 Jan 2020 19:23:13 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0f4e994ca995912529537339b41a85203612b2059e42123c1794774b68b4f8`  
		Last Modified: Wed, 29 Jan 2020 19:23:13 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbd74ef4834ea9585d4ba82856bd04d97ede459ef8f504d359eadbfb7a496fb`  
		Last Modified: Thu, 30 Jan 2020 03:30:26 GMT  
		Size: 102.5 MB (102505803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b081b7b79f3af7379059e39852d1542acf81f62ea26d4e6740f4cd48e5357f`  
		Last Modified: Thu, 30 Jan 2020 03:29:51 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:94ac30ae9e6bd52c93a4b9e1a403428e30e5dbf6cfa8132b46c3b3868be54540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `julia:1.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:ccdfb37d98512c82f2d2abc0e3875a91b710c8a3420e170dcad15647cbc77398
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5832444225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac9ce3d12a3c30b776d1887af69ceaf45e72144c1b74082a9b9cc5fcb7a48222`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 17:24:24 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 15 Jan 2020 17:24:25 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Thu, 30 Jan 2020 03:19:42 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:19:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8a4a80056f3326f47898fc429fd7d157d7757091d7c6e5d242fa87bb3d41f3`  
		Last Modified: Wed, 15 Jan 2020 17:29:46 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cafad9f455c3b56b24d9e8a2580f0a172e9ed52de90d57d49fd4c7f3f176ad`  
		Last Modified: Wed, 15 Jan 2020 17:29:46 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ffe789a407f09cb8b1033a761cc021467224b782296b6c7e0dd8e8e1818b29`  
		Last Modified: Thu, 30 Jan 2020 03:29:30 GMT  
		Size: 107.8 MB (107840203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db4c02c8159ed13e44e6f80443605dbd87c7c4a79e63ea5e880921195fbc867`  
		Last Modified: Thu, 30 Jan 2020 03:29:02 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3`

```console
$ docker pull julia@sha256:85176141b17a747a2ab6450f68cba5c8b93a53dc041ad98c63619c7683d3d35e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3443; amd64
	-	windows version 10.0.17763.973; amd64

### `julia:1.3` - linux; amd64

```console
$ docker pull julia@sha256:2f5edda11e40572230ad37cd4b2923b827b155c4542a6312caec61adb179584b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.9 MB (134893337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f13978756f05b96ca25ea4d71c6589914a77ddf2e349a3761d0367eb55fa0b9`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Jan 2020 01:23:44 GMT
ENV JULIA_VERSION=1.3.1
# Tue, 07 Jan 2020 23:22:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Jan 2020 23:22:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ff93c6b9676e267b87b0701ae8a4a1fd15469fb6cb775bfe0482c05895c54a`  
		Last Modified: Tue, 07 Jan 2020 23:23:13 GMT  
		Size: 103.4 MB (103364524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3` - linux; arm variant v7

```console
$ docker pull julia@sha256:1bfe9380ebd44f7fd18c3290a71e25f6278faa39c77562e1b18d3e9b119c7732
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120290287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4595b8f6040b4ad375efa056027ac9e606ee0ae623de6a3c7a706ca5e5898da4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:34:09 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 18:34:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:34:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc33c18856b9c29ce25a2e310ac0179b18efac98365c421059a8fa3a5dac678c`  
		Last Modified: Sat, 01 Feb 2020 18:39:18 GMT  
		Size: 93.8 MB (93807611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:1a4c0eb118408134679edff728394cbe99b4c4212746134bf8f04f0e2b6a2160
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116459413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a110dfa96e9ee5fa149a28e84c761cf44dd66e0f917a088d76555c083730b1a9`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:08:31 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 20:08:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:09:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99145e615c9c0a7c5aeafdd370a317ac277725ebc627ebb11d0a1c8f52a0c59`  
		Last Modified: Sat, 01 Feb 2020 20:13:29 GMT  
		Size: 86.3 MB (86293332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3` - linux; 386

```console
$ docker pull julia@sha256:15adafbd1bfc00363d5b663c28446058a374b89be8e9fca338aa3c8cdcab0fa7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131608207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a30e007a155af8717d6b257bc5496c6212ad47689fda6e7f4ec0d02094817f19`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:48:00 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 17:48:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:48:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0d35c9e0909ce80f8e46e986854da5cd06baece621bb8529d4ab7cd66e6c2b`  
		Last Modified: Sat, 01 Feb 2020 17:51:28 GMT  
		Size: 99.3 MB (99274918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:30236875171e7c6d54f8d55583330862e9a5db937ab63e55693d8ac33d574dea
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5853668011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a85a381283d750122455d795be2c7ea0996113ffdcd598f2faf84234f380bebb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 17:20:16 GMT
ENV JULIA_VERSION=1.3.1
# Wed, 15 Jan 2020 17:20:18 GMT
ENV JULIA_SHA256=8350ca66f80484c5ca6f7341ffbdb9d5182f8d4231762d585e229567b227ef7f
# Thu, 30 Jan 2020 03:12:43 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:12:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453d305ccea93f036fe51fd37293fd5aee64f8fe68c1096ce6591cf82c005f76`  
		Last Modified: Wed, 15 Jan 2020 17:28:28 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0318d1ad0420adf48ddb3a4911d306b810a69a68a75f1889bd72e2732e98f7d`  
		Last Modified: Wed, 15 Jan 2020 17:28:28 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bbb3d35fcc68e71a0cb1c0f23d09c911dddf22f436026370aad50a8cd14bf3`  
		Last Modified: Thu, 30 Jan 2020 03:26:55 GMT  
		Size: 129.1 MB (129063927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc05b01cfc9f41d5736018505f631cbd708ac93d6ea62c81857f67926cc0645`  
		Last Modified: Thu, 30 Jan 2020 03:26:18 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:ed1ddd20b9e1503e39766f617a3422dfed5cf242e396b7f036e15fd934c74800
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2341155050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97fec4e1fe1475c22c92fdf8fdf98346ba2396bc7ca1e0acba21fe0e0ece4632`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Jan 2020 19:15:23 GMT
ENV JULIA_VERSION=1.3.1
# Wed, 29 Jan 2020 19:15:25 GMT
ENV JULIA_SHA256=8350ca66f80484c5ca6f7341ffbdb9d5182f8d4231762d585e229567b227ef7f
# Thu, 30 Jan 2020 03:15:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:15:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7726a80f05eaa520d72fca444791156a10b3834f6597ac83b61cb27fb3200101`  
		Last Modified: Wed, 29 Jan 2020 19:21:59 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20f6546d9098b8dba4542af815fe5cae976db3c5a520a5579778229dc6b173e`  
		Last Modified: Wed, 29 Jan 2020 19:21:59 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669caefcaa1628658892b7d2bed49af0e63f523b8ece9f911791d36e5b66b366`  
		Last Modified: Thu, 30 Jan 2020 03:28:24 GMT  
		Size: 123.7 MB (123739167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab655bda7afc3539a1ddf6e38766e8e7e09bf4f25c113148bc7bfc595387b2e3`  
		Last Modified: Thu, 30 Jan 2020 03:27:52 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3.1`

```console
$ docker pull julia@sha256:85176141b17a747a2ab6450f68cba5c8b93a53dc041ad98c63619c7683d3d35e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3443; amd64
	-	windows version 10.0.17763.973; amd64

### `julia:1.3.1` - linux; amd64

```console
$ docker pull julia@sha256:2f5edda11e40572230ad37cd4b2923b827b155c4542a6312caec61adb179584b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.9 MB (134893337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f13978756f05b96ca25ea4d71c6589914a77ddf2e349a3761d0367eb55fa0b9`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Jan 2020 01:23:44 GMT
ENV JULIA_VERSION=1.3.1
# Tue, 07 Jan 2020 23:22:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Jan 2020 23:22:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ff93c6b9676e267b87b0701ae8a4a1fd15469fb6cb775bfe0482c05895c54a`  
		Last Modified: Tue, 07 Jan 2020 23:23:13 GMT  
		Size: 103.4 MB (103364524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.1` - linux; arm variant v7

```console
$ docker pull julia@sha256:1bfe9380ebd44f7fd18c3290a71e25f6278faa39c77562e1b18d3e9b119c7732
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120290287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4595b8f6040b4ad375efa056027ac9e606ee0ae623de6a3c7a706ca5e5898da4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:34:09 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 18:34:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:34:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc33c18856b9c29ce25a2e310ac0179b18efac98365c421059a8fa3a5dac678c`  
		Last Modified: Sat, 01 Feb 2020 18:39:18 GMT  
		Size: 93.8 MB (93807611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:1a4c0eb118408134679edff728394cbe99b4c4212746134bf8f04f0e2b6a2160
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116459413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a110dfa96e9ee5fa149a28e84c761cf44dd66e0f917a088d76555c083730b1a9`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:08:31 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 20:08:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:09:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99145e615c9c0a7c5aeafdd370a317ac277725ebc627ebb11d0a1c8f52a0c59`  
		Last Modified: Sat, 01 Feb 2020 20:13:29 GMT  
		Size: 86.3 MB (86293332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.1` - linux; 386

```console
$ docker pull julia@sha256:15adafbd1bfc00363d5b663c28446058a374b89be8e9fca338aa3c8cdcab0fa7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131608207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a30e007a155af8717d6b257bc5496c6212ad47689fda6e7f4ec0d02094817f19`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:48:00 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 17:48:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:48:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0d35c9e0909ce80f8e46e986854da5cd06baece621bb8529d4ab7cd66e6c2b`  
		Last Modified: Sat, 01 Feb 2020 17:51:28 GMT  
		Size: 99.3 MB (99274918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.1` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:30236875171e7c6d54f8d55583330862e9a5db937ab63e55693d8ac33d574dea
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5853668011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a85a381283d750122455d795be2c7ea0996113ffdcd598f2faf84234f380bebb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 17:20:16 GMT
ENV JULIA_VERSION=1.3.1
# Wed, 15 Jan 2020 17:20:18 GMT
ENV JULIA_SHA256=8350ca66f80484c5ca6f7341ffbdb9d5182f8d4231762d585e229567b227ef7f
# Thu, 30 Jan 2020 03:12:43 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:12:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453d305ccea93f036fe51fd37293fd5aee64f8fe68c1096ce6591cf82c005f76`  
		Last Modified: Wed, 15 Jan 2020 17:28:28 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0318d1ad0420adf48ddb3a4911d306b810a69a68a75f1889bd72e2732e98f7d`  
		Last Modified: Wed, 15 Jan 2020 17:28:28 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bbb3d35fcc68e71a0cb1c0f23d09c911dddf22f436026370aad50a8cd14bf3`  
		Last Modified: Thu, 30 Jan 2020 03:26:55 GMT  
		Size: 129.1 MB (129063927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc05b01cfc9f41d5736018505f631cbd708ac93d6ea62c81857f67926cc0645`  
		Last Modified: Thu, 30 Jan 2020 03:26:18 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.1` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:ed1ddd20b9e1503e39766f617a3422dfed5cf242e396b7f036e15fd934c74800
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2341155050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97fec4e1fe1475c22c92fdf8fdf98346ba2396bc7ca1e0acba21fe0e0ece4632`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Jan 2020 19:15:23 GMT
ENV JULIA_VERSION=1.3.1
# Wed, 29 Jan 2020 19:15:25 GMT
ENV JULIA_SHA256=8350ca66f80484c5ca6f7341ffbdb9d5182f8d4231762d585e229567b227ef7f
# Thu, 30 Jan 2020 03:15:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:15:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7726a80f05eaa520d72fca444791156a10b3834f6597ac83b61cb27fb3200101`  
		Last Modified: Wed, 29 Jan 2020 19:21:59 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20f6546d9098b8dba4542af815fe5cae976db3c5a520a5579778229dc6b173e`  
		Last Modified: Wed, 29 Jan 2020 19:21:59 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669caefcaa1628658892b7d2bed49af0e63f523b8ece9f911791d36e5b66b366`  
		Last Modified: Thu, 30 Jan 2020 03:28:24 GMT  
		Size: 123.7 MB (123739167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab655bda7afc3539a1ddf6e38766e8e7e09bf4f25c113148bc7bfc595387b2e3`  
		Last Modified: Thu, 30 Jan 2020 03:27:52 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3.1-buster`

```console
$ docker pull julia@sha256:62facc73cdbfb1f431d0c1ff66ff637e8d12cb68be0f9b3844c6af16e7b0e21f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.3.1-buster` - linux; amd64

```console
$ docker pull julia@sha256:2f5edda11e40572230ad37cd4b2923b827b155c4542a6312caec61adb179584b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.9 MB (134893337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f13978756f05b96ca25ea4d71c6589914a77ddf2e349a3761d0367eb55fa0b9`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Jan 2020 01:23:44 GMT
ENV JULIA_VERSION=1.3.1
# Tue, 07 Jan 2020 23:22:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Jan 2020 23:22:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ff93c6b9676e267b87b0701ae8a4a1fd15469fb6cb775bfe0482c05895c54a`  
		Last Modified: Tue, 07 Jan 2020 23:23:13 GMT  
		Size: 103.4 MB (103364524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.1-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:1bfe9380ebd44f7fd18c3290a71e25f6278faa39c77562e1b18d3e9b119c7732
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120290287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4595b8f6040b4ad375efa056027ac9e606ee0ae623de6a3c7a706ca5e5898da4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:34:09 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 18:34:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:34:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc33c18856b9c29ce25a2e310ac0179b18efac98365c421059a8fa3a5dac678c`  
		Last Modified: Sat, 01 Feb 2020 18:39:18 GMT  
		Size: 93.8 MB (93807611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.1-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:1a4c0eb118408134679edff728394cbe99b4c4212746134bf8f04f0e2b6a2160
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116459413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a110dfa96e9ee5fa149a28e84c761cf44dd66e0f917a088d76555c083730b1a9`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:08:31 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 20:08:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:09:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99145e615c9c0a7c5aeafdd370a317ac277725ebc627ebb11d0a1c8f52a0c59`  
		Last Modified: Sat, 01 Feb 2020 20:13:29 GMT  
		Size: 86.3 MB (86293332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.1-buster` - linux; 386

```console
$ docker pull julia@sha256:15adafbd1bfc00363d5b663c28446058a374b89be8e9fca338aa3c8cdcab0fa7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131608207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a30e007a155af8717d6b257bc5496c6212ad47689fda6e7f4ec0d02094817f19`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:48:00 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 17:48:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:48:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0d35c9e0909ce80f8e46e986854da5cd06baece621bb8529d4ab7cd66e6c2b`  
		Last Modified: Sat, 01 Feb 2020 17:51:28 GMT  
		Size: 99.3 MB (99274918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3.1-stretch`

```console
$ docker pull julia@sha256:733cffa80bf37f47d4d2de3cb28a40a3e06d86b21de64ee06991829722396939
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.3.1-stretch` - linux; amd64

```console
$ docker pull julia@sha256:f16498d133d157f29bd5fefe385f482fbfc0c81ef8b889866989dacdc0bd4bae
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133452200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b507aa80fa4adf054832444d789687c311b4923b77be08f9567fb2c1de1d93c`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:47 GMT
ADD file:90a2c81769a336bed3f731f44a385f2a65b0916f517a0b77c06c224579bf9a9a in / 
# Sat, 28 Dec 2019 04:23:47 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:54:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:54:37 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:54:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:54:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Jan 2020 01:24:05 GMT
ENV JULIA_VERSION=1.3.1
# Tue, 07 Jan 2020 23:22:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Jan 2020 23:22:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:804555ee037604c40de144f9f8da0d826d38db82f15d74cded32790fe279a8f6`  
		Last Modified: Sat, 28 Dec 2019 04:28:38 GMT  
		Size: 22.5 MB (22524609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6aef362d0b91076dc5819a1b925f776504ec063851be5395cadb471b9f3881e`  
		Last Modified: Sat, 28 Dec 2019 13:57:02 GMT  
		Size: 7.6 MB (7555513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71672730cf04ca165569336fedcecf18f18fa7af5bb68b0269336d2cf0104e6d`  
		Last Modified: Tue, 07 Jan 2020 23:23:49 GMT  
		Size: 103.4 MB (103372078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.1-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:c96aa5ec4099d65d449554fe6255b743ea25cfab5a1aa847a3cffca734f0f0ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119407020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:facee1409787ff6bc644dbfa70a17b807cf03b1a47fae35a99ecd4234ab3e1fa`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:29 GMT
ADD file:6ac430a42a1f2a6cc8b0a3565e518bd0e3a47b01d524b86cd3dd4e7f4606fd53 in / 
# Sat, 01 Feb 2020 17:04:31 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:35:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:35:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:35:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:35:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:35:14 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 18:35:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:35:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6bc458b0813423b9e351a5604c0d71a4853d970ea22b23fedc8683af12dbc13c`  
		Last Modified: Sat, 01 Feb 2020 17:11:31 GMT  
		Size: 19.3 MB (19311624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9840e48d64ced9020e882cefaf8fe5cd26dc391522b6acd18cd09eccad69e07`  
		Last Modified: Sat, 01 Feb 2020 18:39:27 GMT  
		Size: 6.3 MB (6292143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8331cb5b72ee568b3cf598db9f378382b4cc073daabb288e06f54994ca3f6ae7`  
		Last Modified: Sat, 01 Feb 2020 18:39:55 GMT  
		Size: 93.8 MB (93803253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.1-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:96635540f0bc528b39750e2c03177d4e85a1bb1c080981eb64742ed7d690f4ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113207625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:877782fd5d403c41cd3e8bd8175bba4fc79ed5a1a96a15b1715dba7334a7740b`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:d3338eed8ee88c2a5856cc2eb73701e4de79a7e551602df07834a1ad4f671435 in / 
# Sat, 01 Feb 2020 16:43:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:09:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:09:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:09:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:09:37 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:09:38 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 20:10:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:10:03 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5c630fa6465ea72ddec15fd68bdd45a6da6fa4b1981895bf7c2852eedf066194`  
		Last Modified: Sat, 01 Feb 2020 16:48:58 GMT  
		Size: 20.4 MB (20385851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaa324c835efe4fe5ac3f0b479d4adcb40046011bef28007c8c399f15705879`  
		Last Modified: Sat, 01 Feb 2020 20:13:39 GMT  
		Size: 6.5 MB (6526685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6646730906734e461b2a9c00c1251ff85515f5fa90cc4ad6b6704a8231c55fe`  
		Last Modified: Sat, 01 Feb 2020 20:14:05 GMT  
		Size: 86.3 MB (86295089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.1-stretch` - linux; 386

```console
$ docker pull julia@sha256:80af7ef3c4f85fc04cbfa89589a63190f25e1f777664ff9df018dd2def1d5c1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (130011823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3b9bf8739ffa78559670835476d3ecc66c66598265715bdc8f0a0841ed6579`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:48:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:48:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:48:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:48:37 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:48:38 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 17:48:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:48:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3eada1d3458b1595fb3469dbe1f9a16519fe362c19186c018a3f71a94b9b38`  
		Last Modified: Sat, 01 Feb 2020 17:51:37 GMT  
		Size: 7.6 MB (7582401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4259c4d7471ff49be69dbeb9e909fbfe48ba5fb8252a848e9634ba0b6ec8dbc8`  
		Last Modified: Sat, 01 Feb 2020 17:52:03 GMT  
		Size: 99.3 MB (99277266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3.1-windowsservercore-1809`

```console
$ docker pull julia@sha256:b56bf68490e4fd22c8a85f9f6e74c9f0d225cc26eada8d04f4241022aa63bb0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `julia:1.3.1-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:ed1ddd20b9e1503e39766f617a3422dfed5cf242e396b7f036e15fd934c74800
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2341155050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97fec4e1fe1475c22c92fdf8fdf98346ba2396bc7ca1e0acba21fe0e0ece4632`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Jan 2020 19:15:23 GMT
ENV JULIA_VERSION=1.3.1
# Wed, 29 Jan 2020 19:15:25 GMT
ENV JULIA_SHA256=8350ca66f80484c5ca6f7341ffbdb9d5182f8d4231762d585e229567b227ef7f
# Thu, 30 Jan 2020 03:15:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:15:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7726a80f05eaa520d72fca444791156a10b3834f6597ac83b61cb27fb3200101`  
		Last Modified: Wed, 29 Jan 2020 19:21:59 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20f6546d9098b8dba4542af815fe5cae976db3c5a520a5579778229dc6b173e`  
		Last Modified: Wed, 29 Jan 2020 19:21:59 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669caefcaa1628658892b7d2bed49af0e63f523b8ece9f911791d36e5b66b366`  
		Last Modified: Thu, 30 Jan 2020 03:28:24 GMT  
		Size: 123.7 MB (123739167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab655bda7afc3539a1ddf6e38766e8e7e09bf4f25c113148bc7bfc595387b2e3`  
		Last Modified: Thu, 30 Jan 2020 03:27:52 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3.1-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:f93277d40384cf15a6fc5e58494cf63394343441256ecd08917e863fa489730e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `julia:1.3.1-windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:30236875171e7c6d54f8d55583330862e9a5db937ab63e55693d8ac33d574dea
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5853668011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a85a381283d750122455d795be2c7ea0996113ffdcd598f2faf84234f380bebb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 17:20:16 GMT
ENV JULIA_VERSION=1.3.1
# Wed, 15 Jan 2020 17:20:18 GMT
ENV JULIA_SHA256=8350ca66f80484c5ca6f7341ffbdb9d5182f8d4231762d585e229567b227ef7f
# Thu, 30 Jan 2020 03:12:43 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:12:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453d305ccea93f036fe51fd37293fd5aee64f8fe68c1096ce6591cf82c005f76`  
		Last Modified: Wed, 15 Jan 2020 17:28:28 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0318d1ad0420adf48ddb3a4911d306b810a69a68a75f1889bd72e2732e98f7d`  
		Last Modified: Wed, 15 Jan 2020 17:28:28 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bbb3d35fcc68e71a0cb1c0f23d09c911dddf22f436026370aad50a8cd14bf3`  
		Last Modified: Thu, 30 Jan 2020 03:26:55 GMT  
		Size: 129.1 MB (129063927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc05b01cfc9f41d5736018505f631cbd708ac93d6ea62c81857f67926cc0645`  
		Last Modified: Thu, 30 Jan 2020 03:26:18 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3-buster`

```console
$ docker pull julia@sha256:62facc73cdbfb1f431d0c1ff66ff637e8d12cb68be0f9b3844c6af16e7b0e21f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.3-buster` - linux; amd64

```console
$ docker pull julia@sha256:2f5edda11e40572230ad37cd4b2923b827b155c4542a6312caec61adb179584b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.9 MB (134893337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f13978756f05b96ca25ea4d71c6589914a77ddf2e349a3761d0367eb55fa0b9`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Jan 2020 01:23:44 GMT
ENV JULIA_VERSION=1.3.1
# Tue, 07 Jan 2020 23:22:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Jan 2020 23:22:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ff93c6b9676e267b87b0701ae8a4a1fd15469fb6cb775bfe0482c05895c54a`  
		Last Modified: Tue, 07 Jan 2020 23:23:13 GMT  
		Size: 103.4 MB (103364524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:1bfe9380ebd44f7fd18c3290a71e25f6278faa39c77562e1b18d3e9b119c7732
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120290287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4595b8f6040b4ad375efa056027ac9e606ee0ae623de6a3c7a706ca5e5898da4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:34:09 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 18:34:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:34:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc33c18856b9c29ce25a2e310ac0179b18efac98365c421059a8fa3a5dac678c`  
		Last Modified: Sat, 01 Feb 2020 18:39:18 GMT  
		Size: 93.8 MB (93807611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:1a4c0eb118408134679edff728394cbe99b4c4212746134bf8f04f0e2b6a2160
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116459413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a110dfa96e9ee5fa149a28e84c761cf44dd66e0f917a088d76555c083730b1a9`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:08:31 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 20:08:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:09:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99145e615c9c0a7c5aeafdd370a317ac277725ebc627ebb11d0a1c8f52a0c59`  
		Last Modified: Sat, 01 Feb 2020 20:13:29 GMT  
		Size: 86.3 MB (86293332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3-buster` - linux; 386

```console
$ docker pull julia@sha256:15adafbd1bfc00363d5b663c28446058a374b89be8e9fca338aa3c8cdcab0fa7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131608207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a30e007a155af8717d6b257bc5496c6212ad47689fda6e7f4ec0d02094817f19`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:48:00 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 17:48:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:48:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0d35c9e0909ce80f8e46e986854da5cd06baece621bb8529d4ab7cd66e6c2b`  
		Last Modified: Sat, 01 Feb 2020 17:51:28 GMT  
		Size: 99.3 MB (99274918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3-stretch`

```console
$ docker pull julia@sha256:733cffa80bf37f47d4d2de3cb28a40a3e06d86b21de64ee06991829722396939
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.3-stretch` - linux; amd64

```console
$ docker pull julia@sha256:f16498d133d157f29bd5fefe385f482fbfc0c81ef8b889866989dacdc0bd4bae
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133452200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b507aa80fa4adf054832444d789687c311b4923b77be08f9567fb2c1de1d93c`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:47 GMT
ADD file:90a2c81769a336bed3f731f44a385f2a65b0916f517a0b77c06c224579bf9a9a in / 
# Sat, 28 Dec 2019 04:23:47 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:54:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:54:37 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:54:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:54:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Jan 2020 01:24:05 GMT
ENV JULIA_VERSION=1.3.1
# Tue, 07 Jan 2020 23:22:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Jan 2020 23:22:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:804555ee037604c40de144f9f8da0d826d38db82f15d74cded32790fe279a8f6`  
		Last Modified: Sat, 28 Dec 2019 04:28:38 GMT  
		Size: 22.5 MB (22524609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6aef362d0b91076dc5819a1b925f776504ec063851be5395cadb471b9f3881e`  
		Last Modified: Sat, 28 Dec 2019 13:57:02 GMT  
		Size: 7.6 MB (7555513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71672730cf04ca165569336fedcecf18f18fa7af5bb68b0269336d2cf0104e6d`  
		Last Modified: Tue, 07 Jan 2020 23:23:49 GMT  
		Size: 103.4 MB (103372078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:c96aa5ec4099d65d449554fe6255b743ea25cfab5a1aa847a3cffca734f0f0ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119407020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:facee1409787ff6bc644dbfa70a17b807cf03b1a47fae35a99ecd4234ab3e1fa`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:29 GMT
ADD file:6ac430a42a1f2a6cc8b0a3565e518bd0e3a47b01d524b86cd3dd4e7f4606fd53 in / 
# Sat, 01 Feb 2020 17:04:31 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:35:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:35:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:35:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:35:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:35:14 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 18:35:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:35:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6bc458b0813423b9e351a5604c0d71a4853d970ea22b23fedc8683af12dbc13c`  
		Last Modified: Sat, 01 Feb 2020 17:11:31 GMT  
		Size: 19.3 MB (19311624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9840e48d64ced9020e882cefaf8fe5cd26dc391522b6acd18cd09eccad69e07`  
		Last Modified: Sat, 01 Feb 2020 18:39:27 GMT  
		Size: 6.3 MB (6292143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8331cb5b72ee568b3cf598db9f378382b4cc073daabb288e06f54994ca3f6ae7`  
		Last Modified: Sat, 01 Feb 2020 18:39:55 GMT  
		Size: 93.8 MB (93803253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:96635540f0bc528b39750e2c03177d4e85a1bb1c080981eb64742ed7d690f4ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113207625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:877782fd5d403c41cd3e8bd8175bba4fc79ed5a1a96a15b1715dba7334a7740b`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:d3338eed8ee88c2a5856cc2eb73701e4de79a7e551602df07834a1ad4f671435 in / 
# Sat, 01 Feb 2020 16:43:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:09:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:09:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:09:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:09:37 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:09:38 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 20:10:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:10:03 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5c630fa6465ea72ddec15fd68bdd45a6da6fa4b1981895bf7c2852eedf066194`  
		Last Modified: Sat, 01 Feb 2020 16:48:58 GMT  
		Size: 20.4 MB (20385851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaa324c835efe4fe5ac3f0b479d4adcb40046011bef28007c8c399f15705879`  
		Last Modified: Sat, 01 Feb 2020 20:13:39 GMT  
		Size: 6.5 MB (6526685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6646730906734e461b2a9c00c1251ff85515f5fa90cc4ad6b6704a8231c55fe`  
		Last Modified: Sat, 01 Feb 2020 20:14:05 GMT  
		Size: 86.3 MB (86295089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3-stretch` - linux; 386

```console
$ docker pull julia@sha256:80af7ef3c4f85fc04cbfa89589a63190f25e1f777664ff9df018dd2def1d5c1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (130011823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3b9bf8739ffa78559670835476d3ecc66c66598265715bdc8f0a0841ed6579`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:48:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:48:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:48:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:48:37 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:48:38 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 17:48:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:48:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3eada1d3458b1595fb3469dbe1f9a16519fe362c19186c018a3f71a94b9b38`  
		Last Modified: Sat, 01 Feb 2020 17:51:37 GMT  
		Size: 7.6 MB (7582401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4259c4d7471ff49be69dbeb9e909fbfe48ba5fb8252a848e9634ba0b6ec8dbc8`  
		Last Modified: Sat, 01 Feb 2020 17:52:03 GMT  
		Size: 99.3 MB (99277266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3-windowsservercore-1809`

```console
$ docker pull julia@sha256:b56bf68490e4fd22c8a85f9f6e74c9f0d225cc26eada8d04f4241022aa63bb0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `julia:1.3-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:ed1ddd20b9e1503e39766f617a3422dfed5cf242e396b7f036e15fd934c74800
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2341155050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97fec4e1fe1475c22c92fdf8fdf98346ba2396bc7ca1e0acba21fe0e0ece4632`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Jan 2020 19:15:23 GMT
ENV JULIA_VERSION=1.3.1
# Wed, 29 Jan 2020 19:15:25 GMT
ENV JULIA_SHA256=8350ca66f80484c5ca6f7341ffbdb9d5182f8d4231762d585e229567b227ef7f
# Thu, 30 Jan 2020 03:15:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:15:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7726a80f05eaa520d72fca444791156a10b3834f6597ac83b61cb27fb3200101`  
		Last Modified: Wed, 29 Jan 2020 19:21:59 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20f6546d9098b8dba4542af815fe5cae976db3c5a520a5579778229dc6b173e`  
		Last Modified: Wed, 29 Jan 2020 19:21:59 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669caefcaa1628658892b7d2bed49af0e63f523b8ece9f911791d36e5b66b366`  
		Last Modified: Thu, 30 Jan 2020 03:28:24 GMT  
		Size: 123.7 MB (123739167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab655bda7afc3539a1ddf6e38766e8e7e09bf4f25c113148bc7bfc595387b2e3`  
		Last Modified: Thu, 30 Jan 2020 03:27:52 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:f93277d40384cf15a6fc5e58494cf63394343441256ecd08917e863fa489730e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `julia:1.3-windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:30236875171e7c6d54f8d55583330862e9a5db937ab63e55693d8ac33d574dea
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5853668011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a85a381283d750122455d795be2c7ea0996113ffdcd598f2faf84234f380bebb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 17:20:16 GMT
ENV JULIA_VERSION=1.3.1
# Wed, 15 Jan 2020 17:20:18 GMT
ENV JULIA_SHA256=8350ca66f80484c5ca6f7341ffbdb9d5182f8d4231762d585e229567b227ef7f
# Thu, 30 Jan 2020 03:12:43 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:12:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453d305ccea93f036fe51fd37293fd5aee64f8fe68c1096ce6591cf82c005f76`  
		Last Modified: Wed, 15 Jan 2020 17:28:28 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0318d1ad0420adf48ddb3a4911d306b810a69a68a75f1889bd72e2732e98f7d`  
		Last Modified: Wed, 15 Jan 2020 17:28:28 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bbb3d35fcc68e71a0cb1c0f23d09c911dddf22f436026370aad50a8cd14bf3`  
		Last Modified: Thu, 30 Jan 2020 03:26:55 GMT  
		Size: 129.1 MB (129063927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc05b01cfc9f41d5736018505f631cbd708ac93d6ea62c81857f67926cc0645`  
		Last Modified: Thu, 30 Jan 2020 03:26:18 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4`

```console
$ docker pull julia@sha256:6e67e53923b8b42dfd8e9644065e6f89c556b2b5e1aecf46e4307d0d50f42bb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3443; amd64
	-	windows version 10.0.17763.973; amd64

### `julia:1.4` - linux; amd64

```console
$ docker pull julia@sha256:26e05991ad2784d52dfbc9b3f9ddd3bbbe14918ff3de95d973d43c4f29a5ffa6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137972998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb7a22ebcff368474e0de1b9f8974a3e06c7d1eab0b806e12e9c02f43b5c7d82`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 30 Jan 2020 02:19:37 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 02:19:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 30 Jan 2020 02:19:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524f70c49516c7568c039fd5b3b1b0919d7c83a73eb83816d02d30322d2fe6e1`  
		Last Modified: Thu, 30 Jan 2020 02:20:38 GMT  
		Size: 106.4 MB (106444185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4` - linux; arm variant v7

```console
$ docker pull julia@sha256:8a954e215423396846a6bf3f7a20edd7040e2a478442e0b8ba9858b9cdba85d5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123188966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb27f1eb6324be2a1cdd4aa7a9aa55c9acd36ab353156ffbc44b0931f3b53ad4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:33:23 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 18:33:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:33:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9324c8e014d9183150a1d11982cb169f4c44d13d2f393dfb91d167d0a8b31f`  
		Last Modified: Sat, 01 Feb 2020 18:38:35 GMT  
		Size: 96.7 MB (96706290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:f4585ee7b9a1a5b34c33a2d157c6709dbfe8cdce7adbf872afe4ef614c45b7d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119460610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7013f15be6f586d42cd9f1594a4b0ee12aba8607ebbc4bba86830a64b1b029e`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 20:08:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:08:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75506d725ccc6f9f17f4222959f216d3bee3944278981f37daca366cb3881c3`  
		Last Modified: Sat, 01 Feb 2020 20:12:53 GMT  
		Size: 89.3 MB (89294529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4` - linux; 386

```console
$ docker pull julia@sha256:4ef5a19cba48c3cc6af71a93b505901b0765307fefe967d08aa99865e7332e7e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135625924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af27c6c53789c4558eb65b4e59ce29123cc6de5139d173dbf4ce93aab854431a`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:47:32 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 17:47:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:47:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b4bb9e23c25e585467e1e235b9a6ca199c106976763a371043f2d7262289d2`  
		Last Modified: Sat, 01 Feb 2020 17:50:54 GMT  
		Size: 103.3 MB (103292635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:e99fa82eacfa9fb0d094e235cb0ce9e517af1f65c788b80e1302e3f110707f13
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5858705045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288f7450b14e7fb17cf7b70f703704a83e9f2893f58e0030f5d3cee81990397c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:02:24 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:02:25 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:05:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:05:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f44cf0312dbd62091dc5611083af53d7021ab979b3df9b05b6854ef12f8e76`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c3a9f637a43e81937bf39dc605098a2f0f2de44dc9883135dd1b1c77519db0`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80b8180e7ef10811cee9b9511c448255de8256ab5ca210f54b8054fb431f28`  
		Last Modified: Thu, 30 Jan 2020 03:24:01 GMT  
		Size: 134.1 MB (134100992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311e8adf83d3f4e49b437398db4e37c9abee5e3c43b06d1b692967b413d7e340`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:79b07715ea0d9fa827f0b465bb1ac7d8ba3ab96d130e88387d9a9d6681ea9170
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2346192159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f8198badbdfffd2e66aee0424c9f518a65b069ec796412c87f67e19caca4d8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:06:13 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:06:14 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:08:53 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:08:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860f7399498f1f144e2d9602758eb16c4e5021fa1fa32d157280506fdfa0c11d`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d6f370ff6bdfcfabe7c80d94802ad8170225c886dff031288ca1faa7377585`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6bb3b070d7f8e9b598db5889d8a124791eab7dd08199e9c2d6411432cfb597`  
		Last Modified: Thu, 30 Jan 2020 03:25:30 GMT  
		Size: 128.8 MB (128776203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff6dba759626604108e222cf0d12036d48bcb992cb40676f232f6f273306fce`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4.0`

```console
$ docker pull julia@sha256:6e67e53923b8b42dfd8e9644065e6f89c556b2b5e1aecf46e4307d0d50f42bb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3443; amd64
	-	windows version 10.0.17763.973; amd64

### `julia:1.4.0` - linux; amd64

```console
$ docker pull julia@sha256:26e05991ad2784d52dfbc9b3f9ddd3bbbe14918ff3de95d973d43c4f29a5ffa6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137972998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb7a22ebcff368474e0de1b9f8974a3e06c7d1eab0b806e12e9c02f43b5c7d82`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 30 Jan 2020 02:19:37 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 02:19:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 30 Jan 2020 02:19:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524f70c49516c7568c039fd5b3b1b0919d7c83a73eb83816d02d30322d2fe6e1`  
		Last Modified: Thu, 30 Jan 2020 02:20:38 GMT  
		Size: 106.4 MB (106444185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0` - linux; arm variant v7

```console
$ docker pull julia@sha256:8a954e215423396846a6bf3f7a20edd7040e2a478442e0b8ba9858b9cdba85d5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123188966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb27f1eb6324be2a1cdd4aa7a9aa55c9acd36ab353156ffbc44b0931f3b53ad4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:33:23 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 18:33:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:33:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9324c8e014d9183150a1d11982cb169f4c44d13d2f393dfb91d167d0a8b31f`  
		Last Modified: Sat, 01 Feb 2020 18:38:35 GMT  
		Size: 96.7 MB (96706290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:f4585ee7b9a1a5b34c33a2d157c6709dbfe8cdce7adbf872afe4ef614c45b7d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119460610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7013f15be6f586d42cd9f1594a4b0ee12aba8607ebbc4bba86830a64b1b029e`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 20:08:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:08:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75506d725ccc6f9f17f4222959f216d3bee3944278981f37daca366cb3881c3`  
		Last Modified: Sat, 01 Feb 2020 20:12:53 GMT  
		Size: 89.3 MB (89294529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0` - linux; 386

```console
$ docker pull julia@sha256:4ef5a19cba48c3cc6af71a93b505901b0765307fefe967d08aa99865e7332e7e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135625924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af27c6c53789c4558eb65b4e59ce29123cc6de5139d173dbf4ce93aab854431a`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:47:32 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 17:47:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:47:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b4bb9e23c25e585467e1e235b9a6ca199c106976763a371043f2d7262289d2`  
		Last Modified: Sat, 01 Feb 2020 17:50:54 GMT  
		Size: 103.3 MB (103292635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:e99fa82eacfa9fb0d094e235cb0ce9e517af1f65c788b80e1302e3f110707f13
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5858705045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288f7450b14e7fb17cf7b70f703704a83e9f2893f58e0030f5d3cee81990397c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:02:24 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:02:25 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:05:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:05:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f44cf0312dbd62091dc5611083af53d7021ab979b3df9b05b6854ef12f8e76`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c3a9f637a43e81937bf39dc605098a2f0f2de44dc9883135dd1b1c77519db0`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80b8180e7ef10811cee9b9511c448255de8256ab5ca210f54b8054fb431f28`  
		Last Modified: Thu, 30 Jan 2020 03:24:01 GMT  
		Size: 134.1 MB (134100992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311e8adf83d3f4e49b437398db4e37c9abee5e3c43b06d1b692967b413d7e340`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:79b07715ea0d9fa827f0b465bb1ac7d8ba3ab96d130e88387d9a9d6681ea9170
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2346192159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f8198badbdfffd2e66aee0424c9f518a65b069ec796412c87f67e19caca4d8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:06:13 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:06:14 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:08:53 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:08:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860f7399498f1f144e2d9602758eb16c4e5021fa1fa32d157280506fdfa0c11d`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d6f370ff6bdfcfabe7c80d94802ad8170225c886dff031288ca1faa7377585`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6bb3b070d7f8e9b598db5889d8a124791eab7dd08199e9c2d6411432cfb597`  
		Last Modified: Thu, 30 Jan 2020 03:25:30 GMT  
		Size: 128.8 MB (128776203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff6dba759626604108e222cf0d12036d48bcb992cb40676f232f6f273306fce`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4.0-buster`

```console
$ docker pull julia@sha256:6bd34fe5a32b5568e0e9dd782c6de54a4d6753bac01b4f6a1f392aa13aa7e269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.4.0-buster` - linux; amd64

```console
$ docker pull julia@sha256:26e05991ad2784d52dfbc9b3f9ddd3bbbe14918ff3de95d973d43c4f29a5ffa6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137972998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb7a22ebcff368474e0de1b9f8974a3e06c7d1eab0b806e12e9c02f43b5c7d82`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 30 Jan 2020 02:19:37 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 02:19:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 30 Jan 2020 02:19:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524f70c49516c7568c039fd5b3b1b0919d7c83a73eb83816d02d30322d2fe6e1`  
		Last Modified: Thu, 30 Jan 2020 02:20:38 GMT  
		Size: 106.4 MB (106444185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:8a954e215423396846a6bf3f7a20edd7040e2a478442e0b8ba9858b9cdba85d5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123188966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb27f1eb6324be2a1cdd4aa7a9aa55c9acd36ab353156ffbc44b0931f3b53ad4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:33:23 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 18:33:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:33:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9324c8e014d9183150a1d11982cb169f4c44d13d2f393dfb91d167d0a8b31f`  
		Last Modified: Sat, 01 Feb 2020 18:38:35 GMT  
		Size: 96.7 MB (96706290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:f4585ee7b9a1a5b34c33a2d157c6709dbfe8cdce7adbf872afe4ef614c45b7d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119460610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7013f15be6f586d42cd9f1594a4b0ee12aba8607ebbc4bba86830a64b1b029e`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 20:08:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:08:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75506d725ccc6f9f17f4222959f216d3bee3944278981f37daca366cb3881c3`  
		Last Modified: Sat, 01 Feb 2020 20:12:53 GMT  
		Size: 89.3 MB (89294529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0-buster` - linux; 386

```console
$ docker pull julia@sha256:4ef5a19cba48c3cc6af71a93b505901b0765307fefe967d08aa99865e7332e7e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135625924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af27c6c53789c4558eb65b4e59ce29123cc6de5139d173dbf4ce93aab854431a`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:47:32 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 17:47:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:47:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b4bb9e23c25e585467e1e235b9a6ca199c106976763a371043f2d7262289d2`  
		Last Modified: Sat, 01 Feb 2020 17:50:54 GMT  
		Size: 103.3 MB (103292635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4.0-rc1`

```console
$ docker pull julia@sha256:6e67e53923b8b42dfd8e9644065e6f89c556b2b5e1aecf46e4307d0d50f42bb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3443; amd64
	-	windows version 10.0.17763.973; amd64

### `julia:1.4.0-rc1` - linux; amd64

```console
$ docker pull julia@sha256:26e05991ad2784d52dfbc9b3f9ddd3bbbe14918ff3de95d973d43c4f29a5ffa6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137972998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb7a22ebcff368474e0de1b9f8974a3e06c7d1eab0b806e12e9c02f43b5c7d82`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 30 Jan 2020 02:19:37 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 02:19:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 30 Jan 2020 02:19:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524f70c49516c7568c039fd5b3b1b0919d7c83a73eb83816d02d30322d2fe6e1`  
		Last Modified: Thu, 30 Jan 2020 02:20:38 GMT  
		Size: 106.4 MB (106444185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0-rc1` - linux; arm variant v7

```console
$ docker pull julia@sha256:8a954e215423396846a6bf3f7a20edd7040e2a478442e0b8ba9858b9cdba85d5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123188966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb27f1eb6324be2a1cdd4aa7a9aa55c9acd36ab353156ffbc44b0931f3b53ad4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:33:23 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 18:33:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:33:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9324c8e014d9183150a1d11982cb169f4c44d13d2f393dfb91d167d0a8b31f`  
		Last Modified: Sat, 01 Feb 2020 18:38:35 GMT  
		Size: 96.7 MB (96706290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0-rc1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:f4585ee7b9a1a5b34c33a2d157c6709dbfe8cdce7adbf872afe4ef614c45b7d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119460610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7013f15be6f586d42cd9f1594a4b0ee12aba8607ebbc4bba86830a64b1b029e`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 20:08:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:08:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75506d725ccc6f9f17f4222959f216d3bee3944278981f37daca366cb3881c3`  
		Last Modified: Sat, 01 Feb 2020 20:12:53 GMT  
		Size: 89.3 MB (89294529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0-rc1` - linux; 386

```console
$ docker pull julia@sha256:4ef5a19cba48c3cc6af71a93b505901b0765307fefe967d08aa99865e7332e7e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135625924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af27c6c53789c4558eb65b4e59ce29123cc6de5139d173dbf4ce93aab854431a`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:47:32 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 17:47:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:47:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b4bb9e23c25e585467e1e235b9a6ca199c106976763a371043f2d7262289d2`  
		Last Modified: Sat, 01 Feb 2020 17:50:54 GMT  
		Size: 103.3 MB (103292635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0-rc1` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:e99fa82eacfa9fb0d094e235cb0ce9e517af1f65c788b80e1302e3f110707f13
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5858705045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288f7450b14e7fb17cf7b70f703704a83e9f2893f58e0030f5d3cee81990397c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:02:24 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:02:25 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:05:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:05:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f44cf0312dbd62091dc5611083af53d7021ab979b3df9b05b6854ef12f8e76`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c3a9f637a43e81937bf39dc605098a2f0f2de44dc9883135dd1b1c77519db0`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80b8180e7ef10811cee9b9511c448255de8256ab5ca210f54b8054fb431f28`  
		Last Modified: Thu, 30 Jan 2020 03:24:01 GMT  
		Size: 134.1 MB (134100992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311e8adf83d3f4e49b437398db4e37c9abee5e3c43b06d1b692967b413d7e340`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0-rc1` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:79b07715ea0d9fa827f0b465bb1ac7d8ba3ab96d130e88387d9a9d6681ea9170
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2346192159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f8198badbdfffd2e66aee0424c9f518a65b069ec796412c87f67e19caca4d8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:06:13 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:06:14 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:08:53 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:08:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860f7399498f1f144e2d9602758eb16c4e5021fa1fa32d157280506fdfa0c11d`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d6f370ff6bdfcfabe7c80d94802ad8170225c886dff031288ca1faa7377585`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6bb3b070d7f8e9b598db5889d8a124791eab7dd08199e9c2d6411432cfb597`  
		Last Modified: Thu, 30 Jan 2020 03:25:30 GMT  
		Size: 128.8 MB (128776203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff6dba759626604108e222cf0d12036d48bcb992cb40676f232f6f273306fce`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4.0-rc1-buster`

```console
$ docker pull julia@sha256:6bd34fe5a32b5568e0e9dd782c6de54a4d6753bac01b4f6a1f392aa13aa7e269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.4.0-rc1-buster` - linux; amd64

```console
$ docker pull julia@sha256:26e05991ad2784d52dfbc9b3f9ddd3bbbe14918ff3de95d973d43c4f29a5ffa6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137972998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb7a22ebcff368474e0de1b9f8974a3e06c7d1eab0b806e12e9c02f43b5c7d82`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 30 Jan 2020 02:19:37 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 02:19:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 30 Jan 2020 02:19:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524f70c49516c7568c039fd5b3b1b0919d7c83a73eb83816d02d30322d2fe6e1`  
		Last Modified: Thu, 30 Jan 2020 02:20:38 GMT  
		Size: 106.4 MB (106444185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0-rc1-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:8a954e215423396846a6bf3f7a20edd7040e2a478442e0b8ba9858b9cdba85d5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123188966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb27f1eb6324be2a1cdd4aa7a9aa55c9acd36ab353156ffbc44b0931f3b53ad4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:33:23 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 18:33:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:33:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9324c8e014d9183150a1d11982cb169f4c44d13d2f393dfb91d167d0a8b31f`  
		Last Modified: Sat, 01 Feb 2020 18:38:35 GMT  
		Size: 96.7 MB (96706290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0-rc1-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:f4585ee7b9a1a5b34c33a2d157c6709dbfe8cdce7adbf872afe4ef614c45b7d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119460610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7013f15be6f586d42cd9f1594a4b0ee12aba8607ebbc4bba86830a64b1b029e`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 20:08:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:08:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75506d725ccc6f9f17f4222959f216d3bee3944278981f37daca366cb3881c3`  
		Last Modified: Sat, 01 Feb 2020 20:12:53 GMT  
		Size: 89.3 MB (89294529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0-rc1-buster` - linux; 386

```console
$ docker pull julia@sha256:4ef5a19cba48c3cc6af71a93b505901b0765307fefe967d08aa99865e7332e7e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135625924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af27c6c53789c4558eb65b4e59ce29123cc6de5139d173dbf4ce93aab854431a`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:47:32 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 17:47:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:47:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b4bb9e23c25e585467e1e235b9a6ca199c106976763a371043f2d7262289d2`  
		Last Modified: Sat, 01 Feb 2020 17:50:54 GMT  
		Size: 103.3 MB (103292635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4.0-rc1-windowsservercore-1809`

```console
$ docker pull julia@sha256:bef5d8cd36dc27d6293dfe4f64541614eba9bdcf293262c0165fcbbd67fb42d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `julia:1.4.0-rc1-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:79b07715ea0d9fa827f0b465bb1ac7d8ba3ab96d130e88387d9a9d6681ea9170
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2346192159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f8198badbdfffd2e66aee0424c9f518a65b069ec796412c87f67e19caca4d8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:06:13 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:06:14 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:08:53 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:08:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860f7399498f1f144e2d9602758eb16c4e5021fa1fa32d157280506fdfa0c11d`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d6f370ff6bdfcfabe7c80d94802ad8170225c886dff031288ca1faa7377585`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6bb3b070d7f8e9b598db5889d8a124791eab7dd08199e9c2d6411432cfb597`  
		Last Modified: Thu, 30 Jan 2020 03:25:30 GMT  
		Size: 128.8 MB (128776203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff6dba759626604108e222cf0d12036d48bcb992cb40676f232f6f273306fce`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4.0-rc1-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:8d8f89f035b02a84ad85e98b07bad9b5479ce8c4c38f4eee80fdbcc7337ae3c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `julia:1.4.0-rc1-windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:e99fa82eacfa9fb0d094e235cb0ce9e517af1f65c788b80e1302e3f110707f13
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5858705045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288f7450b14e7fb17cf7b70f703704a83e9f2893f58e0030f5d3cee81990397c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:02:24 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:02:25 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:05:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:05:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f44cf0312dbd62091dc5611083af53d7021ab979b3df9b05b6854ef12f8e76`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c3a9f637a43e81937bf39dc605098a2f0f2de44dc9883135dd1b1c77519db0`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80b8180e7ef10811cee9b9511c448255de8256ab5ca210f54b8054fb431f28`  
		Last Modified: Thu, 30 Jan 2020 03:24:01 GMT  
		Size: 134.1 MB (134100992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311e8adf83d3f4e49b437398db4e37c9abee5e3c43b06d1b692967b413d7e340`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4.0-windowsservercore-1809`

```console
$ docker pull julia@sha256:bef5d8cd36dc27d6293dfe4f64541614eba9bdcf293262c0165fcbbd67fb42d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `julia:1.4.0-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:79b07715ea0d9fa827f0b465bb1ac7d8ba3ab96d130e88387d9a9d6681ea9170
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2346192159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f8198badbdfffd2e66aee0424c9f518a65b069ec796412c87f67e19caca4d8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:06:13 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:06:14 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:08:53 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:08:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860f7399498f1f144e2d9602758eb16c4e5021fa1fa32d157280506fdfa0c11d`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d6f370ff6bdfcfabe7c80d94802ad8170225c886dff031288ca1faa7377585`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6bb3b070d7f8e9b598db5889d8a124791eab7dd08199e9c2d6411432cfb597`  
		Last Modified: Thu, 30 Jan 2020 03:25:30 GMT  
		Size: 128.8 MB (128776203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff6dba759626604108e222cf0d12036d48bcb992cb40676f232f6f273306fce`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4.0-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:8d8f89f035b02a84ad85e98b07bad9b5479ce8c4c38f4eee80fdbcc7337ae3c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `julia:1.4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:e99fa82eacfa9fb0d094e235cb0ce9e517af1f65c788b80e1302e3f110707f13
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5858705045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288f7450b14e7fb17cf7b70f703704a83e9f2893f58e0030f5d3cee81990397c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:02:24 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:02:25 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:05:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:05:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f44cf0312dbd62091dc5611083af53d7021ab979b3df9b05b6854ef12f8e76`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c3a9f637a43e81937bf39dc605098a2f0f2de44dc9883135dd1b1c77519db0`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80b8180e7ef10811cee9b9511c448255de8256ab5ca210f54b8054fb431f28`  
		Last Modified: Thu, 30 Jan 2020 03:24:01 GMT  
		Size: 134.1 MB (134100992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311e8adf83d3f4e49b437398db4e37c9abee5e3c43b06d1b692967b413d7e340`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4-buster`

```console
$ docker pull julia@sha256:6bd34fe5a32b5568e0e9dd782c6de54a4d6753bac01b4f6a1f392aa13aa7e269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.4-buster` - linux; amd64

```console
$ docker pull julia@sha256:26e05991ad2784d52dfbc9b3f9ddd3bbbe14918ff3de95d973d43c4f29a5ffa6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137972998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb7a22ebcff368474e0de1b9f8974a3e06c7d1eab0b806e12e9c02f43b5c7d82`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 30 Jan 2020 02:19:37 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 02:19:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 30 Jan 2020 02:19:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524f70c49516c7568c039fd5b3b1b0919d7c83a73eb83816d02d30322d2fe6e1`  
		Last Modified: Thu, 30 Jan 2020 02:20:38 GMT  
		Size: 106.4 MB (106444185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:8a954e215423396846a6bf3f7a20edd7040e2a478442e0b8ba9858b9cdba85d5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123188966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb27f1eb6324be2a1cdd4aa7a9aa55c9acd36ab353156ffbc44b0931f3b53ad4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:33:23 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 18:33:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:33:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9324c8e014d9183150a1d11982cb169f4c44d13d2f393dfb91d167d0a8b31f`  
		Last Modified: Sat, 01 Feb 2020 18:38:35 GMT  
		Size: 96.7 MB (96706290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:f4585ee7b9a1a5b34c33a2d157c6709dbfe8cdce7adbf872afe4ef614c45b7d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119460610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7013f15be6f586d42cd9f1594a4b0ee12aba8607ebbc4bba86830a64b1b029e`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 20:08:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:08:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75506d725ccc6f9f17f4222959f216d3bee3944278981f37daca366cb3881c3`  
		Last Modified: Sat, 01 Feb 2020 20:12:53 GMT  
		Size: 89.3 MB (89294529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4-buster` - linux; 386

```console
$ docker pull julia@sha256:4ef5a19cba48c3cc6af71a93b505901b0765307fefe967d08aa99865e7332e7e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135625924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af27c6c53789c4558eb65b4e59ce29123cc6de5139d173dbf4ce93aab854431a`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:47:32 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 17:47:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:47:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b4bb9e23c25e585467e1e235b9a6ca199c106976763a371043f2d7262289d2`  
		Last Modified: Sat, 01 Feb 2020 17:50:54 GMT  
		Size: 103.3 MB (103292635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4-rc`

```console
$ docker pull julia@sha256:6e67e53923b8b42dfd8e9644065e6f89c556b2b5e1aecf46e4307d0d50f42bb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3443; amd64
	-	windows version 10.0.17763.973; amd64

### `julia:1.4-rc` - linux; amd64

```console
$ docker pull julia@sha256:26e05991ad2784d52dfbc9b3f9ddd3bbbe14918ff3de95d973d43c4f29a5ffa6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137972998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb7a22ebcff368474e0de1b9f8974a3e06c7d1eab0b806e12e9c02f43b5c7d82`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 30 Jan 2020 02:19:37 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 02:19:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 30 Jan 2020 02:19:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524f70c49516c7568c039fd5b3b1b0919d7c83a73eb83816d02d30322d2fe6e1`  
		Last Modified: Thu, 30 Jan 2020 02:20:38 GMT  
		Size: 106.4 MB (106444185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4-rc` - linux; arm variant v7

```console
$ docker pull julia@sha256:8a954e215423396846a6bf3f7a20edd7040e2a478442e0b8ba9858b9cdba85d5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123188966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb27f1eb6324be2a1cdd4aa7a9aa55c9acd36ab353156ffbc44b0931f3b53ad4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:33:23 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 18:33:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:33:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9324c8e014d9183150a1d11982cb169f4c44d13d2f393dfb91d167d0a8b31f`  
		Last Modified: Sat, 01 Feb 2020 18:38:35 GMT  
		Size: 96.7 MB (96706290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4-rc` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:f4585ee7b9a1a5b34c33a2d157c6709dbfe8cdce7adbf872afe4ef614c45b7d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119460610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7013f15be6f586d42cd9f1594a4b0ee12aba8607ebbc4bba86830a64b1b029e`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 20:08:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:08:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75506d725ccc6f9f17f4222959f216d3bee3944278981f37daca366cb3881c3`  
		Last Modified: Sat, 01 Feb 2020 20:12:53 GMT  
		Size: 89.3 MB (89294529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4-rc` - linux; 386

```console
$ docker pull julia@sha256:4ef5a19cba48c3cc6af71a93b505901b0765307fefe967d08aa99865e7332e7e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135625924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af27c6c53789c4558eb65b4e59ce29123cc6de5139d173dbf4ce93aab854431a`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:47:32 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 17:47:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:47:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b4bb9e23c25e585467e1e235b9a6ca199c106976763a371043f2d7262289d2`  
		Last Modified: Sat, 01 Feb 2020 17:50:54 GMT  
		Size: 103.3 MB (103292635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4-rc` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:e99fa82eacfa9fb0d094e235cb0ce9e517af1f65c788b80e1302e3f110707f13
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5858705045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288f7450b14e7fb17cf7b70f703704a83e9f2893f58e0030f5d3cee81990397c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:02:24 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:02:25 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:05:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:05:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f44cf0312dbd62091dc5611083af53d7021ab979b3df9b05b6854ef12f8e76`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c3a9f637a43e81937bf39dc605098a2f0f2de44dc9883135dd1b1c77519db0`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80b8180e7ef10811cee9b9511c448255de8256ab5ca210f54b8054fb431f28`  
		Last Modified: Thu, 30 Jan 2020 03:24:01 GMT  
		Size: 134.1 MB (134100992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311e8adf83d3f4e49b437398db4e37c9abee5e3c43b06d1b692967b413d7e340`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4-rc` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:79b07715ea0d9fa827f0b465bb1ac7d8ba3ab96d130e88387d9a9d6681ea9170
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2346192159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f8198badbdfffd2e66aee0424c9f518a65b069ec796412c87f67e19caca4d8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:06:13 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:06:14 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:08:53 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:08:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860f7399498f1f144e2d9602758eb16c4e5021fa1fa32d157280506fdfa0c11d`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d6f370ff6bdfcfabe7c80d94802ad8170225c886dff031288ca1faa7377585`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6bb3b070d7f8e9b598db5889d8a124791eab7dd08199e9c2d6411432cfb597`  
		Last Modified: Thu, 30 Jan 2020 03:25:30 GMT  
		Size: 128.8 MB (128776203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff6dba759626604108e222cf0d12036d48bcb992cb40676f232f6f273306fce`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4-rc-buster`

```console
$ docker pull julia@sha256:6bd34fe5a32b5568e0e9dd782c6de54a4d6753bac01b4f6a1f392aa13aa7e269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.4-rc-buster` - linux; amd64

```console
$ docker pull julia@sha256:26e05991ad2784d52dfbc9b3f9ddd3bbbe14918ff3de95d973d43c4f29a5ffa6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137972998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb7a22ebcff368474e0de1b9f8974a3e06c7d1eab0b806e12e9c02f43b5c7d82`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 30 Jan 2020 02:19:37 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 02:19:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 30 Jan 2020 02:19:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524f70c49516c7568c039fd5b3b1b0919d7c83a73eb83816d02d30322d2fe6e1`  
		Last Modified: Thu, 30 Jan 2020 02:20:38 GMT  
		Size: 106.4 MB (106444185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4-rc-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:8a954e215423396846a6bf3f7a20edd7040e2a478442e0b8ba9858b9cdba85d5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123188966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb27f1eb6324be2a1cdd4aa7a9aa55c9acd36ab353156ffbc44b0931f3b53ad4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:33:23 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 18:33:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:33:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9324c8e014d9183150a1d11982cb169f4c44d13d2f393dfb91d167d0a8b31f`  
		Last Modified: Sat, 01 Feb 2020 18:38:35 GMT  
		Size: 96.7 MB (96706290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4-rc-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:f4585ee7b9a1a5b34c33a2d157c6709dbfe8cdce7adbf872afe4ef614c45b7d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119460610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7013f15be6f586d42cd9f1594a4b0ee12aba8607ebbc4bba86830a64b1b029e`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 20:08:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:08:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75506d725ccc6f9f17f4222959f216d3bee3944278981f37daca366cb3881c3`  
		Last Modified: Sat, 01 Feb 2020 20:12:53 GMT  
		Size: 89.3 MB (89294529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4-rc-buster` - linux; 386

```console
$ docker pull julia@sha256:4ef5a19cba48c3cc6af71a93b505901b0765307fefe967d08aa99865e7332e7e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135625924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af27c6c53789c4558eb65b4e59ce29123cc6de5139d173dbf4ce93aab854431a`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:47:32 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 17:47:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:47:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b4bb9e23c25e585467e1e235b9a6ca199c106976763a371043f2d7262289d2`  
		Last Modified: Sat, 01 Feb 2020 17:50:54 GMT  
		Size: 103.3 MB (103292635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4-rc-windowsservercore-1809`

```console
$ docker pull julia@sha256:bef5d8cd36dc27d6293dfe4f64541614eba9bdcf293262c0165fcbbd67fb42d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `julia:1.4-rc-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:79b07715ea0d9fa827f0b465bb1ac7d8ba3ab96d130e88387d9a9d6681ea9170
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2346192159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f8198badbdfffd2e66aee0424c9f518a65b069ec796412c87f67e19caca4d8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:06:13 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:06:14 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:08:53 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:08:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860f7399498f1f144e2d9602758eb16c4e5021fa1fa32d157280506fdfa0c11d`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d6f370ff6bdfcfabe7c80d94802ad8170225c886dff031288ca1faa7377585`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6bb3b070d7f8e9b598db5889d8a124791eab7dd08199e9c2d6411432cfb597`  
		Last Modified: Thu, 30 Jan 2020 03:25:30 GMT  
		Size: 128.8 MB (128776203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff6dba759626604108e222cf0d12036d48bcb992cb40676f232f6f273306fce`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4-rc-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:8d8f89f035b02a84ad85e98b07bad9b5479ce8c4c38f4eee80fdbcc7337ae3c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `julia:1.4-rc-windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:e99fa82eacfa9fb0d094e235cb0ce9e517af1f65c788b80e1302e3f110707f13
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5858705045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288f7450b14e7fb17cf7b70f703704a83e9f2893f58e0030f5d3cee81990397c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:02:24 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:02:25 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:05:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:05:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f44cf0312dbd62091dc5611083af53d7021ab979b3df9b05b6854ef12f8e76`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c3a9f637a43e81937bf39dc605098a2f0f2de44dc9883135dd1b1c77519db0`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80b8180e7ef10811cee9b9511c448255de8256ab5ca210f54b8054fb431f28`  
		Last Modified: Thu, 30 Jan 2020 03:24:01 GMT  
		Size: 134.1 MB (134100992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311e8adf83d3f4e49b437398db4e37c9abee5e3c43b06d1b692967b413d7e340`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4-windowsservercore-1809`

```console
$ docker pull julia@sha256:bef5d8cd36dc27d6293dfe4f64541614eba9bdcf293262c0165fcbbd67fb42d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `julia:1.4-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:79b07715ea0d9fa827f0b465bb1ac7d8ba3ab96d130e88387d9a9d6681ea9170
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2346192159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f8198badbdfffd2e66aee0424c9f518a65b069ec796412c87f67e19caca4d8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:06:13 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:06:14 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:08:53 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:08:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860f7399498f1f144e2d9602758eb16c4e5021fa1fa32d157280506fdfa0c11d`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d6f370ff6bdfcfabe7c80d94802ad8170225c886dff031288ca1faa7377585`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6bb3b070d7f8e9b598db5889d8a124791eab7dd08199e9c2d6411432cfb597`  
		Last Modified: Thu, 30 Jan 2020 03:25:30 GMT  
		Size: 128.8 MB (128776203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff6dba759626604108e222cf0d12036d48bcb992cb40676f232f6f273306fce`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:8d8f89f035b02a84ad85e98b07bad9b5479ce8c4c38f4eee80fdbcc7337ae3c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `julia:1.4-windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:e99fa82eacfa9fb0d094e235cb0ce9e517af1f65c788b80e1302e3f110707f13
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5858705045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288f7450b14e7fb17cf7b70f703704a83e9f2893f58e0030f5d3cee81990397c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:02:24 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:02:25 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:05:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:05:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f44cf0312dbd62091dc5611083af53d7021ab979b3df9b05b6854ef12f8e76`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c3a9f637a43e81937bf39dc605098a2f0f2de44dc9883135dd1b1c77519db0`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80b8180e7ef10811cee9b9511c448255de8256ab5ca210f54b8054fb431f28`  
		Last Modified: Thu, 30 Jan 2020 03:24:01 GMT  
		Size: 134.1 MB (134100992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311e8adf83d3f4e49b437398db4e37c9abee5e3c43b06d1b692967b413d7e340`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-buster`

```console
$ docker pull julia@sha256:62facc73cdbfb1f431d0c1ff66ff637e8d12cb68be0f9b3844c6af16e7b0e21f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1-buster` - linux; amd64

```console
$ docker pull julia@sha256:2f5edda11e40572230ad37cd4b2923b827b155c4542a6312caec61adb179584b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.9 MB (134893337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f13978756f05b96ca25ea4d71c6589914a77ddf2e349a3761d0367eb55fa0b9`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Jan 2020 01:23:44 GMT
ENV JULIA_VERSION=1.3.1
# Tue, 07 Jan 2020 23:22:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Jan 2020 23:22:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ff93c6b9676e267b87b0701ae8a4a1fd15469fb6cb775bfe0482c05895c54a`  
		Last Modified: Tue, 07 Jan 2020 23:23:13 GMT  
		Size: 103.4 MB (103364524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:1bfe9380ebd44f7fd18c3290a71e25f6278faa39c77562e1b18d3e9b119c7732
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120290287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4595b8f6040b4ad375efa056027ac9e606ee0ae623de6a3c7a706ca5e5898da4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:34:09 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 18:34:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:34:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc33c18856b9c29ce25a2e310ac0179b18efac98365c421059a8fa3a5dac678c`  
		Last Modified: Sat, 01 Feb 2020 18:39:18 GMT  
		Size: 93.8 MB (93807611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:1a4c0eb118408134679edff728394cbe99b4c4212746134bf8f04f0e2b6a2160
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116459413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a110dfa96e9ee5fa149a28e84c761cf44dd66e0f917a088d76555c083730b1a9`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:08:31 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 20:08:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:09:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99145e615c9c0a7c5aeafdd370a317ac277725ebc627ebb11d0a1c8f52a0c59`  
		Last Modified: Sat, 01 Feb 2020 20:13:29 GMT  
		Size: 86.3 MB (86293332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; 386

```console
$ docker pull julia@sha256:15adafbd1bfc00363d5b663c28446058a374b89be8e9fca338aa3c8cdcab0fa7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131608207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a30e007a155af8717d6b257bc5496c6212ad47689fda6e7f4ec0d02094817f19`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:48:00 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 17:48:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:48:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0d35c9e0909ce80f8e46e986854da5cd06baece621bb8529d4ab7cd66e6c2b`  
		Last Modified: Sat, 01 Feb 2020 17:51:28 GMT  
		Size: 99.3 MB (99274918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-stretch`

```console
$ docker pull julia@sha256:733cffa80bf37f47d4d2de3cb28a40a3e06d86b21de64ee06991829722396939
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1-stretch` - linux; amd64

```console
$ docker pull julia@sha256:f16498d133d157f29bd5fefe385f482fbfc0c81ef8b889866989dacdc0bd4bae
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133452200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b507aa80fa4adf054832444d789687c311b4923b77be08f9567fb2c1de1d93c`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:47 GMT
ADD file:90a2c81769a336bed3f731f44a385f2a65b0916f517a0b77c06c224579bf9a9a in / 
# Sat, 28 Dec 2019 04:23:47 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:54:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:54:37 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:54:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:54:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Jan 2020 01:24:05 GMT
ENV JULIA_VERSION=1.3.1
# Tue, 07 Jan 2020 23:22:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Jan 2020 23:22:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:804555ee037604c40de144f9f8da0d826d38db82f15d74cded32790fe279a8f6`  
		Last Modified: Sat, 28 Dec 2019 04:28:38 GMT  
		Size: 22.5 MB (22524609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6aef362d0b91076dc5819a1b925f776504ec063851be5395cadb471b9f3881e`  
		Last Modified: Sat, 28 Dec 2019 13:57:02 GMT  
		Size: 7.6 MB (7555513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71672730cf04ca165569336fedcecf18f18fa7af5bb68b0269336d2cf0104e6d`  
		Last Modified: Tue, 07 Jan 2020 23:23:49 GMT  
		Size: 103.4 MB (103372078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:c96aa5ec4099d65d449554fe6255b743ea25cfab5a1aa847a3cffca734f0f0ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119407020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:facee1409787ff6bc644dbfa70a17b807cf03b1a47fae35a99ecd4234ab3e1fa`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:29 GMT
ADD file:6ac430a42a1f2a6cc8b0a3565e518bd0e3a47b01d524b86cd3dd4e7f4606fd53 in / 
# Sat, 01 Feb 2020 17:04:31 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:35:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:35:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:35:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:35:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:35:14 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 18:35:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:35:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6bc458b0813423b9e351a5604c0d71a4853d970ea22b23fedc8683af12dbc13c`  
		Last Modified: Sat, 01 Feb 2020 17:11:31 GMT  
		Size: 19.3 MB (19311624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9840e48d64ced9020e882cefaf8fe5cd26dc391522b6acd18cd09eccad69e07`  
		Last Modified: Sat, 01 Feb 2020 18:39:27 GMT  
		Size: 6.3 MB (6292143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8331cb5b72ee568b3cf598db9f378382b4cc073daabb288e06f54994ca3f6ae7`  
		Last Modified: Sat, 01 Feb 2020 18:39:55 GMT  
		Size: 93.8 MB (93803253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:96635540f0bc528b39750e2c03177d4e85a1bb1c080981eb64742ed7d690f4ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113207625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:877782fd5d403c41cd3e8bd8175bba4fc79ed5a1a96a15b1715dba7334a7740b`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:d3338eed8ee88c2a5856cc2eb73701e4de79a7e551602df07834a1ad4f671435 in / 
# Sat, 01 Feb 2020 16:43:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:09:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:09:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:09:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:09:37 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:09:38 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 20:10:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:10:03 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5c630fa6465ea72ddec15fd68bdd45a6da6fa4b1981895bf7c2852eedf066194`  
		Last Modified: Sat, 01 Feb 2020 16:48:58 GMT  
		Size: 20.4 MB (20385851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaa324c835efe4fe5ac3f0b479d4adcb40046011bef28007c8c399f15705879`  
		Last Modified: Sat, 01 Feb 2020 20:13:39 GMT  
		Size: 6.5 MB (6526685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6646730906734e461b2a9c00c1251ff85515f5fa90cc4ad6b6704a8231c55fe`  
		Last Modified: Sat, 01 Feb 2020 20:14:05 GMT  
		Size: 86.3 MB (86295089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-stretch` - linux; 386

```console
$ docker pull julia@sha256:80af7ef3c4f85fc04cbfa89589a63190f25e1f777664ff9df018dd2def1d5c1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (130011823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3b9bf8739ffa78559670835476d3ecc66c66598265715bdc8f0a0841ed6579`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:48:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:48:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:48:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:48:37 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:48:38 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 17:48:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:48:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3eada1d3458b1595fb3469dbe1f9a16519fe362c19186c018a3f71a94b9b38`  
		Last Modified: Sat, 01 Feb 2020 17:51:37 GMT  
		Size: 7.6 MB (7582401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4259c4d7471ff49be69dbeb9e909fbfe48ba5fb8252a848e9634ba0b6ec8dbc8`  
		Last Modified: Sat, 01 Feb 2020 17:52:03 GMT  
		Size: 99.3 MB (99277266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-1809`

```console
$ docker pull julia@sha256:b56bf68490e4fd22c8a85f9f6e74c9f0d225cc26eada8d04f4241022aa63bb0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `julia:1-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:ed1ddd20b9e1503e39766f617a3422dfed5cf242e396b7f036e15fd934c74800
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2341155050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97fec4e1fe1475c22c92fdf8fdf98346ba2396bc7ca1e0acba21fe0e0ece4632`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Jan 2020 19:15:23 GMT
ENV JULIA_VERSION=1.3.1
# Wed, 29 Jan 2020 19:15:25 GMT
ENV JULIA_SHA256=8350ca66f80484c5ca6f7341ffbdb9d5182f8d4231762d585e229567b227ef7f
# Thu, 30 Jan 2020 03:15:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:15:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7726a80f05eaa520d72fca444791156a10b3834f6597ac83b61cb27fb3200101`  
		Last Modified: Wed, 29 Jan 2020 19:21:59 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20f6546d9098b8dba4542af815fe5cae976db3c5a520a5579778229dc6b173e`  
		Last Modified: Wed, 29 Jan 2020 19:21:59 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669caefcaa1628658892b7d2bed49af0e63f523b8ece9f911791d36e5b66b366`  
		Last Modified: Thu, 30 Jan 2020 03:28:24 GMT  
		Size: 123.7 MB (123739167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab655bda7afc3539a1ddf6e38766e8e7e09bf4f25c113148bc7bfc595387b2e3`  
		Last Modified: Thu, 30 Jan 2020 03:27:52 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:f93277d40384cf15a6fc5e58494cf63394343441256ecd08917e863fa489730e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `julia:1-windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:30236875171e7c6d54f8d55583330862e9a5db937ab63e55693d8ac33d574dea
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5853668011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a85a381283d750122455d795be2c7ea0996113ffdcd598f2faf84234f380bebb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 17:20:16 GMT
ENV JULIA_VERSION=1.3.1
# Wed, 15 Jan 2020 17:20:18 GMT
ENV JULIA_SHA256=8350ca66f80484c5ca6f7341ffbdb9d5182f8d4231762d585e229567b227ef7f
# Thu, 30 Jan 2020 03:12:43 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:12:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453d305ccea93f036fe51fd37293fd5aee64f8fe68c1096ce6591cf82c005f76`  
		Last Modified: Wed, 15 Jan 2020 17:28:28 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0318d1ad0420adf48ddb3a4911d306b810a69a68a75f1889bd72e2732e98f7d`  
		Last Modified: Wed, 15 Jan 2020 17:28:28 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bbb3d35fcc68e71a0cb1c0f23d09c911dddf22f436026370aad50a8cd14bf3`  
		Last Modified: Thu, 30 Jan 2020 03:26:55 GMT  
		Size: 129.1 MB (129063927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc05b01cfc9f41d5736018505f631cbd708ac93d6ea62c81857f67926cc0645`  
		Last Modified: Thu, 30 Jan 2020 03:26:18 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:buster`

```console
$ docker pull julia@sha256:62facc73cdbfb1f431d0c1ff66ff637e8d12cb68be0f9b3844c6af16e7b0e21f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:buster` - linux; amd64

```console
$ docker pull julia@sha256:2f5edda11e40572230ad37cd4b2923b827b155c4542a6312caec61adb179584b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.9 MB (134893337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f13978756f05b96ca25ea4d71c6589914a77ddf2e349a3761d0367eb55fa0b9`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Jan 2020 01:23:44 GMT
ENV JULIA_VERSION=1.3.1
# Tue, 07 Jan 2020 23:22:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Jan 2020 23:22:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ff93c6b9676e267b87b0701ae8a4a1fd15469fb6cb775bfe0482c05895c54a`  
		Last Modified: Tue, 07 Jan 2020 23:23:13 GMT  
		Size: 103.4 MB (103364524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:1bfe9380ebd44f7fd18c3290a71e25f6278faa39c77562e1b18d3e9b119c7732
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120290287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4595b8f6040b4ad375efa056027ac9e606ee0ae623de6a3c7a706ca5e5898da4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:34:09 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 18:34:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:34:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc33c18856b9c29ce25a2e310ac0179b18efac98365c421059a8fa3a5dac678c`  
		Last Modified: Sat, 01 Feb 2020 18:39:18 GMT  
		Size: 93.8 MB (93807611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:1a4c0eb118408134679edff728394cbe99b4c4212746134bf8f04f0e2b6a2160
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116459413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a110dfa96e9ee5fa149a28e84c761cf44dd66e0f917a088d76555c083730b1a9`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:08:31 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 20:08:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:09:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99145e615c9c0a7c5aeafdd370a317ac277725ebc627ebb11d0a1c8f52a0c59`  
		Last Modified: Sat, 01 Feb 2020 20:13:29 GMT  
		Size: 86.3 MB (86293332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:15adafbd1bfc00363d5b663c28446058a374b89be8e9fca338aa3c8cdcab0fa7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131608207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a30e007a155af8717d6b257bc5496c6212ad47689fda6e7f4ec0d02094817f19`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:48:00 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 17:48:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:48:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0d35c9e0909ce80f8e46e986854da5cd06baece621bb8529d4ab7cd66e6c2b`  
		Last Modified: Sat, 01 Feb 2020 17:51:28 GMT  
		Size: 99.3 MB (99274918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:latest`

```console
$ docker pull julia@sha256:85176141b17a747a2ab6450f68cba5c8b93a53dc041ad98c63619c7683d3d35e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3443; amd64
	-	windows version 10.0.17763.973; amd64

### `julia:latest` - linux; amd64

```console
$ docker pull julia@sha256:2f5edda11e40572230ad37cd4b2923b827b155c4542a6312caec61adb179584b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.9 MB (134893337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f13978756f05b96ca25ea4d71c6589914a77ddf2e349a3761d0367eb55fa0b9`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Jan 2020 01:23:44 GMT
ENV JULIA_VERSION=1.3.1
# Tue, 07 Jan 2020 23:22:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Jan 2020 23:22:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ff93c6b9676e267b87b0701ae8a4a1fd15469fb6cb775bfe0482c05895c54a`  
		Last Modified: Tue, 07 Jan 2020 23:23:13 GMT  
		Size: 103.4 MB (103364524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm variant v7

```console
$ docker pull julia@sha256:1bfe9380ebd44f7fd18c3290a71e25f6278faa39c77562e1b18d3e9b119c7732
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120290287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4595b8f6040b4ad375efa056027ac9e606ee0ae623de6a3c7a706ca5e5898da4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:34:09 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 18:34:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:34:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc33c18856b9c29ce25a2e310ac0179b18efac98365c421059a8fa3a5dac678c`  
		Last Modified: Sat, 01 Feb 2020 18:39:18 GMT  
		Size: 93.8 MB (93807611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:1a4c0eb118408134679edff728394cbe99b4c4212746134bf8f04f0e2b6a2160
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116459413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a110dfa96e9ee5fa149a28e84c761cf44dd66e0f917a088d76555c083730b1a9`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:08:31 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 20:08:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:09:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99145e615c9c0a7c5aeafdd370a317ac277725ebc627ebb11d0a1c8f52a0c59`  
		Last Modified: Sat, 01 Feb 2020 20:13:29 GMT  
		Size: 86.3 MB (86293332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; 386

```console
$ docker pull julia@sha256:15adafbd1bfc00363d5b663c28446058a374b89be8e9fca338aa3c8cdcab0fa7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131608207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a30e007a155af8717d6b257bc5496c6212ad47689fda6e7f4ec0d02094817f19`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:48:00 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 17:48:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:48:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0d35c9e0909ce80f8e46e986854da5cd06baece621bb8529d4ab7cd66e6c2b`  
		Last Modified: Sat, 01 Feb 2020 17:51:28 GMT  
		Size: 99.3 MB (99274918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:30236875171e7c6d54f8d55583330862e9a5db937ab63e55693d8ac33d574dea
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5853668011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a85a381283d750122455d795be2c7ea0996113ffdcd598f2faf84234f380bebb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 17:20:16 GMT
ENV JULIA_VERSION=1.3.1
# Wed, 15 Jan 2020 17:20:18 GMT
ENV JULIA_SHA256=8350ca66f80484c5ca6f7341ffbdb9d5182f8d4231762d585e229567b227ef7f
# Thu, 30 Jan 2020 03:12:43 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:12:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453d305ccea93f036fe51fd37293fd5aee64f8fe68c1096ce6591cf82c005f76`  
		Last Modified: Wed, 15 Jan 2020 17:28:28 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0318d1ad0420adf48ddb3a4911d306b810a69a68a75f1889bd72e2732e98f7d`  
		Last Modified: Wed, 15 Jan 2020 17:28:28 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bbb3d35fcc68e71a0cb1c0f23d09c911dddf22f436026370aad50a8cd14bf3`  
		Last Modified: Thu, 30 Jan 2020 03:26:55 GMT  
		Size: 129.1 MB (129063927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc05b01cfc9f41d5736018505f631cbd708ac93d6ea62c81857f67926cc0645`  
		Last Modified: Thu, 30 Jan 2020 03:26:18 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:ed1ddd20b9e1503e39766f617a3422dfed5cf242e396b7f036e15fd934c74800
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2341155050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97fec4e1fe1475c22c92fdf8fdf98346ba2396bc7ca1e0acba21fe0e0ece4632`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Jan 2020 19:15:23 GMT
ENV JULIA_VERSION=1.3.1
# Wed, 29 Jan 2020 19:15:25 GMT
ENV JULIA_SHA256=8350ca66f80484c5ca6f7341ffbdb9d5182f8d4231762d585e229567b227ef7f
# Thu, 30 Jan 2020 03:15:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:15:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7726a80f05eaa520d72fca444791156a10b3834f6597ac83b61cb27fb3200101`  
		Last Modified: Wed, 29 Jan 2020 19:21:59 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20f6546d9098b8dba4542af815fe5cae976db3c5a520a5579778229dc6b173e`  
		Last Modified: Wed, 29 Jan 2020 19:21:59 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669caefcaa1628658892b7d2bed49af0e63f523b8ece9f911791d36e5b66b366`  
		Last Modified: Thu, 30 Jan 2020 03:28:24 GMT  
		Size: 123.7 MB (123739167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab655bda7afc3539a1ddf6e38766e8e7e09bf4f25c113148bc7bfc595387b2e3`  
		Last Modified: Thu, 30 Jan 2020 03:27:52 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:rc`

```console
$ docker pull julia@sha256:6e67e53923b8b42dfd8e9644065e6f89c556b2b5e1aecf46e4307d0d50f42bb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3443; amd64
	-	windows version 10.0.17763.973; amd64

### `julia:rc` - linux; amd64

```console
$ docker pull julia@sha256:26e05991ad2784d52dfbc9b3f9ddd3bbbe14918ff3de95d973d43c4f29a5ffa6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137972998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb7a22ebcff368474e0de1b9f8974a3e06c7d1eab0b806e12e9c02f43b5c7d82`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 30 Jan 2020 02:19:37 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 02:19:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 30 Jan 2020 02:19:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524f70c49516c7568c039fd5b3b1b0919d7c83a73eb83816d02d30322d2fe6e1`  
		Last Modified: Thu, 30 Jan 2020 02:20:38 GMT  
		Size: 106.4 MB (106444185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - linux; arm variant v7

```console
$ docker pull julia@sha256:8a954e215423396846a6bf3f7a20edd7040e2a478442e0b8ba9858b9cdba85d5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123188966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb27f1eb6324be2a1cdd4aa7a9aa55c9acd36ab353156ffbc44b0931f3b53ad4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:33:23 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 18:33:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:33:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9324c8e014d9183150a1d11982cb169f4c44d13d2f393dfb91d167d0a8b31f`  
		Last Modified: Sat, 01 Feb 2020 18:38:35 GMT  
		Size: 96.7 MB (96706290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:f4585ee7b9a1a5b34c33a2d157c6709dbfe8cdce7adbf872afe4ef614c45b7d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119460610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7013f15be6f586d42cd9f1594a4b0ee12aba8607ebbc4bba86830a64b1b029e`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 20:08:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:08:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75506d725ccc6f9f17f4222959f216d3bee3944278981f37daca366cb3881c3`  
		Last Modified: Sat, 01 Feb 2020 20:12:53 GMT  
		Size: 89.3 MB (89294529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - linux; 386

```console
$ docker pull julia@sha256:4ef5a19cba48c3cc6af71a93b505901b0765307fefe967d08aa99865e7332e7e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135625924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af27c6c53789c4558eb65b4e59ce29123cc6de5139d173dbf4ce93aab854431a`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:47:32 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 17:47:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:47:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b4bb9e23c25e585467e1e235b9a6ca199c106976763a371043f2d7262289d2`  
		Last Modified: Sat, 01 Feb 2020 17:50:54 GMT  
		Size: 103.3 MB (103292635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:e99fa82eacfa9fb0d094e235cb0ce9e517af1f65c788b80e1302e3f110707f13
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5858705045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288f7450b14e7fb17cf7b70f703704a83e9f2893f58e0030f5d3cee81990397c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:02:24 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:02:25 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:05:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:05:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f44cf0312dbd62091dc5611083af53d7021ab979b3df9b05b6854ef12f8e76`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c3a9f637a43e81937bf39dc605098a2f0f2de44dc9883135dd1b1c77519db0`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80b8180e7ef10811cee9b9511c448255de8256ab5ca210f54b8054fb431f28`  
		Last Modified: Thu, 30 Jan 2020 03:24:01 GMT  
		Size: 134.1 MB (134100992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311e8adf83d3f4e49b437398db4e37c9abee5e3c43b06d1b692967b413d7e340`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:79b07715ea0d9fa827f0b465bb1ac7d8ba3ab96d130e88387d9a9d6681ea9170
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2346192159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f8198badbdfffd2e66aee0424c9f518a65b069ec796412c87f67e19caca4d8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:06:13 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:06:14 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:08:53 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:08:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860f7399498f1f144e2d9602758eb16c4e5021fa1fa32d157280506fdfa0c11d`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d6f370ff6bdfcfabe7c80d94802ad8170225c886dff031288ca1faa7377585`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6bb3b070d7f8e9b598db5889d8a124791eab7dd08199e9c2d6411432cfb597`  
		Last Modified: Thu, 30 Jan 2020 03:25:30 GMT  
		Size: 128.8 MB (128776203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff6dba759626604108e222cf0d12036d48bcb992cb40676f232f6f273306fce`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:rc-buster`

```console
$ docker pull julia@sha256:6bd34fe5a32b5568e0e9dd782c6de54a4d6753bac01b4f6a1f392aa13aa7e269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:rc-buster` - linux; amd64

```console
$ docker pull julia@sha256:26e05991ad2784d52dfbc9b3f9ddd3bbbe14918ff3de95d973d43c4f29a5ffa6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137972998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb7a22ebcff368474e0de1b9f8974a3e06c7d1eab0b806e12e9c02f43b5c7d82`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:53:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:53:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:53:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:53:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 30 Jan 2020 02:19:37 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 02:19:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 30 Jan 2020 02:19:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afaf5b9ab4e0b18f92fac2315520aee3f3a44f34bf81d6e19ede6bbfc2d09`  
		Last Modified: Sat, 28 Dec 2019 13:56:34 GMT  
		Size: 4.4 MB (4436539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524f70c49516c7568c039fd5b3b1b0919d7c83a73eb83816d02d30322d2fe6e1`  
		Last Modified: Thu, 30 Jan 2020 02:20:38 GMT  
		Size: 106.4 MB (106444185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:8a954e215423396846a6bf3f7a20edd7040e2a478442e0b8ba9858b9cdba85d5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123188966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb27f1eb6324be2a1cdd4aa7a9aa55c9acd36ab353156ffbc44b0931f3b53ad4`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:33:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:33:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:33:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:33:23 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 18:33:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:33:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6429cb88079b2fb8e762443ca0cc696ca55d3c1f0fe3c3a674c6719879848`  
		Last Modified: Sat, 01 Feb 2020 18:38:05 GMT  
		Size: 3.8 MB (3783538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9324c8e014d9183150a1d11982cb169f4c44d13d2f393dfb91d167d0a8b31f`  
		Last Modified: Sat, 01 Feb 2020 18:38:35 GMT  
		Size: 96.7 MB (96706290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:f4585ee7b9a1a5b34c33a2d157c6709dbfe8cdce7adbf872afe4ef614c45b7d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119460610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7013f15be6f586d42cd9f1594a4b0ee12aba8607ebbc4bba86830a64b1b029e`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:07:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:07:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:07:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:07:50 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 20:08:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:08:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f1d8485a5e3c379e3b42e6c452de3635b43460db384991ff1d865746269b08`  
		Last Modified: Sat, 01 Feb 2020 20:12:26 GMT  
		Size: 4.3 MB (4315422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75506d725ccc6f9f17f4222959f216d3bee3944278981f37daca366cb3881c3`  
		Last Modified: Sat, 01 Feb 2020 20:12:53 GMT  
		Size: 89.3 MB (89294529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-buster` - linux; 386

```console
$ docker pull julia@sha256:4ef5a19cba48c3cc6af71a93b505901b0765307fefe967d08aa99865e7332e7e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135625924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af27c6c53789c4558eb65b4e59ce29123cc6de5139d173dbf4ce93aab854431a`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:47:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:47:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:47:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:47:32 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Sat, 01 Feb 2020 17:47:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9996a9dc0547a97da5157536354645f9a2729b22f35c3d0d9cb42190e6fe3c64' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='a23f735c44f2d5bd60107a6f14c06c528aaffce8dc97a635e5f60f30c8ea7eaf' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='9d1a9c5616b35dc8363cf57833b4538a0825429d18cf7287ffe80edf72b4c884' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='7f6b7888bb77d2959035ffbb27bd7fc91fc2da77e5c678c74bb0723acf730e1d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:47:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a1a114e65b3510d2a6aa01898ca3e6b2b23a6bef40822567b76c876e82d9c8`  
		Last Modified: Sat, 01 Feb 2020 17:50:28 GMT  
		Size: 4.6 MB (4586237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b4bb9e23c25e585467e1e235b9a6ca199c106976763a371043f2d7262289d2`  
		Last Modified: Sat, 01 Feb 2020 17:50:54 GMT  
		Size: 103.3 MB (103292635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:rc-windowsservercore-1809`

```console
$ docker pull julia@sha256:bef5d8cd36dc27d6293dfe4f64541614eba9bdcf293262c0165fcbbd67fb42d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `julia:rc-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:79b07715ea0d9fa827f0b465bb1ac7d8ba3ab96d130e88387d9a9d6681ea9170
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2346192159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f8198badbdfffd2e66aee0424c9f518a65b069ec796412c87f67e19caca4d8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:06:13 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:06:14 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:08:53 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:08:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860f7399498f1f144e2d9602758eb16c4e5021fa1fa32d157280506fdfa0c11d`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d6f370ff6bdfcfabe7c80d94802ad8170225c886dff031288ca1faa7377585`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6bb3b070d7f8e9b598db5889d8a124791eab7dd08199e9c2d6411432cfb597`  
		Last Modified: Thu, 30 Jan 2020 03:25:30 GMT  
		Size: 128.8 MB (128776203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff6dba759626604108e222cf0d12036d48bcb992cb40676f232f6f273306fce`  
		Last Modified: Thu, 30 Jan 2020 03:24:53 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:rc-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:8d8f89f035b02a84ad85e98b07bad9b5479ce8c4c38f4eee80fdbcc7337ae3c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `julia:rc-windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:e99fa82eacfa9fb0d094e235cb0ce9e517af1f65c788b80e1302e3f110707f13
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5858705045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288f7450b14e7fb17cf7b70f703704a83e9f2893f58e0030f5d3cee81990397c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 30 Jan 2020 03:02:24 GMT
ENV JULIA_VERSION=1.4.0-rc1
# Thu, 30 Jan 2020 03:02:25 GMT
ENV JULIA_SHA256=fc718bfd1fa9da9c306376c8994d3dee4b08131d3198036c33f878cf469f7567
# Thu, 30 Jan 2020 03:05:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:05:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f44cf0312dbd62091dc5611083af53d7021ab979b3df9b05b6854ef12f8e76`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c3a9f637a43e81937bf39dc605098a2f0f2de44dc9883135dd1b1c77519db0`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80b8180e7ef10811cee9b9511c448255de8256ab5ca210f54b8054fb431f28`  
		Last Modified: Thu, 30 Jan 2020 03:24:01 GMT  
		Size: 134.1 MB (134100992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311e8adf83d3f4e49b437398db4e37c9abee5e3c43b06d1b692967b413d7e340`  
		Last Modified: Thu, 30 Jan 2020 03:23:20 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:stretch`

```console
$ docker pull julia@sha256:733cffa80bf37f47d4d2de3cb28a40a3e06d86b21de64ee06991829722396939
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:stretch` - linux; amd64

```console
$ docker pull julia@sha256:f16498d133d157f29bd5fefe385f482fbfc0c81ef8b889866989dacdc0bd4bae
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133452200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b507aa80fa4adf054832444d789687c311b4923b77be08f9567fb2c1de1d93c`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:47 GMT
ADD file:90a2c81769a336bed3f731f44a385f2a65b0916f517a0b77c06c224579bf9a9a in / 
# Sat, 28 Dec 2019 04:23:47 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:54:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:54:37 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:54:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:54:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Jan 2020 01:24:05 GMT
ENV JULIA_VERSION=1.3.1
# Tue, 07 Jan 2020 23:22:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Jan 2020 23:22:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:804555ee037604c40de144f9f8da0d826d38db82f15d74cded32790fe279a8f6`  
		Last Modified: Sat, 28 Dec 2019 04:28:38 GMT  
		Size: 22.5 MB (22524609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6aef362d0b91076dc5819a1b925f776504ec063851be5395cadb471b9f3881e`  
		Last Modified: Sat, 28 Dec 2019 13:57:02 GMT  
		Size: 7.6 MB (7555513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71672730cf04ca165569336fedcecf18f18fa7af5bb68b0269336d2cf0104e6d`  
		Last Modified: Tue, 07 Jan 2020 23:23:49 GMT  
		Size: 103.4 MB (103372078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:c96aa5ec4099d65d449554fe6255b743ea25cfab5a1aa847a3cffca734f0f0ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119407020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:facee1409787ff6bc644dbfa70a17b807cf03b1a47fae35a99ecd4234ab3e1fa`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:29 GMT
ADD file:6ac430a42a1f2a6cc8b0a3565e518bd0e3a47b01d524b86cd3dd4e7f4606fd53 in / 
# Sat, 01 Feb 2020 17:04:31 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:35:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:35:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:35:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:35:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:35:14 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 18:35:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:35:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6bc458b0813423b9e351a5604c0d71a4853d970ea22b23fedc8683af12dbc13c`  
		Last Modified: Sat, 01 Feb 2020 17:11:31 GMT  
		Size: 19.3 MB (19311624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9840e48d64ced9020e882cefaf8fe5cd26dc391522b6acd18cd09eccad69e07`  
		Last Modified: Sat, 01 Feb 2020 18:39:27 GMT  
		Size: 6.3 MB (6292143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8331cb5b72ee568b3cf598db9f378382b4cc073daabb288e06f54994ca3f6ae7`  
		Last Modified: Sat, 01 Feb 2020 18:39:55 GMT  
		Size: 93.8 MB (93803253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:96635540f0bc528b39750e2c03177d4e85a1bb1c080981eb64742ed7d690f4ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113207625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:877782fd5d403c41cd3e8bd8175bba4fc79ed5a1a96a15b1715dba7334a7740b`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:d3338eed8ee88c2a5856cc2eb73701e4de79a7e551602df07834a1ad4f671435 in / 
# Sat, 01 Feb 2020 16:43:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:09:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:09:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:09:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:09:37 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:09:38 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 20:10:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:10:03 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5c630fa6465ea72ddec15fd68bdd45a6da6fa4b1981895bf7c2852eedf066194`  
		Last Modified: Sat, 01 Feb 2020 16:48:58 GMT  
		Size: 20.4 MB (20385851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaa324c835efe4fe5ac3f0b479d4adcb40046011bef28007c8c399f15705879`  
		Last Modified: Sat, 01 Feb 2020 20:13:39 GMT  
		Size: 6.5 MB (6526685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6646730906734e461b2a9c00c1251ff85515f5fa90cc4ad6b6704a8231c55fe`  
		Last Modified: Sat, 01 Feb 2020 20:14:05 GMT  
		Size: 86.3 MB (86295089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:stretch` - linux; 386

```console
$ docker pull julia@sha256:80af7ef3c4f85fc04cbfa89589a63190f25e1f777664ff9df018dd2def1d5c1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (130011823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3b9bf8739ffa78559670835476d3ecc66c66598265715bdc8f0a0841ed6579`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:48:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:48:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:48:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:48:37 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:48:38 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 17:48:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:48:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3eada1d3458b1595fb3469dbe1f9a16519fe362c19186c018a3f71a94b9b38`  
		Last Modified: Sat, 01 Feb 2020 17:51:37 GMT  
		Size: 7.6 MB (7582401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4259c4d7471ff49be69dbeb9e909fbfe48ba5fb8252a848e9634ba0b6ec8dbc8`  
		Last Modified: Sat, 01 Feb 2020 17:52:03 GMT  
		Size: 99.3 MB (99277266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-1809`

```console
$ docker pull julia@sha256:b56bf68490e4fd22c8a85f9f6e74c9f0d225cc26eada8d04f4241022aa63bb0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `julia:windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull julia@sha256:ed1ddd20b9e1503e39766f617a3422dfed5cf242e396b7f036e15fd934c74800
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2341155050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97fec4e1fe1475c22c92fdf8fdf98346ba2396bc7ca1e0acba21fe0e0ece4632`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Jan 2020 19:15:23 GMT
ENV JULIA_VERSION=1.3.1
# Wed, 29 Jan 2020 19:15:25 GMT
ENV JULIA_SHA256=8350ca66f80484c5ca6f7341ffbdb9d5182f8d4231762d585e229567b227ef7f
# Thu, 30 Jan 2020 03:15:56 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:15:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7726a80f05eaa520d72fca444791156a10b3834f6597ac83b61cb27fb3200101`  
		Last Modified: Wed, 29 Jan 2020 19:21:59 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20f6546d9098b8dba4542af815fe5cae976db3c5a520a5579778229dc6b173e`  
		Last Modified: Wed, 29 Jan 2020 19:21:59 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669caefcaa1628658892b7d2bed49af0e63f523b8ece9f911791d36e5b66b366`  
		Last Modified: Thu, 30 Jan 2020 03:28:24 GMT  
		Size: 123.7 MB (123739167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab655bda7afc3539a1ddf6e38766e8e7e09bf4f25c113148bc7bfc595387b2e3`  
		Last Modified: Thu, 30 Jan 2020 03:27:52 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:f93277d40384cf15a6fc5e58494cf63394343441256ecd08917e863fa489730e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `julia:windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull julia@sha256:30236875171e7c6d54f8d55583330862e9a5db937ab63e55693d8ac33d574dea
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5853668011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a85a381283d750122455d795be2c7ea0996113ffdcd598f2faf84234f380bebb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 17:20:16 GMT
ENV JULIA_VERSION=1.3.1
# Wed, 15 Jan 2020 17:20:18 GMT
ENV JULIA_SHA256=8350ca66f80484c5ca6f7341ffbdb9d5182f8d4231762d585e229567b227ef7f
# Thu, 30 Jan 2020 03:12:43 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Thu, 30 Jan 2020 03:12:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453d305ccea93f036fe51fd37293fd5aee64f8fe68c1096ce6591cf82c005f76`  
		Last Modified: Wed, 15 Jan 2020 17:28:28 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0318d1ad0420adf48ddb3a4911d306b810a69a68a75f1889bd72e2732e98f7d`  
		Last Modified: Wed, 15 Jan 2020 17:28:28 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bbb3d35fcc68e71a0cb1c0f23d09c911dddf22f436026370aad50a8cd14bf3`  
		Last Modified: Thu, 30 Jan 2020 03:26:55 GMT  
		Size: 129.1 MB (129063927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc05b01cfc9f41d5736018505f631cbd708ac93d6ea62c81857f67926cc0645`  
		Last Modified: Thu, 30 Jan 2020 03:26:18 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
