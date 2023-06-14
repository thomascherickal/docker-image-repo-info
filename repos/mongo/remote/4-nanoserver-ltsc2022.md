## `mongo:4-nanoserver-ltsc2022`

```console
$ docker pull mongo@sha256:fd0fd85d970efecba26ac313d43568e974c7bad4085b7f6e99364b8c55bce80b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `mongo:4-nanoserver-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull mongo@sha256:f4b5e1ec786a26c1c0ed7cf6376fd176d499f436263a2381a65578332f7de66d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.5 MB (365477648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a960b6fc56a4b50171e5550f5b04fd82bc8e3afca411c4d46e72a7099aec9cd3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 08 Jun 2023 12:38:25 GMT
RUN Apply image 10.0.20348.1787
# Wed, 14 Jun 2023 18:50:26 GMT
SHELL [cmd /S /C]
# Wed, 14 Jun 2023 19:21:55 GMT
USER ContainerAdministrator
# Wed, 14 Jun 2023 19:22:11 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 14 Jun 2023 19:22:11 GMT
USER ContainerUser
# Wed, 14 Jun 2023 19:36:33 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Wed, 14 Jun 2023 19:41:31 GMT
ENV MONGO_VERSION=4.4.22
# Wed, 14 Jun 2023 19:41:53 GMT
COPY dir:ba7da3b127dd995e6b5f5a8e9cc5f87caa3174d8a03e6b82fdeaa7d4f4b54ce8 in C:\mongodb 
# Wed, 14 Jun 2023 19:42:05 GMT
RUN mongo --version && mongod --version
# Wed, 14 Jun 2023 19:42:06 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Jun 2023 19:42:06 GMT
EXPOSE 27017
# Wed, 14 Jun 2023 19:42:07 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:f94f5e4cef3f52c830328b87b7298c638fa9ef22a0babf737eda2a2dd6d024c4`  
		Last Modified: Tue, 13 Jun 2023 20:05:48 GMT  
		Size: 120.0 MB (120028549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf26306b7c3ea55d7d8bb15ad1c70de776773883ccc3ce02d9cfac7a8177ccf8`  
		Last Modified: Wed, 14 Jun 2023 19:09:48 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea973e1d3f627a7f78f5f09ff4e4cbe54950ad931a8ac9f6b91800c3f870662`  
		Last Modified: Wed, 14 Jun 2023 19:53:21 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a05d3662d1253cfbf06530db11bb819751c1f3b989def94c06313f77ef96d3`  
		Last Modified: Wed, 14 Jun 2023 19:53:19 GMT  
		Size: 74.0 KB (74005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17495be05e5c0ea68148077f81896256940de4ab199038e806fc1c968454aba1`  
		Last Modified: Wed, 14 Jun 2023 19:53:19 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928b0458fff3f4ca356b373189883b0866063ad5999aefd5b8ca98f443218450`  
		Last Modified: Wed, 14 Jun 2023 20:05:18 GMT  
		Size: 263.4 KB (263405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d44eb987ecaf15fc59769dad7694100d3d72018a0134c19fccef4ab9f7379f3`  
		Last Modified: Wed, 14 Jun 2023 20:09:28 GMT  
		Size: 1.1 KB (1057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866d7584a56e79dff5a1f07a158631b62fbdbb5553c46631695b4650d454570c`  
		Last Modified: Wed, 14 Jun 2023 20:10:10 GMT  
		Size: 245.0 MB (245042964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4bb7b3e16c325ce5bcc1e55b93bd90b59d4e61c1c902f9cbe0c491bd7606c4`  
		Last Modified: Wed, 14 Jun 2023 20:09:26 GMT  
		Size: 61.2 KB (61209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d33d2fd9f3e1da2441ab00b56f267e15a4629828599abd4d2b463affac2aa7d`  
		Last Modified: Wed, 14 Jun 2023 20:09:26 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927672de6c8a25a64ac9cb321f573fe2375cbb56cc8ea5622695cc52db2452e6`  
		Last Modified: Wed, 14 Jun 2023 20:09:26 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ef6ba1fd8b3633a92cbfc376493078306ff7ae234f7290734731b0227b08b5`  
		Last Modified: Wed, 14 Jun 2023 20:09:26 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
