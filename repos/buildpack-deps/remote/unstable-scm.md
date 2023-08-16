## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:3580956c9b85d435795cdcf2244a4e7d190309302f99161995532414d892be08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8a363c27455cd9f6fcde5596efa71102fa5c2cebfbf12fb0c5157e2fd3ab60b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.4 MB (138424099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4cd89db58a3ce0a728b12a56803552a04aa7aacfc0b27734d53addf8a3d8ac2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:26:24 GMT
ADD file:89538c836015e15bfe955d940c080e251ce5b25e2cfaac73d8ce77f8475cd08f in / 
# Thu, 27 Jul 2023 23:26:25 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:05:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:05:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9828fc546889681c4c23160b0ee9abb2a08f99ec58b166856cf38d03e0173700`  
		Last Modified: Thu, 27 Jul 2023 23:32:15 GMT  
		Size: 49.5 MB (49462924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1415ec03edfc71940d466b16992ddd3915658c3368432ddd33223a9bf80a2b`  
		Last Modified: Fri, 28 Jul 2023 03:10:17 GMT  
		Size: 24.3 MB (24286692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32deacfa38b7c02986a841b125a79769d3d74c100e44c5f5b142b35e13831a4`  
		Last Modified: Fri, 28 Jul 2023 03:10:34 GMT  
		Size: 64.7 MB (64674483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:995b60c9e41b030f0344790a1dff3b20c9cae8ee4c703b977c9b0d9430ab4061
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132646146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67a6c98e02bcec94970ee808e61c9a8590a882a8226f1b368af55d851188919a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:49:11 GMT
ADD file:2d486f4790de50d5a173ed5147c22ebcaaade283f5bdf6b62bc072050fc164c1 in / 
# Tue, 15 Aug 2023 23:49:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:44:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb27bc4b8f884dd1bc1129dd87397bcc993ec915005657bd21811eb84745100`  
		Last Modified: Tue, 15 Aug 2023 23:53:08 GMT  
		Size: 47.4 MB (47403781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f883267a6e0fd23a7321e7809daf18ea9fde5af7d382347913aa6b73346ef73`  
		Last Modified: Wed, 16 Aug 2023 00:49:09 GMT  
		Size: 22.9 MB (22942748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ea5e28c6c87005a46ad476c9b4f15160056117290320261d90a2241b5237f2`  
		Last Modified: Wed, 16 Aug 2023 00:49:27 GMT  
		Size: 62.3 MB (62299617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:71e545c4c300ac58377187dbd4799d9b01e698fcb27446348a1c64491d93b188
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127297881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cddd27e18a2b66911c51d5c160ed1e3ce962332301bbd360d705d4c34c88a93`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:18:42 GMT
ADD file:2a1f1ecc1cfa876ccc22e6ef2a3a4ea39a83aec70ecde3f7cdaddee69dac2002 in / 
# Wed, 16 Aug 2023 00:18:43 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:34:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:34:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccc7cdd48defe44f9a45f06f57d69b192155657bc5d244f915958c2027d645c3`  
		Last Modified: Wed, 16 Aug 2023 00:24:10 GMT  
		Size: 45.2 MB (45189279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6609fcf5feea7fb712abd4f4cc12586f4960ac4271da561ebf2ff0717e096c5`  
		Last Modified: Wed, 16 Aug 2023 05:50:44 GMT  
		Size: 22.2 MB (22170662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a916b1beb64303951348c4609b860a99cd5d81954299ea9ae649cc3d0d51fda`  
		Last Modified: Wed, 16 Aug 2023 05:51:01 GMT  
		Size: 59.9 MB (59937940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d2be3ea85b4c5c86e9424499855e28f42a6e36f936bc56f533cb789ae866bc12
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137979799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e5d9a52e4fa2879e47cae94ed7921d770e284c2b20f66a2e9e08faa8857704`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:41:01 GMT
ADD file:8064072457ccf7b4072e08095fa84f96b0fe3387ec8f302afde022186aa3eab5 in / 
# Tue, 15 Aug 2023 23:41:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:26:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4513653e4d749342b34f60c592adaf0ef4af993e76a913a1c086a4229a0e3afe`  
		Last Modified: Tue, 15 Aug 2023 23:45:54 GMT  
		Size: 49.5 MB (49531730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f5de6e756ae0263d5d8056bc2a6f2a8e87f5e28dde8b746fa6cb29bcd33513`  
		Last Modified: Wed, 16 Aug 2023 01:41:04 GMT  
		Size: 23.8 MB (23810620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c5bcfe9fb2496b09fb02f12a4c5eab9ce200446746f7c777fc1a0025d3a400`  
		Last Modified: Wed, 16 Aug 2023 01:41:19 GMT  
		Size: 64.6 MB (64637449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4e2ce5378c4db0184f2a5113732e97908ed485193eb9df0b315b2257f4f2d8f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.3 MB (142260559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:518bb0c85280b757bff997cb92e6a086ab364b971d4d25fa86e8f1e53e0ec81e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:34 GMT
ADD file:d86f66385d3993c597ac040a976cd8a826b097d014cc4f3b69d8ebfaa5aa6eff in / 
# Tue, 15 Aug 2023 23:40:35 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:32:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:32:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e41394c7daa90fb4aae0f67d43af5ee9838fb125e249fc0002bfdc3b90bb6c05`  
		Last Modified: Tue, 15 Aug 2023 23:46:33 GMT  
		Size: 50.6 MB (50631355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fb36009acd0e1d753239daf3a185a717a7e268ceb556a566bab97416024ee1`  
		Last Modified: Wed, 16 Aug 2023 00:38:32 GMT  
		Size: 25.1 MB (25115714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84633700d0e0c5a1fd8bad79e5e4601602218914f21595af58697a382ad3c928`  
		Last Modified: Wed, 16 Aug 2023 00:38:54 GMT  
		Size: 66.5 MB (66513490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:13c2f443dbe0048ee66a2dc9ba3c4726b576afd4987d853bbe4be5fd6c3035e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.8 MB (136780149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b5b566617eecf28afb7200ea107a9a85c4a5a8df702a8b6ef7b47930e217b4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:14:28 GMT
ADD file:5d5d4b53ad51debb95681500ba4a990279ff7fdd2ff80d4d4333b7dc647c0543 in / 
# Thu, 27 Jul 2023 23:14:34 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:28:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:29:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b48d6f46b6cff8bfdf81f7ffbfa05dff828e1d7545e640bf61d5486c1b79892`  
		Last Modified: Thu, 27 Jul 2023 23:25:52 GMT  
		Size: 49.3 MB (49334598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde2d4334b6bd5986094b014a83b3832c21ffb948989d6fb842246593177f671`  
		Last Modified: Fri, 28 Jul 2023 01:37:45 GMT  
		Size: 23.9 MB (23865537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86218b2ed81ed0041845b0b5b1e95efe348740465925fef57859a751cd7a6596`  
		Last Modified: Fri, 28 Jul 2023 01:38:35 GMT  
		Size: 63.6 MB (63580014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1522fa112776c1cbab6ae7bfc1609c9608e3575fa24e818e55ddc5ffe0e5c2a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.6 MB (149631567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bf814f247c4e74e1ae8028615dc5de955a05011d9f2f8a5799e6b4b77fc66d9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:11:08 GMT
ADD file:34567402b37eab48970f90189fd56c47e39acba6d260f0587409ca36a8d36458 in / 
# Wed, 16 Aug 2023 01:11:10 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:49:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:50:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c0db36c7b4f2702f9e0075ee892fe4761e0f37f5cc9d73192725313c01591737`  
		Last Modified: Wed, 16 Aug 2023 01:18:29 GMT  
		Size: 53.6 MB (53551877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08327233d2cd5240264b2d14e300da4220731205ebdb79a082288235d814fe5f`  
		Last Modified: Wed, 16 Aug 2023 02:13:00 GMT  
		Size: 25.9 MB (25943551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5b549a05446434e911aa7f23d6d7d3bbd3e215ad66876361d6e02362eab38a`  
		Last Modified: Wed, 16 Aug 2023 02:13:30 GMT  
		Size: 70.1 MB (70136139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:82b54224e16141b3d128a2c7213a413e390b1216abe389f923a2eaf497c751af
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129394231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4d1a4d2d9108164c640ce2247e18e16b8a958c777fd7a7181f424ddb829d083`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f8b93f818da821e670e126126d6da395bdf2888315b8baa1a6912378c2f4e02c`  
		Last Modified: Thu, 27 Jul 2023 23:12:55 GMT  
		Size: 45.7 MB (45656956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc8d46a9f89f9d06db33ee07cddd8aa1a54e242cd6463179064bb8e0711848`  
		Last Modified: Thu, 27 Jul 2023 23:45:49 GMT  
		Size: 23.4 MB (23350890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a627ecd6eb80659b2ec0c3464124a436336a8496c101d36a4e46180fdb32a2`  
		Last Modified: Thu, 27 Jul 2023 23:47:12 GMT  
		Size: 60.4 MB (60386385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:cfb04e68ce0c0aa89915d342517d5997324c820a3d6fc788f8df7964c3208fe6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.0 MB (136961726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cfcc1107c502eef2ef6942ab279be71a861768c71f2e77d5c0259e1a2da8e0a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:43:50 GMT
ADD file:a27e7d7c954291d644437a8054f06f492700f1ce13d3a9e2c3bbd71afd0869cf in / 
# Tue, 15 Aug 2023 23:43:56 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:24:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:25:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db9f34e47daed3854a411cee94f611a7139b82002ae54802c9a44d3faccaaea7`  
		Last Modified: Tue, 15 Aug 2023 23:49:01 GMT  
		Size: 48.6 MB (48594395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2492f56fd0a0d7311e408655d1a40ad1f5ce8d34da47a127ae2f85baf9cdfd9b`  
		Last Modified: Wed, 16 Aug 2023 04:37:57 GMT  
		Size: 24.5 MB (24455774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45414c0dac5eed7c0002a6ec3f910c9ab1430c15501a8f4ac7399a32a19be528`  
		Last Modified: Wed, 16 Aug 2023 04:38:12 GMT  
		Size: 63.9 MB (63911557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
