## `openjdk:16-nanoserver-1809`

```console
$ docker pull openjdk@sha256:f05913a42a4b202e0b10fabe369a9128af5aa3718e00e12bcf3e325a82b17fd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `openjdk:16-nanoserver-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull openjdk@sha256:33935f702c6731d6f8e25b2f539cfff8de93a1cd47e0caa17c20658369461942
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.1 MB (297108266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff85b73401c57f458e5326b10753bafd28fcd85f8547910bc8ffdf0212eaf47d`
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
# Thu, 17 Sep 2020 23:18:56 GMT
ENV JAVA_VERSION=16-ea+16
# Thu, 17 Sep 2020 23:19:31 GMT
COPY dir:f93bc45673a59a0fd85604c3b59e36545d52954f0cd4d070bfb1a43e34c1a156 in C:\openjdk-16 
# Thu, 17 Sep 2020 23:20:01 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Thu, 17 Sep 2020 23:20:01 GMT
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
	-	`sha256:d433fbca52023b0dd3f70fe20d5a03126e4e87f5a01e2299444af5fbb502d2fc`  
		Last Modified: Thu, 17 Sep 2020 23:25:40 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca5af8fec99b6dcbc90e71059ae1b6bbcf0fda8e35e97bf49c6d876d7e61df1`  
		Last Modified: Thu, 17 Sep 2020 23:26:00 GMT  
		Size: 192.3 MB (192289834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f89f54842827a58b9bd06502fc3dee82094ce95274a8523b55fa7aa096132b0`  
		Last Modified: Thu, 17 Sep 2020 23:25:45 GMT  
		Size: 3.5 MB (3508931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b50f338507b4b357a302c47f88c727c5e7f2d3961153819c4e76666ba1260c5`  
		Last Modified: Thu, 17 Sep 2020 23:25:41 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
