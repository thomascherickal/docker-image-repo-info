## `telegraf:latest`

```console
$ docker pull telegraf@sha256:38d789523a0c960f77d564b997b53378e508d4c34338a0a7e586bc32cf24675c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:e1c81bcb6d24903fb4e6cbb524861096aa36b25c5ff82f58aa1ff13f24b3c510
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122088989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:630d6edf6e4fbfa62eb4ba24fa6ccb21311936416a634a9b586201ea8ac85120`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:47 GMT
ADD file:a290acee3581e1e9c42c0a37b53086a8f070cb0730179be81a6ba24a620b6ee4 in / 
# Wed, 26 Jan 2022 01:40:47 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 Jan 2022 11:28:42 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 11:29:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 27 Jan 2022 11:29:41 GMT
ENV TELEGRAF_VERSION=1.21.2
# Thu, 27 Jan 2022 11:29:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 27 Jan 2022 11:29:47 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 27 Jan 2022 11:29:47 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Thu, 27 Jan 2022 11:29:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Jan 2022 11:29:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a024302f8a017855dd20a107ace079dd543c4bdfa8e7c11472771babbe298d2b`  
		Last Modified: Wed, 26 Jan 2022 01:47:01 GMT  
		Size: 50.4 MB (50437057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289773030fdc98afe6cc53bdd0c05332ea8ff21ad836afa1d3042388953c43f8`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 7.8 MB (7833856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb8b3399fe8dd0b83bd5e32a97e5183ab235d6fb4cc0b5dfabb20e6653e715`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 10.0 MB (9997205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a2c7a10ef219c322572998db3b37e08fb7c0a71b5767641e82de694ea2f50a`  
		Last Modified: Thu, 27 Jan 2022 11:30:14 GMT  
		Size: 17.4 MB (17415400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38d2ffb6435ae10f04900e1da7a08dd941b27c5e1174abbfc597c77a8e078f8`  
		Last Modified: Thu, 27 Jan 2022 11:30:10 GMT  
		Size: 2.9 KB (2904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe30861de9a72b92a45baa97ac1754b3ebf3c3c0c31895605a8a6909d05fcfe`  
		Last Modified: Thu, 27 Jan 2022 11:30:52 GMT  
		Size: 36.4 MB (36402259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93455755b871f26bd429ad71cc614fa2ca934dbd2410ee7c1094bbcf40b2e686`  
		Last Modified: Thu, 27 Jan 2022 11:30:45 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c64a796754527940aa16ec69b304014487a344b8a1903981629e1a695097755d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112303821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38108ae4f8a16556619ed2ff7aa1b4630dba9b0723cb98ac2881ab2351a6cf2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:17 GMT
ADD file:36bf5b8bdd9066b06cc35d26df3f4dad2b1cbcb41985b85f070ed97a3e85f8a9 in / 
# Tue, 21 Dec 2021 02:00:18 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 18:05:01 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 18:05:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Jan 2022 19:58:29 GMT
ENV TELEGRAF_VERSION=1.21.2
# Wed, 05 Jan 2022 19:58:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 05 Jan 2022 19:58:41 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 05 Jan 2022 19:58:42 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Wed, 05 Jan 2022 19:58:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Jan 2022 19:58:42 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:328389035fdd79ece4f520541a84b3de974050fe012ed1566da6b869dd34ea29`  
		Last Modified: Tue, 21 Dec 2021 02:16:11 GMT  
		Size: 45.9 MB (45918102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80397c5626b1d4e58b7b7dd9219674dd86caa03ddcaac1d3d6791189a44b0ff`  
		Last Modified: Tue, 21 Dec 2021 03:14:47 GMT  
		Size: 7.1 MB (7125168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816c475148f8e55cc2b8593f29d0ddd67ad1359f3c69061f043d461495bad179`  
		Last Modified: Tue, 21 Dec 2021 03:14:48 GMT  
		Size: 9.3 MB (9343808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607f3d7f4404cb0dc06799b481c25dde452fc6d23f2bea8b69cdea4043e51b15`  
		Last Modified: Wed, 22 Dec 2021 18:07:16 GMT  
		Size: 16.2 MB (16161072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd5e4e2470e79658cef7e65784eaa20c4e4b5b4a24240bb9b4057d9066947ea`  
		Last Modified: Wed, 22 Dec 2021 18:07:05 GMT  
		Size: 2.9 KB (2903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f14aa6436095875eef055bca633575b10cf6f0107c2c50cd8f996965245af93`  
		Last Modified: Wed, 05 Jan 2022 19:59:55 GMT  
		Size: 33.8 MB (33752459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd50a26b965184e3fa25457d318b0fd44504880085c76ba55500c1614bc5b8ae`  
		Last Modified: Wed, 05 Jan 2022 19:59:31 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:96e416fca6c247244a48bb35aa19ac77a772536405be101b9708c9691a616bf3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116775561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7e05be85c1200a070dd12c0a4ae7a2f64a7bbc9334bb4ee91b877d73b0a4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:14:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 20:03:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 20:04:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 20:05:05 GMT
ENV TELEGRAF_VERSION=1.21.2
# Wed, 26 Jan 2022 20:05:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 26 Jan 2022 20:05:11 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 26 Jan 2022 20:05:13 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Wed, 26 Jan 2022 20:05:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 20:05:14 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3524e6d2c855bef1f32da73e00738b2e5e91e6a346d19f8b33e8e8117c82748`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 7.7 MB (7695112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc9cf00cd9023559aeda43668c7d9d621318631bab103ae03b8a3787260048`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 9.8 MB (9767300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34ec0624fdce392c92171379a77f7d018e7fac8f2e39c8f6bbb2579cc93de47`  
		Last Modified: Wed, 26 Jan 2022 20:05:40 GMT  
		Size: 17.1 MB (17059033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520feaefcdd19ed3e79b582d65947eb00d949353436959210a4c685ea9bd660b`  
		Last Modified: Wed, 26 Jan 2022 20:05:36 GMT  
		Size: 2.9 KB (2875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d44ca63f7c7c2de2ca79a29f286f52c640f52b7e103f121afc224921b779c18`  
		Last Modified: Wed, 26 Jan 2022 20:06:17 GMT  
		Size: 33.0 MB (33027889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22adfe43dff7fe8f5fa544c1a836152222b7b1874dec3ec030c57c6327fa063d`  
		Last Modified: Wed, 26 Jan 2022 20:06:10 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
