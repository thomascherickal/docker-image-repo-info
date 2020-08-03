## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:d24560831cf0c7dd1f3c48f318023db0d67ac45acef116e31011bcdbd29239db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:3af62ad4c65dda932db4c9551b4e30b6e0f2feb70f5b1766c5f763657937534d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109847295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83b2733d8fbba48f231a71cb13788b483c650ae1d95b502528ece036fa88c100`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 22 Jul 2020 02:06:48 GMT
ADD file:f98fe3d719ea765cb59da025d506d0bbd6db7a842b6b63c58c8d4d65b51bdb1f in / 
# Wed, 22 Jul 2020 02:06:48 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 03:11:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 03:11:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Jul 2020 23:29:52 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 22 Jul 2020 23:29:55 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 22 Jul 2020 23:30:10 GMT
ENV KAPACITOR_VERSION=1.5.4
# Wed, 22 Jul 2020 23:30:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 22 Jul 2020 23:30:16 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 22 Jul 2020 23:30:16 GMT
EXPOSE 9092
# Wed, 22 Jul 2020 23:30:16 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 22 Jul 2020 23:30:17 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 22 Jul 2020 23:30:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Jul 2020 23:30:17 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:7e6d8ed603557d9bf077a9ace4ee506501970a4938b9a704f040ad15f22bd4e8`  
		Last Modified: Wed, 22 Jul 2020 02:12:13 GMT  
		Size: 45.4 MB (45369674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43421f771d04c7019cae6594c2b95ad92d692750fc57d201b5108c1bef2d095e`  
		Last Modified: Wed, 22 Jul 2020 03:19:27 GMT  
		Size: 10.8 MB (10750266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36327c39ae4245e3dcfa5b77a55cff18b6d81f2b4ca1b0e107da95ecd6b225f`  
		Last Modified: Wed, 22 Jul 2020 03:19:26 GMT  
		Size: 4.3 MB (4339838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea5eff0a5678d78f893ac5a9a78f02e94f11877e03b3a20ee20d97a49957ada`  
		Last Modified: Wed, 22 Jul 2020 23:30:32 GMT  
		Size: 13.1 MB (13073672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e848ec8993e33112fa0e38bc4fcdf8e5aa88e39b2feb5e7328dd67b5b859cf7`  
		Last Modified: Wed, 22 Jul 2020 23:30:31 GMT  
		Size: 2.8 KB (2776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c8486ca3fc78068e6a6111828c0524657ad6ae8bdf710f318462c5d0197540`  
		Last Modified: Wed, 22 Jul 2020 23:30:46 GMT  
		Size: 36.3 MB (36310613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b532c441a0a861962f6b624e2027fa16bfa9c5d8652e7a6cfdb070315aa481d4`  
		Last Modified: Wed, 22 Jul 2020 23:30:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81163a5d468940e505950d644bad9781f3cc0dc0fea48071130c2ceb8b0f9ea4`  
		Last Modified: Wed, 22 Jul 2020 23:30:40 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:1f8bce1f60ea5438e3781c64fe784ef22f5f72a924349a754e7ddc4b42e99b2f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102773421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7df4c6163b1d86b060e5fe537f8715e3776063a940e242503b9f1959b478d029`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 22 Jul 2020 01:32:02 GMT
ADD file:762e52a5e1d8ff2daa22c3bec2cfdfe4cbcf224deb1e73d7db3af0cbf5658785 in / 
# Wed, 22 Jul 2020 01:32:11 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 05:50:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 05:50:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Jul 2020 20:52:52 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 22 Jul 2020 20:52:57 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Mon, 03 Aug 2020 21:46:59 GMT
ENV KAPACITOR_VERSION=1.5.5
# Mon, 03 Aug 2020 21:47:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Mon, 03 Aug 2020 21:47:11 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Mon, 03 Aug 2020 21:47:12 GMT
EXPOSE 9092
# Mon, 03 Aug 2020 21:47:13 GMT
VOLUME [/var/lib/kapacitor]
# Mon, 03 Aug 2020 21:47:14 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Mon, 03 Aug 2020 21:47:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 03 Aug 2020 21:47:17 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:05dc12a0df610a09562914533797508b791bbd115ae17b6a1b75666ec90263da`  
		Last Modified: Wed, 22 Jul 2020 01:44:04 GMT  
		Size: 42.1 MB (42107480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b998b2d4ee2005b0f51e94b6fc7467091e54a910491e7873b9e0d6f59aabd98`  
		Last Modified: Wed, 22 Jul 2020 06:06:37 GMT  
		Size: 9.4 MB (9444083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15230f55c10a543d54564a792784b1d2e133d4edeadd58978682d9bf02d1425a`  
		Last Modified: Wed, 22 Jul 2020 06:06:34 GMT  
		Size: 3.9 MB (3918506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2628b2d3403c6d5dd3d249c789f8d9aab953458de8b098cbe1387c8f881efb09`  
		Last Modified: Wed, 22 Jul 2020 20:54:05 GMT  
		Size: 13.2 MB (13244196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc214edc871085e1d6821a0bd1eb117723b573a6cbd1c3db20942a47824b723`  
		Last Modified: Wed, 22 Jul 2020 20:53:55 GMT  
		Size: 2.8 KB (2804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3916c553cc72e09483a0303b80282f7fe0e4e40527f16115f16dadf2bbb214`  
		Last Modified: Mon, 03 Aug 2020 21:47:39 GMT  
		Size: 34.1 MB (34055896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20552944b50ad36a626006c284344a64fbda696f351232d4186cf740fe73329`  
		Last Modified: Mon, 03 Aug 2020 21:47:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5513e5e3cb1463bfe94d30c38a0fcdd6a544a1bbbb2c2dc3b966b7e54411f8f`  
		Last Modified: Mon, 03 Aug 2020 21:47:28 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:f3767f7f071ad5405e1b540c57d1d6bc190a1f63f1871df58727531ec2f18474
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.8 MB (103804963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1d1440de494d90c3763d322cfc266be8aaf32d0f8deb09d1e9767ec6a502e0c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 22 Jul 2020 00:43:42 GMT
ADD file:9c5c9df9952cb51291333837bdb462bbdf9f157e91e616f1e3fb8d2fcb1a1983 in / 
# Wed, 22 Jul 2020 00:43:45 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 01:26:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 01:27:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Jul 2020 23:36:13 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 22 Jul 2020 23:36:17 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Mon, 03 Aug 2020 21:59:41 GMT
ENV KAPACITOR_VERSION=1.5.5
# Mon, 03 Aug 2020 21:59:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Mon, 03 Aug 2020 21:59:49 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Mon, 03 Aug 2020 21:59:49 GMT
EXPOSE 9092
# Mon, 03 Aug 2020 21:59:50 GMT
VOLUME [/var/lib/kapacitor]
# Mon, 03 Aug 2020 21:59:51 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Mon, 03 Aug 2020 21:59:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 03 Aug 2020 21:59:52 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:ad4de4f68e9c2c0f5e5e62d379d936bb88ce467505ed002fb1e10c434fefe90c`  
		Last Modified: Wed, 22 Jul 2020 00:49:52 GMT  
		Size: 43.2 MB (43169407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05aedd313900c1f55a004cb5b8a8b93ee320b25c73286390f0669f387fd96c47`  
		Last Modified: Wed, 22 Jul 2020 01:38:43 GMT  
		Size: 9.7 MB (9700532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2bc27f6e0cc82b950064aa77aa261962e402cb805c2c36bef0ece1371fa405`  
		Last Modified: Wed, 22 Jul 2020 01:38:43 GMT  
		Size: 4.1 MB (4094121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490e067e56b5909f93d608850a0633fa64a0b39ddbdf0a7e81b1387473306ee9`  
		Last Modified: Wed, 22 Jul 2020 23:37:01 GMT  
		Size: 12.8 MB (12782021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647caa33ee5744a7f78909a58c2de32ffe78d092482544d9e685b739d30feb7d`  
		Last Modified: Wed, 22 Jul 2020 23:36:57 GMT  
		Size: 2.8 KB (2804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff314f2977d888a02bacfedbf366f75902e80fbad9158d3060ea4b1daa4a222`  
		Last Modified: Mon, 03 Aug 2020 22:00:12 GMT  
		Size: 34.1 MB (34055624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af0a6ab26a19b988ee51f960cc9f86ee02335f72032a428120789639fbbce8`  
		Last Modified: Mon, 03 Aug 2020 22:00:05 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dacc0b39bbf5aa7663232c5af437fc3da89c7afce4385204d3249b8645e69d0`  
		Last Modified: Mon, 03 Aug 2020 22:00:05 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
