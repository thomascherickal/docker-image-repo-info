## `notary:server`

```console
$ docker pull notary@sha256:b201c5d497d0d319f9125c198c848cab8556e92303e126bf0510daac8a8e1068
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:server` - linux; amd64

```console
$ docker pull notary@sha256:5fb572b42f869100019223e88bea7fdb970c99a7bed15d693ebcfb07c30c90d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5b2c7e4c0706a63ad53086ecdc0e2f950b225b49bf1f3807b8ed6080fc1b160`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 01:52:21 GMT
RUN RUN /bin/sh -c adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 01:52:21 GMT
RUN EXPOSE map[4443/tcp:{}]
# Tue, 25 Oct 2022 01:52:21 GMT
RUN ENV INSTALLDIR=/notary/server
# Tue, 25 Oct 2022 01:52:21 GMT
RUN ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 25 Oct 2022 01:52:21 GMT
RUN WORKDIR /notary/server
# Tue, 25 Oct 2022 01:52:41 GMT
RUN COPY /notary-server ./ # buildkit
# Tue, 25 Oct 2022 01:52:41 GMT
RUN RUN /bin/sh -c ./notary-server --version # buildkit
# Tue, 25 Oct 2022 01:52:41 GMT
RUN COPY ./server-config.json . # buildkit
# Tue, 25 Oct 2022 01:52:41 GMT
RUN COPY ./entrypoint.sh . # buildkit
# Tue, 25 Oct 2022 01:52:41 GMT
RUN USER notary
# Tue, 25 Oct 2022 01:52:41 GMT
RUN ENTRYPOINT ["entrypoint.sh"]
# Tue, 25 Oct 2022 01:52:41 GMT
RUN CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae0db85ee62912972b015b43b47b5849f5b66900a08ad146a42f7c16d02def`  
		Last Modified: Tue, 25 Oct 2022 01:53:00 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae714b9c46c68b869025bf262b5afec2bb7f99f3739cdae14e11604248f87fd`  
		Last Modified: Tue, 25 Oct 2022 01:52:58 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb5988268b5ce114ad501a67026ee4c7beaaa4ceb5e0caeecb1323f69081ee4`  
		Last Modified: Tue, 25 Oct 2022 01:52:59 GMT  
		Size: 5.1 MB (5143114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633a0f4a6583d329246e2cb77d177b072ad76c5d91fc75833979d5903902e3e2`  
		Last Modified: Tue, 25 Oct 2022 01:52:58 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85eadab3113f2431afe68461f05df57b0d365862172a791d600e30f47b8b849b`  
		Last Modified: Tue, 25 Oct 2022 01:52:58 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6232df1b1bcee75f7d4edb89236c13e7ef4d4359076262d966d77c33d5edd8`  
		Last Modified: Tue, 25 Oct 2022 01:52:58 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm variant v6

