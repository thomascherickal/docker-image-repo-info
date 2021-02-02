## `influxdb:latest`

```console
$ docker pull influxdb@sha256:02908edd69cade1f916895d6577aa0cd1712f92ce2deb7c22d73d7144b0b2282
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:ada4dcc9a67b815529696d164a3eb7124059a92f63006fbac8e25626b2dfe1a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125444383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:552d5be6631f3705c870d04deb412ff12285192b401efa33cb285ef143bcd17f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:05 GMT
ADD file:166cd044a29ad501c753917f07d638932f2ce960a8570b12d9155e8c38d1e917 in / 
# Tue, 12 Jan 2021 00:35:06 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 04:00:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 04:00:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jan 2021 00:03:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 02 Feb 2021 22:20:21 GMT
ENV INFLUXDB_VERSION=1.8.4
# Tue, 02 Feb 2021 22:20:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 02 Feb 2021 22:20:27 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 02 Feb 2021 22:20:28 GMT
EXPOSE 8086
# Tue, 02 Feb 2021 22:20:28 GMT
VOLUME [/var/lib/influxdb]
# Tue, 02 Feb 2021 22:20:28 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 02 Feb 2021 22:20:28 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 02 Feb 2021 22:20:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 Feb 2021 22:20:29 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:2587235a7635c6991dfee9791c7977ab29694cf73bc64c3c5a79097ca99364d1`  
		Last Modified: Tue, 12 Jan 2021 00:43:05 GMT  
		Size: 45.4 MB (45380014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953fe5c215cb5f929e0e42e5a1011f33edce9278a650faf10655e855a670f79f`  
		Last Modified: Tue, 12 Jan 2021 04:08:01 GMT  
		Size: 10.8 MB (10753468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d3f270c7deffd353181076af3b5746c8dbeac5abf454169a75e7822587bdab`  
		Last Modified: Tue, 12 Jan 2021 04:07:59 GMT  
		Size: 4.3 MB (4340646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81696497404d5b0c28802af968f980fe26d1a5ad4f1336891f53d07cea78c20`  
		Last Modified: Wed, 13 Jan 2021 00:05:21 GMT  
		Size: 2.8 KB (2824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b211c9173929e95d49aadec1ef15875f7e3e673e09ba2ea4dc42a3a449380ea`  
		Last Modified: Tue, 02 Feb 2021 22:21:44 GMT  
		Size: 65.0 MB (64965713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a458127ebd4a9630243b2f2c226b454c6e7ecbb2c8882eecd652386d5331fb`  
		Last Modified: Tue, 02 Feb 2021 22:21:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec98458b93cd4307ccf4270f348d58cf0cc3363f4e3d096ebb14517e02b83f81`  
		Last Modified: Tue, 02 Feb 2021 22:21:34 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc38ca6f0e74d6da860b16360551fcb25ac2e2bd41cdcd7ffd91b3fb2b0fb994`  
		Last Modified: Tue, 02 Feb 2021 22:21:34 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:a5511924771266d18e4edbf85a636664cb656d9b1a0b87b27d3ba08f543bdac7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.6 MB (116550123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0050b91b2f6a3929c8630674855a22f29039db4e367c9e83b68c301dcccfa59`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:19 GMT
ADD file:9c744a203d36aa8c515bbc11873a4a479cdf3fe9f020ca1ef207b53e6b3a251e in / 
# Tue, 12 Jan 2021 00:05:23 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:21:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 17:20:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 02 Feb 2021 21:59:13 GMT
ENV INFLUXDB_VERSION=1.8.4
# Tue, 02 Feb 2021 21:59:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 02 Feb 2021 21:59:26 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 02 Feb 2021 21:59:27 GMT
EXPOSE 8086
# Tue, 02 Feb 2021 21:59:27 GMT
VOLUME [/var/lib/influxdb]
# Tue, 02 Feb 2021 21:59:28 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 02 Feb 2021 21:59:29 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 02 Feb 2021 21:59:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 Feb 2021 21:59:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f5de2649c1cd9091872f81b8ceb6a67890124f113d9fce9c52bf60d5a6e19f43`  
		Last Modified: Tue, 12 Jan 2021 00:15:23 GMT  
		Size: 42.1 MB (42119951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cae60aac6e598935e2b14216dc4265434ba03d17c82f622b18abb712577d2c`  
		Last Modified: Tue, 12 Jan 2021 01:34:01 GMT  
		Size: 9.4 MB (9446203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9694e28a75917ff08caeaee5ed8729a2f12d2110bf203781d578006a0ef2f7`  
		Last Modified: Tue, 12 Jan 2021 01:33:59 GMT  
		Size: 3.9 MB (3919958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9af4291e32292c1b3e0baa3521c9903226273223480ec660c81d82cec54e2b`  
		Last Modified: Tue, 12 Jan 2021 17:21:15 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576599399aa29cbfc79e30b281278d325b4825c71877ef9d7c7f4df971ffd02`  
		Last Modified: Tue, 02 Feb 2021 22:00:00 GMT  
		Size: 61.1 MB (61059440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a000ac17508af47f0ff85be0948a069573a660b0cefc9ea0b444503c4b6691`  
		Last Modified: Tue, 02 Feb 2021 21:59:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908d04411340b65bf9345e8c6190a556bb150e0df319ab1b000f609870b0b10e`  
		Last Modified: Tue, 02 Feb 2021 21:59:44 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3111337156de93fb9ee062547534d3aafd5d2e2970eabc8d12f5dd73d2cd6e52`  
		Last Modified: Tue, 02 Feb 2021 21:59:44 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:f9680f0d6743384c581c145bfdef0aa10b6f2325c7a932d1cb7964c4ab90eddc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117609891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e67d892ba832e27c0dcfbc8e625ce11a8343756882d45cb76e5503e68388c3ba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jan 2021 00:45:18 GMT
ADD file:bc4af94773a01defa7a79adb22199dde2229843dae224d13d3385c522cb71652 in / 
# Tue, 12 Jan 2021 00:45:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:30:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:30:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 23:29:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 02 Feb 2021 22:39:56 GMT
ENV INFLUXDB_VERSION=1.8.4
# Tue, 02 Feb 2021 22:40:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 02 Feb 2021 22:40:07 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 02 Feb 2021 22:40:08 GMT
EXPOSE 8086
# Tue, 02 Feb 2021 22:40:09 GMT
VOLUME [/var/lib/influxdb]
# Tue, 02 Feb 2021 22:40:10 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 02 Feb 2021 22:40:11 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 02 Feb 2021 22:40:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 Feb 2021 22:40:14 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:ec4f0a0f30ab1b4fc2e412a926b8608502de98203ca1994c7916de2017136729`  
		Last Modified: Tue, 12 Jan 2021 00:54:45 GMT  
		Size: 43.2 MB (43177964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0d21e1234248b5afd95bc41f061ec505353daeca6d4d5312a0167507857e72`  
		Last Modified: Tue, 12 Jan 2021 01:41:51 GMT  
		Size: 9.7 MB (9703645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e47f4b9ead7d5e8caca5072922207d5aa928f0144af32c78cf5a7e165f1898b`  
		Last Modified: Tue, 12 Jan 2021 01:41:48 GMT  
		Size: 4.1 MB (4095462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb8222116769c919fbd19b3d4994234f15315cce32dcf5094060adde3b4024bc`  
		Last Modified: Tue, 12 Jan 2021 23:30:53 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347222c27cbeeaff87dab72f84d2b4510b94853009e68827af1f83a89eee2e02`  
		Last Modified: Tue, 02 Feb 2021 22:40:42 GMT  
		Size: 60.6 MB (60628247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5894457fd7ac4718d1be902227a6a3720afd9859f3b4ab8464d1593e83e10b`  
		Last Modified: Tue, 02 Feb 2021 22:40:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba20db67c9969ddab0048caa36938ae32ee2d8d87d1f33d1c664a639bcd0335`  
		Last Modified: Tue, 02 Feb 2021 22:40:29 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003ab9aa1c4ec997514417eb2b6bd2a7ac890a16c63b3524d505f9af7b9d971a`  
		Last Modified: Tue, 02 Feb 2021 22:40:29 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
