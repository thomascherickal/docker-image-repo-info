## `openjdk:21-nanoserver`

```console
$ docker pull openjdk@sha256:5e334f4bfccf6acb688cee64c94a8eba2fdbccdce3d95d90668eef48338a690f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `openjdk:21-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull openjdk@sha256:db132861beee14c339b67df14f587a0b185ee6fc59313a022397c6122b761f75
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.3 MB (306283925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c89e09c04d25ab67b2eeb144824be2d9ce41adde9f2dbbecde06401d76c9730`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 21 Jun 2023 07:40:33 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:41:51 GMT
SHELL [cmd /s /c]
# Sat, 24 Jun 2023 03:10:41 GMT
ENV JAVA_HOME=C:\openjdk-21
# Sat, 24 Jun 2023 03:10:42 GMT
USER ContainerAdministrator
# Sat, 24 Jun 2023 03:10:51 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Sat, 24 Jun 2023 03:10:52 GMT
USER ContainerUser
# Tue, 04 Jul 2023 01:45:55 GMT
ENV JAVA_VERSION=21-ea+29
# Tue, 04 Jul 2023 01:46:09 GMT
COPY dir:b2c8a1460f9dc3bf94b24e32099408512a224fe452f01fc38dadba3f014c800b in C:\openjdk-21 
# Tue, 04 Jul 2023 01:46:20 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Tue, 04 Jul 2023 01:46:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:09087aac643f57e5e24f95fe0a1c8519d0f93dfcf4500263516c0f3874290109`  
		Last Modified: Fri, 23 Jun 2023 02:23:11 GMT  
		Size: 104.4 MB (104400893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09be2e47b3dff420361e93d34eaadedcfd9549c9be5bd77936370792babf874`  
		Last Modified: Sat, 24 Jun 2023 01:24:43 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1761082022ac41b0f9e56c60b660a94c5cc48216abc4ee6585d75e5f639b8b83`  
		Last Modified: Sat, 24 Jun 2023 03:15:39 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3d43ae3625180a30ce5075af37248f9b8bfb36b35d98ea87e0c69dd6309c66`  
		Last Modified: Sat, 24 Jun 2023 03:15:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7bf66e4a671426e237a857427cbba03c02b51ed5e66b0d72fc65d78ec04f91`  
		Last Modified: Sat, 24 Jun 2023 03:15:39 GMT  
		Size: 67.2 KB (67224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68960e43d220da8539c1fcad0e31945a1a70a4be19f3182a2d989413baa9e212`  
		Last Modified: Sat, 24 Jun 2023 03:15:37 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62bc87f448d21e830379cdb8bf549fa2aea98810072be9ec2cfc4f8cde2f8ee`  
		Last Modified: Tue, 04 Jul 2023 01:50:25 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ef46c9ef593b2ce34d0d208c28afa4f2770784486d51949660ee65edc51aa4`  
		Last Modified: Tue, 04 Jul 2023 01:50:42 GMT  
		Size: 198.0 MB (197989981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288fbc344d36389eb4e9710031bfde7d020f396b71f6b9952f0cb035eb3a9584`  
		Last Modified: Tue, 04 Jul 2023 01:50:26 GMT  
		Size: 3.8 MB (3818941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e91b64e76953b746301aac8eb09aea7c5aac97d1143c57707d3100f66dc2ca`  
		Last Modified: Tue, 04 Jul 2023 01:50:25 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
