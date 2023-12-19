## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:4b82d7c9b7735332f0acc5f21092e198a7354d1a6e30aa514562efb7497c0f3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:bullseye-backports` - linux; amd64

```console
$ docker pull debian@sha256:decc0c65d7e5a13f007e39a90c1e3945cc222e97c6468409e1cb7a2352ce615d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55057566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb6c2e998719eb35eff8cba99932591d48c98a01cdcc853e7408a8161b11056`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:38 GMT
ADD file:d3a2f1f42338ba7066e352cea3b7bf4c7576e6b96fef785e8da763114f337c0e in / 
# Tue, 19 Dec 2023 01:20:38 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:20:42 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:18f2c3b7ca52caba205d748b9ce41784eb010ca83ece9e84e2a09130a5ec3cbc`  
		Last Modified: Tue, 19 Dec 2023 01:25:17 GMT  
		Size: 55.1 MB (55057340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309c3bae10728ad648ee51dde69b9681e3ed07e164d4779afe2972834739ee22`  
		Last Modified: Tue, 19 Dec 2023 01:25:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:34b8a451f1e14aedfa93b1fba98e219e56ca0605996f34bc846271f1ade9c642
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52562467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2de47928eb69b4c1914e3a487b824c3d79dbf5d6517e2f7a54badb1070f9e63`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:29 GMT
ADD file:10a67a16f03367965d9105db3d368f8cf27493769f1551c2bfdc274485bd7f6d in / 
# Tue, 19 Dec 2023 01:55:30 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:55:32 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:476954b0dbc0bbf3e36983f98ae01dfefa01670a85ffcb7ed6916095b71bdd38`  
		Last Modified: Tue, 19 Dec 2023 01:58:55 GMT  
		Size: 52.6 MB (52562242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cbcc8f3c0741ee494f9cd848e3a80a7befd0f66b4d3dd5c4db2237de16e021a`  
		Last Modified: Tue, 19 Dec 2023 01:59:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:2512bcb857c5b87587336cfa5fa2cddf5c157cf10847bd0b0408d9830477f926
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50216002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7ce034d0400d8f882526473a99f722236dd40fe2ac9a27bad00a6f2f5081535`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:07:59 GMT
ADD file:3b623bed8ec2536cb513edda1de6f79d2c8e06d6f82df2543202544dbba3ae3e in / 
# Tue, 19 Dec 2023 02:08:00 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:08:02 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1b42212018867046767b36eb95cf15c4b66bbb7b4fb552aab446d9822de5765c`  
		Last Modified: Tue, 19 Dec 2023 02:12:11 GMT  
		Size: 50.2 MB (50215775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde7fbebd50e1e42d2df66caca61107981d738fec1d70a89635f2a742f93e9ae`  
		Last Modified: Tue, 19 Dec 2023 02:12:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:bcbfa66fabf80558c47fffc36c4e7f868cf74d9026bd6d35ff320daaa112d984
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53708316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956b97918f6cccf0caa6fe5375dbfd585f9bf7dd2cbc743ac414adb77ba450ee`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:17 GMT
ADD file:06ba7e39a2f8e1a7bcbb929fa9d1e6fb1f8bdcf5096dc903576af8f7014e353b in / 
# Tue, 19 Dec 2023 01:41:18 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:41:20 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:396a672fee8bade1a7c9f228d919717447f110f39046d8b5ed21ad45ae13ab61`  
		Last Modified: Tue, 19 Dec 2023 01:44:57 GMT  
		Size: 53.7 MB (53708091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1566f330ad23d5f7ebeed3d0ff30a94c7a957eeeb25102f911ad49909010a6`  
		Last Modified: Tue, 19 Dec 2023 01:45:11 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:1a03c37aae778dfb3fa1a4833114a387e9d10fe8d330cdf44cc4596d7d932e8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56046563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4c1f75367648eeb1227c02c9fb390f6993187eb48f68a9c758af66d83c28c7f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:19 GMT
ADD file:8a328fced7ae3a6fc868bbb95c23191103e595c9d22b2626c16f155bc48b51a8 in / 
# Tue, 19 Dec 2023 01:39:20 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:39:23 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a789657fd5416b1ccfd519597a8f5e57bd5a80d04d1b1b7b2770df4469f4dd44`  
		Last Modified: Tue, 19 Dec 2023 01:44:07 GMT  
		Size: 56.0 MB (56046336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660b475a9f7ba9af5886957db01b226a82b7e0fcf0d9c73f458e7db719cc2a80`  
		Last Modified: Tue, 19 Dec 2023 01:44:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:eb488e732349ffb0a0a3f7c738d27bc7954c997e232974999fe16ae9b879f6c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53289236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e18080c85759223816319cbafb3baed5a276b3617857d97fee3124a1ca72d153`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:14:09 GMT
ADD file:95472c5be6ea30c4b6d715a3000e1bafb8e371897a96c9115040c4a7d2bb2c80 in / 
# Tue, 19 Dec 2023 02:14:15 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:14:29 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4d8f97806f78898e256ac429d0634dfcccbd6f6e81547afde1469a5968e33b18`  
		Last Modified: Tue, 19 Dec 2023 02:25:21 GMT  
		Size: 53.3 MB (53289008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ebc3e0e9969d90254c7e6fd17761c02df7500bc1fb43881ad30684d76f75e6`  
		Last Modified: Tue, 19 Dec 2023 02:25:36 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:22f6b914764984555586ea8f85a4a6410d6d08bd0fe8b165b63d4d84ee66a514
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58930138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d5c9d997e6e34230bc8d09c987519e1d3c6527517a1598003b595cd0e67937`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:22:03 GMT
ADD file:240a318dbc8a7ec4b3a6af5afec173d3579c94c27738b0f79750242acce5dd2f in / 
# Tue, 19 Dec 2023 01:22:06 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:22:11 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bdab4f9926bc1dc6c30480616baa760641ee4feeca1b5215d5c420b718c5a1a3`  
		Last Modified: Tue, 19 Dec 2023 01:26:44 GMT  
		Size: 58.9 MB (58929912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602ab58ea9671b7d229335b67ec555ea6791eae9566d2cfc2418c56231544cc2`  
		Last Modified: Tue, 19 Dec 2023 01:26:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:159ba0a800898989af57b2380c3523f55cfdfc18e5efa811c7dcee1bc87e1cb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53296185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:434fa8cd39312f1532cb083dde4fc87eb0d85bc2d03e09e6df0a6ed60687718e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:51 GMT
ADD file:f3ff7311d9c8e7c83e0b7746d9402fed156fb05bd0c704d49535b4ece7f33177 in / 
# Tue, 19 Dec 2023 01:42:55 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:43:02 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a7334865824cce0a21e0af9d1f48eaee160e0ac01a54ca220a9814e8d2059646`  
		Last Modified: Tue, 19 Dec 2023 01:47:52 GMT  
		Size: 53.3 MB (53295959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffdf035d0d51f4eff2b55cf1fb8c84181b393c81fa6e5e48c1b3889e453f1833`  
		Last Modified: Tue, 19 Dec 2023 01:48:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
