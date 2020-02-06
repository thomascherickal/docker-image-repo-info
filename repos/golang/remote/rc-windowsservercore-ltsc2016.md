## `golang:rc-windowsservercore-ltsc2016`

```console
$ docker pull golang@sha256:8bed551eac672c2f7c60b6c1829331f6ccae3360b2661d94d11de7c7fa86ff4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `golang:rc-windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull golang@sha256:0bc29154b6740ddc43b1942475cce255b3d13e133eef3e2d870453a1b91cf3f2
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5903150485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660accc3205bbe7a80f045149ce7eeb883b6ff84efb7bb2e3262463b87960cfc`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 13:12:27 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Jan 2020 13:12:28 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Jan 2020 13:12:29 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Jan 2020 13:12:30 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Jan 2020 13:14:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Jan 2020 13:14:10 GMT
ENV GOPATH=C:\gopath
# Wed, 15 Jan 2020 13:15:21 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Feb 2020 00:21:42 GMT
ENV GOLANG_VERSION=1.14rc1
# Thu, 06 Feb 2020 00:28:10 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '4f714ebb1904b96e1a5fe551ba195d9bcef7a41706d5b34e377d0106020b3f04'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Feb 2020 00:28:12 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928afb74ac8a072334bcabee201bfbc0936217d2fa1e8aba5d7e377cb995f48a`  
		Last Modified: Wed, 15 Jan 2020 14:17:15 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d950deb3f160624c0675efc8314222a7ebb6a525dc9b4c667a022a3d796aa8b9`  
		Last Modified: Wed, 15 Jan 2020 14:17:14 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12bab48f96d12c3da7ce1da86d0aaf6d30c4ea98ca0eee9c0a6f61ce03a143ad`  
		Last Modified: Wed, 15 Jan 2020 14:17:11 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ad2d905ad861e3648e8b50913912b3c9e5e82ba47963995a5b04eaea4b2d5a`  
		Last Modified: Wed, 15 Jan 2020 14:17:11 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579b374cfb25041394c6240e13b17f10073fcbd5c0f48b368cbf62a60bce25df`  
		Last Modified: Wed, 15 Jan 2020 14:17:26 GMT  
		Size: 30.5 MB (30488416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2daa5fc01c4917b7d04ae05018cc91d5b73b43c628028ce489eb6e1b59e2415`  
		Last Modified: Wed, 15 Jan 2020 14:17:08 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91594379dcd19aa8896900708133e96d09286f185753d4f84e9e4b075f1077fb`  
		Last Modified: Wed, 15 Jan 2020 14:17:10 GMT  
		Size: 5.3 MB (5343427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c3843219eec4606158c8bf0d625e6de5e5e8cf8284b53855956c555697e929`  
		Last Modified: Thu, 06 Feb 2020 00:41:21 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbc7647294b03042949ed30751b6de781c99fe4390b981937f64df88d0650a3`  
		Last Modified: Thu, 06 Feb 2020 00:43:52 GMT  
		Size: 142.7 MB (142709617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47c81c928f1b5a28da7fdcd7f6a3b6e5a5bd66cbd18f36b8f72cf5782a7d714`  
		Last Modified: Thu, 06 Feb 2020 00:41:21 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
