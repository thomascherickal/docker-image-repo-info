## `chronograf:latest`

```console
$ docker pull chronograf@sha256:2820623517af57335cacb1d423d06494591a5ba3198cbc3ee0f99b84fa89b97c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:d7fdd90ad0b1117dbced65f2a47c67c381112cbc5a17a5e1fd46c22a04cd73e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68562735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a24f6e0014e29782f7fc05ce98357c5a086f5fe9fb87ae58f9016297b1402ee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:15:39 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 28 Feb 2020 01:20:04 GMT
ENV CHRONOGRAF_VERSION=1.8.0
# Fri, 28 Feb 2020 01:20:15 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Feb 2020 01:20:15 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 28 Feb 2020 01:20:16 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 28 Feb 2020 01:20:16 GMT
EXPOSE 8888
# Fri, 28 Feb 2020 01:20:16 GMT
VOLUME [/var/lib/chronograf]
# Fri, 28 Feb 2020 01:20:16 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 28 Feb 2020 01:20:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 01:20:17 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f878ed3f571cef34099acbbbb2582f64051e11e88b899a5cfe4ef47d003542f`  
		Last Modified: Wed, 26 Feb 2020 02:17:16 GMT  
		Size: 4.5 MB (4503576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e454c33c8c6f9a4de0f767d6da317b38a58d459254fbf8604798a491abf048a4`  
		Last Modified: Fri, 28 Feb 2020 01:21:08 GMT  
		Size: 41.5 MB (41521400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea49d70782a09b527bce1697cf33bad4f27e3da7974651db0998d2b040c5698`  
		Last Modified: Fri, 28 Feb 2020 01:21:02 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cef5051ac1daa01e32dc068aa82007d3098f9d7b128d603902be56bada8c55`  
		Last Modified: Fri, 28 Feb 2020 01:21:01 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bd6389f3722b8212107be1af7a007f8a8d54fc075e0a3aff74e3ac3b3c5454`  
		Last Modified: Fri, 28 Feb 2020 01:21:01 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:bf9a855735ceb7733e1e6bf6c8b2dcde555b59d320b5d46f6ae25fa3e06da5f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61979493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc82010da74c060152e94a4ef5f62decb4792637d7e46faffa40b01a78171320`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:29:13 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 28 Feb 2020 01:03:11 GMT
ENV CHRONOGRAF_VERSION=1.8.0
# Fri, 28 Feb 2020 01:03:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Feb 2020 01:03:39 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 28 Feb 2020 01:03:40 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 28 Feb 2020 01:03:40 GMT
EXPOSE 8888
# Fri, 28 Feb 2020 01:03:41 GMT
VOLUME [/var/lib/chronograf]
# Fri, 28 Feb 2020 01:03:42 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 28 Feb 2020 01:03:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 01:03:43 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15634d01c3f3a1bece118d96c09deb143bac89f0f8ab71aeb0c0629360a460f`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 3.9 MB (3877306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3240a3a7b219ecf570076b612a7d5aac06fc710fda3f8b166a3cc399d17105`  
		Last Modified: Fri, 28 Feb 2020 01:04:26 GMT  
		Size: 38.8 MB (38779447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ce217f1ce08e8bbd6bcbf1801e7f4fced07b2987011d044993543ebc600124`  
		Last Modified: Fri, 28 Feb 2020 01:04:14 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c004f6223ca0d5c2200f5b8b1af677da199902d40ed86883385f7d895780ee29`  
		Last Modified: Fri, 28 Feb 2020 01:04:15 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff433bb8cee205aa10e5c92076debbeb7b21d28a3c03641819aaeb8bcb5ffaea`  
		Last Modified: Fri, 28 Feb 2020 01:04:14 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:95b6f9a482a886f7f2fe526f89d354352dc4e4c38cf3ba9110cbfb2db2f13673
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63163830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:544b844fd5358a434ca76d6395371cf4915db5cd7199e5cadd8f742aa39d0170`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:10:29 GMT
RUN set -ex &&     apt-get update && apt-get install -y gpg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 28 Feb 2020 01:40:17 GMT
ENV CHRONOGRAF_VERSION=1.8.0
# Fri, 28 Feb 2020 01:40:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Feb 2020 01:40:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Fri, 28 Feb 2020 01:40:45 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Fri, 28 Feb 2020 01:40:48 GMT
EXPOSE 8888
# Fri, 28 Feb 2020 01:40:51 GMT
VOLUME [/var/lib/chronograf]
# Fri, 28 Feb 2020 01:40:53 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Fri, 28 Feb 2020 01:40:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 01:40:57 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f797dde9809216bf453cb02c743c00da5fed52ec53e5d746f9a7cfdb99720f`  
		Last Modified: Wed, 26 Feb 2020 04:12:22 GMT  
		Size: 4.1 MB (4080742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48780f7890892dae31b3d1274dfc8aff3c5c34ad58ae0f0bf5e1afbb238741a`  
		Last Modified: Fri, 28 Feb 2020 01:41:39 GMT  
		Size: 38.7 MB (38688710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dee94acf4498804a9d5a261e4df1ffe38798a5ff04352873de9764dfc5ffd23`  
		Last Modified: Fri, 28 Feb 2020 01:41:29 GMT  
		Size: 12.2 KB (12249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788706574837e9824494df99fc75fda33d7f4e909002ca901bf7cb56a480e811`  
		Last Modified: Fri, 28 Feb 2020 01:41:29 GMT  
		Size: 11.9 KB (11911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1311dfcdba68ef5487fbe417ac6484b4efb1fb3f285c268700a86549ae4345`  
		Last Modified: Fri, 28 Feb 2020 01:41:29 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
