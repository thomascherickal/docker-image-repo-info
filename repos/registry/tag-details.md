<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `registry`

-	[`registry:2`](#registry2)
-	[`registry:2.7`](#registry27)
-	[`registry:2.7.1`](#registry271)
-	[`registry:latest`](#registrylatest)

## `registry:2`

```console
$ docker pull registry@sha256:169211e20e2f2d5d115674681eb79d21a217b296b43374b8e39f97fcf866b375
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `registry:2` - linux; amd64

```console
$ docker pull registry@sha256:36cb5b157911061fb610d8884dc09e0b0300a767a350563cbfd88b4b85324ce4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9941588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8604a3fe8543c9e6afc29550de05b36cd162a97aa9b2833864ea8a5be11f3e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:17 GMT
ADD file:efe2d94a88cdbbd01c3ef095f0a2473cec9e74804b49cd6fb9b837d362631409 in / 
# Fri, 12 Nov 2021 17:20:17 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:22:49 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Sat, 13 Nov 2021 06:22:50 GMT
COPY file:21256ff7df5369f7ad2e19c6d020a644303aded200bdbec4d46648f38d55df78 in /bin/registry 
# Sat, 13 Nov 2021 06:22:50 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Sat, 13 Nov 2021 06:22:50 GMT
VOLUME [/var/lib/registry]
# Sat, 13 Nov 2021 06:22:51 GMT
EXPOSE 5000
# Sat, 13 Nov 2021 06:22:51 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Sat, 13 Nov 2021 06:22:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:22:51 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:79e9f2f55bf5465a02ee6a6170e66005b20c7aa6b115af6fcd04fad706ea651a`  
		Last Modified: Fri, 12 Nov 2021 17:21:24 GMT  
		Size: 2.8 MB (2817409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d96da54f60b86a4d869d44b44cfca69d71c4776b81d361bc057d6666ec0d878`  
		Last Modified: Sat, 13 Nov 2021 06:23:02 GMT  
		Size: 299.6 KB (299640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b27040df4a23c90c3837d926f633fb327fb3af9ac4fa5d5bc3520ad578acb10`  
		Last Modified: Sat, 13 Nov 2021 06:23:03 GMT  
		Size: 6.8 MB (6823927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ead8259a04d39492c25c9548078200c5ec429f628dcf7b7535137954cc2df0`  
		Last Modified: Sat, 13 Nov 2021 06:23:01 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3790aef225b922bc97aaba099fe762f7b115aec55a0083824b548a6a1e610719`  
		Last Modified: Sat, 13 Nov 2021 06:23:01 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2` - linux; arm variant v6

```console
$ docker pull registry@sha256:eafd2cdf8e847216f62e1acb756f992689f4861baf943610ad4127df3cacee29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9315138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8a56425636efd3a5e4337640baf5cb2264890edab9753f228a1bffe4fe52e2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Fri, 12 Nov 2021 16:50:22 GMT
ADD file:c219ee7662a2b29c4e06be5bf332f2f53b326937277057af61516f5cf5abce1e in / 
# Fri, 12 Nov 2021 16:50:23 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:39:50 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Fri, 12 Nov 2021 18:39:52 GMT
COPY file:29c6c1625420a558a03cc7ed253192f8138cba6212b64e30217fb6488af668e2 in /bin/registry 
# Fri, 12 Nov 2021 18:39:52 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 12 Nov 2021 18:39:53 GMT
VOLUME [/var/lib/registry]
# Fri, 12 Nov 2021 18:39:53 GMT
EXPOSE 5000
# Fri, 12 Nov 2021 18:39:54 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 12 Nov 2021 18:39:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:39:54 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:5cb8b15578b20b3c847454a0e0743b923ddea3e4f22ffa95f6f41b0c551a391e`  
		Last Modified: Fri, 12 Nov 2021 16:52:20 GMT  
		Size: 2.6 MB (2623510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f42adccaa3d4922795f3649d07292e4ce62f4d385383fd4e692f127d1d8d4ac`  
		Last Modified: Fri, 12 Nov 2021 18:40:26 GMT  
		Size: 299.9 KB (299931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33cdd19516437a0bd6d652b69c0243f481402a421101d6f55d015341cc0966d`  
		Last Modified: Fri, 12 Nov 2021 18:40:30 GMT  
		Size: 6.4 MB (6391083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa54e3652a6c452d8957014ed3a2a9be3a879ae1d7f9e9d4b8976527df0b821`  
		Last Modified: Fri, 12 Nov 2021 18:40:26 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef5fbcd41180f8f78fb1db49ef015abb3418b6e5225c4ecf7dd972748a96032`  
		Last Modified: Fri, 12 Nov 2021 18:40:26 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:e9c2d646078211f8353e482caac9d9b12f38b42bc29cb30c453841cf144037b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9269387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bf57bb5c31c49b2fb6d0a86234b5f59a97d559072dc273a1a6ea6789abb720`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:19 GMT
ADD file:bffb4828c6bba0115b766f72c49407938059b204ac9edf130d023af34871d3d0 in / 
# Fri, 12 Nov 2021 16:40:19 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:53:00 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Fri, 12 Nov 2021 18:53:02 GMT
COPY file:51a441e6eceff49ef32609e7070b64e8d5690648e4f915cc825274e6fe37aed2 in /bin/registry 
# Fri, 12 Nov 2021 18:53:03 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 12 Nov 2021 18:53:03 GMT
VOLUME [/var/lib/registry]
# Fri, 12 Nov 2021 18:53:04 GMT
EXPOSE 5000
# Fri, 12 Nov 2021 18:53:06 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 12 Nov 2021 18:53:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:53:07 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:b48a9fe99aba73065302163e59c82a1b0054810c7b9ef85eee6f1b495b162461`  
		Last Modified: Fri, 12 Nov 2021 16:41:35 GMT  
		Size: 2.7 MB (2728748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095878aa44caf2b7927dcf6de1a53e40f016b5ce43b2c885c8e0ecb90fc5f403`  
		Last Modified: Fri, 12 Nov 2021 18:53:25 GMT  
		Size: 299.9 KB (299858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04df0d597e2b057779cd387b32c7d76c5f06254f0c29ea7f3977487fb29a6e2a`  
		Last Modified: Fri, 12 Nov 2021 18:53:26 GMT  
		Size: 6.2 MB (6240198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0594d0cd6d662a93dda81e2bcde210e3279fef169f331f784e66e742c83b2c2`  
		Last Modified: Fri, 12 Nov 2021 18:53:25 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a758d8738abf69bbb372dcfd778368e8c0f74f7cbbf4519eddb0d4a1ef9e81`  
		Last Modified: Fri, 12 Nov 2021 18:53:25 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `registry:2.7`

```console
$ docker pull registry@sha256:169211e20e2f2d5d115674681eb79d21a217b296b43374b8e39f97fcf866b375
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `registry:2.7` - linux; amd64

```console
$ docker pull registry@sha256:36cb5b157911061fb610d8884dc09e0b0300a767a350563cbfd88b4b85324ce4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9941588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8604a3fe8543c9e6afc29550de05b36cd162a97aa9b2833864ea8a5be11f3e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:17 GMT
ADD file:efe2d94a88cdbbd01c3ef095f0a2473cec9e74804b49cd6fb9b837d362631409 in / 
# Fri, 12 Nov 2021 17:20:17 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:22:49 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Sat, 13 Nov 2021 06:22:50 GMT
COPY file:21256ff7df5369f7ad2e19c6d020a644303aded200bdbec4d46648f38d55df78 in /bin/registry 
# Sat, 13 Nov 2021 06:22:50 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Sat, 13 Nov 2021 06:22:50 GMT
VOLUME [/var/lib/registry]
# Sat, 13 Nov 2021 06:22:51 GMT
EXPOSE 5000
# Sat, 13 Nov 2021 06:22:51 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Sat, 13 Nov 2021 06:22:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:22:51 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:79e9f2f55bf5465a02ee6a6170e66005b20c7aa6b115af6fcd04fad706ea651a`  
		Last Modified: Fri, 12 Nov 2021 17:21:24 GMT  
		Size: 2.8 MB (2817409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d96da54f60b86a4d869d44b44cfca69d71c4776b81d361bc057d6666ec0d878`  
		Last Modified: Sat, 13 Nov 2021 06:23:02 GMT  
		Size: 299.6 KB (299640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b27040df4a23c90c3837d926f633fb327fb3af9ac4fa5d5bc3520ad578acb10`  
		Last Modified: Sat, 13 Nov 2021 06:23:03 GMT  
		Size: 6.8 MB (6823927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ead8259a04d39492c25c9548078200c5ec429f628dcf7b7535137954cc2df0`  
		Last Modified: Sat, 13 Nov 2021 06:23:01 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3790aef225b922bc97aaba099fe762f7b115aec55a0083824b548a6a1e610719`  
		Last Modified: Sat, 13 Nov 2021 06:23:01 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.7` - linux; arm variant v6

```console
$ docker pull registry@sha256:eafd2cdf8e847216f62e1acb756f992689f4861baf943610ad4127df3cacee29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9315138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8a56425636efd3a5e4337640baf5cb2264890edab9753f228a1bffe4fe52e2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Fri, 12 Nov 2021 16:50:22 GMT
ADD file:c219ee7662a2b29c4e06be5bf332f2f53b326937277057af61516f5cf5abce1e in / 
# Fri, 12 Nov 2021 16:50:23 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:39:50 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Fri, 12 Nov 2021 18:39:52 GMT
COPY file:29c6c1625420a558a03cc7ed253192f8138cba6212b64e30217fb6488af668e2 in /bin/registry 
# Fri, 12 Nov 2021 18:39:52 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 12 Nov 2021 18:39:53 GMT
VOLUME [/var/lib/registry]
# Fri, 12 Nov 2021 18:39:53 GMT
EXPOSE 5000
# Fri, 12 Nov 2021 18:39:54 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 12 Nov 2021 18:39:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:39:54 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:5cb8b15578b20b3c847454a0e0743b923ddea3e4f22ffa95f6f41b0c551a391e`  
		Last Modified: Fri, 12 Nov 2021 16:52:20 GMT  
		Size: 2.6 MB (2623510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f42adccaa3d4922795f3649d07292e4ce62f4d385383fd4e692f127d1d8d4ac`  
		Last Modified: Fri, 12 Nov 2021 18:40:26 GMT  
		Size: 299.9 KB (299931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33cdd19516437a0bd6d652b69c0243f481402a421101d6f55d015341cc0966d`  
		Last Modified: Fri, 12 Nov 2021 18:40:30 GMT  
		Size: 6.4 MB (6391083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa54e3652a6c452d8957014ed3a2a9be3a879ae1d7f9e9d4b8976527df0b821`  
		Last Modified: Fri, 12 Nov 2021 18:40:26 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef5fbcd41180f8f78fb1db49ef015abb3418b6e5225c4ecf7dd972748a96032`  
		Last Modified: Fri, 12 Nov 2021 18:40:26 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.7` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:e9c2d646078211f8353e482caac9d9b12f38b42bc29cb30c453841cf144037b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9269387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bf57bb5c31c49b2fb6d0a86234b5f59a97d559072dc273a1a6ea6789abb720`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:19 GMT
ADD file:bffb4828c6bba0115b766f72c49407938059b204ac9edf130d023af34871d3d0 in / 
# Fri, 12 Nov 2021 16:40:19 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:53:00 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Fri, 12 Nov 2021 18:53:02 GMT
COPY file:51a441e6eceff49ef32609e7070b64e8d5690648e4f915cc825274e6fe37aed2 in /bin/registry 
# Fri, 12 Nov 2021 18:53:03 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 12 Nov 2021 18:53:03 GMT
VOLUME [/var/lib/registry]
# Fri, 12 Nov 2021 18:53:04 GMT
EXPOSE 5000
# Fri, 12 Nov 2021 18:53:06 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 12 Nov 2021 18:53:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:53:07 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:b48a9fe99aba73065302163e59c82a1b0054810c7b9ef85eee6f1b495b162461`  
		Last Modified: Fri, 12 Nov 2021 16:41:35 GMT  
		Size: 2.7 MB (2728748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095878aa44caf2b7927dcf6de1a53e40f016b5ce43b2c885c8e0ecb90fc5f403`  
		Last Modified: Fri, 12 Nov 2021 18:53:25 GMT  
		Size: 299.9 KB (299858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04df0d597e2b057779cd387b32c7d76c5f06254f0c29ea7f3977487fb29a6e2a`  
		Last Modified: Fri, 12 Nov 2021 18:53:26 GMT  
		Size: 6.2 MB (6240198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0594d0cd6d662a93dda81e2bcde210e3279fef169f331f784e66e742c83b2c2`  
		Last Modified: Fri, 12 Nov 2021 18:53:25 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a758d8738abf69bbb372dcfd778368e8c0f74f7cbbf4519eddb0d4a1ef9e81`  
		Last Modified: Fri, 12 Nov 2021 18:53:25 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `registry:2.7.1`

```console
$ docker pull registry@sha256:169211e20e2f2d5d115674681eb79d21a217b296b43374b8e39f97fcf866b375
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `registry:2.7.1` - linux; amd64

```console
$ docker pull registry@sha256:36cb5b157911061fb610d8884dc09e0b0300a767a350563cbfd88b4b85324ce4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9941588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8604a3fe8543c9e6afc29550de05b36cd162a97aa9b2833864ea8a5be11f3e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:17 GMT
ADD file:efe2d94a88cdbbd01c3ef095f0a2473cec9e74804b49cd6fb9b837d362631409 in / 
# Fri, 12 Nov 2021 17:20:17 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:22:49 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Sat, 13 Nov 2021 06:22:50 GMT
COPY file:21256ff7df5369f7ad2e19c6d020a644303aded200bdbec4d46648f38d55df78 in /bin/registry 
# Sat, 13 Nov 2021 06:22:50 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Sat, 13 Nov 2021 06:22:50 GMT
VOLUME [/var/lib/registry]
# Sat, 13 Nov 2021 06:22:51 GMT
EXPOSE 5000
# Sat, 13 Nov 2021 06:22:51 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Sat, 13 Nov 2021 06:22:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:22:51 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:79e9f2f55bf5465a02ee6a6170e66005b20c7aa6b115af6fcd04fad706ea651a`  
		Last Modified: Fri, 12 Nov 2021 17:21:24 GMT  
		Size: 2.8 MB (2817409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d96da54f60b86a4d869d44b44cfca69d71c4776b81d361bc057d6666ec0d878`  
		Last Modified: Sat, 13 Nov 2021 06:23:02 GMT  
		Size: 299.6 KB (299640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b27040df4a23c90c3837d926f633fb327fb3af9ac4fa5d5bc3520ad578acb10`  
		Last Modified: Sat, 13 Nov 2021 06:23:03 GMT  
		Size: 6.8 MB (6823927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ead8259a04d39492c25c9548078200c5ec429f628dcf7b7535137954cc2df0`  
		Last Modified: Sat, 13 Nov 2021 06:23:01 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3790aef225b922bc97aaba099fe762f7b115aec55a0083824b548a6a1e610719`  
		Last Modified: Sat, 13 Nov 2021 06:23:01 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.7.1` - linux; arm variant v6

```console
$ docker pull registry@sha256:eafd2cdf8e847216f62e1acb756f992689f4861baf943610ad4127df3cacee29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9315138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8a56425636efd3a5e4337640baf5cb2264890edab9753f228a1bffe4fe52e2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Fri, 12 Nov 2021 16:50:22 GMT
ADD file:c219ee7662a2b29c4e06be5bf332f2f53b326937277057af61516f5cf5abce1e in / 
# Fri, 12 Nov 2021 16:50:23 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:39:50 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Fri, 12 Nov 2021 18:39:52 GMT
COPY file:29c6c1625420a558a03cc7ed253192f8138cba6212b64e30217fb6488af668e2 in /bin/registry 
# Fri, 12 Nov 2021 18:39:52 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 12 Nov 2021 18:39:53 GMT
VOLUME [/var/lib/registry]
# Fri, 12 Nov 2021 18:39:53 GMT
EXPOSE 5000
# Fri, 12 Nov 2021 18:39:54 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 12 Nov 2021 18:39:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:39:54 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:5cb8b15578b20b3c847454a0e0743b923ddea3e4f22ffa95f6f41b0c551a391e`  
		Last Modified: Fri, 12 Nov 2021 16:52:20 GMT  
		Size: 2.6 MB (2623510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f42adccaa3d4922795f3649d07292e4ce62f4d385383fd4e692f127d1d8d4ac`  
		Last Modified: Fri, 12 Nov 2021 18:40:26 GMT  
		Size: 299.9 KB (299931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33cdd19516437a0bd6d652b69c0243f481402a421101d6f55d015341cc0966d`  
		Last Modified: Fri, 12 Nov 2021 18:40:30 GMT  
		Size: 6.4 MB (6391083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa54e3652a6c452d8957014ed3a2a9be3a879ae1d7f9e9d4b8976527df0b821`  
		Last Modified: Fri, 12 Nov 2021 18:40:26 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef5fbcd41180f8f78fb1db49ef015abb3418b6e5225c4ecf7dd972748a96032`  
		Last Modified: Fri, 12 Nov 2021 18:40:26 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.7.1` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:e9c2d646078211f8353e482caac9d9b12f38b42bc29cb30c453841cf144037b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9269387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bf57bb5c31c49b2fb6d0a86234b5f59a97d559072dc273a1a6ea6789abb720`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:19 GMT
ADD file:bffb4828c6bba0115b766f72c49407938059b204ac9edf130d023af34871d3d0 in / 
# Fri, 12 Nov 2021 16:40:19 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:53:00 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Fri, 12 Nov 2021 18:53:02 GMT
COPY file:51a441e6eceff49ef32609e7070b64e8d5690648e4f915cc825274e6fe37aed2 in /bin/registry 
# Fri, 12 Nov 2021 18:53:03 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 12 Nov 2021 18:53:03 GMT
VOLUME [/var/lib/registry]
# Fri, 12 Nov 2021 18:53:04 GMT
EXPOSE 5000
# Fri, 12 Nov 2021 18:53:06 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 12 Nov 2021 18:53:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:53:07 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:b48a9fe99aba73065302163e59c82a1b0054810c7b9ef85eee6f1b495b162461`  
		Last Modified: Fri, 12 Nov 2021 16:41:35 GMT  
		Size: 2.7 MB (2728748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095878aa44caf2b7927dcf6de1a53e40f016b5ce43b2c885c8e0ecb90fc5f403`  
		Last Modified: Fri, 12 Nov 2021 18:53:25 GMT  
		Size: 299.9 KB (299858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04df0d597e2b057779cd387b32c7d76c5f06254f0c29ea7f3977487fb29a6e2a`  
		Last Modified: Fri, 12 Nov 2021 18:53:26 GMT  
		Size: 6.2 MB (6240198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0594d0cd6d662a93dda81e2bcde210e3279fef169f331f784e66e742c83b2c2`  
		Last Modified: Fri, 12 Nov 2021 18:53:25 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a758d8738abf69bbb372dcfd778368e8c0f74f7cbbf4519eddb0d4a1ef9e81`  
		Last Modified: Fri, 12 Nov 2021 18:53:25 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `registry:latest`

```console
$ docker pull registry@sha256:169211e20e2f2d5d115674681eb79d21a217b296b43374b8e39f97fcf866b375
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `registry:latest` - linux; amd64

```console
$ docker pull registry@sha256:36cb5b157911061fb610d8884dc09e0b0300a767a350563cbfd88b4b85324ce4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9941588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8604a3fe8543c9e6afc29550de05b36cd162a97aa9b2833864ea8a5be11f3e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:17 GMT
ADD file:efe2d94a88cdbbd01c3ef095f0a2473cec9e74804b49cd6fb9b837d362631409 in / 
# Fri, 12 Nov 2021 17:20:17 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:22:49 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Sat, 13 Nov 2021 06:22:50 GMT
COPY file:21256ff7df5369f7ad2e19c6d020a644303aded200bdbec4d46648f38d55df78 in /bin/registry 
# Sat, 13 Nov 2021 06:22:50 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Sat, 13 Nov 2021 06:22:50 GMT
VOLUME [/var/lib/registry]
# Sat, 13 Nov 2021 06:22:51 GMT
EXPOSE 5000
# Sat, 13 Nov 2021 06:22:51 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Sat, 13 Nov 2021 06:22:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:22:51 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:79e9f2f55bf5465a02ee6a6170e66005b20c7aa6b115af6fcd04fad706ea651a`  
		Last Modified: Fri, 12 Nov 2021 17:21:24 GMT  
		Size: 2.8 MB (2817409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d96da54f60b86a4d869d44b44cfca69d71c4776b81d361bc057d6666ec0d878`  
		Last Modified: Sat, 13 Nov 2021 06:23:02 GMT  
		Size: 299.6 KB (299640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b27040df4a23c90c3837d926f633fb327fb3af9ac4fa5d5bc3520ad578acb10`  
		Last Modified: Sat, 13 Nov 2021 06:23:03 GMT  
		Size: 6.8 MB (6823927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ead8259a04d39492c25c9548078200c5ec429f628dcf7b7535137954cc2df0`  
		Last Modified: Sat, 13 Nov 2021 06:23:01 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3790aef225b922bc97aaba099fe762f7b115aec55a0083824b548a6a1e610719`  
		Last Modified: Sat, 13 Nov 2021 06:23:01 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm variant v6

```console
$ docker pull registry@sha256:eafd2cdf8e847216f62e1acb756f992689f4861baf943610ad4127df3cacee29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9315138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8a56425636efd3a5e4337640baf5cb2264890edab9753f228a1bffe4fe52e2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Fri, 12 Nov 2021 16:50:22 GMT
ADD file:c219ee7662a2b29c4e06be5bf332f2f53b326937277057af61516f5cf5abce1e in / 
# Fri, 12 Nov 2021 16:50:23 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:39:50 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Fri, 12 Nov 2021 18:39:52 GMT
COPY file:29c6c1625420a558a03cc7ed253192f8138cba6212b64e30217fb6488af668e2 in /bin/registry 
# Fri, 12 Nov 2021 18:39:52 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 12 Nov 2021 18:39:53 GMT
VOLUME [/var/lib/registry]
# Fri, 12 Nov 2021 18:39:53 GMT
EXPOSE 5000
# Fri, 12 Nov 2021 18:39:54 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 12 Nov 2021 18:39:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:39:54 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:5cb8b15578b20b3c847454a0e0743b923ddea3e4f22ffa95f6f41b0c551a391e`  
		Last Modified: Fri, 12 Nov 2021 16:52:20 GMT  
		Size: 2.6 MB (2623510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f42adccaa3d4922795f3649d07292e4ce62f4d385383fd4e692f127d1d8d4ac`  
		Last Modified: Fri, 12 Nov 2021 18:40:26 GMT  
		Size: 299.9 KB (299931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33cdd19516437a0bd6d652b69c0243f481402a421101d6f55d015341cc0966d`  
		Last Modified: Fri, 12 Nov 2021 18:40:30 GMT  
		Size: 6.4 MB (6391083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa54e3652a6c452d8957014ed3a2a9be3a879ae1d7f9e9d4b8976527df0b821`  
		Last Modified: Fri, 12 Nov 2021 18:40:26 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef5fbcd41180f8f78fb1db49ef015abb3418b6e5225c4ecf7dd972748a96032`  
		Last Modified: Fri, 12 Nov 2021 18:40:26 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:e9c2d646078211f8353e482caac9d9b12f38b42bc29cb30c453841cf144037b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9269387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bf57bb5c31c49b2fb6d0a86234b5f59a97d559072dc273a1a6ea6789abb720`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:19 GMT
ADD file:bffb4828c6bba0115b766f72c49407938059b204ac9edf130d023af34871d3d0 in / 
# Fri, 12 Nov 2021 16:40:19 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:53:00 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Fri, 12 Nov 2021 18:53:02 GMT
COPY file:51a441e6eceff49ef32609e7070b64e8d5690648e4f915cc825274e6fe37aed2 in /bin/registry 
# Fri, 12 Nov 2021 18:53:03 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 12 Nov 2021 18:53:03 GMT
VOLUME [/var/lib/registry]
# Fri, 12 Nov 2021 18:53:04 GMT
EXPOSE 5000
# Fri, 12 Nov 2021 18:53:06 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 12 Nov 2021 18:53:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:53:07 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:b48a9fe99aba73065302163e59c82a1b0054810c7b9ef85eee6f1b495b162461`  
		Last Modified: Fri, 12 Nov 2021 16:41:35 GMT  
		Size: 2.7 MB (2728748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095878aa44caf2b7927dcf6de1a53e40f016b5ce43b2c885c8e0ecb90fc5f403`  
		Last Modified: Fri, 12 Nov 2021 18:53:25 GMT  
		Size: 299.9 KB (299858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04df0d597e2b057779cd387b32c7d76c5f06254f0c29ea7f3977487fb29a6e2a`  
		Last Modified: Fri, 12 Nov 2021 18:53:26 GMT  
		Size: 6.2 MB (6240198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0594d0cd6d662a93dda81e2bcde210e3279fef169f331f784e66e742c83b2c2`  
		Last Modified: Fri, 12 Nov 2021 18:53:25 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a758d8738abf69bbb372dcfd778368e8c0f74f7cbbf4519eddb0d4a1ef9e81`  
		Last Modified: Fri, 12 Nov 2021 18:53:25 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
