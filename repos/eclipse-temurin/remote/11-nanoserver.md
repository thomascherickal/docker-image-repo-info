## `eclipse-temurin:11-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:46c0ffadead0c2274ddbe21d4dc38cc226996303b8879bee73e8a683afe71458
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `eclipse-temurin:11-nanoserver` - windows version 10.0.20348.1547; amd64

```console
$ docker pull eclipse-temurin@sha256:7307010b86801c3e033cc76b31e77b816ca4248a57846766a651aeff735675ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.2 MB (315174229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ea30aa6aef46896ce57c995cd090c2d4728aaf01537725f9a4204d2f614f77`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Feb 2023 11:05:29 GMT
RUN Apply image 10.0.20348.1547
# Wed, 15 Feb 2023 23:34:03 GMT
SHELL [cmd /s /c]
# Wed, 15 Feb 2023 23:35:52 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Wed, 15 Feb 2023 23:35:53 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 15 Feb 2023 23:35:54 GMT
USER ContainerAdministrator
# Wed, 15 Feb 2023 23:36:06 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 15 Feb 2023 23:36:07 GMT
USER ContainerUser
# Wed, 15 Feb 2023 23:36:25 GMT
COPY dir:3631bd3b4ae70db635b51d6f7ad3f3254aa758db5b0d079379d506c898ecba14 in C:\openjdk-11 
# Wed, 15 Feb 2023 23:36:53 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 15 Feb 2023 23:36:54 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2e8a1636f1721beefd71f8e0c7176faabfe00d7503a69e909468fd63ac3a4992`  
		Last Modified: Thu, 16 Feb 2023 00:30:27 GMT  
		Size: 122.1 MB (122119166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f21b41cddbbbe3e6e7b8691f9cfc05eac50290ddadabfd44482b251564c6481`  
		Last Modified: Thu, 16 Feb 2023 07:21:04 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985430554fb89d662596c204cc828ee8c8780d460dae0d82bdefdbdb41a19aa9`  
		Last Modified: Thu, 16 Feb 2023 07:21:50 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec87a3c2d56bc7bee3681f3cbf3bcff7b5ea15792be07a26236dfff85cbcb25`  
		Last Modified: Thu, 16 Feb 2023 07:21:49 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71364a1354c17d15bef10666b7737cba0d1756a09889840c1221c1a0a1db64fc`  
		Last Modified: Thu, 16 Feb 2023 07:21:50 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44388c02ea69efa530973287f79b6b344b60c3ec97e7cd3e3d17b2dbc16609d1`  
		Last Modified: Thu, 16 Feb 2023 07:21:47 GMT  
		Size: 85.3 KB (85269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ce2305f078863311e40f625dc48ffdfc5f4e8b4f223f7568e33d4f7be60c70`  
		Last Modified: Thu, 16 Feb 2023 07:21:47 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6172fdac63e2ebf7730d5fb7f2350051ef80ec3d11984010d7b1cc45d13183e4`  
		Last Modified: Thu, 16 Feb 2023 07:22:15 GMT  
		Size: 192.9 MB (192887804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3671c5a7010e7355218f94a964ca13c74c6e480d5ccbfb433a5c917ac318221`  
		Last Modified: Thu, 16 Feb 2023 07:21:48 GMT  
		Size: 75.4 KB (75428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b638e8afa218700d105ea297c7f4693ec8c211bbb9f4884bc2374c8fa0315f1`  
		Last Modified: Thu, 16 Feb 2023 07:21:47 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-nanoserver` - windows version 10.0.17763.4010; amd64

```console
$ docker pull eclipse-temurin@sha256:68c70568376b65402031d5f64e63642387a23b37219630f7be4da21ab3a729d1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.7 MB (299745996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77e9c25288109a5beb50c7b97a72adcabc5ea377f3524d8df57294a856e9faef`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Feb 2023 10:14:28 GMT
RUN Apply image 10.0.17763.4010
# Wed, 15 Feb 2023 22:46:15 GMT
SHELL [cmd /s /c]
# Wed, 15 Feb 2023 23:00:27 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Wed, 15 Feb 2023 23:00:28 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 15 Feb 2023 23:00:29 GMT
USER ContainerAdministrator
# Wed, 15 Feb 2023 23:00:42 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 15 Feb 2023 23:00:43 GMT
USER ContainerUser
# Wed, 15 Feb 2023 23:00:59 GMT
COPY dir:3631bd3b4ae70db635b51d6f7ad3f3254aa758db5b0d079379d506c898ecba14 in C:\openjdk-11 
# Wed, 15 Feb 2023 23:01:28 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 15 Feb 2023 23:01:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:00eaf3341cd3cc6b72f91399cb3bd1aba30eb7eead7596532fe54c4bf1b010d7`  
		Last Modified: Thu, 16 Feb 2023 00:31:21 GMT  
		Size: 106.7 MB (106674970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0185f49bd9e9c2d18b1dcf8f1f67123b4146383e07a158cb4623d96fb2d18c05`  
		Last Modified: Thu, 16 Feb 2023 02:29:16 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eacd283645088b748f2236c3603cb5b4ca410d489109d7387d2418bceb646a55`  
		Last Modified: Thu, 16 Feb 2023 07:12:39 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef6a2a475b6478f866f64610af04abc980de3ce18fab63fd0a60090584da045`  
		Last Modified: Thu, 16 Feb 2023 07:12:40 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f57adb7c019cf106d5ba65ea8d4d187376ac500274b00a34d353d93b08aecf1`  
		Last Modified: Thu, 16 Feb 2023 07:12:39 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514262b1ee7b992f1767c1bff598e30a20984736a824b8d5844812f2f5403b40`  
		Last Modified: Thu, 16 Feb 2023 07:12:37 GMT  
		Size: 69.3 KB (69264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e07a29aba56ecf28c6116fc1547bb56c795f39be19e69650b61b8b680d87e6`  
		Last Modified: Thu, 16 Feb 2023 07:12:37 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5404676b12ff7c508ab6b88fdcca5fc97789ca919aa2df0ff09b68c1751680`  
		Last Modified: Thu, 16 Feb 2023 07:13:02 GMT  
		Size: 192.9 MB (192904154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6549eaafe74090c2f02eb5edc56cdb82dcc216a61ddf19b992d8ec51806ce51`  
		Last Modified: Thu, 16 Feb 2023 07:12:37 GMT  
		Size: 90.6 KB (90620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc489fc94ea331f169df82c80b965bfaa8269f569bf5fdbab3b774a6f42e96f`  
		Last Modified: Thu, 16 Feb 2023 07:12:37 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
