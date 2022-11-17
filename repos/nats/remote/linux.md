## `nats:linux`

```console
$ docker pull nats@sha256:26a7092afff4cfbdd0fc17bd33dbf3308383876690a72fd95b009500d840dce2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:6fc6aee58f7a448bb3bbd803f3addfa0c9512b5083376ce20781b9b635c381cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4918825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974c838918842c11cbf59d7af83a073f753537c9d4b14f47231d3c1c7ba41c9e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:88cbf98679a4e287b67a701a1fb77e0e0928e75cc0e1e669916e033ecf774fdc in /nats-server 
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:21:46 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:21:46 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:21:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c8ce17c05ed27e7e08286a74c292d54eb2d5902af8f901dab4505ba83f7296f5`  
		Last Modified: Thu, 17 Nov 2022 20:22:33 GMT  
		Size: 4.9 MB (4918317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3d57c92f61ccff2db59e857c959bc11ca2ed1a6ca7f5494aa479c513196f7`  
		Last Modified: Thu, 17 Nov 2022 20:22:32 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:9e5158db138340db27aef59e820bafe7a09359e8910c2cef451b58348dd329ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c60a8afd73cd47b032a2d66e4968bf12f1aed52fee0f708cf184ef6c09b960`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:75f2ce97960bd08a17d41dd00b0f977ff54641b0f3d5b35f613c50553a59e8e1 in /nats-server 
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:49:49 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e27c576ee7d0df355bb5ab346016b3a399e8048fe3f938263b3b77e343d9243f`  
		Last Modified: Thu, 17 Nov 2022 20:51:22 GMT  
		Size: 4.7 MB (4682651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fb9f41d9d2c69e1f5737db95b3d0e754d24cd75bdd8d94a80166b8c97d6b6`  
		Last Modified: Thu, 17 Nov 2022 20:51:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:e4c874e4f9f5eafa49bdd7fed9a022da8958f69cc70e245af8bb9ebf7cad0c0c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc64213c48245d6c2d479e5be4d5043a6d811cb9d273ae36c8dfa157accbd04`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:ebca823a5dac00609e9fb9733528840572067b84b58dcccbe67a2df698f2869e in /nats-server 
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:58:06 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:58:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2c415cfba68b644bd88b057d832ff5015af29e04439812f5bd2e6873b3d7b8fd`  
		Last Modified: Thu, 17 Nov 2022 20:59:39 GMT  
		Size: 4.7 MB (4679272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875032eeefdff15b8e0c04ffba01805fa83a04cad983b8322b99f53b04e9c1fe`  
		Last Modified: Thu, 17 Nov 2022 20:59:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d5eefe444c9be5d4f08fd3ccf8277d186014689ef84ea0f59c59dc11acb4904
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ac0ab188af08ab1a9c049a3f6c349d0d2df9595cee8e6626c19a913526dcb2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:d11c7b340550df0716193331cacb3d06f2cb3b9971e90e006a9c153aaadc50f8 in /nats-server 
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:40:45 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:40:45 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:40:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3e01af3796e331721cc924f0d95499739cea560e1ac4bac35c11176033c94c8`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 4.5 MB (4503550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0b7a277e0d621acb2a17025b4318262de852c8be74070453c2f8c9983601ad`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
