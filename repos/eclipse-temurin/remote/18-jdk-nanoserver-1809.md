## `eclipse-temurin:18-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:f4134514a0aad9aeb6e835c16ecd8b92e7ce35fe72e2fca453b21d374111c49f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `eclipse-temurin:18-jdk-nanoserver-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull eclipse-temurin@sha256:92474400c41325e77bb8fc96892cc6528cc5da239f2f6ccd2cfe94643e7449ff
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.2 MB (293168744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bebcd8df39971d32881557d7ec84f94e72e0da542ecc8cf6ca84dc9d0933aeaa`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:49:49 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 15:17:11 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 11 May 2022 15:17:11 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 11 May 2022 15:17:12 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 15:17:21 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 May 2022 15:17:22 GMT
USER ContainerUser
# Wed, 11 May 2022 15:17:37 GMT
COPY dir:dd9b13d03f0f59427148f5f854823680c639cd938d50ff4813e6410f92c7aca7 in C:\openjdk-18 
# Wed, 11 May 2022 15:18:04 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 11 May 2022 15:18:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5592374182790eb41396d922d16be86f39a125562f29ea3ed221a94aeec2af45`  
		Last Modified: Wed, 11 May 2022 16:00:35 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932168d2a841e72a2f7aa4e6e4ceb658cc49fb857d20f25b6df0a1ba3ae9ada4`  
		Last Modified: Wed, 18 May 2022 13:40:43 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23a48d381b79496bd03d17f3dc7d85911ca74ec0f4934915a4acaa24cf1001d`  
		Last Modified: Wed, 18 May 2022 13:40:43 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8884618775190e454a9daac184259eca381568414ee0755e99c57f42fe4a95`  
		Last Modified: Wed, 18 May 2022 13:40:43 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c902b1c5d9ecd421c4cfe2b1e768a78722666b89f6d49d41c8a2b4fda7af9e`  
		Last Modified: Wed, 18 May 2022 13:40:40 GMT  
		Size: 72.0 KB (71993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295c01d0a06b53e0ad6831f9c1b9d6f400122229fa154dce8e9eaf6cf4f3a96d`  
		Last Modified: Wed, 18 May 2022 13:40:41 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e2dab5a18b476849c6148eff2b700264b095f29b9085d0a955424e63073e60`  
		Last Modified: Wed, 18 May 2022 13:41:00 GMT  
		Size: 186.4 MB (186439134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71ad8a0921a0ad584c8a6811b2293c99d52262494427d665f924fde7cd290eb`  
		Last Modified: Wed, 18 May 2022 13:40:44 GMT  
		Size: 3.5 MB (3516861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755d410008167d4a0d1421f697054c2ac88b930a26bbe05920456add361614bf`  
		Last Modified: Wed, 18 May 2022 13:40:40 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
