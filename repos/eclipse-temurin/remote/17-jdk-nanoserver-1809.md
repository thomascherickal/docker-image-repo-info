## `eclipse-temurin:17-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:67ba0da51291c6cd445a20c55bb9adb3db4671565cab1ccecb538452f855d04c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:17-jdk-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull eclipse-temurin@sha256:00b4289bab0ae24fe3d78ff9cc3043a594ee0849e2666b588d1f0ba6e98219b4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.8 MB (291824866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9660a60c67daaf2ee31b4964c548e0d0ba947bdb4e6fc4500dddc389ec994d5`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 15:16:11 GMT
SHELL [cmd /s /c]
# Wed, 13 Apr 2022 15:37:47 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Wed, 13 Apr 2022 15:37:48 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 13 Apr 2022 15:37:49 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 15:37:56 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Apr 2022 15:37:56 GMT
USER ContainerUser
# Wed, 13 Apr 2022 15:38:10 GMT
COPY dir:af72ba1102e9cda7f5ea9974b0cafbe96b2f97690adb0743202a1c732a987a84 in C:\openjdk-17 
# Wed, 13 Apr 2022 15:38:22 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Apr 2022 15:38:22 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ea4009814dceb50337c66614a6008cfc2fb73ce53e62162bce071ef6ea1adf2d`  
		Last Modified: Wed, 13 Apr 2022 15:58:06 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c673da2302df4dcb79c5b7dabb77e1f397e971140f7d7938e9901fdf129f88`  
		Last Modified: Wed, 13 Apr 2022 16:27:19 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70d5e20305f53db451834484636ee7a11afd0bf1ac918d07a034ad86fa47289`  
		Last Modified: Wed, 13 Apr 2022 16:27:18 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7c4a0de67fdccc000e65345b45fabc73816689b9c0e10e43abdd3a6d978ee2`  
		Last Modified: Wed, 13 Apr 2022 16:27:18 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73b77168ca14497b8087af81bcfdc1c12bf6294ff077284c7b295c94da6bd80`  
		Last Modified: Wed, 13 Apr 2022 16:27:16 GMT  
		Size: 73.1 KB (73055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1db9eebee9ed6a67444d1a78877299c5be7671b6f68d388f5de8040b651edd`  
		Last Modified: Wed, 13 Apr 2022 16:27:15 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a788a198133e07519aa60fa445c61ee54f3fef4df87ff3c3c268fbb4004da5`  
		Last Modified: Wed, 13 Apr 2022 16:27:34 GMT  
		Size: 185.0 MB (185023019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e347ecd41531cd0302278f4c984cd39a155b06c1c14a861fc2fdbb90d74bd6`  
		Last Modified: Wed, 13 Apr 2022 16:27:16 GMT  
		Size: 3.6 MB (3625853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9c82ff303ad77c09479d97bf60f804591585c8b55ab99c21f570431d0abd05`  
		Last Modified: Wed, 13 Apr 2022 16:27:15 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
