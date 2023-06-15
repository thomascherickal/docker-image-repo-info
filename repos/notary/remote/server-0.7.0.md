## `notary:server-0.7.0`

```console
$ docker pull notary@sha256:dd038cc58c0cb2ab6178880a5ee4e9cbd34c7acbd689fa9859121eb856027f57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:server-0.7.0` - linux; amd64

```console
$ docker pull notary@sha256:0d22b3ab283d7f5bcb192eeca5b6c23dda524157086d9e2c5d4d941e609279ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7957732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b728fde414ad94a52862cf23bc0cc6b35ac0d63dda5511fae249f74b36fe737`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4443/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-server ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-server --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./server-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006de58a565eab12a85c007364709b9c3158a5cbe003d17c9c062ee51475613b`  
		Last Modified: Thu, 15 Jun 2023 05:47:42 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2ec587a5759864fc13b2e7450cf598303cecf104e8f293ec1e55babfc26db2`  
		Last Modified: Thu, 15 Jun 2023 05:47:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cfce3badea30b8735aa4542e1931c9506417a32bb385630a56d4946b40a890`  
		Last Modified: Thu, 15 Jun 2023 05:47:40 GMT  
		Size: 5.1 MB (5147840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431ae8a3fcd9bef0edea649363bdab23d1f043b54e88d7e74c10f478d1fe9034`  
		Last Modified: Thu, 15 Jun 2023 05:47:39 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e793247138b5cd0ebd5e2aa37ea21151c1a822d5b7c6b31022e0e7add2f118`  
		Last Modified: Thu, 15 Jun 2023 05:47:39 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d523bb7866745ebf0b5dd24ced08363c6c6000028945591072802211694ceb`  
		Last Modified: Thu, 15 Jun 2023 05:47:40 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; arm variant v6

