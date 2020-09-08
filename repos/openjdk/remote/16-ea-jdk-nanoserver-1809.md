## `openjdk:16-ea-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:0eb410936493ece50aa9d42fd67ce8b0b88998d44a57dee79506b66f0949cf22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `openjdk:16-ea-jdk-nanoserver-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull openjdk@sha256:6dd6d6bbbbe6f219fbe919dc42cb1cc7105afcfe133964db852f1d70e023fd8f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (297016892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8e166e97d074582652c5b606d1bb90d49b72434cc4ad913f4eeefb03674f462`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Tue, 08 Sep 2020 20:13:38 GMT
SHELL [cmd /s /c]
# Tue, 08 Sep 2020 20:13:38 GMT
ENV JAVA_HOME=C:\openjdk-16
# Tue, 08 Sep 2020 20:13:39 GMT
USER ContainerAdministrator
# Tue, 08 Sep 2020 20:13:53 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Tue, 08 Sep 2020 20:13:54 GMT
USER ContainerUser
# Tue, 08 Sep 2020 20:13:54 GMT
ENV JAVA_VERSION=16-ea+14
# Tue, 08 Sep 2020 20:14:34 GMT
COPY dir:a5e28348581cbcfe74370f928bd713422359b2a2d48ea7b5eee249098d990378 in C:\openjdk-16 
# Tue, 08 Sep 2020 20:14:56 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Tue, 08 Sep 2020 20:14:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f72ec155bceaba8b4a5cdbd7aa79586c7296a801af5364a691c46191c910e2da`  
		Last Modified: Tue, 08 Sep 2020 22:29:01 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b2192657885f813dd6fa78d8ba65d02e35934c0c45121f5cb3004298998876`  
		Last Modified: Tue, 08 Sep 2020 22:28:59 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe914594cd5b7b9a0b5c0080fe6c643b51eecedb3197955dbea30a0005a9132`  
		Last Modified: Tue, 08 Sep 2020 22:28:59 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4324dc65079aab4e95e3a823193385145a250bbb9e13cd9c5e02a35844069217`  
		Last Modified: Tue, 08 Sep 2020 22:29:00 GMT  
		Size: 65.1 KB (65142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bee2eb45cc55aae1760d1937d9de7b70abd95c9488b97a8288d08b472684fb5`  
		Last Modified: Tue, 08 Sep 2020 22:28:57 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d36e9ba800b411b99e0d5981ec6ca8e9c1da69fe1fe315d1ad485cc0bd7ec0`  
		Last Modified: Tue, 08 Sep 2020 22:28:57 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da4a8a9078f8d69497b09686037a1af22daf3025f0cb6d721c052edc44dbb35`  
		Last Modified: Tue, 08 Sep 2020 22:29:17 GMT  
		Size: 192.2 MB (192221399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efd5d9a79cc4f7a78e2fab37eb96c28b109cc1e627bb9b610f011c12a84f441`  
		Last Modified: Tue, 08 Sep 2020 22:28:58 GMT  
		Size: 3.5 MB (3485958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dae9bc650d0d928db2258a731b0c38997be89489d06d2aa7ae3deb0f03ea542`  
		Last Modified: Tue, 08 Sep 2020 22:28:57 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
