## `openjdk:16-ea-23-nanoserver`

```console
$ docker pull openjdk@sha256:ae4f0c01ceae8ed6137d5414c9d5b42ea94a1eb5a41cfb829633884320d96ad3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `openjdk:16-ea-23-nanoserver` - windows version 10.0.17763.1577; amd64

```console
$ docker pull openjdk@sha256:e29931e699237519b8acc040c86b16d55be0319719b95053dd5becb589cdf7a4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.7 MB (283680468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8616d8d8335258476bd4809799d44c8ec5ac082ed6eb492f8de98f128c6298d1`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 31 Oct 2020 05:10:43 GMT
RUN Apply image 1809-amd64
# Wed, 11 Nov 2020 17:53:16 GMT
SHELL [cmd /s /c]
# Wed, 11 Nov 2020 17:53:16 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 11 Nov 2020 17:53:17 GMT
USER ContainerAdministrator
# Wed, 11 Nov 2020 17:53:32 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 11 Nov 2020 17:53:32 GMT
USER ContainerUser
# Wed, 11 Nov 2020 17:53:33 GMT
ENV JAVA_VERSION=16-ea+23
# Wed, 11 Nov 2020 17:54:14 GMT
COPY dir:32805abd9af50dd1ad5b5a4bc83c7f61360fd8cc7b0d8a6e1fd0108cebd60472 in C:\openjdk-16 
# Wed, 11 Nov 2020 17:54:34 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Wed, 11 Nov 2020 17:54:35 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f1b217fe8837d4d85cb8228a52344d3504d7aa51ba30167a20a6a4cb80cdcaa0`  
		Size: 101.3 MB (101279682 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:41b7be9dc08821cf81d29b16e0df54f7f3e3aeaa6407f43520c6259f2d84b10c`  
		Last Modified: Wed, 11 Nov 2020 18:27:27 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e637122599038842d743045a8ebfbfa35dbadf7dfee0adcc2ba903e891ab072d`  
		Last Modified: Wed, 11 Nov 2020 18:27:25 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7fa5c85bf3c3dc79cf3bec9aba597aa0b5c38c234952da905e86d7a556b6f3`  
		Last Modified: Wed, 11 Nov 2020 18:27:25 GMT  
		Size: 912.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9c6b451f516c5e78ab16ded450d01a2a45dd13d0cac12cb9b043f5d87f993a`  
		Last Modified: Wed, 11 Nov 2020 18:27:25 GMT  
		Size: 67.3 KB (67302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac0f27f5ace77a66a18d26e72bf8f24216110f8ed5b6f951597b9a42d3ae52b`  
		Last Modified: Wed, 11 Nov 2020 18:27:22 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447e11262b099f581a186a1fb6faee57740ba6dc8aee3e4f5bafa0687c3052bf`  
		Last Modified: Wed, 11 Nov 2020 18:27:22 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761a312547b3cfa36ddd02473dbdd93352f9176226cc9601b7cbe86ebe2abf25`  
		Last Modified: Wed, 11 Nov 2020 18:27:50 GMT  
		Size: 178.7 MB (178726367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e9e890db95a28d6736a97d911f823e92b766d8e7feae3dcf20153bd116a9b5`  
		Last Modified: Wed, 11 Nov 2020 18:27:23 GMT  
		Size: 3.6 MB (3601848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e470bdc8781e5f15f187c7f8876ab4ed6cb8583af473b34f5b197f15e2c8a082`  
		Last Modified: Wed, 11 Nov 2020 18:27:22 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
