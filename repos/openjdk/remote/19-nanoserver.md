## `openjdk:19-nanoserver`

```console
$ docker pull openjdk@sha256:40dc055682d400518ce2c75be62a47322f602cf6e769f874c67aed93b607fc3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `openjdk:19-nanoserver` - windows version 10.0.17763.3046; amd64

```console
$ docker pull openjdk@sha256:050153142ea7b30ac4bd243e3896429c364f1ab18dd78c03f7420e548f20e76f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.1 MB (298118413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:317355dac5f0deb88b05d8503c2888a60ea8109a338444279645ccc498d24fc3`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 09 Jun 2022 19:20:11 GMT
RUN Apply image 10.0.17763.3046
# Wed, 15 Jun 2022 17:30:58 GMT
SHELL [cmd /s /c]
# Wed, 15 Jun 2022 19:36:19 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 15 Jun 2022 19:36:20 GMT
USER ContainerAdministrator
# Wed, 15 Jun 2022 19:36:30 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 15 Jun 2022 19:36:31 GMT
USER ContainerUser
# Wed, 22 Jun 2022 00:51:02 GMT
ENV JAVA_VERSION=19-ea+27
# Wed, 22 Jun 2022 00:51:16 GMT
COPY dir:ed46686ceea2d5c9ca4073721dee3434d3066dab570dfe491f66ee273234d56e in C:\openjdk-19 
# Wed, 22 Jun 2022 00:51:38 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 22 Jun 2022 00:51:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d555a7e4de4dd775379d5c43c1419374bff7908670dc7444be5e8e8f386f3d26`  
		Size: 103.2 MB (103153235 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92b4c385cd5cbb12fb09cb31c12b5e5de38cf7b380c8681286caac242c06d3ed`  
		Last Modified: Wed, 15 Jun 2022 18:22:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b58c89b4b822d0d5d5f1bc8225f7a37f7dc8a316f92594090c400a34a1a51ff`  
		Last Modified: Wed, 15 Jun 2022 20:10:09 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb2fbbb0972907c5181cdfabed7833e7b033a86dcac9a55e84b1e6dc2861652`  
		Last Modified: Wed, 15 Jun 2022 20:10:09 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28327af37fa2c35b8687ad7e3ec93de3a24924e9504e2eaadb1ef6cd98728065`  
		Last Modified: Wed, 15 Jun 2022 20:10:09 GMT  
		Size: 68.9 KB (68857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266bdb7d76259c486b3300ec15922ed2162301ab3c50cfd1c9f8b1ed4ca95b1f`  
		Last Modified: Wed, 15 Jun 2022 20:10:06 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff0dab7c168d1f68c02e47ebed9647b2913bbceeb36cc518356f198e798715d`  
		Last Modified: Wed, 22 Jun 2022 02:40:08 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826a81e6c36dd5c7d3f483e1522b64bc196392bb8e19c8c1d9abbd41d7d80856`  
		Last Modified: Wed, 22 Jun 2022 02:43:37 GMT  
		Size: 191.2 MB (191174474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af117a16dfa3945f95e57526e1504d650e2184369b687c0903c30c3934ce536`  
		Last Modified: Wed, 22 Jun 2022 02:40:09 GMT  
		Size: 3.7 MB (3714838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e88ae9b0d627824f6bc6492c710922a16c0c67f23e7e491f85a3b3ae07a4a9d`  
		Last Modified: Wed, 22 Jun 2022 02:40:08 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
