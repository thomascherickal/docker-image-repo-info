## `docker:20-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:e3874f5facf1b519743f7b34b14b899c7f64b792989eeabc0a7833babba5642b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `docker:20-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull docker@sha256:563f72bba4b3447e891e9174152d3fb0b775b034782930e583b565b850c0eff6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2372200414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd85fd96499fb932f4298347820c3f9cd1a7a0b644a634124189903823e3ac9`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 19:15:35 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Mon, 12 Sep 2022 22:15:07 GMT
ENV DOCKER_VERSION=20.10.18
# Mon, 12 Sep 2022 22:15:08 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.18.zip
# Mon, 12 Sep 2022 22:15:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53d970c61010f2b55c869d8c51b4f9c6e6156fb44d5da363e0e4cb4ab747bba`  
		Last Modified: Wed, 17 Aug 2022 01:15:43 GMT  
		Size: 622.4 KB (622449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec94a5cb0dc71e7bf6fbb63cdb2034f2a4e7a88c063790e82ad90cd977e12c7`  
		Last Modified: Mon, 12 Sep 2022 22:18:06 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1710107c20a322bf45e6917994c522f0ded8024e5a8475d2de967302eb1d2f`  
		Last Modified: Mon, 12 Sep 2022 22:18:05 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e644fdc713caa9806557109bb4913fc3e6085e42f7e814e588ba273420e1b673`  
		Last Modified: Mon, 12 Sep 2022 22:18:15 GMT  
		Size: 54.7 MB (54684530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
