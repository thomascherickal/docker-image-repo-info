## `debian:stretch-backports`

```console
$ docker pull debian@sha256:3bff1a549280f1ae20b3c2ba9a1a310a6c68dc24f687fa8516201f4078cf7b32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:stretch-backports` - linux; amd64

```console
$ docker pull debian@sha256:67b81553bf6a9d199b1b643a5de2b30a2abb090f7799c965a77505894814863e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45367004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85da5d54e71670ef03f44a75a738b7b11b7c124c71eda6eeedb93ee05846e208`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:13 GMT
ADD file:a8742c34bf12f231279dd5086b8ec1310224c740a95170b916217f22a68eb9a7 in / 
# Tue, 13 Oct 2020 01:44:13 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:44:21 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0400ac8f7460260a663e0e97c24d7dfd8a2c947736f0351752b45c53e26d6e02`  
		Last Modified: Tue, 13 Oct 2020 01:50:49 GMT  
		Size: 45.4 MB (45366778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e82c6880dc78f8505175ffce24031776035e0a213f53a667ccc6ac256a44b1`  
		Last Modified: Tue, 13 Oct 2020 01:50:54 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:dca31317fb2c701a2c3fe0512e411d43f1a8f4cdbfe368a6f46e521a97053fcb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44081174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:698f7193c2e7e7d8b2bf9bbb113be2387d38f07d9a86383a116d07fadb94f1e0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:57:04 GMT
ADD file:6f4d3470472b5212e1dbd38ea2cd6a5a484b5063f1fa9ebdc91648203964bb75 in / 
# Tue, 13 Oct 2020 01:57:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:57:15 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a64fd53844c1eb87fd33b20580df3bee11b29cdc3cca7f4aa4af0cc066e9ed4d`  
		Last Modified: Tue, 13 Oct 2020 02:05:13 GMT  
		Size: 44.1 MB (44080948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619b4d4fd4b10cbc1b5cf043ee124f53c51daf78d2b402bd89c910f4b7a04efc`  
		Last Modified: Tue, 13 Oct 2020 02:05:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:fa01f87d7254717d37b1ccddb587301f13bb158f13f0926a49f4f06f853fcbaf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42111510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:435c9f8cf516b8684930fe2cd3cb7132ee1d58f4dcb6e28738c13d4fefc01da7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:04:04 GMT
ADD file:fb1dab6b0ac08f52870fca9435eedd2f707a3b8a5d28e5d1c2ff88e096f695ec in / 
# Tue, 13 Oct 2020 01:04:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:04:13 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1b636fdf37230c276ff1507a9f2b0067182f369cd669d1852bf5b9f5ba3a43bf`  
		Last Modified: Tue, 13 Oct 2020 01:12:25 GMT  
		Size: 42.1 MB (42111286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d41fe2c9b4f084135e9707ded608f600424ca17158d4ed00cbc06a266692ae4`  
		Last Modified: Tue, 13 Oct 2020 01:12:34 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:1cf223a060c5a759e10c261f6a61648eeadc4f7592b13a58984928dca2313a55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43171768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b50b0684de9598489f9e986dc4cefdc28668dcff304b17538c70d296a6dad63`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:43:49 GMT
ADD file:2752d391988f4ad7e086be863c36a83a3226e31e44ea816ca4c89d6a410727b1 in / 
# Tue, 13 Oct 2020 01:43:51 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:44:05 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:19e4d0e7f8f2c5cb8a0a8d0e741e9e387c34bd673da69cdcc8e758a5c4dbc106`  
		Last Modified: Tue, 13 Oct 2020 01:50:49 GMT  
		Size: 43.2 MB (43171543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34dab338b48caac6336869a77ce07c89ff7c619d588cdaad7688e751223af29b`  
		Last Modified: Tue, 13 Oct 2020 01:51:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; 386

```console
$ docker pull debian@sha256:daf30eecbcb5b1b5640b657881dec346205feed74df7b1a74a943acf756eed0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46087090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c95d2d093a976884a7d3febc399ddcde74e09680704c55be4fba831ac5c3ebac`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:45:07 GMT
ADD file:2c53d7197ae361c4b9c751cf700f3d286a3cf5c77cf07d16756f36f61666bb40 in / 
# Tue, 13 Oct 2020 01:45:07 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:45:14 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3e5030fa46456155e6836658abedeff054349492fdd554f0476a8dd26a0da3d9`  
		Last Modified: Tue, 13 Oct 2020 01:51:57 GMT  
		Size: 46.1 MB (46086868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc0d35ee25c2b51569f6d67e9926f828ac089dff9633279c6dbd5dcf6455c84`  
		Last Modified: Tue, 13 Oct 2020 01:52:02 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
