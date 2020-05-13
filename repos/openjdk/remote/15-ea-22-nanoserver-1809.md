## `openjdk:15-ea-22-nanoserver-1809`

```console
$ docker pull openjdk@sha256:8802c38d4777b0d43d0f07074c23825b030fa55857555d607657c31d2f649a92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `openjdk:15-ea-22-nanoserver-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull openjdk@sha256:f6572e89ed0d9088a34e1e09f827af23ab0ab5a294c63a2dad394c48e44363ae
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.2 MB (292154882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a45e4f2bf8a33f5335f5142a19989a7fb46b434cacbfa5354ddec05a5116fd02`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 15:30:41 GMT
SHELL [cmd /s /c]
# Wed, 13 May 2020 15:30:42 GMT
ENV JAVA_HOME=C:\openjdk-15
# Wed, 13 May 2020 15:30:43 GMT
USER ContainerAdministrator
# Wed, 13 May 2020 15:31:00 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 13 May 2020 15:31:01 GMT
USER ContainerUser
# Wed, 13 May 2020 15:31:02 GMT
ENV JAVA_VERSION=15-ea+22
# Wed, 13 May 2020 15:31:54 GMT
COPY dir:2f3367520b3c419024b6707c817295e284534707809e0e97170d6114ec04ea5f in C:\openjdk-15 
# Wed, 13 May 2020 15:32:14 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Wed, 13 May 2020 15:32:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c597e8fceaeb76628095f6dcfa538d497e85739068a817b45d73be2b96a3b37`  
		Last Modified: Wed, 13 May 2020 16:09:16 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe4a1ac076e1dee08c07748ed0bf748357ec3c058f29131ddb0c6903b01c5b3`  
		Last Modified: Wed, 13 May 2020 16:09:16 GMT  
		Size: 837.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00cb774af18b914ba24ccfaba030aaee1af53cc965b45edd9166b2cbdc59558`  
		Last Modified: Wed, 13 May 2020 16:09:15 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0bbbe06e51300ecf6f12747f98fa77f8b3370196f85b87015dca501577f4aa`  
		Last Modified: Wed, 13 May 2020 16:09:14 GMT  
		Size: 64.1 KB (64131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0840576e1fb16bf2edf823eb58f597b05345e558ebba64301d718163d95b93d`  
		Last Modified: Wed, 13 May 2020 16:09:12 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd43407eb67f93b9bb425124bfb79a381eb419f9397463ee718d2acefee4b4ed`  
		Last Modified: Wed, 13 May 2020 16:09:12 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44261277c1ae8090a217e994b10e734593d4a0c124d9251445524de16257ee5f`  
		Last Modified: Wed, 13 May 2020 16:09:43 GMT  
		Size: 187.6 MB (187559543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc508808e56a2d798a986b973269c8ae4db27a9e05b8f101f576eafda371f8c9`  
		Last Modified: Wed, 13 May 2020 16:09:13 GMT  
		Size: 3.5 MB (3505993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260956e017538e9791fe407e48b8c80897bb0fd541f1238d686be901bbb95b82`  
		Last Modified: Wed, 13 May 2020 16:09:13 GMT  
		Size: 913.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
