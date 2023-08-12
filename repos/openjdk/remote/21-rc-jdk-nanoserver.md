## `openjdk:21-rc-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:0bc928ae2a742a54b12103fbaf0fcc0cf73f9cf4beec083c76de631c7a37c147
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `openjdk:21-rc-jdk-nanoserver` - windows version 10.0.17763.4737; amd64

```console
$ docker pull openjdk@sha256:84a8302ad563a96e8411ed5a0df4063af44ab5d5036764473c2e0ca734e7b10b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.4 MB (306385388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76bb3a969d180203474040f95973b65e26168db3bc4c071cb8d9d454f2071347`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Wed, 09 Aug 2023 23:39:50 GMT
SHELL [cmd /s /c]
# Thu, 10 Aug 2023 02:47:12 GMT
ENV JAVA_HOME=C:\openjdk-21
# Thu, 10 Aug 2023 02:47:13 GMT
USER ContainerAdministrator
# Thu, 10 Aug 2023 02:47:23 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Thu, 10 Aug 2023 02:47:23 GMT
USER ContainerUser
# Sat, 12 Aug 2023 00:06:50 GMT
ENV JAVA_VERSION=21
# Sat, 12 Aug 2023 00:07:06 GMT
COPY dir:ab44a5695be5306db50e482755419b90c734a5e54efb6807b2ffc8de111bd777 in C:\openjdk-21 
# Sat, 12 Aug 2023 00:07:19 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 12 Aug 2023 00:07:19 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7e08c5247c8c7d832882da17ac85015e9dd4d4dfc9e4114fc14746eb2abded`  
		Last Modified: Thu, 10 Aug 2023 00:21:01 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3434ed9deffc375ad0cb38e443dc5fc1360d844968c96f2b511ba8ea8d59c0f4`  
		Last Modified: Thu, 10 Aug 2023 02:52:12 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54f8430a84d34adc8f8adefa5c8bdf90fee0c09900855cd07da50d6010c2fec`  
		Last Modified: Thu, 10 Aug 2023 02:52:12 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a23bc62e51ea7bc2fecb15f3693ab4a41cbdcc4acfebd18e8dd6c5f5ce9c9ea`  
		Last Modified: Thu, 10 Aug 2023 02:52:12 GMT  
		Size: 69.7 KB (69701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520aa82f2ac0e8998feb41298f7ff989a63d8da7cdea2c2e926533fe6db48c20`  
		Last Modified: Thu, 10 Aug 2023 02:52:10 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9615a8f5f09203a44f3eac9d2977adabd335a94702ab5bc654443a5787befbd8`  
		Last Modified: Sat, 12 Aug 2023 00:11:53 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1946a2ed775970d81c34d907253e3f035da2edbc9dfb848d3efa713e4a43d33`  
		Last Modified: Sat, 12 Aug 2023 00:12:14 GMT  
		Size: 198.0 MB (198033413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fd44cddc836fe402da977c24ae41acd047512b63323642b98731778760fa37`  
		Last Modified: Sat, 12 Aug 2023 00:11:54 GMT  
		Size: 3.8 MB (3816199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c651e7547ab96105f268c30256e311a1ecdf00b9f789c69ec99ea626db0e87e`  
		Last Modified: Sat, 12 Aug 2023 00:11:53 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
