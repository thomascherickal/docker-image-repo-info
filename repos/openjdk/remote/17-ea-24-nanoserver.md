## `openjdk:17-ea-24-nanoserver`

```console
$ docker pull openjdk@sha256:c4e7002aca24475f1012a99c8af4a41a825dc734b0f7f9b2184a797bb047f9eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `openjdk:17-ea-24-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull openjdk@sha256:d1a378d353abee5b2200f97cedacd91ccdc90e8b01c1062aa5aa1db068d06975
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.3 MB (286255888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43e57834537f51ec05e7d14bf6dca9c12e9cbbc1766636b53819cf540d68240d`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 16:42:56 GMT
SHELL [cmd /s /c]
# Wed, 12 May 2021 16:42:56 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 12 May 2021 16:42:57 GMT
USER ContainerAdministrator
# Wed, 12 May 2021 16:43:20 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 12 May 2021 16:43:21 GMT
USER ContainerUser
# Thu, 27 May 2021 23:19:00 GMT
ENV JAVA_VERSION=17-ea+24
# Thu, 27 May 2021 23:19:17 GMT
COPY dir:c3e819033741488ca95dfb326c175618f20ad013496a2e995353bd880bfd0e3e in C:\openjdk-17 
# Thu, 27 May 2021 23:19:53 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 27 May 2021 23:19:54 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ea91a7775c05d55a850a2983043468ce6ded7406743836cf8f33afb037aba1a8`  
		Last Modified: Wed, 12 May 2021 17:16:41 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0a5b4dd190af3527c02bb783babc5d88014a4de37555355c2f7a59dd21449`  
		Last Modified: Wed, 12 May 2021 17:16:40 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aab5fc14de7c93823ea1579b64e1e79017e9738a39e5d165aeed23c15bf7ffd`  
		Last Modified: Wed, 12 May 2021 17:16:40 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1954cb2ae96dfb0f537ce02738b91077c41cda7743ff097b99d8a6cfc74e211f`  
		Last Modified: Wed, 12 May 2021 17:16:40 GMT  
		Size: 69.5 KB (69533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95581d66523cc5b44afdfbd1f1e7732689ad5d73bf1c1352ef8f1e669dceede2`  
		Last Modified: Wed, 12 May 2021 17:16:37 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2cdacfde00690d31329197641d60f8cb583d83f61425323c6d8349db5fc776`  
		Last Modified: Thu, 27 May 2021 23:27:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cf9ea70716dd59ad8dfdd5465525dc9b18d96e40f518a6281d262a30713e92`  
		Last Modified: Thu, 27 May 2021 23:27:47 GMT  
		Size: 181.2 MB (181166860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5359f0b2faf06d364c7ef12d81a07e80dc7b1633fa28c384805c02aa732dfba4`  
		Last Modified: Thu, 27 May 2021 23:27:32 GMT  
		Size: 3.6 MB (3637359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6d3b2eb24195ae4a14622969cc3bac8820270ae6cc0efcc55b6a4e53e319de`  
		Last Modified: Thu, 27 May 2021 23:27:27 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
