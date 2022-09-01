## `openjdk:20-ea-nanoserver-1809`

```console
$ docker pull openjdk@sha256:4961bcb9400376914b6f960e7bc3412d57b5b08a6258410d85cf627a793a771f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `openjdk:20-ea-nanoserver-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull openjdk@sha256:6c5e62d308e0e14b1c6e11ae5bdcfc8bcc0a5ac9b5850b5497076a63ca56fb6b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.2 MB (299248969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:236a5acb4c7138200cf9bd4b354a0bc32e426d5272ce996ac8cb8284667953c8`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:57:07 GMT
SHELL [cmd /s /c]
# Wed, 10 Aug 2022 17:00:08 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 10 Aug 2022 17:00:09 GMT
USER ContainerAdministrator
# Wed, 10 Aug 2022 17:00:18 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 10 Aug 2022 17:00:18 GMT
USER ContainerUser
# Thu, 01 Sep 2022 22:18:18 GMT
ENV JAVA_VERSION=20-ea+13
# Thu, 01 Sep 2022 22:18:32 GMT
COPY dir:064abd947c77d5fa6cbcd7ad9b634d2cc59583d83d1fbed55bc633d87a0007c4 in C:\openjdk-20 
# Thu, 01 Sep 2022 22:18:54 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 01 Sep 2022 22:18:55 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0f4438539876006761cb687527bd8cb94cc7a273cf8bb47563981044f2e1771e`  
		Last Modified: Wed, 10 Aug 2022 16:38:40 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151c855f0d179e8547473b92e962fb22b468853448fe0849dadde3526c52aceb`  
		Last Modified: Wed, 10 Aug 2022 17:28:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3386f9f9687d0a909a16379459e37c52a2de2070297d81d4167037a0602e3e86`  
		Last Modified: Wed, 10 Aug 2022 17:28:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28092505f98fc516238306cba539a3a8a6d7f48ca19dc6e6c3cca668dc6f466c`  
		Last Modified: Wed, 10 Aug 2022 17:28:35 GMT  
		Size: 75.6 KB (75615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfea14a612ecceac1dd16eaa1da4863923aa41d796fd4f9c1fae46d918d4299`  
		Last Modified: Wed, 10 Aug 2022 17:28:33 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e8757b7576b94662db9f0251e488a9d5e1a9b760b0e9005f621447a1ca47ea`  
		Last Modified: Thu, 01 Sep 2022 22:22:32 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e2ff4768278f2c55ef0e7f712283a58049964c7bc89364606979996dd86c4d`  
		Last Modified: Thu, 01 Sep 2022 22:22:51 GMT  
		Size: 192.3 MB (192254501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa08b1d36ee065bd8dedb2e059bad505c094fb5135a992c7469645123ba2ae1`  
		Last Modified: Thu, 01 Sep 2022 22:22:33 GMT  
		Size: 3.7 MB (3707835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2211171eb2252087cce346231db5b33d4ca8ecdd5ccf2b7469005c4ce66645d`  
		Last Modified: Thu, 01 Sep 2022 22:22:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
