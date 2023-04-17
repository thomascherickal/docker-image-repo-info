## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:22004a7ecb45dc07b6511629748e9178246378a6b013f7a037e8fb4022544932
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:1a8745712d00a54265c8552863b8d15a568b138368f4fcb090c075e361124c14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a48bccf54f8248bddd0509da6d1cc1fe8b97638f6120c98e4c9fb191f6f1723`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:31:40 GMT
COPY file:379a895964ce5e0c1d6e137ee5ee8f0cbfb7fdbb8cb20ace28a5de2e106737eb in /nats-streaming-server 
# Thu, 12 Jan 2023 19:31:40 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:31:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:31:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:27e278d5ae53768a5d47168e25eb6824c8445f2866af5ea11943739d93ce14dd`  
		Last Modified: Thu, 12 Jan 2023 19:32:24 GMT  
		Size: 7.7 MB (7666171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:4e885fec2085aaed30489d10934af3b0b4166d8f8c839d7026b4edf2b8c79716
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7201921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad0b6cc06f140648f388a6e9366a026925dc2bd02d37897824abb681755774f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 17 Apr 2023 21:59:05 GMT
COPY file:3255864650458d4de1b6cf5163bf31d1a443358d07fd422dbee0573fefbfa26d in /nats-streaming-server 
# Mon, 17 Apr 2023 21:59:05 GMT
EXPOSE 4222 8222
# Mon, 17 Apr 2023 21:59:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 17 Apr 2023 21:59:06 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7738682950a04fadd9a82a6d85ff413291b711a3dd1cd63eebf7044be2e16243`  
		Last Modified: Mon, 17 Apr 2023 21:59:35 GMT  
		Size: 7.2 MB (7201921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:bcefecfcb6986469865e3d3d3fbb31f8101c56a77b76a3c3cb076ae08ab06ae8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7318728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6202a592a6aad13e30bce4ac90570fe13d8f28740d9ca9b75958c204953b43bd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 19:25:37 GMT
COPY file:58653f0fa67e6667e5ec024a8b7912bc01a12570dac2c7550d04c2e617252bf1 in /nats-streaming-server 
# Wed, 29 Mar 2023 19:25:37 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:25:37 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 29 Mar 2023 19:25:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:edc8f5310312ee44896e1639c9af8d17c77c9fc7cfad03f8c1268ab57def8348`  
		Last Modified: Thu, 12 Jan 2023 19:12:45 GMT  
		Size: 7.3 MB (7318728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:56dfb1bed3b56ea0b72be1b79a49422abdde1189777ebfb55eda7223819eb6d3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7019428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7533789a178d97f2445ccdb62e46c98a1cec7249342ad21b5c40f38ee0652bff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:49:56 GMT
COPY file:33b7386a5076cd63bc03cf5c4de0f89afe8fd8034e8fd3a792715c6cb567514b in /nats-streaming-server 
# Thu, 12 Jan 2023 19:49:56 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:49:56 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7cbef42b1eb11c382f636b05c7fea54926364454d6b2727ea8e52f63785a536`  
		Last Modified: Thu, 12 Jan 2023 19:50:42 GMT  
		Size: 7.0 MB (7019428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
