## `openjdk:17-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:6a284f8a401a3af3ab4ad3a9e4d96050bfd42773e693dd8c452345406f5c6595
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `openjdk:17-jdk-nanoserver-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull openjdk@sha256:90db48446653883a5b281242305d2887a0f05fe7eafb75a1b9b44e369c2f5e87
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.0 MB (286037086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b0260996f8acf0930fe388f0cfb3708079769119ee4015f4ff7757fa2b682d1`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:53:40 GMT
SHELL [cmd /s /c]
# Wed, 14 Apr 2021 16:53:41 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 14 Apr 2021 16:53:42 GMT
USER ContainerAdministrator
# Wed, 14 Apr 2021 16:54:02 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 14 Apr 2021 16:54:03 GMT
USER ContainerUser
# Mon, 10 May 2021 23:31:40 GMT
ENV JAVA_VERSION=17-ea+21
# Mon, 10 May 2021 23:31:58 GMT
COPY dir:cfac9f56777a5d91e0879764fa534bb67fcf5d706baf09e8f4a88eedb9974a0b in C:\openjdk-17 
# Mon, 10 May 2021 23:32:39 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Mon, 10 May 2021 23:32:40 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c2c727299531adc7c2aacb1f062d72fd42cec96a0d235b3e5b0afe03e9ddbc7d`  
		Last Modified: Wed, 14 Apr 2021 17:41:13 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4846a68a532c85058f47e1e9b777bab26eb5ad132cdeb3d646bc51d43346f1f8`  
		Last Modified: Wed, 14 Apr 2021 17:41:12 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dede727741920ec94cb8aac2b231667fd531dbedb64b47f6dddc1577123fcd85`  
		Last Modified: Wed, 14 Apr 2021 17:41:10 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7be7a926f02c08c32de5bc4e57d18923e0441090bd084aeb1b7dafaeb4ece58`  
		Last Modified: Wed, 14 Apr 2021 17:41:09 GMT  
		Size: 65.7 KB (65686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f5a6de061f5f5be316a0cf2d8471cf2baf8b3927a20b9d29826dc97bef2e54`  
		Last Modified: Wed, 14 Apr 2021 17:41:06 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9875593acbae6673d0c5d93c03471e559ccaf9f08b0afa67b0b35e9f08a8fcb5`  
		Last Modified: Mon, 10 May 2021 23:41:24 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f4e2a60af65180cf1e32ec6eb149427068959d48a05547b2c6490256b097a9`  
		Last Modified: Mon, 10 May 2021 23:41:46 GMT  
		Size: 181.0 MB (180987230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d3fe8a2b0caac734454b881230cd5d169976ddf064fc61469cbf630d13ed9d`  
		Last Modified: Mon, 10 May 2021 23:41:25 GMT  
		Size: 3.6 MB (3637071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c595642f23258a2887d1bbeaa8e94fc7516b59caaed29394c7a422a42f683b5d`  
		Last Modified: Mon, 10 May 2021 23:41:24 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
