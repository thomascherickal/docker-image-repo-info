## `docker:rc-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:6e5fef1d6e4fcf4a0f0e7bea6112a8651bb0168d6e4b79881c1a1e1e3bf418df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `docker:rc-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull docker@sha256:4d4eacbd93ae392a4f6ea27353fb9e9e47ad3ee16cbb73cb90eddff24d562dcf
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2327281792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56afb70cebd9c762c45f75575cd18c19e26b046460b7fbdbf35f9e19937b8d3e`
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
# Wed, 10 Aug 2022 19:15:36 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Wed, 10 Aug 2022 19:15:37 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-22.06.0-beta.0.zip
# Wed, 10 Aug 2022 19:16:05 GMT
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
	-	`sha256:2215c7dac46631e652ba670fe87b06b65a31e0c9d7c95fc64c1d75a756464527`  
		Last Modified: Wed, 17 Aug 2022 01:15:43 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac2af1154bca50e684c4684bd3e7b1e6b49068ce664c3dc48096b178dad248e`  
		Last Modified: Wed, 17 Aug 2022 01:15:43 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008425f9a745672e17cb4c3c6149b8e9785f7c7266c10d574006ac76c8ab4811`  
		Last Modified: Wed, 17 Aug 2022 01:15:45 GMT  
		Size: 9.8 MB (9766158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
