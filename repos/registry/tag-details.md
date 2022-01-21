<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `registry`

-	[`registry:2`](#registry2)
-	[`registry:2.7`](#registry27)
-	[`registry:2.7.1`](#registry271)
-	[`registry:2.8.0-beta.1`](#registry280-beta1)
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

## `registry:2.8.0-beta.1`

```console
$ docker pull registry@sha256:a773fbd76b7f798ad1c4278c11af066582cf4f231919b32c69861b2d765079fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `registry:2.8.0-beta.1` - linux; amd64

```console
$ docker pull registry@sha256:68013e9fe5816080e3e08dafb71069feda627a30be409517a76f862a5bc2ebec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9203399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22a0ae0b740dcca5280dd6dbe4a267c7c3652fa799f67ed41f376ba0c57b6831`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:21:45 GMT
RUN apk add --no-cache ca-certificates
# Fri, 21 Jan 2022 20:35:10 GMT
RUN set -eux; 	version='2.8.0-beta.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='d69d68406a30466070d8e47c21fafaadae5c048239df41b50b28a79fa12945ab' ;; 		aarch64) arch='arm64';   sha256='2a080694ae2528a628245cf5177d4d2e55d430c5dd76cbbf61e5aee08e75abf6' ;; 		armhf)   arch='armv6';   sha256='b5092556fd196f59c7d2a8d4e4460c193588d9f7f39d825d17f299d7fc856ca1' ;; 		armv7)   arch='armv7';   sha256='f479d7d42a4c6086ee9a51f605386fcfb953198bf9ab48c515ffdde33ad46e5d' ;; 		ppc64le) arch='ppc64le'; sha256='dc0444e672511b4f8dc19fcec1624a33fdaf49a72ff3c1a69bae9bd3399cd074' ;; 		s390x)   arch='s390x';   sha256='4b814d1cb60ee7881e59c1ee52635755c2279196861892cface92e58aa6ac749' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 21 Jan 2022 20:35:10 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 21 Jan 2022 20:35:11 GMT
VOLUME [/var/lib/registry]
# Fri, 21 Jan 2022 20:35:11 GMT
EXPOSE 5000
# Fri, 21 Jan 2022 20:35:11 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 21 Jan 2022 20:35:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 20:35:11 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666ba61612fd7c93393f9a5bc1751d8a9929e32d51501dba691da9e8232bc87b`  
		Last Modified: Tue, 30 Nov 2021 04:36:04 GMT  
		Size: 282.2 KB (282159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4909f6b47270f299efdb8e59ba685a37761a451b6e17d04dbb87dfbe724ce8c8`  
		Last Modified: Fri, 21 Jan 2022 20:35:27 GMT  
		Size: 6.1 MB (6102214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94eb48d3d1bb54fab96b0e8641a774565b864d56206847303675ed3e169074`  
		Last Modified: Fri, 21 Jan 2022 20:35:25 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9502f93854206250a1f624d622643c82983bd9f55e69088b2cb11fda3b04aaf9`  
		Last Modified: Fri, 21 Jan 2022 20:35:25 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8.0-beta.1` - linux; arm variant v6

```console
$ docker pull registry@sha256:c664d884d9cd482e0d487e658eaa0e220d4f1ecbf6ba1427a50d968b8ac91e0a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8582090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90c22c14e051215c9cd60f933ab676b9765a259c9482aa7769725200c531727e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 02:32:18 GMT
RUN apk add --no-cache ca-certificates
# Fri, 21 Jan 2022 22:08:14 GMT
RUN set -eux; 	version='2.8.0-beta.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='d69d68406a30466070d8e47c21fafaadae5c048239df41b50b28a79fa12945ab' ;; 		aarch64) arch='arm64';   sha256='2a080694ae2528a628245cf5177d4d2e55d430c5dd76cbbf61e5aee08e75abf6' ;; 		armhf)   arch='armv6';   sha256='b5092556fd196f59c7d2a8d4e4460c193588d9f7f39d825d17f299d7fc856ca1' ;; 		armv7)   arch='armv7';   sha256='f479d7d42a4c6086ee9a51f605386fcfb953198bf9ab48c515ffdde33ad46e5d' ;; 		ppc64le) arch='ppc64le'; sha256='dc0444e672511b4f8dc19fcec1624a33fdaf49a72ff3c1a69bae9bd3399cd074' ;; 		s390x)   arch='s390x';   sha256='4b814d1cb60ee7881e59c1ee52635755c2279196861892cface92e58aa6ac749' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 21 Jan 2022 22:08:15 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 21 Jan 2022 22:08:15 GMT
VOLUME [/var/lib/registry]
# Fri, 21 Jan 2022 22:08:16 GMT
EXPOSE 5000
# Fri, 21 Jan 2022 22:08:16 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 21 Jan 2022 22:08:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 22:08:17 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228ad0256439cce3fe9db355991b0557f55241d8cca8690f4f741e1c2d8fb8b9`  
		Last Modified: Tue, 30 Nov 2021 02:47:28 GMT  
		Size: 282.1 KB (282105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f404c9519f92bee75387bf2be52c6ad66867da624e8e8f4b3bb1a07a5adecdd1`  
		Last Modified: Fri, 21 Jan 2022 22:09:05 GMT  
		Size: 5.7 MB (5667951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21863962e82a5e9a5cfe9bd816e37444cd4f81e525388a9159dd8cf21b8a249f`  
		Last Modified: Fri, 21 Jan 2022 22:09:01 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d086aa143c4663bcd1b142172585082b892e6afb52a23d314f464dc9cc2c2fc4`  
		Last Modified: Fri, 21 Jan 2022 22:09:01 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8.0-beta.1` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:15ef405da19611db38d95617a7ca4f842a6a3d1f32fd8106249ba8d4b171cbca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8541458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:860726fe7ffb6492ce815b250278fa9e411b683d1387777c5e9cd8c1c77bc038`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 01:54:59 GMT
RUN apk add --no-cache ca-certificates
# Fri, 21 Jan 2022 22:18:48 GMT
RUN set -eux; 	version='2.8.0-beta.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='d69d68406a30466070d8e47c21fafaadae5c048239df41b50b28a79fa12945ab' ;; 		aarch64) arch='arm64';   sha256='2a080694ae2528a628245cf5177d4d2e55d430c5dd76cbbf61e5aee08e75abf6' ;; 		armhf)   arch='armv6';   sha256='b5092556fd196f59c7d2a8d4e4460c193588d9f7f39d825d17f299d7fc856ca1' ;; 		armv7)   arch='armv7';   sha256='f479d7d42a4c6086ee9a51f605386fcfb953198bf9ab48c515ffdde33ad46e5d' ;; 		ppc64le) arch='ppc64le'; sha256='dc0444e672511b4f8dc19fcec1624a33fdaf49a72ff3c1a69bae9bd3399cd074' ;; 		s390x)   arch='s390x';   sha256='4b814d1cb60ee7881e59c1ee52635755c2279196861892cface92e58aa6ac749' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 21 Jan 2022 22:18:50 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 21 Jan 2022 22:18:50 GMT
VOLUME [/var/lib/registry]
# Fri, 21 Jan 2022 22:18:51 GMT
EXPOSE 5000
# Fri, 21 Jan 2022 22:18:53 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 21 Jan 2022 22:18:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 22:18:54 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a89e8eeedd549875510e5e4e14010906a58878526814e6df25d14009856c6ff`  
		Last Modified: Tue, 30 Nov 2021 02:05:10 GMT  
		Size: 281.9 KB (281899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c1186b17b7a1a4b5dd18bc453d11a55fa9db24921e44934ea445bd516de17d`  
		Last Modified: Fri, 21 Jan 2022 22:19:17 GMT  
		Size: 5.5 MB (5543541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf51e8ccd13672fe43d69f7b3e49f8e43e0b00786ac2ae0e2096a5aa27a26b0`  
		Last Modified: Fri, 21 Jan 2022 22:19:16 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a230db5a70e19dbe7ceceb79a7f365747811d399b7d74541ce0422dcd1a03472`  
		Last Modified: Fri, 21 Jan 2022 22:19:16 GMT  
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
