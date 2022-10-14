## `docker:20-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:26bb2693ca5a173e9fb59ec91f039c8e67088ddd1775be729190ce49d08becdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1129; amd64

### `docker:20-windowsservercore-ltsc2022` - windows version 10.0.20348.1129; amd64

```console
$ docker pull docker@sha256:53103c262a61595aba2d3cc01e346ab57024ab613b9f544f37f0abacddfe4b15
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2471473648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905f3156d58e77b4965df3d9a2e7e22a3eb11deb151e3ab881c91330bc986450`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 18:07:47 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 13 Oct 2022 23:23:15 GMT
ENV DOCKER_VERSION=20.10.19
# Thu, 13 Oct 2022 23:23:16 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.19.zip
# Thu, 13 Oct 2022 23:23:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb3038ebf46d13f3797c5bef150bfa682c8a25ee893c0ae7b1e9220a0fc1cad`  
		Last Modified: Wed, 12 Oct 2022 18:13:35 GMT  
		Size: 608.0 KB (607995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d97068b4604de25f15f17680cdbbfdb00b4f6d7491b59cb0e9c3bb5068ff65`  
		Last Modified: Thu, 13 Oct 2022 23:25:47 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87cfe7a32a58d03af2eb89703bbeebc5e776faf20caa9d3211def7e4c054bc0`  
		Last Modified: Thu, 13 Oct 2022 23:25:47 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6042b6c80f5d94cb282771b0b2cd2abf9cae2aa0a52a2ffe3d64fc0ca7ce2edc`  
		Last Modified: Thu, 13 Oct 2022 23:25:57 GMT  
		Size: 54.6 MB (54638027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
