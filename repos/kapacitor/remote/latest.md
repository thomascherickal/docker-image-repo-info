## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:ff6dcb7acc29863942a3bbb8c2c13f7c9b643c53a0e9793ab5fede6a39182e8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:6a772aed3a8cdeaee2ac615a1fd6cc7577b9f7fa1914df803f0fb7e0f060ba90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.3 MB (135256941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1657e593b35f337f8e14e868605825a5a252209cc9946e72a1197bbbdc7b9f02`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:10 GMT
ADD file:4c5e0bec5f780d9c6bfbafcb9e6ed641781dd7f7c2853a0c49d6613e9fef9516 in / 
# Thu, 23 Jun 2022 00:22:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:54:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:54:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 15:23:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 23 Jun 2022 15:23:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 15:23:26 GMT
ENV KAPACITOR_VERSION=1.6.4
# Thu, 23 Jun 2022 15:23:31 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 23 Jun 2022 15:23:32 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 23 Jun 2022 15:23:32 GMT
EXPOSE 9092
# Thu, 23 Jun 2022 15:23:32 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 23 Jun 2022 15:23:32 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 23 Jun 2022 15:23:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 15:23:32 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:8372a04f222be82bf67eb0010a59644b1e52f1246b3da9034edaa98f3d591cae`  
		Last Modified: Thu, 23 Jun 2022 00:29:36 GMT  
		Size: 45.4 MB (45430020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1728fee80d376293a9ef5fdcc0acd3f6398fc4159b12064ce4c1e66f67e7e9d`  
		Last Modified: Thu, 23 Jun 2022 01:02:01 GMT  
		Size: 11.3 MB (11302923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cf50aa0a4b80b39d1bf4be232d404da0b1ad38cdd3bb1a017b727947b5f4bb`  
		Last Modified: Thu, 23 Jun 2022 01:02:00 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ca30eaa3f2e4a14053445907d290c9e29fe087a4cd7f7607ea7ced493a2405`  
		Last Modified: Thu, 23 Jun 2022 15:23:51 GMT  
		Size: 13.4 MB (13436157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88da6edad4b4d98978e4fd397110c9d2f14f317fd3846dc196f8d8c95d1ba632`  
		Last Modified: Thu, 23 Jun 2022 15:23:50 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719d31fd73df954adfd5d7ef9285d3371214e12b411e85abacef111b4a18b7b6`  
		Last Modified: Thu, 23 Jun 2022 15:24:13 GMT  
		Size: 60.7 MB (60741606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff316b9b33ac965938bebc4dd0c7067bf5bee8e7143814ab032139cecd90e8b7`  
		Last Modified: Thu, 23 Jun 2022 15:24:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c471860c641e700a795da2ded0f303b3aee1b7a5312fcf44d5248ea96cd41dc2`  
		Last Modified: Thu, 23 Jun 2022 15:24:05 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:0453659e300b211a8e0f06f997c3a52a4aa936dfcbaaf143648a9e268949d6cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127206755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bc55ffd190130f7a4e75667387f5ce9a7f73688297215047444595575e3a115`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 28 May 2022 00:42:45 GMT
ADD file:93d675ee0bc32a88dc4d6c0872276c4678dc31f0b6eb8b936cb823f191bc07f0 in / 
# Sat, 28 May 2022 00:42:46 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:10:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:11:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 00:31:24 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sun, 29 May 2022 00:31:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 00:31:46 GMT
ENV KAPACITOR_VERSION=1.6.4
# Sun, 29 May 2022 00:31:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sun, 29 May 2022 00:31:53 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sun, 29 May 2022 00:31:53 GMT
EXPOSE 9092
# Sun, 29 May 2022 00:31:54 GMT
VOLUME [/var/lib/kapacitor]
# Sun, 29 May 2022 00:31:56 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sun, 29 May 2022 00:31:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 00:31:57 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:de7fc2a3b80bcd193de687188fc9051c8be6c61ec81fec3aeae61c079f71e69e`  
		Last Modified: Sat, 28 May 2022 00:51:21 GMT  
		Size: 43.2 MB (43212871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee73573552502f742607ea1dcdefcee9aeafa4ad8d5deca24b48a262f4ba108`  
		Last Modified: Sat, 28 May 2022 11:20:36 GMT  
		Size: 10.2 MB (10218522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05d3983d65175e68348dcb2cd43933f2af4d2d8c1bf36c9d5f237394c9fa53b`  
		Last Modified: Sat, 28 May 2022 11:20:35 GMT  
		Size: 3.9 MB (3874461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8f74dae4587aae058149bbff22363d653b738ecb28be02f413d1bf034b7c6`  
		Last Modified: Sun, 29 May 2022 00:32:16 GMT  
		Size: 12.9 MB (12902056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d454c1b46feace219c701415f116ab5443d39199d58e0c949182ad86976c1a03`  
		Last Modified: Sun, 29 May 2022 00:32:14 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3851da6043768a64a997e2f7785dcc44f251fc1765506c856ed744937bc288`  
		Last Modified: Sun, 29 May 2022 00:32:38 GMT  
		Size: 57.0 MB (56995561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4de92e6d38a9dfb8350dbaf6671cd7d65f183c3081d8baf3c9330569aa4f82`  
		Last Modified: Sun, 29 May 2022 00:32:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66f3b4f34ed8366d81c4218b1cbf18d2d9abc857a7ed9918142dd75d2402b8b`  
		Last Modified: Sun, 29 May 2022 00:32:30 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
