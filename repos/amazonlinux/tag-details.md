<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20210617.0`](#amazonlinux20202106170)
-	[`amazonlinux:2.0.20210617.0-with-sources`](#amazonlinux20202106170-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20210521.1`](#amazonlinux2018030202105211)
-	[`amazonlinux:2018.03.0.20210521.1-with-sources`](#amazonlinux2018030202105211-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:d8db8960d84895fb10e491080d4069ac542aa06205a9ccf3af202a927d561bab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7326b7afba891588bce0cb6a6244f9bb205bbbb7ad7b6a719e356ad8e878102b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62233767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07431b5cc2148664c7fd5c2f4e6c47bc7386eca1abd67ccc506240521e2a6dc4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Jun 2021 23:47:34 GMT
ADD file:d54600120dd0df387f02c9986b95553c7be4690d3226e5693a0621e1bbba9c79 in / 
# Thu, 03 Jun 2021 23:47:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8aa1c9f768e700368fba92ab67c462b5757d5e5d801b2309ce0ac018cc7a13e9`  
		Last Modified: Thu, 03 Jun 2021 23:48:24 GMT  
		Size: 62.2 MB (62233767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:bd7aca583738a44ccabf6582caa32ea1b3dbd5ffff26e0606c0f1a6a0515d8d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:80878ae39f9fe1a9a950ff72ea175f41144032442c3e84f3635a135f7de32f57
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449096717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce78d0c69b908a315c3a8930d9e6bccef3317b485528e31c72acff0cb546755a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Jun 2021 23:47:34 GMT
ADD file:d54600120dd0df387f02c9986b95553c7be4690d3226e5693a0621e1bbba9c79 in / 
# Thu, 03 Jun 2021 23:47:35 GMT
CMD ["/bin/bash"]
# Thu, 03 Jun 2021 23:47:54 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-dc5d92c927a9f79aab7658e5c05df877dd40282d7bf9b4b11a5eb11b225cb7ad.tar.gz"  && echo "03509f1ca8f0593cf761a9fda3dc71baf0f45752a0d8908a04ccd9937bd1ddfc  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8aa1c9f768e700368fba92ab67c462b5757d5e5d801b2309ce0ac018cc7a13e9`  
		Last Modified: Thu, 03 Jun 2021 23:48:24 GMT  
		Size: 62.2 MB (62233767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732b4f3ad9bb7c123e4d3b3582e82bff05e5f83438191ad98a2d271e235ff1c2`  
		Last Modified: Thu, 03 Jun 2021 23:48:58 GMT  
		Size: 386.9 MB (386862950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:2e42b5d170dbb6d54d35b3b64627480de9687b52cfbab2086267a0fd2acd7bef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:aac2387683b83dfcd94ee4bf6ddd3523158c144f90dcf04b572494e9a6d20f9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61940054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7443854fbdb0d9c0c252f05d84f628851dc716a3e2c935dd877282489928fe59`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Jun 2021 17:19:49 GMT
ADD file:dc851f79dbfc66e08196951041e8c856c41a3cc24b8bc27e66722210d51e87cf in / 
# Fri, 25 Jun 2021 17:19:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:85ee02fe1a09b50ffaacc1e7482fdbb3e80c577256420503196fc549b9e4ef29`  
		Last Modified: Fri, 25 Jun 2021 00:50:03 GMT  
		Size: 61.9 MB (61940054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f296106273fa7073dfedea9fc7ec545d7faddfedbceb9155f101eef220209c15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63564395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8e1c3f1064f998721e227db671b9c7e7aaf1c0447ed01aa8738b99826f0c540`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Jun 2021 17:39:34 GMT
ADD file:d4d6f883cd1ba97522a617c6f7b0125b0a82e12101c702ca57ac48063f0e3707 in / 
# Fri, 25 Jun 2021 17:39:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b19e557e673ca4274c5ee576b0d897c535e4329a596ac20b3ff70225b734a125`  
		Last Modified: Fri, 25 Jun 2021 00:50:31 GMT  
		Size: 63.6 MB (63564395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:6492874e3eb5c5f17a672f13302e4750829dd47a769c724b6cf18d7384351851
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:11756a8e8e058aad96da6e33f405e4da59d3314030708c217a5ebec61d345eac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.9 MB (542892752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0633f60cd20857b93c8fb3306b608c8db61833ecc053df7c28c6c4bcc0a5cad4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Jun 2021 17:19:49 GMT
ADD file:dc851f79dbfc66e08196951041e8c856c41a3cc24b8bc27e66722210d51e87cf in / 
# Fri, 25 Jun 2021 17:19:50 GMT
CMD ["/bin/bash"]
# Fri, 25 Jun 2021 17:20:17 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-802f7b2589030657b0b80f3e6055fdd0a78fb8c62cd9535d8ffe15cb8b199160.tar.gz"  && echo "397633fadc78e78bba3fce8c756b34cbc069ff0547c587f8084d562df42492ea  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:85ee02fe1a09b50ffaacc1e7482fdbb3e80c577256420503196fc549b9e4ef29`  
		Last Modified: Fri, 25 Jun 2021 00:50:03 GMT  
		Size: 61.9 MB (61940054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36147721d5864a12cbe2bd4c4a6364fb01f85bc3ce9b78b0155cc8b85eeac3f`  
		Last Modified: Fri, 25 Jun 2021 17:21:20 GMT  
		Size: 481.0 MB (480952698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:42475fd6ee0c35275f2d8bdef3ddb1db45966e020195ff192961282734c341e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544517089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:474b6b6ee3943a9adb6fbc53219ab0a45a7569d6b15a7108a8e0b51bc355a424`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Jun 2021 17:39:34 GMT
ADD file:d4d6f883cd1ba97522a617c6f7b0125b0a82e12101c702ca57ac48063f0e3707 in / 
# Fri, 25 Jun 2021 17:39:35 GMT
CMD ["/bin/bash"]
# Fri, 25 Jun 2021 17:39:57 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-802f7b2589030657b0b80f3e6055fdd0a78fb8c62cd9535d8ffe15cb8b199160.tar.gz"  && echo "397633fadc78e78bba3fce8c756b34cbc069ff0547c587f8084d562df42492ea  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:b19e557e673ca4274c5ee576b0d897c535e4329a596ac20b3ff70225b734a125`  
		Last Modified: Fri, 25 Jun 2021 00:50:31 GMT  
		Size: 63.6 MB (63564395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1214f708d37e96eba6f344682eb9f0bb8d4ed7ad7e03b4062c8db057ff3443`  
		Last Modified: Fri, 25 Jun 2021 17:41:18 GMT  
		Size: 481.0 MB (480952694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20210617.0`

```console
$ docker pull amazonlinux@sha256:2e42b5d170dbb6d54d35b3b64627480de9687b52cfbab2086267a0fd2acd7bef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20210617.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:aac2387683b83dfcd94ee4bf6ddd3523158c144f90dcf04b572494e9a6d20f9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61940054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7443854fbdb0d9c0c252f05d84f628851dc716a3e2c935dd877282489928fe59`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Jun 2021 17:19:49 GMT
ADD file:dc851f79dbfc66e08196951041e8c856c41a3cc24b8bc27e66722210d51e87cf in / 
# Fri, 25 Jun 2021 17:19:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:85ee02fe1a09b50ffaacc1e7482fdbb3e80c577256420503196fc549b9e4ef29`  
		Last Modified: Fri, 25 Jun 2021 00:50:03 GMT  
		Size: 61.9 MB (61940054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20210617.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f296106273fa7073dfedea9fc7ec545d7faddfedbceb9155f101eef220209c15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63564395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8e1c3f1064f998721e227db671b9c7e7aaf1c0447ed01aa8738b99826f0c540`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Jun 2021 17:39:34 GMT
ADD file:d4d6f883cd1ba97522a617c6f7b0125b0a82e12101c702ca57ac48063f0e3707 in / 
# Fri, 25 Jun 2021 17:39:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b19e557e673ca4274c5ee576b0d897c535e4329a596ac20b3ff70225b734a125`  
		Last Modified: Fri, 25 Jun 2021 00:50:31 GMT  
		Size: 63.6 MB (63564395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20210617.0-with-sources`

```console
$ docker pull amazonlinux@sha256:6492874e3eb5c5f17a672f13302e4750829dd47a769c724b6cf18d7384351851
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20210617.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:11756a8e8e058aad96da6e33f405e4da59d3314030708c217a5ebec61d345eac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.9 MB (542892752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0633f60cd20857b93c8fb3306b608c8db61833ecc053df7c28c6c4bcc0a5cad4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Jun 2021 17:19:49 GMT
ADD file:dc851f79dbfc66e08196951041e8c856c41a3cc24b8bc27e66722210d51e87cf in / 
# Fri, 25 Jun 2021 17:19:50 GMT
CMD ["/bin/bash"]
# Fri, 25 Jun 2021 17:20:17 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-802f7b2589030657b0b80f3e6055fdd0a78fb8c62cd9535d8ffe15cb8b199160.tar.gz"  && echo "397633fadc78e78bba3fce8c756b34cbc069ff0547c587f8084d562df42492ea  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:85ee02fe1a09b50ffaacc1e7482fdbb3e80c577256420503196fc549b9e4ef29`  
		Last Modified: Fri, 25 Jun 2021 00:50:03 GMT  
		Size: 61.9 MB (61940054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36147721d5864a12cbe2bd4c4a6364fb01f85bc3ce9b78b0155cc8b85eeac3f`  
		Last Modified: Fri, 25 Jun 2021 17:21:20 GMT  
		Size: 481.0 MB (480952698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20210617.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:42475fd6ee0c35275f2d8bdef3ddb1db45966e020195ff192961282734c341e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544517089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:474b6b6ee3943a9adb6fbc53219ab0a45a7569d6b15a7108a8e0b51bc355a424`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Jun 2021 17:39:34 GMT
ADD file:d4d6f883cd1ba97522a617c6f7b0125b0a82e12101c702ca57ac48063f0e3707 in / 
# Fri, 25 Jun 2021 17:39:35 GMT
CMD ["/bin/bash"]
# Fri, 25 Jun 2021 17:39:57 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-802f7b2589030657b0b80f3e6055fdd0a78fb8c62cd9535d8ffe15cb8b199160.tar.gz"  && echo "397633fadc78e78bba3fce8c756b34cbc069ff0547c587f8084d562df42492ea  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:b19e557e673ca4274c5ee576b0d897c535e4329a596ac20b3ff70225b734a125`  
		Last Modified: Fri, 25 Jun 2021 00:50:31 GMT  
		Size: 63.6 MB (63564395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1214f708d37e96eba6f344682eb9f0bb8d4ed7ad7e03b4062c8db057ff3443`  
		Last Modified: Fri, 25 Jun 2021 17:41:18 GMT  
		Size: 481.0 MB (480952694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:d8db8960d84895fb10e491080d4069ac542aa06205a9ccf3af202a927d561bab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7326b7afba891588bce0cb6a6244f9bb205bbbb7ad7b6a719e356ad8e878102b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62233767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07431b5cc2148664c7fd5c2f4e6c47bc7386eca1abd67ccc506240521e2a6dc4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Jun 2021 23:47:34 GMT
ADD file:d54600120dd0df387f02c9986b95553c7be4690d3226e5693a0621e1bbba9c79 in / 
# Thu, 03 Jun 2021 23:47:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8aa1c9f768e700368fba92ab67c462b5757d5e5d801b2309ce0ac018cc7a13e9`  
		Last Modified: Thu, 03 Jun 2021 23:48:24 GMT  
		Size: 62.2 MB (62233767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:bd7aca583738a44ccabf6582caa32ea1b3dbd5ffff26e0606c0f1a6a0515d8d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:80878ae39f9fe1a9a950ff72ea175f41144032442c3e84f3635a135f7de32f57
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449096717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce78d0c69b908a315c3a8930d9e6bccef3317b485528e31c72acff0cb546755a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Jun 2021 23:47:34 GMT
ADD file:d54600120dd0df387f02c9986b95553c7be4690d3226e5693a0621e1bbba9c79 in / 
# Thu, 03 Jun 2021 23:47:35 GMT
CMD ["/bin/bash"]
# Thu, 03 Jun 2021 23:47:54 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-dc5d92c927a9f79aab7658e5c05df877dd40282d7bf9b4b11a5eb11b225cb7ad.tar.gz"  && echo "03509f1ca8f0593cf761a9fda3dc71baf0f45752a0d8908a04ccd9937bd1ddfc  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8aa1c9f768e700368fba92ab67c462b5757d5e5d801b2309ce0ac018cc7a13e9`  
		Last Modified: Thu, 03 Jun 2021 23:48:24 GMT  
		Size: 62.2 MB (62233767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732b4f3ad9bb7c123e4d3b3582e82bff05e5f83438191ad98a2d271e235ff1c2`  
		Last Modified: Thu, 03 Jun 2021 23:48:58 GMT  
		Size: 386.9 MB (386862950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20210521.1`

```console
$ docker pull amazonlinux@sha256:d8db8960d84895fb10e491080d4069ac542aa06205a9ccf3af202a927d561bab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20210521.1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7326b7afba891588bce0cb6a6244f9bb205bbbb7ad7b6a719e356ad8e878102b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62233767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07431b5cc2148664c7fd5c2f4e6c47bc7386eca1abd67ccc506240521e2a6dc4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Jun 2021 23:47:34 GMT
ADD file:d54600120dd0df387f02c9986b95553c7be4690d3226e5693a0621e1bbba9c79 in / 
# Thu, 03 Jun 2021 23:47:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8aa1c9f768e700368fba92ab67c462b5757d5e5d801b2309ce0ac018cc7a13e9`  
		Last Modified: Thu, 03 Jun 2021 23:48:24 GMT  
		Size: 62.2 MB (62233767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20210521.1-with-sources`

```console
$ docker pull amazonlinux@sha256:bd7aca583738a44ccabf6582caa32ea1b3dbd5ffff26e0606c0f1a6a0515d8d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20210521.1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:80878ae39f9fe1a9a950ff72ea175f41144032442c3e84f3635a135f7de32f57
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449096717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce78d0c69b908a315c3a8930d9e6bccef3317b485528e31c72acff0cb546755a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Jun 2021 23:47:34 GMT
ADD file:d54600120dd0df387f02c9986b95553c7be4690d3226e5693a0621e1bbba9c79 in / 
# Thu, 03 Jun 2021 23:47:35 GMT
CMD ["/bin/bash"]
# Thu, 03 Jun 2021 23:47:54 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-dc5d92c927a9f79aab7658e5c05df877dd40282d7bf9b4b11a5eb11b225cb7ad.tar.gz"  && echo "03509f1ca8f0593cf761a9fda3dc71baf0f45752a0d8908a04ccd9937bd1ddfc  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8aa1c9f768e700368fba92ab67c462b5757d5e5d801b2309ce0ac018cc7a13e9`  
		Last Modified: Thu, 03 Jun 2021 23:48:24 GMT  
		Size: 62.2 MB (62233767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732b4f3ad9bb7c123e4d3b3582e82bff05e5f83438191ad98a2d271e235ff1c2`  
		Last Modified: Thu, 03 Jun 2021 23:48:58 GMT  
		Size: 386.9 MB (386862950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:2e42b5d170dbb6d54d35b3b64627480de9687b52cfbab2086267a0fd2acd7bef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:aac2387683b83dfcd94ee4bf6ddd3523158c144f90dcf04b572494e9a6d20f9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61940054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7443854fbdb0d9c0c252f05d84f628851dc716a3e2c935dd877282489928fe59`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Jun 2021 17:19:49 GMT
ADD file:dc851f79dbfc66e08196951041e8c856c41a3cc24b8bc27e66722210d51e87cf in / 
# Fri, 25 Jun 2021 17:19:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:85ee02fe1a09b50ffaacc1e7482fdbb3e80c577256420503196fc549b9e4ef29`  
		Last Modified: Fri, 25 Jun 2021 00:50:03 GMT  
		Size: 61.9 MB (61940054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f296106273fa7073dfedea9fc7ec545d7faddfedbceb9155f101eef220209c15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63564395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8e1c3f1064f998721e227db671b9c7e7aaf1c0447ed01aa8738b99826f0c540`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Jun 2021 17:39:34 GMT
ADD file:d4d6f883cd1ba97522a617c6f7b0125b0a82e12101c702ca57ac48063f0e3707 in / 
# Fri, 25 Jun 2021 17:39:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b19e557e673ca4274c5ee576b0d897c535e4329a596ac20b3ff70225b734a125`  
		Last Modified: Fri, 25 Jun 2021 00:50:31 GMT  
		Size: 63.6 MB (63564395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:6492874e3eb5c5f17a672f13302e4750829dd47a769c724b6cf18d7384351851
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:11756a8e8e058aad96da6e33f405e4da59d3314030708c217a5ebec61d345eac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.9 MB (542892752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0633f60cd20857b93c8fb3306b608c8db61833ecc053df7c28c6c4bcc0a5cad4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Jun 2021 17:19:49 GMT
ADD file:dc851f79dbfc66e08196951041e8c856c41a3cc24b8bc27e66722210d51e87cf in / 
# Fri, 25 Jun 2021 17:19:50 GMT
CMD ["/bin/bash"]
# Fri, 25 Jun 2021 17:20:17 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-802f7b2589030657b0b80f3e6055fdd0a78fb8c62cd9535d8ffe15cb8b199160.tar.gz"  && echo "397633fadc78e78bba3fce8c756b34cbc069ff0547c587f8084d562df42492ea  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:85ee02fe1a09b50ffaacc1e7482fdbb3e80c577256420503196fc549b9e4ef29`  
		Last Modified: Fri, 25 Jun 2021 00:50:03 GMT  
		Size: 61.9 MB (61940054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36147721d5864a12cbe2bd4c4a6364fb01f85bc3ce9b78b0155cc8b85eeac3f`  
		Last Modified: Fri, 25 Jun 2021 17:21:20 GMT  
		Size: 481.0 MB (480952698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:42475fd6ee0c35275f2d8bdef3ddb1db45966e020195ff192961282734c341e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544517089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:474b6b6ee3943a9adb6fbc53219ab0a45a7569d6b15a7108a8e0b51bc355a424`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Jun 2021 17:39:34 GMT
ADD file:d4d6f883cd1ba97522a617c6f7b0125b0a82e12101c702ca57ac48063f0e3707 in / 
# Fri, 25 Jun 2021 17:39:35 GMT
CMD ["/bin/bash"]
# Fri, 25 Jun 2021 17:39:57 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-802f7b2589030657b0b80f3e6055fdd0a78fb8c62cd9535d8ffe15cb8b199160.tar.gz"  && echo "397633fadc78e78bba3fce8c756b34cbc069ff0547c587f8084d562df42492ea  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:b19e557e673ca4274c5ee576b0d897c535e4329a596ac20b3ff70225b734a125`  
		Last Modified: Fri, 25 Jun 2021 00:50:31 GMT  
		Size: 63.6 MB (63564395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1214f708d37e96eba6f344682eb9f0bb8d4ed7ad7e03b4062c8db057ff3443`  
		Last Modified: Fri, 25 Jun 2021 17:41:18 GMT  
		Size: 481.0 MB (480952694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
