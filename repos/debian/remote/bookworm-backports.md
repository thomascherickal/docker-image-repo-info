## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:1c89c723e6258d375ba56b32440f73d8077b1bd4b2f1979047cda5f62839a99f
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

### `debian:bookworm-backports` - linux; amd64

```console
$ docker pull debian@sha256:72eead981f579e6b9cfb68b7729fb4e8d09991ffd454613f4aecf2e4053c56c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.6 MB (55584550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e76ff19cecc31b46fb39690c33b2492cceb851270502fcc96a2be1b2e0757e0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:21:48 GMT
ADD file:084dc3db6641669bf09de94b7a32f3180ca32152a22a677961428ad78324f10c in / 
# Tue, 29 Mar 2022 00:21:48 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:21:51 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6673186ed4ed62930866783fb71f9386d0ece250e264d269d06e238753c30392`  
		Last Modified: Tue, 29 Mar 2022 00:26:08 GMT  
		Size: 55.6 MB (55584323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbe4f2656365d715d1846a8c3f0340d520cf11ac973fa908f291ba72db8717a`  
		Last Modified: Tue, 29 Mar 2022 00:26:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:e2d661d16fe6595df5b419c0dddda22a650cc261a87214f4b9c716065d33b015
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52995752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58f9147e6c6b9c205c65ebf6a1c33c09eae68d777b2b3b5386ae4285c48e09f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:07 GMT
ADD file:6b5b5c095508b777a2c8b2633d97d6143bfab0320bed58e8e335179bfd681fc9 in / 
# Tue, 29 Mar 2022 00:49:08 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:49:19 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9b209f6efb315c2c09d16e50d6077a10a401191c741a83c3c6c0767fe202d69d`  
		Last Modified: Tue, 29 Mar 2022 01:03:30 GMT  
		Size: 53.0 MB (52995524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08fd506ad8b11a6995ff0d3355d95bd68f0132ea316c6325d5f0cec940941ec`  
		Last Modified: Tue, 29 Mar 2022 01:03:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:6a5ee7b5b875a2767b92a0abb98f0cc28d5916b46e9bfdc22cebae0b284649c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50610028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac9386130d42b43f0a6aa0ba7b15d2bcefbd0fe80b757b6ffc3311fc5a7da7f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:16:59 GMT
ADD file:5ab9a8a4847f677425562eebef8854e58592bb57501d4bc6f521315d90815c3c in / 
# Tue, 29 Mar 2022 02:17:01 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 02:17:13 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c7c8b286eb908a262d0005e4560150fabc15db4a3531f7e00f77b76643457e6c`  
		Last Modified: Tue, 29 Mar 2022 02:32:14 GMT  
		Size: 50.6 MB (50609802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f44aedd4e60510861dcb7935a8a1c48882ad350349c54e886ef5f07f034098d`  
		Last Modified: Tue, 29 Mar 2022 02:32:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:fed9b23556c6cc16a2c043c03dc4b4359aadd6607fc21d6807c2eaddce5a94f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54505402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53e5de5e2c263e0f7a1cb5e64a838b9d95a46499dd1bf307d8643d6b324b27b2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:37 GMT
ADD file:8a0795f999cb36975538f6060cde3753f8d82b0c997ba2861ab1e317b5dd52a1 in / 
# Tue, 29 Mar 2022 00:42:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:42:44 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8fa507a56d88ff151c2943292a587b9de276f98f32670b4a39659e57e5f891f6`  
		Last Modified: Tue, 29 Mar 2022 00:48:52 GMT  
		Size: 54.5 MB (54505175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a17f6a83531300f36825012f5d2060c834f7a987d963f6183412afe7037a36`  
		Last Modified: Tue, 29 Mar 2022 00:49:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:ea850cc0c0300e16631a5152a791423326531417f404d2779f4bfef1082c9617
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56628446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3fd4f59f10b2528647b2c2ddc0f47516142f5e7f4849a7b2ec757eb418836c1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:20 GMT
ADD file:828aa883b729cb9e3bbc9efef043626425a2803461bd7b07862d746e2df08c10 in / 
# Tue, 29 Mar 2022 00:41:21 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:41:27 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4e0acfe1e9e31a265994eee72788e1a0b4b33edc5c9d6fc978fd65d87aa94b53`  
		Last Modified: Tue, 29 Mar 2022 00:47:47 GMT  
		Size: 56.6 MB (56628219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd41cbda449a264c8118f874c26f32089f9845fd6868ec89b0875623505026b`  
		Last Modified: Tue, 29 Mar 2022 00:47:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:ec04aac659110ff0d16d859c8dd5fe83169023189ae9e095c07157b7fcfb4566
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54339389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f20fd1f0c77bf581bc8c2f47be04361166d7c5e6aacb0d6bc2ad3b513d83199c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 08:51:08 GMT
ADD file:550d1d8a058f07f217e9d0ec1e582f897b1cd24ad6c6c3697d5c89039c5ae265 in / 
# Thu, 17 Mar 2022 08:51:13 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:51:33 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f4e5d74924161483e853a5bf08fcf297bf47b3124d7d1840e280c5f487a8750d`  
		Last Modified: Thu, 17 Mar 2022 10:41:21 GMT  
		Size: 54.3 MB (54339160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb49043182bf319c24e01b82b438cda684de59f98da186692abc812b40e48a4`  
		Last Modified: Thu, 17 Mar 2022 10:41:31 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:d0430aabdd1681c17f7cf96bcb1d27d94a977567d47b31b40b627cf987b6a5e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (59999648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db205419660895e5fcc1894bc73068a4671088be6afa3b37a6a447d668bbb336`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:20:10 GMT
ADD file:c9ff325b9fe680d344c36e7e25729f90711bdf646908892ebdc0f3a53d92bc50 in / 
# Tue, 29 Mar 2022 00:20:29 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:21:00 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fc5522fc3ca5c5e9e4af133a35ed8a4e104c9366b7ab66c3cc5601aef68f175a`  
		Last Modified: Tue, 29 Mar 2022 00:30:15 GMT  
		Size: 60.0 MB (59999423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d5116f2188bf2a8e74c4da46e1d7f424271f8c17836b62f3ec039898c7d564`  
		Last Modified: Tue, 29 Mar 2022 00:30:28 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:8d295f958c6a9539ada7f61e5adf7cca5b51f472624e5bdc3dfa646a06993954
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53839290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4b3ba1b73b6da5647126b52dded17237bf57bcf89467e1f475cae21a8460ae4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:05 GMT
ADD file:9a99e896abdfac4163e20511778572abbec89bf317a3c3dad1f6fe0c63b126b1 in / 
# Tue, 29 Mar 2022 00:51:11 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:51:18 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4c231abb22533340c714e28363f98b83f5da88a6702fdfc7d06ed65b8f2e70e1`  
		Last Modified: Tue, 29 Mar 2022 00:57:13 GMT  
		Size: 53.8 MB (53839067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abbe3ac21a3fb5ce958ee5dccbe9a4c48d2c4b7b73fa159cf6f116722e60645`  
		Last Modified: Tue, 29 Mar 2022 00:58:27 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
