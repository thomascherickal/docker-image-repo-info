## `nats:latest`

```console
$ docker pull nats@sha256:c3e75f817f347640bbfd05d134f47a0a04fe0df86265985e5e4ee9f5fbe72010
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:684baaa35e7d8a0a37f5e62ff68dd3c3ddf62a523392a7b00f5b2440620681a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a518b2e63bf6fd16443c123d65a0a15f3860ba0601b9d8640ab7e3cef2a64f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 02:03:48 GMT
COPY file:1099ac4333f9709bdb701d77f49a9e3dfc443f1986fbf71cf0622f44b130cee0 in /nats-server 
# Thu, 05 Aug 2021 02:03:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 02:03:49 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 02:03:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 02:03:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95139cea5d13d0e375a0e733a39d4f87cf133a9b2c8b9baf4cced90467ce4bbd`  
		Last Modified: Thu, 05 Aug 2021 02:06:14 GMT  
		Size: 4.2 MB (4174321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3970e4d2766394cc6ac0abee7ea43c436a324c9033b31b4116287a025feab571`  
		Last Modified: Thu, 05 Aug 2021 02:06:11 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:730384625ce5b4079ddcac6880f1490ee9597ae6bc21828aaa77fa16532f5c0b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107312800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cc7723929ee86cd0b079266209ee6d5a7b6868ab2ccb6c25353fe3c894572a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:07:57 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Wed, 25 Aug 2021 16:07:58 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:08:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121849591f6022d5eb46ce6c232c4dd82c98ce40d0141bce3f4fd492ca1c7a59`  
		Last Modified: Wed, 25 Aug 2021 16:11:22 GMT  
		Size: 4.6 MB (4565853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ee09fe8225a9ce0552a9e934917caed425dfd666edee7135321ace67b098b4`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba323a5abf6dad7d1a718aa3170520980aa1fbd31c381d54cc7471102fb2d915`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7e3410faa2bff42c96e80f70ded6c98662c693d5110b30b9e8ea8e4d6323ba`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a3a7ef27ca50d4664393cf2b8e76b982f1169704081f714d56003e9fae41cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
