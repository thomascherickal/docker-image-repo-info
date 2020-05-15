## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:3b8f751d99657f6a977dede0e15bcbbafa861d524df1998743a7163a1219c342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:3876027c3fcd9cf0045f206533d4a535094a71e6815f77aadb47de34c4c08905
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45375392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4ee2294186c83b10bb665e0a5dc76c0ea5d47ce843fa8b0a42b7c290a09861b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:31:04 GMT
ADD file:37b9b59ff14f2acc18c4b2d704e57ff8293114a40a34347a3664543864a39738 in / 
# Fri, 15 May 2020 06:31:04 GMT
CMD ["bash"]
# Fri, 15 May 2020 06:31:12 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8bfa9979f36663ad5f264c79ec562de99c90ee8651d1303e465922033afde055`  
		Last Modified: Fri, 15 May 2020 06:39:20 GMT  
		Size: 45.4 MB (45375165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f400e58c254e6c81d2c441f7fa9464977745614b179165d5b8bfbf895017bf`  
		Last Modified: Fri, 15 May 2020 06:39:25 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:6811c499e19a6fb9360a10df22064e55bff174c6e9d5c37aaac228689cc6260e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44072065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e733af377333cba2bc48f18d0c8a2d71410b25490f79ebf69d4a8ba9b9fd7b9e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:39:52 GMT
ADD file:6a3873172bb05469b39267e97faaa5a88b26d10163455ce92858ab00b41403d6 in / 
# Thu, 14 May 2020 22:39:58 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:40:06 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a02dc173a7c3af68f27ba7bd2c84ad3bd4f5bea223b3221684760db06547d99f`  
		Last Modified: Thu, 14 May 2020 22:48:42 GMT  
		Size: 44.1 MB (44071839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0173ca5a4fe85d95bc7c8740e5ff479329cc1d55cdebc25305d0520841d4ea8a`  
		Last Modified: Thu, 14 May 2020 22:48:48 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:02c5ba8b80d3c4eebc9b47aab2ea222ee2c58f54058aa8de5c4cfe3f9647d81a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42104566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82ba2063a6a6eac9af6e9191540b40649ae7316a3c8c83b334ddf44b9527da9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 01:03:00 GMT
ADD file:b70996930efc92ef82442e29285863d25b4752968a27e17713d02a049ae3a80e in / 
# Fri, 15 May 2020 01:03:04 GMT
CMD ["bash"]
# Fri, 15 May 2020 01:03:12 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:968153165585368b1b1ab25931c78d0f5b0307ef01cdeeecdf94a2b9955c4c7a`  
		Last Modified: Fri, 15 May 2020 01:12:58 GMT  
		Size: 42.1 MB (42104340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f15308b1e219d0328fbdb103745bcbb6d999cedb03b91d1181b7e01b503b8a9`  
		Last Modified: Fri, 15 May 2020 01:13:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:c8a3ec8d593bc76d3d32fe26c861151ba55306f323d772752df18603e8d23b24
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43159178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a2229551dbc8eaf910064355df75e94274c78c627c511905313a8d8008e7237`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:44:18 GMT
ADD file:dec7fc852e537016129a47b5cc0eb374c6b09fd17076b51eb1f3d92cdd9ad4d4 in / 
# Wed, 13 May 2020 21:44:22 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:44:30 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:451c2749d61ce76b7d1709f64624274d850bfb86aea7dc0c21833feee377fad1`  
		Last Modified: Wed, 13 May 2020 21:54:05 GMT  
		Size: 43.2 MB (43158952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8b2672f85cad68449279f42973fe3652834731c736a6ef48f800f10431e4b5`  
		Last Modified: Wed, 13 May 2020 21:54:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:1acee3bffeb4fe1c10b4da51d72bfa2c0cfcca7e89ad3912a2fa660c1274c3ec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46094423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b44cdb4090911d6f4016da89ea7f373ea31aa032494fe2a8cee46345aeaf968b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 07:10:09 GMT
ADD file:3c2d5842310981befad4f477c954f48b954cf78ec4b8cf60029e4107b8dbf3fa in / 
# Fri, 15 May 2020 07:10:10 GMT
CMD ["bash"]
# Fri, 15 May 2020 07:10:16 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:028cf857dd88f16fbdcb3a4b83546cf0510233507394f8a6bd028b1f1bc27c43`  
		Last Modified: Fri, 15 May 2020 07:20:29 GMT  
		Size: 46.1 MB (46094198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9854968e1b8ba98d4c46dd5ddb8727036c1e1a0e9cb9a930bedbd950d37d2c`  
		Last Modified: Fri, 15 May 2020 07:20:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:17b743ba9fcfaaf4ccd251c6ce2ec07e3144a575931aaf0eac4930064cd30476
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45050102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13265596b0a105ab9474a32becbe49bc84cd411d040f51dd93970ae10ec8bc11`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 04:48:46 GMT
ADD file:1b71c07d820c2979d63c3646bcb632b5f2f8dc73daeef2ae26ddccc70fa32cf2 in / 
# Fri, 15 May 2020 04:48:47 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:48:54 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1bbf7d0d9c5c4b6af2e8f0eef03b2f0f65b931c5c57c2d7dbc57a3a0078c61e0`  
		Last Modified: Fri, 15 May 2020 04:57:56 GMT  
		Size: 45.0 MB (45049875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0552409f8d4c64450dd255601a2f5f1cd5774317a6478eef120afc99ee3896`  
		Last Modified: Fri, 15 May 2020 04:58:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:74c9ad3400ad1107cb4d2b520fef0d5a657b8bb6a510bb5c356409f21a31319a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45646476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31cecff44695f5f3e47bbaecfa217f65fd6b01967a8f819e80ce8d5ca68a43da`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:24:15 GMT
ADD file:6443a668a74fcf32c5f82767f4c12add1107287df828576bf5d06f38f8f75f44 in / 
# Wed, 13 May 2020 22:24:19 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:24:44 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:923a4cedc3d159656a04021e9503d6cecd76cc101ab226fda7e4a2ac888a1026`  
		Last Modified: Wed, 13 May 2020 22:58:39 GMT  
		Size: 45.6 MB (45646248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5485ef1e0a6864d57a87b0dd3731bac16ec4b4590d057483e812388365a56e9`  
		Last Modified: Wed, 13 May 2020 22:58:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:8efb1077ad028523cc75acef0d3935cbb268f7634fc480e7fe4257e8ad324cd9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45232363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c245b53ff53e485f2a0159d01636c15c4d8b2f026d8960a17efeb32de3ca37b3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:06:53 GMT
ADD file:7bb64228e15ddc34d5624c8a3329ef68be997e4d299b95cceace485e00a24d8e in / 
# Thu, 14 May 2020 23:06:56 GMT
CMD ["bash"]
# Thu, 14 May 2020 23:07:00 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b28e354f80f29bc9dbe7da5033d0a531dd9687922cabd20419a093a8bceff95a`  
		Last Modified: Thu, 14 May 2020 23:11:38 GMT  
		Size: 45.2 MB (45232139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27d67238a4eabfc82e170009c93727210a4f5c11ff520d670e04128e2b2ac3a`  
		Last Modified: Thu, 14 May 2020 23:11:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
