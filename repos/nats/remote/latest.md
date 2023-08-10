## `nats:latest`

```console
$ docker pull nats@sha256:a75b6817e3135f1f789e970a62980e49b9efa3d3cdfc7db4193312f12cb44b3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4737; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:cf96338e314ee46e307626e8936dc31b9ef7c67e299b29b7753896d11b52fe8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5455cadbb1bd4919947f5a918491add0f2a8fe5d9aa4a801ca79a4ac8fb308f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:26:10 GMT
COPY file:975a38b1520c81a5e1d0876325548b4aefe0036b6deee1ae7ee20db6abbcc080 in /nats-server 
# Mon, 07 Aug 2023 19:26:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:26:11 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:26:11 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:26:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc02d5ba29398595681917073dcd141022b8ad8d0da9a18b6f5752e56c86ceea`  
		Last Modified: Mon, 07 Aug 2023 19:26:56 GMT  
		Size: 5.2 MB (5169747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9457cd0af5e7125dfe4a44e1d6d003e2bdaf42da9d1c5f7b313069a145e639`  
		Last Modified: Mon, 07 Aug 2023 19:26:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:3a3792aaaf193e57879f3594e95501c1372bd2a537965db2bc68fd85c13b8cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4932529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966d4a644152a12918ae66827a94561e477b28d10bd2698612566a5c989612f1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:447be8988a65ae095af689a396d155107ebc910fe545508c6e6af6f1c2d2c4d4 in /nats-server 
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:50:31 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:50:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:50:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:590d3f4a49d783a9889465cc7862cf43dc4d3a60e0fb075544618efee1ef93e1`  
		Last Modified: Mon, 07 Aug 2023 19:51:13 GMT  
		Size: 4.9 MB (4932022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901e46e20099bb53f1d1b41e9f1cbf04d9af77173e45873723bd9d7825fbbcf0`  
		Last Modified: Mon, 07 Aug 2023 19:51:12 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:3be04f93d99a8e23e99fff2608d9c0d76a4ee2c9c301441f57a2d0b9225c16e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4924573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec722342be0e9d946cb8ac26674a30ff2854116e2e8e1ba75461b3f90d97ecc8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:a28d4beb7d3acaa71be2e58ce3a707a2f5be041842f8a1e4eb4c54dd72e865eb in /nats-server 
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 20:16:33 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 20:16:33 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 20:16:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:68043f4483bff82380b8666c025686881f5483ff754784192f65aa4ec9b662fe`  
		Last Modified: Mon, 07 Aug 2023 20:17:27 GMT  
		Size: 4.9 MB (4924065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443d8f0ff2c43f481bd49043e2c13423203b3a99754a3baff7df20850bf0e56`  
		Last Modified: Mon, 07 Aug 2023 20:17:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24cb726cdaa647f5307f6d5fa448b299535141c96367b79636f23597407b5071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4734399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2f013bc2559b3a905b049fd4b09738b17a4c87d62bed5a1830c6a6e13b1cda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:815b9c4a7d715138f02171cd656c9e8dc6d80e72107c92661c99f6dd24ae2721 in /nats-server 
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:44:14 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:44:14 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:44:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07116324214b64589e3a471932fe7f6b892068a7cd9cf9bb72a8ea25f8a92200`  
		Last Modified: Mon, 07 Aug 2023 19:44:57 GMT  
		Size: 4.7 MB (4733893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615975e7d25e46607f561d13c4c244d070bb41701a0ac2103df98dcb33e8a4eb`  
		Last Modified: Mon, 07 Aug 2023 19:44:56 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:d8a94368172a3df5204943029b32d7b56dda869dadef4983129598ed86fcec67
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109707647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1b071e5cf657d3db4c3347053329658550fdb8b09ae38a2618af5b119a8565`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 10 Aug 2023 02:34:53 GMT
RUN cmd /S /C #(nop) COPY file:3b8a3a4f656cc66920d77ff06f41851caa37056073cec32caf7e7024bea62100 in C:\nats-server.exe 
# Thu, 10 Aug 2023 02:34:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:56 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43534c571f8fdc71038e0f4b4c33a30adb0bbc8b292454d35930557ced33408`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6810a6f695e6275423db76be5637667297faaa666b58a9658e1690efe300b007`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 5.2 MB (5242246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fbe96bd125f3ebe2f71079f2d8c4ca1d226d4aa3de1dd2a0fefb0e50421464`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c6c360e7d8fa0f4858a220d96a5d13e7c65c195bb8513191b47c1d3b0c6b91`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3db71fcfd8d9cd70e2947e60d0f27dee2449c365fcd7dde18997017f1f7a443`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112aff03752bdfd32ed33505dc8c488a27bdc249bd506edd30af3d47c0d9b4a2`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
