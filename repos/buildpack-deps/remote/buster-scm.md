## `buildpack-deps:buster-scm`

```console
$ docker pull buildpack-deps@sha256:f286a76d3edba5b7b14fb17c62bb72c3a52d84ec09dd7f3ad87323ca05f57b39
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

### `buildpack-deps:buster-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:6ffab0f004cd762450c55f762e8331aeab22bce8b2b67b12b2507ff02057e9de
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120024874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc45518e647bba1a745edb215364e98f89991f16888e7bb6cd6b5e442cc21a47`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:47:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5573c4b3094956931fd68c310ae92c9eb1a787f0c77ac2730be9d16cce172d5e`  
		Last Modified: Tue, 09 Jun 2020 02:00:08 GMT  
		Size: 51.8 MB (51827493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:33863959880c6d40d93abdbefc58b6c2741bf9cf0cee8a2b3927834bcbecb0e8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114727171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ccccb2ab5c6ea05f6a400eabe041a31370602a85ce862fd217194afab8b2f57`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:51:35 GMT
ADD file:2f1cc936406bc9d491f8bcacebb22061ff4c710311b85c5e852ce0d319421b68 in / 
# Tue, 09 Jun 2020 00:51:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:28:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:28:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:29:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3e588deec0981579bbdb8fdc5c1dde7b354b6df6fe9aaca73c69aa0bc697d812`  
		Last Modified: Tue, 09 Jun 2020 00:59:03 GMT  
		Size: 48.1 MB (48107094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b72a58ca618497267d363d547aa0cac4e121092ef4d192f9cd40d48fbaa46c`  
		Last Modified: Tue, 09 Jun 2020 01:58:04 GMT  
		Size: 7.4 MB (7360856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45fb48ce42ec95f1caafdac679b5a64b2cd2863a624e7e3cad6d34546279f720`  
		Last Modified: Tue, 09 Jun 2020 01:58:04 GMT  
		Size: 9.7 MB (9686959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19b56b1fead8edb93db924ab12912143e0a0529ae8bfac7b332b343489ce954`  
		Last Modified: Tue, 09 Jun 2020 01:58:29 GMT  
		Size: 49.6 MB (49572262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:84702e411d35a2b15682e78eb9eeb5ae71d075d1a743594cab4673d0d63aaccd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109666800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:066228d85836aefcf8216150e24969ac702c1a5a91e2e25c2c63ae28e847d042`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:00:40 GMT
ADD file:35073a186411c4b773a9d4d540ec0693ced845cb847b43d8465f9579174cd2b0 in / 
# Tue, 09 Jun 2020 01:00:45 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:48:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cff0731da2e4f4a0ae8329840eb7fed7ea6aac11aecbfa15c6e684caec03920d`  
		Last Modified: Tue, 09 Jun 2020 01:09:57 GMT  
		Size: 45.9 MB (45868949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbeb0ded58d68be17265763fda36a4e1a520234a291d66f370d98a3e0d6e591`  
		Last Modified: Tue, 09 Jun 2020 02:11:21 GMT  
		Size: 7.1 MB (7097860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6159fbed770bb99a219eae06828da55caaa649879843c0b9df18ddda9b698b3`  
		Last Modified: Tue, 09 Jun 2020 02:11:20 GMT  
		Size: 9.3 MB (9343524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba732bafeb6b1467fd6908c64c6e8d10ffb27e44e3a25ab4c6c38e8f753baa5`  
		Last Modified: Tue, 09 Jun 2020 02:11:43 GMT  
		Size: 47.4 MB (47356467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e03e49d67c8d810e1604e49d9ce241588701d1ee073f35c8ca96036b0e53e795
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118992875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f1c94a29e8fb05169d40efaa77f7533081e3d256c4178b5e6dedacb41c69878`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 12:43:21 GMT
ADD file:be06dd722febf4e72f7e626f70029986a5c75880941cabd553f695dd66bcbaff in / 
# Fri, 15 May 2020 12:43:25 GMT
CMD ["bash"]
# Fri, 15 May 2020 20:06:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:06:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 20:07:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d23bf71de5e1fea32788576972e233e80db7c51d831ed7edb269102dab298bf1`  
		Last Modified: Fri, 15 May 2020 12:53:11 GMT  
		Size: 49.2 MB (49170530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f6b089b3526111514262a58bbb27c5a292d7ef355184883365cdce9a7c61e5`  
		Last Modified: Fri, 15 May 2020 20:19:12 GMT  
		Size: 7.7 MB (7681693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34690136adb76fac1a121f6c4a9b5a63de1def4d65e0b2f99ff84c392ed8244`  
		Last Modified: Fri, 15 May 2020 20:19:13 GMT  
		Size: 10.0 MB (9983897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4287f76f52e4c390d78182615c75d2b3d6a5cd5b2c28dc554707a7cfbfa91f2b`  
		Last Modified: Fri, 15 May 2020 20:19:34 GMT  
		Size: 52.2 MB (52156755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8b3662eca72c56bb76c611d77807e16843962a48b3720efa331a9a5a1d72a363
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122905392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c73c3faa94101b6708e2e8d7cde35010215ca207a81515b742c1ed31f940f95`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:39:33 GMT
ADD file:f95fda6e1e7823d93ca50dd67a1ab99bdc8a7dea372ef27426915702500d54a2 in / 
# Tue, 09 Jun 2020 01:39:33 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:11:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:11:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:12:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca172633df711443e1bcc46650b24074efa097045feee542ecbb4934ae3ae01b`  
		Last Modified: Tue, 09 Jun 2020 01:44:44 GMT  
		Size: 51.2 MB (51156157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e4e2e742db8627ba5d7e0f076114e90c4fea4407cedd3599355e4c00828543`  
		Last Modified: Tue, 09 Jun 2020 02:32:03 GMT  
		Size: 8.0 MB (7981054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ba43d083b56bb094a5bac45d723e9bec0fe65d033950b3c4dc392e890c7e41`  
		Last Modified: Tue, 09 Jun 2020 02:32:03 GMT  
		Size: 10.3 MB (10338453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2391b0310a0be022e7ac6e202273ea7cc0ac5f16e862e5cb19c43c5db30b5b`  
		Last Modified: Tue, 09 Jun 2020 02:32:24 GMT  
		Size: 53.4 MB (53429728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:102fd83583ef2a480f1a44da5e486cbd6b9f7e4f11e343f0aa709bbad673f4af
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.1 MB (117105917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7940f3b16f0ec25a65f7764c65f1219b6fcfdc0025782644655c02ab3902221`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:09:44 GMT
ADD file:b51eae556569a7654c89a15b745fafdb0477ed08e8a06f7fcd6363145123d67f in / 
# Tue, 09 Jun 2020 01:09:45 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:51:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:51:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:52:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8084fc3b4d2453eb8005c0b33e3c542e3615868e22652e74e19fec36df3c488e`  
		Last Modified: Tue, 09 Jun 2020 01:17:30 GMT  
		Size: 49.0 MB (49019818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df088964944d43608e89126d7ae55a47489499bad77148bac16c1593e8ff69a`  
		Last Modified: Tue, 09 Jun 2020 02:10:24 GMT  
		Size: 7.2 MB (7231469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a34d1c06dc4557c94a0e8dc1d4f49ee8f512c443dea9748d2bb00fc4e1f6502`  
		Last Modified: Tue, 09 Jun 2020 02:10:24 GMT  
		Size: 10.0 MB (10015784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaedff7ebdd283f729f3eb0635079193636dc776885aa0339370ed36edfbc2f`  
		Last Modified: Tue, 09 Jun 2020 02:11:18 GMT  
		Size: 50.8 MB (50838846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:84895d57d7f38156db0636d4e5d189e61878ae5d5e9ecf94e09f4a0b1677d86e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130582816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fba7835f4d49633e0b09854a0720bd0d5cd8f97adc336d32abfce96e4ce26fa7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:20:32 GMT
ADD file:ed5dc7bd2c0c0dafef9ca4829cd89719c538cd23991fb941589e7fd3bf96b407 in / 
# Wed, 13 May 2020 22:20:38 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:43:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:44:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:45:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:19aca0f2a5b89bbc37caa77bbd1612566fadbbce5c3381246fe356d7e5d14774`  
		Last Modified: Wed, 13 May 2020 22:57:18 GMT  
		Size: 54.1 MB (54142914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556cd6fadc0f341d090a18ecfc4b6aedccd3d99f6eb6a336e3bee33f096c095f`  
		Last Modified: Thu, 14 May 2020 00:28:57 GMT  
		Size: 8.3 MB (8252823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633177125031b056c9e79b442829845cc6886ad14d5de3cc2459317eaa054d94`  
		Last Modified: Thu, 14 May 2020 00:28:59 GMT  
		Size: 10.7 MB (10727164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e762e21652d78f0bcf2f8011e2751e5d6be323a639e89c083f93a086fe1b6005`  
		Last Modified: Thu, 14 May 2020 00:30:19 GMT  
		Size: 57.5 MB (57459915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7458281d34a89854f9edc7ab8d5c06def106eff532ccf989913b50d3a3415a87
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117599751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a00d6adfabaa891485b6fc5cb7332bd413faa61a52f2071c855a01738eecdec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:21 GMT
ADD file:525b5566f1fb9dfef74a4f49170a50bba0f0ed22a8bd627a8f802803236f1db8 in / 
# Tue, 09 Jun 2020 01:42:23 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:09:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:09:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76dae9e9a8f2b69403c29a068363410a0b491d889452a410e1a846db24918418`  
		Last Modified: Tue, 09 Jun 2020 01:46:14 GMT  
		Size: 49.0 MB (48965925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea4ddfd9cac861440dd774171c0df5d003bcf031cc856603f0dcc1a569a7614`  
		Last Modified: Tue, 09 Jun 2020 02:18:01 GMT  
		Size: 7.4 MB (7385198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4340e9fce6caba0ffebdee007c25f4ed849de61e56dcee1ed7e081edbcf1e5`  
		Last Modified: Tue, 09 Jun 2020 02:18:06 GMT  
		Size: 9.9 MB (9882055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89446217dee5ed85681993c919acbdf28494151380677fdefa88b6b5e481573c`  
		Last Modified: Tue, 09 Jun 2020 02:18:19 GMT  
		Size: 51.4 MB (51366573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