```console
$ docker pull notary@sha256:449c89eee37b082013c6846cc531711c3e4e2d77a7ad7e0d136da30bc7ff0767
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7511373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f389c9336e8801ef6cd83cab750eb3363c7dee34086865188f949ddd4b0883f7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:28 GMT
ADD file:41a85835978e4acba9d92833f0d5e20084da50779e52d8832d576b003a7aa1bb in / 
# Wed, 14 Jun 2023 18:49:29 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4443/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-server ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-server --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./server-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:053f9b31dd2e619ba14dc3733515fcd65e92851f612b94453db88ea1d27ab0ea`  
		Last Modified: Wed, 14 Jun 2023 18:50:10 GMT  
		Size: 2.6 MB (2615570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8b1ea8ec24955304373c42ddad13462ec8177200b715cdae1220f4372b27ae`  
		Last Modified: Thu, 15 Jun 2023 00:03:34 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d8bfd5064c36b13e7990e5b4d4034b9248ab5e803f32073ba3dec6ee678899`  
		Last Modified: Thu, 15 Jun 2023 00:03:32 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa4735db51b68a16da59724f275087f706e1dc85f98b756e77012beb7e7f1c7`  
		Last Modified: Thu, 15 Jun 2023 00:03:33 GMT  
		Size: 4.9 MB (4893576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1544046379bafd9f16c386e348572696174a7e5de3d39cb1dbe0513f4c2590d`  
		Last Modified: Thu, 15 Jun 2023 00:03:32 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0afcf911966e6028390980e4519af147da9b40f87540a11229bfa15618e2fad`  
		Last Modified: Thu, 15 Jun 2023 00:03:32 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8225d1b24b673d04afdf4f3d8affeb8bbaaffd894f9b119a035c3145c40930eb`  
		Last Modified: Thu, 15 Jun 2023 00:03:32 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:e477b0c3162ca645b8aeac5983bb96f5cd95e9617c66ee23a190b9e3626dea89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7444590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:988ebdf8bae58a74eddc8ed4986a4ab9e74884ed8a0de07a7060a93e7f7e73c3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4443/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-server ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-server --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./server-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a70fe37c8d33b219ba725d1903a536b2d54bd47305e1c9d9a969b379ece36`  
		Last Modified: Thu, 15 Jun 2023 03:04:58 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a034e17957ae3c49bb611a8be82f0a3471bf7c65d72c9a3222f117b057f486`  
		Last Modified: Thu, 15 Jun 2023 03:04:56 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a624c4a09b1e59b84d684f8415dcdf778395842b4feb9b5cf5417203e2ceef`  
		Last Modified: Thu, 15 Jun 2023 03:04:57 GMT  
		Size: 4.7 MB (4734457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593363fb96cc338299b1dfada96ecd19bb7cc3768d1247ebfe8ccf8dcac7e9bb`  
		Last Modified: Thu, 15 Jun 2023 03:04:57 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f9b840c78778ec16ae9c0775d99005e75fb2be7e630f8c52b4bf59c4fa1271`  
		Last Modified: Thu, 15 Jun 2023 03:04:56 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f92033697d8ecc6b52f80f9f56c2f981021c9949fca2c8c5f934f7479b8c4a`  
		Last Modified: Thu, 15 Jun 2023 03:04:56 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; 386

```console
$ docker pull notary@sha256:84eb0aab5ebee3bcfc1c24256c4e35cc37ef2b02c5641ad1dd9ed0a858444fe2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7763585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a146d79703d434557631c112bab99daa6d907f489ac521d21d58e4002aa50f84`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:30 GMT
ADD file:9b22a3b9a2009266eccfbbf15fbc348f6c854a6c496df29e5c4f0a832b796c67 in / 
# Wed, 14 Jun 2023 22:33:30 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4443/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-server ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-server --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./server-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:ca79a18e143c0859a7d07fda202e645a6564d97bbda6a486c576b234535bda07`  
		Last Modified: Wed, 14 Jun 2023 22:34:09 GMT  
		Size: 2.8 MB (2810568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a41c79ffa0a1ed1ad6af485640f3cedcf7b3926deb902b5424bee397e0fac9`  
		Last Modified: Thu, 15 Jun 2023 03:36:32 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0648edf28f959e77ec50d12972b003ebae06abfd7df1bb236d303cdb7a4a6918`  
		Last Modified: Thu, 15 Jun 2023 03:36:30 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca61c39639a94e641c6fc58ce98880a5ece9acc2495d8e15f8fa1ed939200d7`  
		Last Modified: Thu, 15 Jun 2023 03:36:32 GMT  
		Size: 5.0 MB (4950789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dddef864f09b4749199f9753648d1c4281d43c5ffd5a431e4a7f319a3149177`  
		Last Modified: Thu, 15 Jun 2023 03:36:30 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b57badf1629b0aa0aa66af4a18ba8f7c87d6e89a9e34e77ed33cfba69de3969`  
		Last Modified: Thu, 15 Jun 2023 03:36:30 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e0b2ed17860f50516c620b3281c1f6dd402a01915bc6e153252046bcf1344d`  
		Last Modified: Thu, 15 Jun 2023 03:36:30 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; ppc64le

```console
$ docker pull notary@sha256:ce0b67e544a88c87ad1f824441dcaa583562d3de4313ab3e048c2a128da7134d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7443646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78ea24582f74966e81fb8a183e96a95a172c1ec23e4fc0f502ee10575801346f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Thu, 15 Jun 2023 00:40:03 GMT
ADD file:687ce61613e63c93be9debda827167f433a51769ad625312ea1250ee87b62f30 in / 
# Thu, 15 Jun 2023 00:40:03 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4443/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-server ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-server --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./server-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:a2010c6a5435acd9b63d7f294696ba1d313d4393be0848195e1e655583ca50af`  
		Last Modified: Thu, 15 Jun 2023 00:40:48 GMT  
		Size: 2.8 MB (2802263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae01cf59efaf0a10f9728f0d6f10af743f74c6440f154139a12f2d2449f7fce`  
		Last Modified: Thu, 15 Jun 2023 05:17:42 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009021b9d40b0bb461550370b9421d57e94763920238325a8c6157caf5c73e23`  
		Last Modified: Thu, 15 Jun 2023 05:17:39 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89dacd8d489d6acbe4b5c8e18ec68c964d128e38522000fd94d823a64a250ee`  
		Last Modified: Thu, 15 Jun 2023 05:17:41 GMT  
		Size: 4.6 MB (4639154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a5c1f9ba1362d33ba089b83cb1ce7aadbefb2f2f0763cca56d8097065100df`  
		Last Modified: Thu, 15 Jun 2023 05:17:39 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ea7f6433ab8a50a77ea8880a7a040385baf78d2b7e9164975c7e97357bce41`  
		Last Modified: Thu, 15 Jun 2023 05:17:39 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6526c495e5182922d044f4346da94939eccea5c2525ddb6de6673ea3dd8498f8`  
		Last Modified: Thu, 15 Jun 2023 05:17:39 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; s390x

```console
$ docker pull notary@sha256:46222102af49c089bdd985dc3a9c9e396e4132f7472daf8bbc8c0948eaaedde0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7572110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc73865af693435b5f688b2cefee44b2d4bf02679a776101a457ed1d85949b8`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 18:45:37 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 02 May 2023 18:45:37 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 02 May 2023 18:45:37 GMT
ENV INSTALLDIR=/notary/server
# Tue, 02 May 2023 18:45:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 02 May 2023 18:45:37 GMT
WORKDIR /notary/server
# Tue, 02 May 2023 18:45:37 GMT
COPY /notary-server ./ # buildkit
# Tue, 02 May 2023 18:45:37 GMT
RUN ./notary-server --version # buildkit
# Tue, 02 May 2023 18:45:37 GMT
COPY ./server-config.json . # buildkit
# Tue, 02 May 2023 18:45:37 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 02 May 2023 18:45:37 GMT
USER notary
# Tue, 02 May 2023 18:45:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 02 May 2023 18:45:37 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d718f433f226a10233b1c2fd202d613455bab7210ecab0e649f578786e27cc7`  
		Last Modified: Tue, 02 May 2023 19:14:49 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1be685ead59433921acfa36285b0d513c970b7e82ab7594887f7bdd7ae37527`  
		Last Modified: Tue, 02 May 2023 19:14:48 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ab63e1bbe686eb9921ae2cc757a2f3a08a4f9ca3ff21a92c5e585ff02419a8`  
		Last Modified: Tue, 02 May 2023 19:14:49 GMT  
		Size: 5.0 MB (4976490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c85d7ee22e60d478fbf8ea9d90ea62a303179efb20bdc85955876a100ffb6b`  
		Last Modified: Tue, 02 May 2023 19:14:48 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c832954401746d66fbcb12d064382b41ae4fec14f65e876b184628387f802604`  
		Last Modified: Tue, 02 May 2023 19:14:48 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb44149a8d8cccb958cf42b938950bc2199a6db43ff94dd7a1f10585d896467`  
		Last Modified: Tue, 02 May 2023 19:14:48 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
