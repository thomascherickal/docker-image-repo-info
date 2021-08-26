## `openjdk:11-jre-nanoserver-1809`

```console
$ docker pull openjdk@sha256:ccf58ac1b14d2a94735f5f5b9ba30e57429c3483ce45db8e3cb87c4fdd422dbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `openjdk:11-jre-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull openjdk@sha256:d3b6dbec2f81e091eff08b671e46a1ecab804d7c568b6cedb626ed243da2207c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142381820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2343cc24d7880287bff3c26b39b754c378983101f50ec1f79d44899ffbc1fca`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:34:07 GMT
SHELL [cmd /s /c]
# Wed, 25 Aug 2021 17:23:44 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 25 Aug 2021 17:23:45 GMT
USER ContainerAdministrator
# Wed, 25 Aug 2021 17:23:54 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 25 Aug 2021 17:23:55 GMT
USER ContainerUser
# Wed, 25 Aug 2021 17:23:55 GMT
ENV JAVA_VERSION=11.0.12
# Wed, 25 Aug 2021 17:27:19 GMT
COPY dir:cfe6877c6b81ca46843a524b803b574bd01e43f05b821b8b183eb47cd476c286 in C:\openjdk-11 
# Wed, 25 Aug 2021 17:27:32 GMT
RUN echo Verifying install ... 	&& echo   java --version && java --version 	&& echo Complete.
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9191bd6656c8ea186f621f667fb09a30387fae304b3e7817fd7e8258c022d185`  
		Last Modified: Wed, 25 Aug 2021 23:21:14 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e68364679802af47e0250344dc510ceb25c74053d47e8dea0f75e8f149132d8`  
		Last Modified: Thu, 26 Aug 2021 00:45:40 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c105a23ad13b255cc8ad442cc53e5f67b70d3e834eb15e3e8a48e06feba67081`  
		Last Modified: Thu, 26 Aug 2021 00:45:40 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5edae3021df653237884936ec3ec2f746cd3bd4873f52ea3bd6177c7d97867b`  
		Last Modified: Thu, 26 Aug 2021 00:45:40 GMT  
		Size: 69.5 KB (69540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71195e19fc625e2df55c96e4c0f645ccdd5e50b9843e6cad2781b1feab272256`  
		Last Modified: Thu, 26 Aug 2021 00:45:38 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca62150454fe1fcd3a2526f2c3efb2a9d58c4ff946912b82e9bcd01dbd202e2`  
		Last Modified: Thu, 26 Aug 2021 00:45:37 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32af74f431f36bb95474470fb6c0956dbdcd97a8952c2011c6dec77b170324da`  
		Last Modified: Thu, 26 Aug 2021 00:47:39 GMT  
		Size: 39.5 MB (39483672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104e4d557e99a17a74747407d6f1e7059b781cb34cb5b931cecd519195979acc`  
		Last Modified: Thu, 26 Aug 2021 00:47:31 GMT  
		Size: 81.8 KB (81754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
