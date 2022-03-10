## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:9f8cedbf2e74e6679e9ab44848904ad048f1f9202d1dd72e203002605ba4a331
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2686; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eea355922fa3e329228180c171fe18939205a5828944f3c0ec23c0816eef7982
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7081263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db0f18c883ff929dfaae3de15de5562de5be34b4a941aa05c6d52112b8e4c84`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:21:18 GMT
COPY file:6fcfe62a6cc0951979b80258fb3d207e13828d9234e227e1398cab40548702d7 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:21:18 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:21:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:64b920df5d588d78c6c317a08480a016eb7b6433705c1a3811a22e4e422e61d0`  
		Last Modified: Wed, 09 Mar 2022 23:22:00 GMT  
		Size: 7.1 MB (7081263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:36364386127a72bc130f59fb33c4119222fc6c671e33aea460f694025b82cd46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6597197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a965dc95f8a3e6631c5ca714f0aafd2acc1508a1f6d3298300876536949f11b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:49:55 GMT
COPY file:d62d923585419f7f9d263c0018d56cc159b1092bf7bae749223f339a514a81d9 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:49:56 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:49:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0b00cb53513f9c5bd72363c73ee281128c2cedd1d7653aa7278a2a6536c86a14`  
		Last Modified: Wed, 09 Mar 2022 23:51:50 GMT  
		Size: 6.6 MB (6597197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:c786255507edae1bf8167b3adbe962fa9c4ba18fd683462921df662c86e5f36f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6589565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb16b4f9d4a38de66adad0c74fd19049b37e96277e0cd459805b74bdf9474ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:29:51 GMT
COPY file:a5f2524f76b038dc99564d67f8cf6396171fe569b86b60aa9892eca88643b977 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:29:52 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:29:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:29:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:271fefa5e75537e471ab2e96d1b28b6614b2103db059b37f0e60bcc9b8ab40d8`  
		Last Modified: Wed, 09 Mar 2022 23:31:44 GMT  
		Size: 6.6 MB (6589565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bb6e16886863d8c84bc6427c4a45c43bca8f97adcddd602756dddc70fa826a6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6510632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd1fc4d49faf17ca5b2a9d116b2758a93de1af0ea5b526e23128bd6bbd00b5f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:41:07 GMT
COPY file:f47e5ea058ace7f6cdb8bca186dec2b15d364fff4ff67303ae8d2cfe38435050 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:41:07 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:41:08 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:41:09 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9e32cf3eae8c97676148171d71a3cc25149de87eecd89a137222b3b382cdf8f2`  
		Last Modified: Wed, 09 Mar 2022 23:42:13 GMT  
		Size: 6.5 MB (6510632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats-streaming@sha256:bf5f4238170d36fdc3b99a4ab8acea5c5755564d3d97131d48d0730dee33bbdc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110249474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68219116c19a9ac4e2603cd23ba4233e15f3ab67ba4a4e9169a2c000801679cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:21:44 GMT
RUN cmd /S /C #(nop) COPY file:2bdfa73d50ba6f64f600945ecab061708a66086f5dd80ec5e00ad93c8bf3b8b6 in C:\nats-streaming-server.exe 
# Wed, 09 Mar 2022 23:21:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Mar 2022 23:21:47 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128e56b52a1dd66549cb7830a9bc9f9352ab11829fe936a4bd03858ac830160`  
		Last Modified: Wed, 09 Mar 2022 23:22:35 GMT  
		Size: 7.2 MB (7190251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c581f41ddfe2959d4092845a36fa343eaddd42a160cd818cbca5c31671bff`  
		Last Modified: Wed, 09 Mar 2022 23:22:33 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ba79d16ae428589a386d36328db720a9ac0eb1abd0014da9992cb03cf4df1e`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c567d244b9f979dfa1c24fe471a72b7dc849619f91830d175ca5454f357a2eb`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
