## `mongo:4-nanoserver`

```console
$ docker pull mongo@sha256:7bcef2b09c748eaed28be9703b9130d3d3583d57bb023eac25901ab812bf2737
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1668; amd64
	-	windows version 10.0.17763.4252; amd64

### `mongo:4-nanoserver` - windows version 10.0.20348.1668; amd64

```console
$ docker pull mongo@sha256:98bb12614949371eeaa0d7d8a41704285eb17af0c66a2c868fac35e89148c217
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.8 MB (367764223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd8e1538248a091b41ce19866f77798be91c0c392866990af674a23966e1284`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:16 GMT
RUN Apply image 10.0.20348.1668
# Wed, 12 Apr 2023 00:22:09 GMT
SHELL [cmd /S /C]
# Wed, 12 Apr 2023 00:22:09 GMT
USER ContainerAdministrator
# Wed, 12 Apr 2023 00:22:24 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 12 Apr 2023 00:22:25 GMT
USER ContainerUser
# Wed, 12 Apr 2023 00:30:22 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Wed, 26 Apr 2023 20:24:58 GMT
ENV MONGO_VERSION=4.4.21
# Wed, 26 Apr 2023 20:25:18 GMT
COPY dir:8ba32aff2ca9d923768f5236ed254b74cf5dce4d9a2947fd8bbd311a3e350b3d in C:\mongodb 
# Wed, 26 Apr 2023 20:25:30 GMT
RUN mongo --version && mongod --version
# Wed, 26 Apr 2023 20:25:30 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 26 Apr 2023 20:25:31 GMT
EXPOSE 27017
# Wed, 26 Apr 2023 20:25:32 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:e06b772d586b58466a653b72002aee7c59496110e9ae402ff58f026e44452506`  
		Last Modified: Wed, 12 Apr 2023 02:34:14 GMT  
		Size: 122.3 MB (122328782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329579f5fc95fa89293545a20f4e45221db45261002e7012b86c4d3233edd1f8`  
		Last Modified: Wed, 12 Apr 2023 02:33:39 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ffee768115c8d7d69b2fd027383a36010ef0fdee82af33f03b9d4cd96300e0`  
		Last Modified: Wed, 12 Apr 2023 07:24:29 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b01eaee96d583c766fda2075c2b3f0d0ecbaae5f80349e49fd0231ded90b88c`  
		Last Modified: Wed, 12 Apr 2023 07:24:27 GMT  
		Size: 87.9 KB (87861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8632bd61e3a0f1116d090e2b6cafc76d6bb3c3b5cf14ac1fc393c94e4a1bc6`  
		Last Modified: Wed, 12 Apr 2023 07:24:27 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec487c1ab7e5a979f4fbd7e80f7bb8436646e0494b27aceb9005ca7e57dbba4`  
		Last Modified: Wed, 12 Apr 2023 07:29:50 GMT  
		Size: 263.5 KB (263515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efce86fd33351317c5ae336a1dcaefc84de40792d713a296c385a109e7101cf`  
		Last Modified: Wed, 26 Apr 2023 20:34:22 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03945120e668fc3b9d99470dddcfb8a772b39d353ee96a9426000d279a288e2`  
		Last Modified: Wed, 26 Apr 2023 20:35:01 GMT  
		Size: 245.0 MB (245025790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587a683f1a68b7339dc1edae7cccc5f380e2e71a3820f0e5548288537678ec7c`  
		Last Modified: Wed, 26 Apr 2023 20:34:20 GMT  
		Size: 50.1 KB (50120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9bb57ccff800434412ac235d740f49b96c2f3f6f2b8498bac8154c3c21b02b`  
		Last Modified: Wed, 26 Apr 2023 20:34:20 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961ec9a728d48e83db07bcf1a32d434b171fa045b73c838222918ac55b0b8cdc`  
		Last Modified: Wed, 26 Apr 2023 20:34:20 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e69742cf36f085bb74f3912c413e14d2ab15264292a8995595facca668595c`  
		Last Modified: Wed, 26 Apr 2023 20:34:20 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-nanoserver` - windows version 10.0.17763.4252; amd64

```console
$ docker pull mongo@sha256:a22f29a0f45ede5b534e6d8e9ccb11264da0c4c3e5c850e94ffd73a1420e05e3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.2 MB (352235899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8fb64f14eba43c8ef194817d46e1a1f953ea00895aeeb0f0fc20156edc7202b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 00:23:53 GMT
SHELL [cmd /S /C]
# Wed, 12 Apr 2023 00:23:54 GMT
USER ContainerAdministrator
# Wed, 12 Apr 2023 00:24:05 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 12 Apr 2023 00:24:06 GMT
USER ContainerUser
# Wed, 12 Apr 2023 00:31:26 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Wed, 26 Apr 2023 20:25:42 GMT
ENV MONGO_VERSION=4.4.21
# Wed, 26 Apr 2023 20:26:02 GMT
COPY dir:8ba32aff2ca9d923768f5236ed254b74cf5dce4d9a2947fd8bbd311a3e350b3d in C:\mongodb 
# Wed, 26 Apr 2023 20:26:14 GMT
RUN mongo --version && mongod --version
# Wed, 26 Apr 2023 20:26:14 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 26 Apr 2023 20:26:15 GMT
EXPOSE 27017
# Wed, 26 Apr 2023 20:26:16 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e9c90f3a763714533d4a634f7ab3d23374e5208e2ac8bae4288243917bd972`  
		Last Modified: Wed, 12 Apr 2023 02:34:36 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6552b5bd1c6568d6f39240a39a0344d31519e6acaf2437760d33a2f1bd16ebb4`  
		Last Modified: Wed, 12 Apr 2023 07:26:01 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb24d44a5b22599181c1f6c9ebdf5458cb1fc58facdffff33b51e656ba5a14b`  
		Last Modified: Wed, 12 Apr 2023 07:25:59 GMT  
		Size: 68.8 KB (68801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61d7e4579b59b23268c08766daece41ab2483fa4867cc1a017edcfc07642639`  
		Last Modified: Wed, 12 Apr 2023 07:25:59 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f852ca225da877b3fd9632d1eaf590255b257c97045bc7165d49cc5d006e62`  
		Last Modified: Wed, 12 Apr 2023 07:31:00 GMT  
		Size: 263.4 KB (263379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45a728f33875b87ec5f0473cef780968bf4e4017fb38bd3f1de9bfa0a8aaf81`  
		Last Modified: Wed, 26 Apr 2023 20:35:15 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752732bd7e65c1f3d1ab87cbd118d2e502fa17e17a7dd4767f3faa511f2fe783`  
		Last Modified: Wed, 26 Apr 2023 20:35:54 GMT  
		Size: 245.0 MB (245025883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8430e8bbc629497cf9a8d1e412f8f01e16e37b55853f131509e6c89160460a`  
		Last Modified: Wed, 26 Apr 2023 20:35:13 GMT  
		Size: 80.8 KB (80776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2124ff5d80fb7f13a2f419e1bf99b5b5937f546261b983293a3dc7f07a0d02ee`  
		Last Modified: Wed, 26 Apr 2023 20:35:13 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaddd0ca68d93e7860624333e090b32f03de753384c32e164f1bae1aad4efdb`  
		Last Modified: Wed, 26 Apr 2023 20:35:13 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276d40722a8ed5ff3c7f0daf8591b0ac109b4cfc3152f4363acf8969005649f4`  
		Last Modified: Wed, 26 Apr 2023 20:35:13 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
