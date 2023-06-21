## `openjdk:22-nanoserver-1809`

```console
$ docker pull openjdk@sha256:d8fa1237983ac6aa8b65b2e1ee7a44a67704b7e2987ecb0a54283abee9b63feb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `openjdk:22-nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull openjdk@sha256:bc92ecccb82f3ffc0f02989690667ba262f1f98ff8115e7efc4f2059601d82fa
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.0 MB (306965793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:764849f6176cfd3ec82317561ef11daaef59069022f1e30a24606a39dac9644e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:41:42 GMT
SHELL [cmd /s /c]
# Wed, 14 Jun 2023 20:28:06 GMT
ENV JAVA_HOME=C:\openjdk-22
# Wed, 14 Jun 2023 20:28:06 GMT
USER ContainerAdministrator
# Wed, 14 Jun 2023 20:28:15 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 14 Jun 2023 20:28:16 GMT
USER ContainerUser
# Wed, 21 Jun 2023 01:56:25 GMT
ENV JAVA_VERSION=22-ea+2
# Wed, 21 Jun 2023 01:56:42 GMT
COPY dir:6d9c714281a3c7e59d25d87792b8695c68bbf07943977649cc7d491f592a7088 in C:\openjdk-22 
# Wed, 21 Jun 2023 01:56:55 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 21 Jun 2023 01:56:56 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2364e413270ecc5b57d2596b092fb57b828229b59e810d9f345fc0d31ca535d`  
		Last Modified: Wed, 14 Jun 2023 18:26:46 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816e92368fa87f9798749d97162f386f464e5cb0e4a668b35ac6929b5f9bdbab`  
		Last Modified: Wed, 14 Jun 2023 20:35:15 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d241a7335cf0716c38d3ab576802c34648d69d25e847638aa7db2132e881461e`  
		Last Modified: Wed, 14 Jun 2023 20:35:16 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6d759053b47bb836ae8319abce7846d93cfdf210fb3e4b0bcce271fbda6d9e`  
		Last Modified: Wed, 14 Jun 2023 20:35:15 GMT  
		Size: 74.6 KB (74612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3005cad1749dc64b4a46eb5a441e05083078d3075dbdb1cac2beba0044199668`  
		Last Modified: Wed, 14 Jun 2023 20:35:13 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4274fb107daf9c5673d5e220fa0b2448d088d6b5f43595209064667f187ad4`  
		Last Modified: Wed, 21 Jun 2023 02:02:24 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11a12892c110e3382130bbc1f571af447967841445cf15a9f6824c164b77830`  
		Last Modified: Wed, 21 Jun 2023 02:02:45 GMT  
		Size: 198.7 MB (198710197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725b1cf517da1bc61d9e90a1a6f9c2c83266cd38e860499b8a0d28e079fd6ffb`  
		Last Modified: Wed, 21 Jun 2023 02:02:25 GMT  
		Size: 3.8 MB (3776615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04445c2f41aaf5ae6bb1dc7162f1f495604442bb8a02849166e11e322a7b7f0`  
		Last Modified: Wed, 21 Jun 2023 02:02:24 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