```console
$ docker pull notary@sha256:cd85f7c5e426f0dc5f13ec8da1c031f68b4075eaf15b74caec1ff04998f05ccf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7504111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abac8fc8e1787bc7a4d995a392a9e6c27b2d2703eb3d06421dedac9cbfba9ca0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 05:30:38 GMT
RUN RUN /bin/sh -c adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 05:30:38 GMT
RUN EXPOSE map[4443/tcp:{}]
# Tue, 25 Oct 2022 05:30:38 GMT
RUN ENV INSTALLDIR=/notary/server
# Tue, 25 Oct 2022 05:30:38 GMT
RUN ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 25 Oct 2022 05:30:38 GMT
RUN WORKDIR /notary/server
# Tue, 25 Oct 2022 05:31:03 GMT
RUN COPY /notary-server ./ # buildkit
# Tue, 25 Oct 2022 05:31:03 GMT
RUN RUN /bin/sh -c ./notary-server --version # buildkit
# Tue, 25 Oct 2022 05:31:03 GMT
RUN COPY ./server-config.json . # buildkit
# Tue, 25 Oct 2022 05:31:04 GMT
RUN COPY ./entrypoint.sh . # buildkit
# Tue, 25 Oct 2022 05:31:04 GMT
RUN USER notary
# Tue, 25 Oct 2022 05:31:04 GMT
RUN ENTRYPOINT ["entrypoint.sh"]
# Tue, 25 Oct 2022 05:31:04 GMT
RUN CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719245ee64918db6e14bc8a74787353276669a8486a5743651ec04a1872a4357`  
		Last Modified: Tue, 25 Oct 2022 05:31:43 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507f3b2412355e8361b78d3945186fcdf4be76d2e96b01137a4c3e9ee7a93ce0`  
		Last Modified: Tue, 25 Oct 2022 05:31:41 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6f25f398f550ff10d59e48ae2c5a5a2b6bf97d8a977ec91dde4c710dec3805`  
		Last Modified: Tue, 25 Oct 2022 05:31:42 GMT  
		Size: 4.9 MB (4887950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f5d829ac0b13d3052e233eed5e2d8fe792599aabf6ec130b4875e60db05ed3`  
		Last Modified: Tue, 25 Oct 2022 05:31:41 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ec865cd16045f97258edba5adce5b423c643a80391d42f06589d8f54a30fd6`  
		Last Modified: Tue, 25 Oct 2022 05:31:41 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe654f8a95498d4a4119b1b2f5438bff27408c96a5542674bdc8a90d0db00bd`  
		Last Modified: Tue, 25 Oct 2022 05:31:41 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:4be9b285b7046d696789a50897604d3d036a5e768d596f7da445329cb96f87c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7440931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80b24c2f22d4f982ab8d489bf1e6c80ef20065074fe2e52fd7348cdc088f00e1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 05:54:03 GMT
RUN RUN /bin/sh -c adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 05:54:03 GMT
RUN EXPOSE map[4443/tcp:{}]
# Tue, 25 Oct 2022 05:54:03 GMT
RUN ENV INSTALLDIR=/notary/server
# Tue, 25 Oct 2022 05:54:03 GMT
RUN ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 25 Oct 2022 05:54:03 GMT
RUN WORKDIR /notary/server
# Wed, 26 Oct 2022 18:53:13 GMT
RUN COPY /notary-server ./ # buildkit
# Wed, 26 Oct 2022 18:53:14 GMT
RUN RUN /bin/sh -c ./notary-server --version # buildkit
# Wed, 26 Oct 2022 18:53:14 GMT
RUN COPY ./server-config.json . # buildkit
# Wed, 26 Oct 2022 18:53:14 GMT
RUN COPY ./entrypoint.sh . # buildkit
# Wed, 26 Oct 2022 18:53:14 GMT
RUN USER notary
# Wed, 26 Oct 2022 18:53:14 GMT
RUN ENTRYPOINT ["entrypoint.sh"]
# Wed, 26 Oct 2022 18:53:14 GMT
RUN CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19c11ef8813c7c7e52078792213cc1951b797dfeda0933eb53237672542be0d`  
		Last Modified: Tue, 25 Oct 2022 05:54:34 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19eb1e9176b5da3983b2cb1e27af9a2fa727b656a122553479f995fbf2b46e1b`  
		Last Modified: Tue, 25 Oct 2022 05:54:31 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf5f5cf9f4e5f76615534e8e8f6f8624be20a801206af2a91ff0ecdba1ca38d`  
		Last Modified: Wed, 26 Oct 2022 18:53:31 GMT  
		Size: 4.7 MB (4731033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4762c84b839ac4befc019d732aedf85eaee520e460e6adaa4464f894d6a3624`  
		Last Modified: Wed, 26 Oct 2022 18:53:31 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:becae9fb2f07b10316a31f2254dc161d7f3d75dc56ac687e38d25851415e5623`  
		Last Modified: Wed, 26 Oct 2022 18:53:31 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfda209d0ca4589d64de82e5548f2f54d5e7d907dc719b25b1ab0792e75e1678`  
		Last Modified: Wed, 26 Oct 2022 18:53:31 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; 386

```console
$ docker pull notary@sha256:1d2ad1c6dda3d2829ee9fedbaa5aeab8960cfe932ab32bfa863dc5b6ff3e3158
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7753067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9b78e68ca88358074d9c7c068d76c543d5b9c33f113da1dc80e1bf34678b5b7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 02:33:41 GMT
RUN adduser -D -H -g "" notary
# Tue, 25 Oct 2022 02:33:42 GMT
EXPOSE 4443
# Tue, 25 Oct 2022 02:33:43 GMT
ENV INSTALLDIR=/notary/server
# Tue, 25 Oct 2022 02:33:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 25 Oct 2022 02:33:45 GMT
WORKDIR /notary/server
# Tue, 25 Oct 2022 02:33:47 GMT
COPY file:5d9f133868e3851315b5246c139c97b27b0946539c8682d4f17a932de9570b38 in ./ 
# Tue, 25 Oct 2022 02:33:47 GMT
RUN ./notary-server --version
# Tue, 25 Oct 2022 02:33:49 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Tue, 25 Oct 2022 02:33:50 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Tue, 25 Oct 2022 02:33:50 GMT
USER notary
# Tue, 25 Oct 2022 02:33:51 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 25 Oct 2022 02:33:52 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c692a1d61ff49f4083804ea05880254cdbf59904eff09aa2c9284e77eed914b`  
		Last Modified: Tue, 25 Oct 2022 02:34:26 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3d42d44a8b5ecb98b422ef1b15781ffa3f5b72a6f1f05f7de4c10f738d4e12`  
		Last Modified: Tue, 25 Oct 2022 02:34:26 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452aee5fe4cb441366a67c62f7c06a9ecad24ee5b667e6078e45a040ed6a621f`  
		Last Modified: Tue, 25 Oct 2022 02:34:27 GMT  
		Size: 4.9 MB (4943845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9c72b070bdd09f2a36d05929f75430d69f1be59b0f85dae40ecd13d77735a1`  
		Last Modified: Tue, 25 Oct 2022 02:34:26 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9d5265ea668e90ef9f056d5aa9ee3bdc71c0ac7ddfaa3f4ed3c4025bd5b10c`  
		Last Modified: Tue, 25 Oct 2022 02:34:26 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; ppc64le

```console
$ docker pull notary@sha256:8c9a5b585ca88a57b4efebdcc918f99ae7cb339e0e046a71e09daac41009157d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7438257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4703f54e37ce4a34b4be6bb22d78b4b6ba726321eef4f57192c273bdc497a0c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 03:23:54 GMT
RUN RUN /bin/sh -c adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 03:23:54 GMT
RUN EXPOSE map[4443/tcp:{}]
# Tue, 25 Oct 2022 03:23:54 GMT
RUN ENV INSTALLDIR=/notary/server
# Tue, 25 Oct 2022 03:23:54 GMT
RUN ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 25 Oct 2022 03:23:54 GMT
RUN WORKDIR /notary/server
# Tue, 25 Oct 2022 03:24:25 GMT
RUN COPY /notary-server ./ # buildkit
# Tue, 25 Oct 2022 03:24:25 GMT
RUN RUN /bin/sh -c ./notary-server --version # buildkit
# Tue, 25 Oct 2022 03:24:26 GMT
RUN COPY ./server-config.json . # buildkit
# Tue, 25 Oct 2022 03:24:26 GMT
RUN COPY ./entrypoint.sh . # buildkit
# Tue, 25 Oct 2022 03:24:26 GMT
RUN USER notary
# Tue, 25 Oct 2022 03:24:26 GMT
RUN ENTRYPOINT ["entrypoint.sh"]
# Tue, 25 Oct 2022 03:24:26 GMT
RUN CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28847305e982967909062e053ecacc81ae6035a3f7b3587b0e54677ab21f709c`  
		Last Modified: Tue, 25 Oct 2022 03:25:00 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7d5711e3906a11f7dc77d3091b7991f23e497d88cd28b0d987afae0a8d597f`  
		Last Modified: Tue, 25 Oct 2022 03:24:57 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128561de73e004acf02b2095c06b596e859870d8293b8f3908c13f03196a4cf9`  
		Last Modified: Tue, 25 Oct 2022 03:24:58 GMT  
		Size: 4.6 MB (4632709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b791f376b42ba52a136f5f76245ff6623bb9712d4040ea3ad31b3172cda963`  
		Last Modified: Tue, 25 Oct 2022 03:24:57 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9d0153d617a9657a348b5f81675bee3b1216cfd048580b1dd98ae2d0c8655d`  
		Last Modified: Tue, 25 Oct 2022 03:24:57 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80653d8d1f736570e499144190ec6c02820f55cb389b3a3ea1f16a3a0eb2ce31`  
		Last Modified: Tue, 25 Oct 2022 03:24:57 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; s390x

```console
$ docker pull notary@sha256:5f0d8363d713d58005c200e30235ebbad1efd30d126fa6e8b921bef23dc549f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7560845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fa0f87211b3a607ac91983abd06c400f17981935a09b074bcf4e6fa517d0a55`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 01:21:39 GMT
RUN RUN /bin/sh -c adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 01:21:39 GMT
RUN EXPOSE map[4443/tcp:{}]
# Tue, 25 Oct 2022 01:21:39 GMT
RUN ENV INSTALLDIR=/notary/server
# Tue, 25 Oct 2022 01:21:39 GMT
RUN ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 25 Oct 2022 01:21:39 GMT
RUN WORKDIR /notary/server
# Tue, 25 Oct 2022 01:22:02 GMT
RUN COPY /notary-server ./ # buildkit
# Tue, 25 Oct 2022 01:22:02 GMT
RUN RUN /bin/sh -c ./notary-server --version # buildkit
# Tue, 25 Oct 2022 01:22:02 GMT
RUN COPY ./server-config.json . # buildkit
# Tue, 25 Oct 2022 01:22:02 GMT
RUN COPY ./entrypoint.sh . # buildkit
# Tue, 25 Oct 2022 01:22:02 GMT
RUN USER notary
# Tue, 25 Oct 2022 01:22:02 GMT
RUN ENTRYPOINT ["entrypoint.sh"]
# Tue, 25 Oct 2022 01:22:02 GMT
RUN CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e57b7c2a2dbd108e38c96fd7b110170d3b57a921f34c3b015736a93b17e5ad`  
		Last Modified: Tue, 25 Oct 2022 01:22:34 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb73212e82f7d46920138e024d3233301bdffa778ba147338014ae69d65ba43c`  
		Last Modified: Tue, 25 Oct 2022 01:22:33 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6932c1633389acd33f1d9f659c505be3568406222966cef27e8ba12b8e99f2`  
		Last Modified: Tue, 25 Oct 2022 01:22:34 GMT  
		Size: 5.0 MB (4968022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8343a44b4f6777d4568e22ad69163d4b47cfd5210a1bd7d7b8299f0375980b1c`  
		Last Modified: Tue, 25 Oct 2022 01:22:33 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35439890b4d9dfb792c63c9afbed662ba45d800f8fd549997b8d5bd1952a4c86`  
		Last Modified: Tue, 25 Oct 2022 01:22:33 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9b2fbcdeb33d0cf5ed9e7962b4e280767c894054d34bc8e0de779a5f39e634`  
		Last Modified: Tue, 25 Oct 2022 01:22:33 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
