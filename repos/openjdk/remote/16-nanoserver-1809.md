## `openjdk:16-nanoserver-1809`

```console
$ docker pull openjdk@sha256:b20bbfed19c1780a4450e235c53b914f0a62e4da4e1cb08f111ce220c2a7011e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `openjdk:16-nanoserver-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull openjdk@sha256:75c6b7b5990271853d946d6b4b6fa667b08bb5100418c7d752fa5767875d631c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.5 MB (299498414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77156b37474be0bdfed824b17f7dd4a45dc97c9d0688897e70fd8305e48d09d7`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 17:46:04 GMT
SHELL [cmd /s /c]
# Wed, 14 Oct 2020 17:46:05 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 14 Oct 2020 17:46:06 GMT
USER ContainerAdministrator
# Wed, 14 Oct 2020 17:46:21 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 14 Oct 2020 17:46:22 GMT
USER ContainerUser
# Thu, 22 Oct 2020 23:19:58 GMT
ENV JAVA_VERSION=16-ea+21
# Thu, 22 Oct 2020 23:20:31 GMT
COPY dir:0c605f3a9326fdca4c2284fc216ef9036c7194c4b028bdf7333d9263d8a9b916 in C:\openjdk-16 
# Thu, 22 Oct 2020 23:21:01 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Thu, 22 Oct 2020 23:21:02 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:40f59dc77cd194db29e444ce30cc9a91a3d555f7d4d7329fb6f46c13e559dc2f`  
		Last Modified: Wed, 14 Oct 2020 18:31:55 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2c5c7ff5b97e2384ad57c7cd4094b1a40907ea3634e923a539236764052c20`  
		Last Modified: Wed, 14 Oct 2020 18:31:53 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e535cf22ef1ca77aebd1948de6ab3937b1f63d64895ea717d71cff42d95815`  
		Last Modified: Wed, 14 Oct 2020 18:31:54 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a209bbfc514f45496baa96d8592838b00434aae4cd11fb8ffbcf643dfe386c`  
		Last Modified: Wed, 14 Oct 2020 18:31:52 GMT  
		Size: 72.2 KB (72249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc31a2a793752d0400745705f15ea0e51a67ed288dc5bc3c6eda4520ca139549`  
		Last Modified: Wed, 14 Oct 2020 18:31:50 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a0938c4d7fe11d971aac889fa456476be22d6407ffdaa62d91e7227db64000`  
		Last Modified: Thu, 22 Oct 2020 23:35:25 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c746d556fe2a93c07ebabcc1fdfa0e9ff007b64e6a866c8ff7ddc5239048c0`  
		Last Modified: Thu, 22 Oct 2020 23:35:44 GMT  
		Size: 194.5 MB (194537691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61e46023ebacb15f446eae971f088f2cc46298f9d1ea7e33e74c975b1793982`  
		Last Modified: Thu, 22 Oct 2020 23:35:26 GMT  
		Size: 3.7 MB (3677991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a46c4752f41c4fa80d0e9fa55509917570895c744a5fa3f7ad48e3ec424a1e1`  
		Last Modified: Thu, 22 Oct 2020 23:35:25 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
