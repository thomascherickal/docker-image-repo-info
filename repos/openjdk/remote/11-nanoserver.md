## `openjdk:11-nanoserver`

```console
$ docker pull openjdk@sha256:aa85ab7f7a60955321a5a103bf900c5d01d147f3f99ff65e1249adbd8d6492bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `openjdk:11-nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull openjdk@sha256:c4f24f5e389645910073382e0adaa75c104561b98476f2c462b1cb296c25ca8e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.8 MB (293794480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d328ea4d2e41d547d5334592ad8940479aed765f227f68aeb475a3b6c28b1d8`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 18:17:55 GMT
SHELL [cmd /s /c]
# Thu, 14 Oct 2021 00:59:21 GMT
ENV JAVA_HOME=C:\openjdk-11
# Thu, 14 Oct 2021 00:59:22 GMT
USER ContainerAdministrator
# Thu, 14 Oct 2021 00:59:32 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Thu, 14 Oct 2021 00:59:32 GMT
USER ContainerUser
# Thu, 21 Oct 2021 23:27:05 GMT
ENV JAVA_VERSION=11.0.13
# Thu, 21 Oct 2021 23:27:27 GMT
COPY dir:f01eefe625ed2bb6eb89bcf5026bd8d3026198beb85b7d142c1a8700b8e43668 in C:\openjdk-11 
# Thu, 21 Oct 2021 23:27:59 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 21 Oct 2021 23:28:00 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ceff24c3c0c2c360cd3788fcde5c41e1d6601339f4944623c732558a6030e631`  
		Last Modified: Wed, 13 Oct 2021 19:12:58 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43342c8994cfe8e109320781e376005858ed6af7b5e15090c692a48ddee1c9d1`  
		Last Modified: Sat, 16 Oct 2021 00:48:14 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf3a714ac5c06b6ff3556dd1e4f015c50841a0819a87a526dcbdc6dbf295478`  
		Last Modified: Sat, 16 Oct 2021 00:48:14 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d5e43d0b80f79ad39e7b8a9d5f3b829595776b1abdf47c07fe87891d489583`  
		Last Modified: Sat, 16 Oct 2021 00:48:14 GMT  
		Size: 75.1 KB (75090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20aa72adc10eb6d0803d15b38f310dd050e3662bf077f683fea6ff85482f1a69`  
		Last Modified: Sat, 16 Oct 2021 00:48:12 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e6b5288ff0d6fb76adfaa52452f0fba92ab92936e6793b14e0264de7152a12`  
		Last Modified: Thu, 21 Oct 2021 23:48:54 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7739567a1fbcb4ddf3bef9d23385335f72ffcdeefe010feb56b73026615aa3d9`  
		Last Modified: Thu, 21 Oct 2021 23:52:25 GMT  
		Size: 191.0 MB (190994809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b60effc203016cf6e5322875be29de3c4e74600bb8e07a386c6d650ba4e0042`  
		Last Modified: Thu, 21 Oct 2021 23:48:54 GMT  
		Size: 56.3 KB (56334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce039dc6738b3288c03bb75f4d0abaa0a706fb74c789c8c3c4cbe53648116e1`  
		Last Modified: Thu, 21 Oct 2021 23:48:54 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
