## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:3c3743ac33e26851442f987b8795ee50d310292c71de242a1489150af92a93c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ce49a5d54788eb0754c038d3fdc1ed815da00be1df787c03cafea1503766fcc1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **476.8 MB (476804109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71fadd5eaa0b1347722638a6d12ce8057456acecc2e2f414e41c886205250c1f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 22:20:10 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-4a2709d0b184c9b7a5e4b01c08f0a95ddb949a8af3fb12847920b6fc8cad8033.tar.gz"  && echo "d51679d0ed0ab3b0a8eb3c2a40b03e5c5e6d7b11a13fa6f729b2461204dfb1b0  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77428ba98702146aeb373ef1d9192fe64ca55636a3109ee715326ffdb55e5e5`  
		Last Modified: Fri, 31 Jul 2020 22:21:01 GMT  
		Size: 415.1 MB (415087569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:cd692aec3252035c3d14c7386ec5406849408549330e60806bdcd01c1290e59b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.4 MB (478441746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651c803e19552789f769d884bb2769ef41c271610c4088b7884fa4d4df10a9a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 22:43:55 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-4a2709d0b184c9b7a5e4b01c08f0a95ddb949a8af3fb12847920b6fc8cad8033.tar.gz"  && echo "d51679d0ed0ab3b0a8eb3c2a40b03e5c5e6d7b11a13fa6f729b2461204dfb1b0  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d50d139b41b697f140b30c7d2f1dcbd3831e9fba6f5b054207ba00f64fef78`  
		Last Modified: Fri, 31 Jul 2020 22:45:12 GMT  
		Size: 415.1 MB (415087610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
