<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20211223.0`](#amazonlinux20202112230)
-	[`amazonlinux:2.0.20211223.0-with-sources`](#amazonlinux20202112230-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20211201.0`](#amazonlinux2018030202112010)
-	[`amazonlinux:2018.03.0.20211201.0-with-sources`](#amazonlinux2018030202112010-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:07602b51b89bd986c01777ebf06af227541337c0483395cc550e14c1cb0204ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9739ed1453449dac5824684cb1189478978dece8ac856560f96c55101a57710a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62408287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7cbfc406b7ed062fb9c08cfcad0a8dc85028c1420e7a3bf65c9bd0f083f796`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 23:20:40 GMT
ADD file:b40f5b5df3c73d89ec477953753f29f16b9ebd38006d73c41b1468302e274d6f in / 
# Thu, 02 Dec 2021 23:20:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6ce5a5560ab28234e783487f84e4b59ecf9cdd051947c044d6b557746ded7630`  
		Last Modified: Thu, 02 Dec 2021 23:22:29 GMT  
		Size: 62.4 MB (62408287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:d4d921a4a191944d7e028f22efa418f978ae39d9b6d451b6d19f8fc1cdbaeab3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:da16df68ae7f6ce6fad4123e255ba51d0917030f796e1ef4086a3deaf51e8101
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515029612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa111552ce92b077f0e226fd14d250252ec4643eead06a1010743c65016ee472`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 23:20:40 GMT
ADD file:b40f5b5df3c73d89ec477953753f29f16b9ebd38006d73c41b1468302e274d6f in / 
# Thu, 02 Dec 2021 23:20:40 GMT
CMD ["/bin/bash"]
# Thu, 02 Dec 2021 23:21:04 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-d9420f93e86b4ae7e03c24f0e4f98c3c9ea9a63b39646e47c86b1dbadc8bdec5.tar.gz"  && echo "c30aa8fe6299b9787f1287c9b7508bad1f31a056d26cf106d87670b6fe99c16f  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:6ce5a5560ab28234e783487f84e4b59ecf9cdd051947c044d6b557746ded7630`  
		Last Modified: Thu, 02 Dec 2021 23:22:29 GMT  
		Size: 62.4 MB (62408287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309de403a6353bf47267c55cbbfd3ce20772653b054e31dd83b30bc40380451e`  
		Last Modified: Thu, 02 Dec 2021 23:22:59 GMT  
		Size: 452.6 MB (452621325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:2654d8123f179de5ce136e12a1ab66ef1348698d9d2be60bd24710df6e62262b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:dbd5d14eed18549d53d4f4b214514917b816d14b573361683d18a43e049139bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62090346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d4a99f25425e3061b16f0b23f643aaa99df7d92d074ea937a4535de151a720`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 23:20:03 GMT
ADD file:4eca58da351122eac20ffd87e3af2c0313089cb81650bdd4c2ef95a556fb842a in / 
# Thu, 02 Dec 2021 23:20:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8b8a142162d22658bdf0283afcd00a9dd216c6637943ffe5f2ba53c4e3da0bd9`  
		Last Modified: Thu, 02 Dec 2021 06:01:08 GMT  
		Size: 62.1 MB (62090346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:7e9896533f552171f29da8eb550aa2ee4f430e7b9d4ec99206ab10aa0fa53804
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63692547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fbac2e4cd8c610c103ed56f38ab52b37cda9101552f73e0fe69809ce710c7ec`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 21:25:17 GMT
ADD file:1f2ecfca149ab81a0527241077c1b366afd95b6b7a1dd91bddfd6c40988ba994 in / 
# Thu, 02 Dec 2021 21:25:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:74f9a6be36f3bc3bf6041c40376d548e3a8b720a0455674b19e9174a9e567078`  
		Last Modified: Thu, 02 Dec 2021 21:26:12 GMT  
		Size: 63.7 MB (63692547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:d405a6c5b9846c3ed5ed8d7f44b6d77dc3fcd43f7e2bba68a4dbb6741b39659f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:75d8cb5c1b54c6d52291947cd5af3ee93a9dc460a1710d2e26882f1c2c27031d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **483.9 MB (483904679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0488a7690d0bcb379eea149c4b2e2e3e2595fd681b8b451f1670fe143c1f049c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 23:20:03 GMT
ADD file:4eca58da351122eac20ffd87e3af2c0313089cb81650bdd4c2ef95a556fb842a in / 
# Thu, 02 Dec 2021 23:20:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Dec 2021 23:20:26 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-faddacaa94ce45cab3ebd75298e985ccc4100e074eae55e6692f4139b7719f13.tar.gz"  && echo "821fcdbe479764a7bf796e4f23a04df2ad960dc88f93f9dfb4492deb77ec6522  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8b8a142162d22658bdf0283afcd00a9dd216c6637943ffe5f2ba53c4e3da0bd9`  
		Last Modified: Thu, 02 Dec 2021 06:01:08 GMT  
		Size: 62.1 MB (62090346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91651260faf90717a94bbd9d94719ad7b8c7a8019e1d6678c1913528d70f780c`  
		Last Modified: Thu, 02 Dec 2021 23:22:07 GMT  
		Size: 421.8 MB (421814333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f430c04ebeb56b96104035a268952662f973de96c4643d53f5ffc56fb8e1e4fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.5 MB (485506862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0843a85e5d33304d882cf4a230dcc700a1e35540601466316552791924470a7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 21:25:17 GMT
ADD file:1f2ecfca149ab81a0527241077c1b366afd95b6b7a1dd91bddfd6c40988ba994 in / 
# Thu, 02 Dec 2021 21:25:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Dec 2021 21:25:41 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-faddacaa94ce45cab3ebd75298e985ccc4100e074eae55e6692f4139b7719f13.tar.gz"  && echo "821fcdbe479764a7bf796e4f23a04df2ad960dc88f93f9dfb4492deb77ec6522  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:74f9a6be36f3bc3bf6041c40376d548e3a8b720a0455674b19e9174a9e567078`  
		Last Modified: Thu, 02 Dec 2021 21:26:12 GMT  
		Size: 63.7 MB (63692547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d2f71867fbb5d9040a4eeaff7f0e49f8cbb45e0b4a563c6f2a7d151c4cd47c`  
		Last Modified: Thu, 02 Dec 2021 21:26:51 GMT  
		Size: 421.8 MB (421814315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20211223.0`

**does not exist** (yet?)

## `amazonlinux:2.0.20211223.0-with-sources`

**does not exist** (yet?)

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:07602b51b89bd986c01777ebf06af227541337c0483395cc550e14c1cb0204ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9739ed1453449dac5824684cb1189478978dece8ac856560f96c55101a57710a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62408287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7cbfc406b7ed062fb9c08cfcad0a8dc85028c1420e7a3bf65c9bd0f083f796`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 23:20:40 GMT
ADD file:b40f5b5df3c73d89ec477953753f29f16b9ebd38006d73c41b1468302e274d6f in / 
# Thu, 02 Dec 2021 23:20:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6ce5a5560ab28234e783487f84e4b59ecf9cdd051947c044d6b557746ded7630`  
		Last Modified: Thu, 02 Dec 2021 23:22:29 GMT  
		Size: 62.4 MB (62408287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:d4d921a4a191944d7e028f22efa418f978ae39d9b6d451b6d19f8fc1cdbaeab3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:da16df68ae7f6ce6fad4123e255ba51d0917030f796e1ef4086a3deaf51e8101
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515029612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa111552ce92b077f0e226fd14d250252ec4643eead06a1010743c65016ee472`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 23:20:40 GMT
ADD file:b40f5b5df3c73d89ec477953753f29f16b9ebd38006d73c41b1468302e274d6f in / 
# Thu, 02 Dec 2021 23:20:40 GMT
CMD ["/bin/bash"]
# Thu, 02 Dec 2021 23:21:04 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-d9420f93e86b4ae7e03c24f0e4f98c3c9ea9a63b39646e47c86b1dbadc8bdec5.tar.gz"  && echo "c30aa8fe6299b9787f1287c9b7508bad1f31a056d26cf106d87670b6fe99c16f  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:6ce5a5560ab28234e783487f84e4b59ecf9cdd051947c044d6b557746ded7630`  
		Last Modified: Thu, 02 Dec 2021 23:22:29 GMT  
		Size: 62.4 MB (62408287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309de403a6353bf47267c55cbbfd3ce20772653b054e31dd83b30bc40380451e`  
		Last Modified: Thu, 02 Dec 2021 23:22:59 GMT  
		Size: 452.6 MB (452621325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20211201.0`

```console
$ docker pull amazonlinux@sha256:07602b51b89bd986c01777ebf06af227541337c0483395cc550e14c1cb0204ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20211201.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9739ed1453449dac5824684cb1189478978dece8ac856560f96c55101a57710a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62408287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7cbfc406b7ed062fb9c08cfcad0a8dc85028c1420e7a3bf65c9bd0f083f796`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 23:20:40 GMT
ADD file:b40f5b5df3c73d89ec477953753f29f16b9ebd38006d73c41b1468302e274d6f in / 
# Thu, 02 Dec 2021 23:20:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6ce5a5560ab28234e783487f84e4b59ecf9cdd051947c044d6b557746ded7630`  
		Last Modified: Thu, 02 Dec 2021 23:22:29 GMT  
		Size: 62.4 MB (62408287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20211201.0-with-sources`

```console
$ docker pull amazonlinux@sha256:d4d921a4a191944d7e028f22efa418f978ae39d9b6d451b6d19f8fc1cdbaeab3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20211201.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:da16df68ae7f6ce6fad4123e255ba51d0917030f796e1ef4086a3deaf51e8101
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515029612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa111552ce92b077f0e226fd14d250252ec4643eead06a1010743c65016ee472`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 23:20:40 GMT
ADD file:b40f5b5df3c73d89ec477953753f29f16b9ebd38006d73c41b1468302e274d6f in / 
# Thu, 02 Dec 2021 23:20:40 GMT
CMD ["/bin/bash"]
# Thu, 02 Dec 2021 23:21:04 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-d9420f93e86b4ae7e03c24f0e4f98c3c9ea9a63b39646e47c86b1dbadc8bdec5.tar.gz"  && echo "c30aa8fe6299b9787f1287c9b7508bad1f31a056d26cf106d87670b6fe99c16f  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:6ce5a5560ab28234e783487f84e4b59ecf9cdd051947c044d6b557746ded7630`  
		Last Modified: Thu, 02 Dec 2021 23:22:29 GMT  
		Size: 62.4 MB (62408287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309de403a6353bf47267c55cbbfd3ce20772653b054e31dd83b30bc40380451e`  
		Last Modified: Thu, 02 Dec 2021 23:22:59 GMT  
		Size: 452.6 MB (452621325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:2654d8123f179de5ce136e12a1ab66ef1348698d9d2be60bd24710df6e62262b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:dbd5d14eed18549d53d4f4b214514917b816d14b573361683d18a43e049139bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62090346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d4a99f25425e3061b16f0b23f643aaa99df7d92d074ea937a4535de151a720`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 23:20:03 GMT
ADD file:4eca58da351122eac20ffd87e3af2c0313089cb81650bdd4c2ef95a556fb842a in / 
# Thu, 02 Dec 2021 23:20:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8b8a142162d22658bdf0283afcd00a9dd216c6637943ffe5f2ba53c4e3da0bd9`  
		Last Modified: Thu, 02 Dec 2021 06:01:08 GMT  
		Size: 62.1 MB (62090346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:7e9896533f552171f29da8eb550aa2ee4f430e7b9d4ec99206ab10aa0fa53804
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63692547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fbac2e4cd8c610c103ed56f38ab52b37cda9101552f73e0fe69809ce710c7ec`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 21:25:17 GMT
ADD file:1f2ecfca149ab81a0527241077c1b366afd95b6b7a1dd91bddfd6c40988ba994 in / 
# Thu, 02 Dec 2021 21:25:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:74f9a6be36f3bc3bf6041c40376d548e3a8b720a0455674b19e9174a9e567078`  
		Last Modified: Thu, 02 Dec 2021 21:26:12 GMT  
		Size: 63.7 MB (63692547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:d405a6c5b9846c3ed5ed8d7f44b6d77dc3fcd43f7e2bba68a4dbb6741b39659f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:75d8cb5c1b54c6d52291947cd5af3ee93a9dc460a1710d2e26882f1c2c27031d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **483.9 MB (483904679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0488a7690d0bcb379eea149c4b2e2e3e2595fd681b8b451f1670fe143c1f049c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 23:20:03 GMT
ADD file:4eca58da351122eac20ffd87e3af2c0313089cb81650bdd4c2ef95a556fb842a in / 
# Thu, 02 Dec 2021 23:20:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Dec 2021 23:20:26 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-faddacaa94ce45cab3ebd75298e985ccc4100e074eae55e6692f4139b7719f13.tar.gz"  && echo "821fcdbe479764a7bf796e4f23a04df2ad960dc88f93f9dfb4492deb77ec6522  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8b8a142162d22658bdf0283afcd00a9dd216c6637943ffe5f2ba53c4e3da0bd9`  
		Last Modified: Thu, 02 Dec 2021 06:01:08 GMT  
		Size: 62.1 MB (62090346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91651260faf90717a94bbd9d94719ad7b8c7a8019e1d6678c1913528d70f780c`  
		Last Modified: Thu, 02 Dec 2021 23:22:07 GMT  
		Size: 421.8 MB (421814333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f430c04ebeb56b96104035a268952662f973de96c4643d53f5ffc56fb8e1e4fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.5 MB (485506862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0843a85e5d33304d882cf4a230dcc700a1e35540601466316552791924470a7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 21:25:17 GMT
ADD file:1f2ecfca149ab81a0527241077c1b366afd95b6b7a1dd91bddfd6c40988ba994 in / 
# Thu, 02 Dec 2021 21:25:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Dec 2021 21:25:41 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-faddacaa94ce45cab3ebd75298e985ccc4100e074eae55e6692f4139b7719f13.tar.gz"  && echo "821fcdbe479764a7bf796e4f23a04df2ad960dc88f93f9dfb4492deb77ec6522  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:74f9a6be36f3bc3bf6041c40376d548e3a8b720a0455674b19e9174a9e567078`  
		Last Modified: Thu, 02 Dec 2021 21:26:12 GMT  
		Size: 63.7 MB (63692547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d2f71867fbb5d9040a4eeaff7f0e49f8cbb45e0b4a563c6f2a7d151c4cd47c`  
		Last Modified: Thu, 02 Dec 2021 21:26:51 GMT  
		Size: 421.8 MB (421814315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
