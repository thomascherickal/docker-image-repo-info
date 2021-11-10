## `eclipse-temurin:16-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:d44359ca595d136c48bdeee76ff12925c84192ca391f885d09fcd86dd4592280
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `eclipse-temurin:16-jdk-nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull eclipse-temurin@sha256:93f8b708558720797f9110fc35bb6383e2f45acaf71cf28d30cf7ac57134850d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.3 MB (305279903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7119befe4460d21ffc5d3b2c0dfddff059ba9b29960b043a74ed11ba1a238a90`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:13:20 GMT
SHELL [cmd /s /c]
# Wed, 10 Nov 2021 17:40:16 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Wed, 10 Nov 2021 17:40:17 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 10 Nov 2021 17:40:17 GMT
USER ContainerAdministrator
# Wed, 10 Nov 2021 17:40:26 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 10 Nov 2021 17:40:26 GMT
USER ContainerUser
# Wed, 10 Nov 2021 17:40:43 GMT
COPY dir:9a7ef5975d9ba9576c4744dc049616bbcb218f14c3c0bd967851cd46479d6134 in C:\openjdk-16 
# Wed, 10 Nov 2021 17:40:56 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 10 Nov 2021 17:40:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e60ec86b90e1492e0e0ed2cbebcf624990a34862e24207343fd85b84b3544c8e`  
		Last Modified: Wed, 10 Nov 2021 18:01:59 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59fc507804c2c1414ead337f5b4e9250a91418e08fc6fbdb0ff52d067f5f817`  
		Last Modified: Wed, 10 Nov 2021 18:37:47 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8132e83fd910755279e3f884b1aba3a9ceda31d99cce55a0d10e8d459ff62e`  
		Last Modified: Wed, 10 Nov 2021 18:37:47 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cebe5f9fcefc181085ef3ee3c22c5d2756b9ad0bdd1a1a334a638a63350fe24`  
		Last Modified: Wed, 10 Nov 2021 18:37:47 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c545d8134d9e84b3b8b7140a84960279aff46991d3f42f8b1be4c205bbef624`  
		Last Modified: Wed, 10 Nov 2021 18:37:45 GMT  
		Size: 74.8 KB (74794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576fb784e8d5d438f1e1961e526d1f0341a4aef3655ed6fdabe32298b19e0c65`  
		Last Modified: Wed, 10 Nov 2021 18:37:45 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16fb2eda96839a81641a17e507008a908a7beb1480a476e43843acfbc61ecd0`  
		Last Modified: Wed, 10 Nov 2021 18:38:04 GMT  
		Size: 198.8 MB (198757774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09318d3d08ad6c4c49579e60aee3ddfaf08e0c685f5878efde1609506db8e79`  
		Last Modified: Wed, 10 Nov 2021 18:37:46 GMT  
		Size: 3.7 MB (3657398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f3e4aad9071c811f8a72a5c68cd987cd0233c19fb57f22cdd39b27d402c26e`  
		Last Modified: Wed, 10 Nov 2021 18:37:45 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
