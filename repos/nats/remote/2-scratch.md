## `nats:2-scratch`

```console
$ docker pull nats@sha256:1d7bb9e29604d123da90fc254e181ca742f3327340de6cc7c3666230a7e25520
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:e6916a74a9af2d54502bfa1459a3e0702c00faa14327b3f3b812262e8ada0966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4933617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0263a71ad823c35b7c360c016e57737a4367ef1c4909a859acb0ddb4ab19a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:ac560677dbfad917be71a9245045f536b2801212b542bc63c664d6d11156f4dc in /nats-server 
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:43:58 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:43:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:43:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5668bc7ee19e1c51e1510bfeee7245e2b2cc66a8b8f8b0f988f4b3bca8729cec`  
		Last Modified: Tue, 07 Feb 2023 02:44:45 GMT  
		Size: 4.9 MB (4933108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d5b4d77a0e7f6c3fed0f1ae97dbe1b22a3ed4e6af873e7782a0b1d2b992779`  
		Last Modified: Tue, 07 Feb 2023 02:44:44 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e1ba487c56a25895759177de201768f40c51ceeedca983afa03875039445bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4739851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b60b5d45617b9109e120de34ac32b0647324dba3d69d2c56366545e50c2484c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:614e1182091dacdaa5043752e8239600bae8aa334cfd383cc326d1753d3eba64 in /nats-server 
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:49:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:49:36 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:49:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d859c106d4072b51eee7be282394c7f0c288186311ae904751cd95c3cf9468ae`  
		Last Modified: Thu, 02 Mar 2023 18:50:54 GMT  
		Size: 4.7 MB (4739343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7000b41bf11d721897d126c1e72201203bcc8e9716daad77d7d42ae97853a`  
		Last Modified: Thu, 02 Mar 2023 18:50:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:644eac35d964521bc85286defaf1bae093b36618fe862eedff9a996e330fc60c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4731109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e814afeda8d92b2fb3dcdacf4648234504c6e4cd7fc24cce256cc588a439d7e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:a63786ae76c5e718a4952dd30b2265019e1ca48099ad19279d2e77e5ad704bfc in /nats-server 
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:57:50 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:57:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:57:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e714c80855fb90cb44f135a04bf323493a749536bb9106eb3ef4e69a70682897`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 4.7 MB (4730600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e020ba411c44ee7d23b6bdbd966700955c2d087afd3d79a9ad51e0390e8e7b6`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:35ef84ac5e9bb0d0229fb1a773677d6ee7b23bb58937427d20aaa36987562373
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f367536d7ef4331c52bf405914c6f7affdccdb8eed05fb4c981efe519fd06f00`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:23081283f9b4d8145ad2b3a276cc08fcb49c4850e322db9560525e495d1bf362 in /nats-server 
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:40:16 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:40:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:40:16 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:40:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a910efaa632bb8401dbca7cfe541f6dc4da71ea38708992ef153250254493114`  
		Last Modified: Thu, 02 Mar 2023 18:41:09 GMT  
		Size: 4.6 MB (4558972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be7fc9abf13897cf1a5e7026f6a49b3308d5a864640e1f4b6e526ee95f093fc`  
		Last Modified: Thu, 02 Mar 2023 18:41:08 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
