## `docker:20-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:1ab7eaf7340a8a7ce3a77d03563b47769141c84fd09150af1d40318c90146f32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1129; amd64

### `docker:20-windowsservercore-ltsc2022` - windows version 10.0.20348.1129; amd64

```console
$ docker pull docker@sha256:c8bab1c855318f01912944744094ec01d9903bcfd4b84c73af921a8e5a4a40e1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2471473954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aa16d5f5fcce57dda283ce77f9b3f59f31483155adacd6210eac154346a33b1`
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
# Wed, 12 Oct 2022 18:11:05 GMT
ENV DOCKER_VERSION=20.10.18
# Wed, 12 Oct 2022 18:11:06 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.18.zip
# Wed, 12 Oct 2022 18:11:35 GMT
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
	-	`sha256:f5ae5525fbe4100d404193596121574da20b050330816004655900640a41564b`  
		Last Modified: Wed, 12 Oct 2022 18:14:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f34121ecfae79291940d488bfe0b4dd9e461789085174971ede2d053f77087`  
		Last Modified: Wed, 12 Oct 2022 18:14:03 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5712406db49f70d04d515f00bf541d2565a24b25d0d8b12ef23bf5cbd12e88e`  
		Last Modified: Wed, 12 Oct 2022 18:14:13 GMT  
		Size: 54.6 MB (54638378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
