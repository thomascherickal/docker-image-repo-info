## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:c655b47452976cba832b40f1a3998ae9c14e08a874973299c849e3806308940b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:088641e46e1803982060ea31fc485f6308e2a7376f4a1f8c1a5aaf4fe72748b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.5 MB (111512566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9150b2814fc207efe27321ab5c9af985cf7d3d9768453c9cfb498c9e66ce3f30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 13 May 2021 01:43:22 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 13 May 2021 01:43:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 13 May 2021 01:43:38 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 13 May 2021 01:43:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 13 May 2021 01:43:43 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 13 May 2021 01:43:43 GMT
EXPOSE 9092
# Thu, 13 May 2021 01:43:43 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 13 May 2021 01:43:44 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 13 May 2021 01:43:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 13 May 2021 01:43:44 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0042c1082cde4e37d2eb2589de52f9c297b550a5df3a548239ab8294cefceda4`  
		Last Modified: Thu, 13 May 2021 01:44:04 GMT  
		Size: 13.3 MB (13280729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f22be644154272e8ffebcb8045df1b26830dac802dd45a439a87fe46645e4a2`  
		Last Modified: Thu, 13 May 2021 01:44:02 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff884058edd891c1078a3d7297910e024f60087b88d71b226af9b1bb90237bc0`  
		Last Modified: Thu, 13 May 2021 01:44:25 GMT  
		Size: 37.2 MB (37219582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d281f90161e24c4a6375052fbf3bd14ff5562ad5c75785232c822ebdc22646`  
		Last Modified: Thu, 13 May 2021 01:44:19 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26cffe07e7ede9cf38eca98a08d59705da07a4d2f15c0ae8495e647e8fb5f2f`  
		Last Modified: Thu, 13 May 2021 01:44:19 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:11b893a390d4f14d475156d2316c008d3aad37aa488772ef7e5b367f03c20b63
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104253572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d7b614afc4796360163f90f0be676ab2bc192d6aa5ea0fd6fd80d1437904588`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 12 May 2021 01:11:51 GMT
ADD file:81cfd4e746bdfcc19847240b77012487652be22dbd5741ccb2485a4207f2b73f in / 
# Wed, 12 May 2021 01:11:56 GMT
CMD ["bash"]
# Thu, 27 May 2021 00:45:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:45:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 15:24:13 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 27 May 2021 15:24:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 27 May 2021 15:24:29 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 27 May 2021 15:24:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 27 May 2021 15:24:34 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 27 May 2021 15:24:34 GMT
EXPOSE 9092
# Thu, 27 May 2021 15:24:34 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 27 May 2021 15:24:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 27 May 2021 15:24:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 May 2021 15:24:35 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:55b9a6b6b2552c5b2eac0a316e75a7bc18092819ee25c4f1d4d54700bcc1d3dc`  
		Last Modified: Wed, 12 May 2021 01:21:23 GMT  
		Size: 42.1 MB (42120307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba756a0ca8996787a145d62543ecf7cec523a638705be132f442d2013655149`  
		Last Modified: Thu, 27 May 2021 01:06:39 GMT  
		Size: 10.0 MB (9950803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61945aef6a8fee06fbe4dccead7cbad9da46ba174cee1eae1f813541ddb76b3`  
		Last Modified: Thu, 27 May 2021 01:06:38 GMT  
		Size: 3.9 MB (3921169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f0caaed9872f09cfec75a2a6ae01a4bf47adb5f7bad5d63bb822f235fa7538`  
		Last Modified: Thu, 27 May 2021 15:25:04 GMT  
		Size: 13.5 MB (13471332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f7b135b7305744606fa4269bd800266ba98474e8d1448b372418d65dbd28fc`  
		Last Modified: Thu, 27 May 2021 15:25:01 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc129f582c7b2ad5e74a23eb114991e4437fadd5f5f0b563da5736e6fe8704a`  
		Last Modified: Thu, 27 May 2021 15:25:27 GMT  
		Size: 34.8 MB (34786652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc39b8bac4be3a50381a992e2a62fa2da54b90031d9790fe3e7c60c13caa99`  
		Last Modified: Thu, 27 May 2021 15:25:21 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36170f3dbd5926adbbaef991792135405c512502786fc88dbfc7fc91f16fb8fe`  
		Last Modified: Thu, 27 May 2021 15:25:21 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:24dfe8ac7fca92649bb754592134fa03fd39b60c2a8bc5308b310527df24ad0b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105059188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fca6192994de70947ed75db98334f8a3c6336ee728eae3131ef3472393da040`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:55 GMT
ADD file:02285d0bd3ea996a7ebbe069a83e508701cbaf14f53fdeaa123775acd7e0537f in / 
# Tue, 22 Jun 2021 23:50:56 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:27:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:27:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 18:30:27 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 23 Jun 2021 18:30:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 23 Jun 2021 18:30:40 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 23 Jun 2021 18:30:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 23 Jun 2021 18:30:43 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 23 Jun 2021 18:30:43 GMT
EXPOSE 9092
# Wed, 23 Jun 2021 18:30:44 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 23 Jun 2021 18:30:44 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 23 Jun 2021 18:30:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 18:30:44 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:0789e4a342a11c7c57a241829a41af53fbd194e6dede60c6d6f63d69e403b2cd`  
		Last Modified: Tue, 22 Jun 2021 23:57:52 GMT  
		Size: 43.2 MB (43177421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd2ed69368e8a7d296f1c91060e897753bed4a79ab68ed47c544e1f4d6fadcd`  
		Last Modified: Wed, 23 Jun 2021 00:35:58 GMT  
		Size: 10.2 MB (10214577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c76e514669ff971481e0d19dc0581f90d72eab2d0e117a5761ae016e14f213`  
		Last Modified: Wed, 23 Jun 2021 00:35:57 GMT  
		Size: 4.1 MB (4096534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2de4768a1c15ce3980cc7ad3cb98882f89999a553fb1328ee0ea58ca1a1a22`  
		Last Modified: Wed, 23 Jun 2021 18:31:05 GMT  
		Size: 13.0 MB (13006392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae8c40d5b6ee697f7d91f741516f12b3b77ba2e7f2659cf27640152496aef83`  
		Last Modified: Wed, 23 Jun 2021 18:31:03 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271cc6c4cc1d0584ef6813f00a7465e15d77ba403296321f11c6be76a8dea274`  
		Last Modified: Wed, 23 Jun 2021 18:31:25 GMT  
		Size: 34.6 MB (34560953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a251bef91330d334e7f4ae9ccf4cdcc9f097b48744320a9d0c7405e3b019458f`  
		Last Modified: Wed, 23 Jun 2021 18:31:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e75f9e176592ceb800838fbf17f5bbc3417520f888ced9d4f01288e462f6acd`  
		Last Modified: Wed, 23 Jun 2021 18:31:20 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
