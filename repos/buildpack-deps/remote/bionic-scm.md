## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:c7004cb9e4ff4451f9b569ef6e4afc2c15b0c2fffb895ccb6e91e1f118420042
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c51055e4b555caf528965c8aff7cdb7560534b069b47dac734165fa1c5302710
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81860597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d13cec4cb20b7ae42df3ae0ff9700dfb4e62b73fcc03ee5342505f4a9f16dbb0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 01:27:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:27:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Apr 2022 01:27:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d74cdf65aa24870bf2345d9c4fa42388a09f5388e94469f3e6f08644a35dba`  
		Last Modified: Fri, 22 Apr 2022 01:43:43 GMT  
		Size: 6.6 MB (6641787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29dc3910681266625514ae173ec9b5aad8bd2bcc5b5ed7ce0e668a4f43e1a93c`  
		Last Modified: Fri, 22 Apr 2022 01:43:42 GMT  
		Size: 3.0 MB (3022435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeeabe337490f3baa39daf3ec713767aea729f5abf9f3f763910203571419504`  
		Last Modified: Fri, 22 Apr 2022 01:44:00 GMT  
		Size: 45.5 MB (45486492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c42d465acd1b874155ab78eb6e2e3477a7eff26c54d4115b7b263189daac0ac3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71290710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96af719060deb35f5a625e808317745d4dd3a6fa2d53529b88343dfd039a2fe3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:51:56 GMT
ADD file:4b33ada37adb95859d134226d5b4c6e5ffef998aedb9a3458a11343c62932bf9 in / 
# Fri, 22 Apr 2022 21:51:57 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:34:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:34:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Apr 2022 01:35:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34c8e4a8441a3ead578ea0979cd16b5e2ce41f1e30b62e3a67d21ba35122cf87`  
		Last Modified: Tue, 19 Apr 2022 13:11:05 GMT  
		Size: 22.3 MB (22302622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603b6f8e63d3918b8113638b37fca889b94365fb2eb62cec70d3141768ed840a`  
		Last Modified: Sat, 23 Apr 2022 01:54:39 GMT  
		Size: 5.7 MB (5712315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a361aa78b41ab54cbe55ee69f360cd925b724edec3326be3df8996e8de80f493`  
		Last Modified: Sat, 23 Apr 2022 01:54:36 GMT  
		Size: 2.6 MB (2584795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94eb8cf112839e50dc58f86c0b10eaffed447e3e9075dee81f4331ec39e5d166`  
		Last Modified: Sat, 23 Apr 2022 01:55:19 GMT  
		Size: 40.7 MB (40690978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:be838359b364a6aa99ad64fef8115db961c35c96f28acc7346a4ea51989d61fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75675548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0c2d456be3c8eee64d4c3cc70a6391e8bfb911599a42647d7c21fb4a208a47a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:01 GMT
ADD file:5c0ff944739f8966900c55d6a77ba4ba6031b585962994b1684845dcd411c2fb in / 
# Fri, 22 Apr 2022 00:54:02 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:29:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:29:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Apr 2022 04:30:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:945d527fe80d536e4da70ea808f70d90bc97d7930c7ae2c61b5dabd1dba19e07`  
		Last Modified: Tue, 19 Apr 2022 13:10:40 GMT  
		Size: 23.7 MB (23734459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31dd4f068bf0b02d321355a3f8fb2eaaecdb976b6c1e065e3316599c0ccf8dd5`  
		Last Modified: Fri, 22 Apr 2022 04:38:56 GMT  
		Size: 6.1 MB (6082554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f02ffc7642bf1096d5f4511822ad6d8e2c6a6da8a483abdc1b95902454ae8fe`  
		Last Modified: Fri, 22 Apr 2022 04:38:55 GMT  
		Size: 2.6 MB (2570164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b35cad735bb5ee52e0db045775ead9ac2da3682386e82c32e4a5d7832794979`  
		Last Modified: Fri, 22 Apr 2022 04:39:14 GMT  
		Size: 43.3 MB (43288371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:94166da72e77bc7918bd3c870e15de97672e11dd1b5e0d012f8768754e615316
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84215943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0a39a5b76b70e3761ed95913efab532bc9d09d2c0b0db0512f02eacdebe3fa6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:53:57 GMT
ADD file:164f0ee7842870b8f94ab2ee8f9151b49e08f461b99fdfa1b7586fa864d4a320 in / 
# Thu, 21 Apr 2022 23:53:57 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 00:16:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 00:16:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Apr 2022 00:17:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57fda0d035c311017871931fe2f2a2c241e46b4bc95d2a87dbf533afd8e72668`  
		Last Modified: Tue, 19 Apr 2022 13:11:34 GMT  
		Size: 27.2 MB (27163453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80020c29fe6d0575254dda040fc655dfaa84bca26136ce9b29f390d4fbb29b6`  
		Last Modified: Fri, 22 Apr 2022 00:22:15 GMT  
		Size: 6.9 MB (6929643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cdf0da60441cb8fc028c8ef1f25bf94a0e154a9fe189221f99d9d7e17e0579`  
		Last Modified: Fri, 22 Apr 2022 00:22:14 GMT  
		Size: 3.0 MB (3038571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e7e0cc8bbbca0f6e3c427507a389d0fa1ede6bdc4b6510939e3a64d6efa643`  
		Last Modified: Fri, 22 Apr 2022 00:22:35 GMT  
		Size: 47.1 MB (47084276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:85f97a4fa99c43fc39f23187372745f308b34ed95c839ec43f2f5f52b96e1980
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94948027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bcf3cb312add486e04df9adca8f2fabae20d0df0518932ec0b037275621383c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 08:07:45 GMT
ADD file:d5447cb8fcc4a12030e43cda74f87e1bec09c6d1093307e25164127500f5e0d9 in / 
# Fri, 22 Apr 2022 08:07:52 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 09:06:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 09:07:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Apr 2022 09:09:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00422cde8b22ee0ff419263739625132280d08ffe78075ad3fb44dd003fab8e2`  
		Last Modified: Tue, 19 Apr 2022 13:12:05 GMT  
		Size: 30.4 MB (30442273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d587db8c583825f01547d10158ffcd670b22090b1d7e22c4cc5e38a8d66de0`  
		Last Modified: Fri, 22 Apr 2022 09:40:32 GMT  
		Size: 7.1 MB (7056674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9dc57e211ce75e162542827ed82b7296b4e38b40d85577df3c9df74cc13ae0`  
		Last Modified: Fri, 22 Apr 2022 09:40:31 GMT  
		Size: 3.7 MB (3719458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f3d85745514e470e8c7feb12770beffb279852e12e73b52443c36b69c39fc4`  
		Last Modified: Fri, 22 Apr 2022 09:40:56 GMT  
		Size: 53.7 MB (53729622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b84bb24a44f586de67d288d759cce3e5ef14caca682a4d3559e1824490f40f35
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79702735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49781059f49f247126bde4df1f26ade34ae68baadc79952bb30b7c37e2e9ae24`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:17 GMT
ADD file:bc2c78cc62a5e94931f8bd76f2fa050b19598c050fc18aa56bbd202826ec784b in / 
# Fri, 22 Apr 2022 00:39:19 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 01:30:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:31:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Apr 2022 01:31:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:18c1f746bcbccc4e7599497df0d1d562571c9ecd9effcfb7bee0bbe17d1156b5`  
		Last Modified: Tue, 19 Apr 2022 13:12:34 GMT  
		Size: 25.4 MB (25365079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8405e5ec3de7029a8d9e579e70b8ad1e1c0c54178d2bceeddbddd9891f208caf`  
		Last Modified: Fri, 22 Apr 2022 01:50:36 GMT  
		Size: 6.3 MB (6332722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75f8f2095b8a73b68dac155f8b672164e44e681428870a909eb95d1bbadfd2d`  
		Last Modified: Fri, 22 Apr 2022 01:50:36 GMT  
		Size: 3.0 MB (2975175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef53d077886666b6b48b25300b869d8cf8d6cdbaf6ce678b6e3eb7cbaf4f6f2b`  
		Last Modified: Fri, 22 Apr 2022 01:50:52 GMT  
		Size: 45.0 MB (45029759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
