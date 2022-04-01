## `telegraf:latest`

```console
$ docker pull telegraf@sha256:1ff45b21d3e3c2de446ea01f14de3bcfa563e4211e6a7b35292ea89230224242
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:425d7915e4c0b5c26a3bca98572f898be3cbb626b7e570a08de32ecfa71be5e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128703039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9e2b2b325832b09aa049eee6f079aa8fc2743b8a54ee5cca9a474fb2687f43a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:07 GMT
ADD file:e8d512b08fe2ddc6f2c85831c73e4c72b9c850fa428913d19da4bb1a34f84cf2 in / 
# Tue, 29 Mar 2022 00:22:08 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:29:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:29:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 31 Mar 2022 01:07:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 01:07:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 31 Mar 2022 01:07:32 GMT
ENV TELEGRAF_VERSION=1.22.0
# Thu, 31 Mar 2022 01:07:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 31 Mar 2022 01:07:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 31 Mar 2022 01:07:36 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 31 Mar 2022 01:07:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 01:07:36 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:dbba69284b2786013fe94fefe0c2e66a7d3cecbb20f6d691d71dac891ee37be5`  
		Last Modified: Tue, 29 Mar 2022 00:26:47 GMT  
		Size: 54.9 MB (54937710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baf437a1badb6aad2dae5f2cd4a7b53a6c7ab6c14cba1ed1ecb42b4822b0e87`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 5.2 MB (5155705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ade5c59e324bd7cf369c72ad781c23d37e8fb48c9bbb4abbecafafd9be4cc35`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 10.9 MB (10874957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0680c11313d76d20633a102c6fc665961c9980b9ecd297f17faf934ec5857281`  
		Last Modified: Thu, 31 Mar 2022 01:08:01 GMT  
		Size: 18.8 MB (18760136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f43e04d38451e900ebbdf9d41cd22c6433e09055242093664915f81b411fcf`  
		Last Modified: Thu, 31 Mar 2022 01:07:57 GMT  
		Size: 2.9 KB (2900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7762e1308d94056cd014dd773e13755505e8f9208653c693464a169541ed3ed7`  
		Last Modified: Thu, 31 Mar 2022 01:08:39 GMT  
		Size: 39.0 MB (38971290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c37f1343ecb3eb111e2d63f49e1521618400013d8f0d644312f394afd5e6ac`  
		Last Modified: Thu, 31 Mar 2022 01:08:32 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c682efa2cf4fa51501680b746e1713c8b5db8bfc4ef9277466eb903191c643be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118853629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7966a3bd2c35751c633a732cc60435ef2724553f603017fdb83d0333012392b8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 02:17:58 GMT
ADD file:d8d3280d101d611090968c237af923598174e090c533c24bcee805d174e4a6f5 in / 
# Tue, 29 Mar 2022 02:17:59 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:06:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:06:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Apr 2022 01:33:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Apr 2022 01:33:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 01 Apr 2022 01:34:16 GMT
ENV TELEGRAF_VERSION=1.22.0
# Fri, 01 Apr 2022 01:34:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 01 Apr 2022 01:34:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Apr 2022 01:34:29 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 01 Apr 2022 01:34:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Apr 2022 01:34:30 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:fc87a15f2d540adb88546a549e56aa0a378d5719bbfd07399e467a095e27d5df`  
		Last Modified: Tue, 29 Mar 2022 02:33:28 GMT  
		Size: 50.1 MB (50133868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7991e015792e592929b68328873d303aff48f6941208e2954283895889e665b3`  
		Last Modified: Wed, 30 Mar 2022 20:30:28 GMT  
		Size: 4.9 MB (4924893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4aa6896142430c96d4b31e28c4d0e3c383d9ae671ce052f26fc7cf68189c058`  
		Last Modified: Wed, 30 Mar 2022 20:30:30 GMT  
		Size: 10.2 MB (10217881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44e9e10874218753b33c76d93ab63fcf6c0c7b13070898eaf005cdf13228180`  
		Last Modified: Fri, 01 Apr 2022 01:35:26 GMT  
		Size: 17.5 MB (17462337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547efda312530826eab241fb2b7aff4b8a1d622fee3c2acac2cf2e17abaaecae`  
		Last Modified: Fri, 01 Apr 2022 01:35:14 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a4e5c15c9c1da9825522e56d650c37a465fa65d3392fb91417589265628fb1`  
		Last Modified: Fri, 01 Apr 2022 01:36:51 GMT  
		Size: 36.1 MB (36111409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be25be2bd652e1422318a69e00931ae94316be5b84fa03cda0b46c55337e35f`  
		Last Modified: Fri, 01 Apr 2022 01:36:26 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:92b030cbc5b0a84d82c9c058577bae0f7b0295fbaca51af8a2ef112c0385e9f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122899972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c38a08475161948eea1eb79633f4b3d0fe9170fa1433fd56262d9d1b74525d5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:01 GMT
ADD file:5e8f8c10da6d37a727fb5e1ed13b3dd78769f0ca7e91f0c3510e2edd25177117 in / 
# Tue, 29 Mar 2022 00:43:03 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:13:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:13:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 23:18:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 23:18:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 30 Mar 2022 23:19:27 GMT
ENV TELEGRAF_VERSION=1.22.0
# Wed, 30 Mar 2022 23:19:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 30 Mar 2022 23:19:33 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 30 Mar 2022 23:19:34 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 30 Mar 2022 23:19:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 30 Mar 2022 23:19:35 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:fa223d8c149d7beec8e997e1415ee4961473cafaf88a932f70baf3da56f2c564`  
		Last Modified: Tue, 29 Mar 2022 00:49:33 GMT  
		Size: 53.6 MB (53633710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ffbd2ab15985c19f9e1e3199cdce06090266d20d11dbd3d55fba45de2fcc27`  
		Last Modified: Wed, 30 Mar 2022 02:24:13 GMT  
		Size: 4.9 MB (4938638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3953e76cee2ab175d909ccec1a3399912a690ad621ae88cff787d98419b97bb`  
		Last Modified: Wed, 30 Mar 2022 02:24:14 GMT  
		Size: 10.7 MB (10656993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a939508bbfeff08431d12b3d89969385801628a957c0a7d2b6fa2b55d54025a`  
		Last Modified: Wed, 30 Mar 2022 23:20:02 GMT  
		Size: 18.4 MB (18382668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699770afbd04634c5c13054a9ea8927682515ddfaf2a80cc4f91345063910d0c`  
		Last Modified: Wed, 30 Mar 2022 23:19:59 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac24096c1f6cabb104ad4825ad5248bfb39f658b7e398b246732ed29dd94af52`  
		Last Modified: Wed, 30 Mar 2022 23:20:38 GMT  
		Size: 35.3 MB (35284748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84458c7c9459225f2c31cc25fa6b966857e84b7c6b9a92bd25979f996980188`  
		Last Modified: Wed, 30 Mar 2022 23:20:32 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
