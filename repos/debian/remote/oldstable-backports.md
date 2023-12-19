## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:2507ae34a4da6f62e02a57cbe26b1dc90495830528ad9fe652688000a6657ff2
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

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:45fa0cc0f913f1a4e2074f463a116a899276c1eecdd841859cfb0d54c94fce16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55057583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f96d36f8bc23507a834eaee58637ccbc3bf592ff03d76fb8ee73719d3e2343`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:43 GMT
ADD file:a256fd7b775e0858606b47f71a6c17bf5f4b19ec370f63c81d8360bc023c9016 in / 
# Tue, 19 Dec 2023 01:21:43 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:21:47 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:af4bb5d950c2169fd8e2b5e6eeb632e050b11508a4e534314025e6d68acb55d3`  
		Last Modified: Tue, 19 Dec 2023 01:27:19 GMT  
		Size: 55.1 MB (55057358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26ee852607153a4fcaf60df5012f6ec4614a9ff3465aa7947f2e5355c868737`  
		Last Modified: Tue, 19 Dec 2023 01:27:30 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:207e6cf6d73a98ffb12d6167d1eef4c40e510952153c489d9962898e24bb46d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52562509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc3295360e6b812c4cf53bc03788f504df7938f209d9092ceed613a18423e263`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:45 GMT
ADD file:9a206a61da09ef667a5835f06c3853bcd727291a9a07e1da86e73d156da09899 in / 
# Tue, 19 Dec 2023 01:55:46 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:55:48 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:455223f1f1685c2b7809878927b0fab0ee1eda1ecb10e51fdb3df277a998ebfe`  
		Last Modified: Tue, 19 Dec 2023 01:59:43 GMT  
		Size: 52.6 MB (52562283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79dd19b23a0579b515fcfb661c5810c4f1da74d3aecfe8b9d21801279cb5e303`  
		Last Modified: Tue, 19 Dec 2023 01:59:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:d28eff86ad511ed9f6203dcb32da5a1a8dd0fa77d4283f3fca4c96158d12e30f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50215996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:385ab292ebd76c3f0e6f3c23e7f43d1e7a9edbb9dbe6e19c4573874a03599b00`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:54 GMT
ADD file:07e819a7652eed6ad0744a33f91c3395be0ebd2f1800907e9cc1bef17bba0a5b in / 
# Tue, 19 Dec 2023 02:08:55 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:08:58 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:98a479ed90983736e2dc2d1539c15e7b3a5acaa2a1b960b036905ea3ee884060`  
		Last Modified: Tue, 19 Dec 2023 02:14:04 GMT  
		Size: 50.2 MB (50215772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7a1582c79165c32736b9c8ca39c2753a4d898358f157e320bcb8cfaa0dacea`  
		Last Modified: Tue, 19 Dec 2023 02:14:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:1ed615bd115f7c73d8d66aaafde5659ea8743637b1fc42628b949568f771e3f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53708335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8deacdc406fb41636861b91a2e5faae7ef2f38d738f42eaf1fa97a0f528b1ffe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:59 GMT
ADD file:08d23120303636c47a9638de424f73156ed488df7dbe850bdc224518313fcdd7 in / 
# Tue, 19 Dec 2023 01:41:59 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:42:02 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9f50317d72ce64f4d5cf4a4a1e718848fb4d8a3f7e45c8e7ce0efc6e68881cda`  
		Last Modified: Tue, 19 Dec 2023 01:46:52 GMT  
		Size: 53.7 MB (53708108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93fb8a0c1638e5c9be1edd45eb2e611bf8ac2c3b597483f248a6b93bdb3baf2`  
		Last Modified: Tue, 19 Dec 2023 01:47:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:70d132fb9ef08e220c63380d59b8ea2c84621440fc6b6a62a1f5a62ceac36969
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56046573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9198499879aac4d37c101ab122410a095cd9ee5e0c6e53aba4a3c7ef3d6b662`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:40:24 GMT
ADD file:c8c207b2b9664485501fb4d901521c1917e0a13c397f1754c3283d0edbb4cb03 in / 
# Tue, 19 Dec 2023 01:40:25 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:40:29 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:05911176939a2f5a1f36835d00068dd2778b34ef7f2c2f98eec5d7f9beca2880`  
		Last Modified: Tue, 19 Dec 2023 01:46:19 GMT  
		Size: 56.0 MB (56046346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa4a5ab22c030a289cc6c7ac6f32538bc4919f6906a3b66d9035df226b058e5`  
		Last Modified: Tue, 19 Dec 2023 01:46:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:3007a2de37f7f36a81ec0e7ea430851e871e2a808310baf49bab7eb1defbc49f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53289212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a403ecb5725514761ed5ec74b02bada75eaf30312a420d38846a92fd935c055`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:15:24 GMT
ADD file:29da39aa8ca95d240d83dd122971dad61011bad34879f927e7d326b136e2b6d1 in / 
# Tue, 19 Dec 2023 02:15:30 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:15:45 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ec5d0f68a2320f2747f9efbc2d4276fe7723960fcb889dc46c9f86d3ceac4c9e`  
		Last Modified: Tue, 19 Dec 2023 02:26:48 GMT  
		Size: 53.3 MB (53288984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9745a612490a16441f36701c719bca25df322d7e219eda1986c16d9eea0086c2`  
		Last Modified: Tue, 19 Dec 2023 02:26:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:921658f04a01fd69e7dce0fbf66852d9c745849ccbe604a2a2928830cd5e7e52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58930149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:775fa8ca3d7b2f1c4609eea4694bc6f9565dbaa418193500e93f0c692f7a5b4b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:22:32 GMT
ADD file:6d4bdf7d922b75f6a16b5c2e0faceb63db690dad977dfed65b6bb0e3d006b15c in / 
# Tue, 19 Dec 2023 01:22:36 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:22:41 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4b8a9f9c32f0a17c308c1d6404d8037a55cfad4cc80bae692d34c4b72d96535b`  
		Last Modified: Tue, 19 Dec 2023 01:27:36 GMT  
		Size: 58.9 MB (58929922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870074ec260b05c7a2b9429533dfb7ff18e6ed42fd2b04dda38e994819fa1680`  
		Last Modified: Tue, 19 Dec 2023 01:27:45 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:845c5958e86cb7d0d3b2ad78f2f7e1ba17663def1d09926e3f663ab758388106
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53296187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:013ec14901f2929d6a2107265bfa8d41b68dc6aa56e740984073a30a24f62669`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:43:25 GMT
ADD file:8cbd16e53c55e62cc86d57938fea4be5cbafec8b7585ec2c869a6ed6868101f6 in / 
# Tue, 19 Dec 2023 01:43:29 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:43:35 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:faf91f5425124fb5d6a85c2909beca1708f00a645a6abc12554763638cc28cfd`  
		Last Modified: Tue, 19 Dec 2023 01:48:21 GMT  
		Size: 53.3 MB (53295962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81324aaefd64542cd417abe3668f000fb25d5abe5389cfaed1bfe84cfc29e160`  
		Last Modified: Tue, 19 Dec 2023 01:48:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
