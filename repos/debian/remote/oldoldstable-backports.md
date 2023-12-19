## `debian:oldoldstable-backports`

```console
$ docker pull debian@sha256:7927a1a970daebc616b71bd8917497525dee96b6f6d334a8c0f214ac14b35a2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldoldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:da9aba74348780998af2e3a946ce7f3bb0157b6da5c4a5778cc6561dd2d57eff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50500648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fec7766fdb40275ed544dfbe6bd2d06f06620c89bb0de9a0600f32d5f4515e72`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:22 GMT
ADD file:bbc11f96990693bbea714e77ec242f2aceace6e0c62eee4d94e17e6bb0e7cb24 in / 
# Tue, 19 Dec 2023 01:21:22 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:21:26 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c21e4de82652c5b63bd662ebcd5a9962068176f68faa6506ce365d1bf5352a0e`  
		Last Modified: Tue, 19 Dec 2023 01:26:39 GMT  
		Size: 50.5 MB (50500421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d916cf7b57a4473a93860a5af0c50579171706e2e10d80d4a325db99906ede8a`  
		Last Modified: Tue, 19 Dec 2023 01:26:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:8ba4edc04366bf9213ed0fe02fcfd892cd21f8847d53ff9e8805714370602fd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45967871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02a4d75ca3211e495376811656f447eceb603e858da50f405b29b4324a1ada13`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:35 GMT
ADD file:5500e132393af7a300d91f1dee2496d5bb6264e262876d133740a23849889a7d in / 
# Tue, 19 Dec 2023 02:08:36 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:08:39 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:101c41b9fd02385a3dad0838943e2cc5b9f6d675638608434822ca3da4fa8ac8`  
		Last Modified: Tue, 19 Dec 2023 02:13:31 GMT  
		Size: 46.0 MB (45967645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1cbe90934dfe155bbb654296f89368820d2328b6e3d9c956597f0fdd17bce7`  
		Last Modified: Tue, 19 Dec 2023 02:13:41 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:0838869733c9807f234ae070053f98aadac386d903863b236245521cb441970b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49289272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7eed2d089395c7652cbb5692ce1e441ad24ced4868b0b1eaaf8e232224e4f2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:45 GMT
ADD file:508906545ca32de29467e22d951b0a0e82cea987c01065b229c95e11e2f1b443 in / 
# Tue, 19 Dec 2023 01:41:46 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:41:48 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8dadfd881a838a5295cee22b635167fbf762c05e03c037e0ad776a1626d97d88`  
		Last Modified: Tue, 19 Dec 2023 01:46:19 GMT  
		Size: 49.3 MB (49289045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77abec20e6833a4aed6e6bc02d8a524bf7e3dc62f71c0076548f8f856a9e7d1f`  
		Last Modified: Tue, 19 Dec 2023 01:46:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:984af5a4ce8883d213c37fa8b30053ba201cf766129167c66fede8d8cc8b4d66
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51255679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d93dadeb451f092502cda10df271ee5a2c7e6bbc41240b1d1977d37ba86f5c3d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:40:03 GMT
ADD file:ec09f24b151e99e54f7d476c00719c3c065f4c6004e23f41c8812a9f72cb3fb3 in / 
# Tue, 19 Dec 2023 01:40:04 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:40:07 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:330d1a7174f035d420568e46a6178d9fdf43d42902dfe8cdf31f89f7615eec2b`  
		Last Modified: Tue, 19 Dec 2023 01:45:41 GMT  
		Size: 51.3 MB (51255452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f52b47a2d3ef02c39fee5db51d85945105792d117fdd73c269cc7393b47e90d`  
		Last Modified: Tue, 19 Dec 2023 01:45:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
