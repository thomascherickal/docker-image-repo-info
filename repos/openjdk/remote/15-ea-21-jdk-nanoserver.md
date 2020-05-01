## `openjdk:15-ea-21-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:9b7769bac74645e87831b0bf8a828ce71f06f2e832b69d8a785230bc1d59e703
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `openjdk:15-ea-21-jdk-nanoserver` - windows version 10.0.17763.1158; amd64

```console
$ docker pull openjdk@sha256:6e4839c75b6803106a6ea2b423cb91088ced5136258635f412254f56d056ea85
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.3 MB (292282811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7927aeaa96a26a028c52c96ae4cc862a3033794d32cbf9e34bba79f6140b90c8`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 12 Apr 2020 11:41:03 GMT
RUN Apply image 1809-amd64
# Tue, 14 Apr 2020 21:42:38 GMT
SHELL [cmd /s /c]
# Tue, 14 Apr 2020 21:42:39 GMT
ENV JAVA_HOME=C:\openjdk-15
# Tue, 14 Apr 2020 21:42:39 GMT
USER ContainerAdministrator
# Tue, 14 Apr 2020 21:42:54 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Tue, 14 Apr 2020 21:42:54 GMT
USER ContainerUser
# Fri, 01 May 2020 00:19:31 GMT
ENV JAVA_VERSION=15-ea+21
# Fri, 01 May 2020 00:20:14 GMT
COPY dir:5c9ae1c51b3b343e39abe0a7a69910adeb5229db4fd5f55476c185dc38bc2e34 in C:\openjdk-15 
# Fri, 01 May 2020 00:20:34 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Fri, 01 May 2020 00:20:35 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:0fe89239909ba300aeb9b977458b61ae3fbbcd2d9591086ed05ca023209d3122`  
		Size: 101.1 MB (101118377 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:895ca47ba9cf1a5b61a0721217cfcc038bbe9a4987c7536321c3ac51ef8e5e0c`  
		Last Modified: Tue, 14 Apr 2020 22:17:22 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcf297e34b7d011805160436d6acaba77887d05e2acd81e88acd84ad22cdff1`  
		Last Modified: Tue, 14 Apr 2020 22:17:22 GMT  
		Size: 830.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9641626825020cd19b05bbf1f20b92df3d267d2aade5a84deef0163b791a895b`  
		Last Modified: Tue, 14 Apr 2020 22:17:22 GMT  
		Size: 819.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062e1c072d6c921a1b4e4db61fa592b7f9ccbc231f6c5cc8dfd4417fc317438c`  
		Last Modified: Tue, 14 Apr 2020 22:17:21 GMT  
		Size: 67.0 KB (67045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe221d18f1e3ca2b86519debf76a76b4ba0e95f42490a1a161bffea2d3306309`  
		Last Modified: Tue, 14 Apr 2020 22:17:19 GMT  
		Size: 824.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930338d174abcdf5b2bf150bd9887b30a5641b7928e424c5119434fb797c76fd`  
		Last Modified: Fri, 01 May 2020 00:25:40 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7cb91153b2230bd441700995002d8e6552923a3ca9156afa3eb2db5e6b52ff`  
		Last Modified: Fri, 01 May 2020 00:26:09 GMT  
		Size: 187.6 MB (187594209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98c880105357c267746e1b19155255a127fdc6a832a6079f2eeda0a15d12a51`  
		Last Modified: Fri, 01 May 2020 00:25:42 GMT  
		Size: 3.5 MB (3498117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2467ec45325eb9895c54110c33b7fd6a699ec7c2ce6b41b7bea858a21ed5455`  
		Last Modified: Fri, 01 May 2020 00:25:40 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
