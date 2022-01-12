## `golang:windowsservercore-ltsc2016`

```console
$ docker pull golang@sha256:7ac89f46f0f9b4f7c8b6ee8905fb98b9580cf54ab7659c727717504e9538c0ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4886; amd64

### `golang:windowsservercore-ltsc2016` - windows version 10.0.14393.4886; amd64

```console
$ docker pull golang@sha256:6f0754f78696154649226d43f7e5b15549ed17dcb1ebb1b0280bd27e9f3116e6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6453808037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce978954ec9498e578ee29e9d6fcd065bb578f441f6b3fd1ed501b33e80c39a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:14:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 23:34:03 GMT
ENV GIT_VERSION=2.23.0
# Tue, 11 Jan 2022 23:34:05 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 11 Jan 2022 23:34:06 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 11 Jan 2022 23:34:07 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 11 Jan 2022 23:35:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:35:42 GMT
ENV GOPATH=C:\go
# Tue, 11 Jan 2022 23:36:45 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 11 Jan 2022 23:57:30 GMT
ENV GOLANG_VERSION=1.17.6
# Wed, 12 Jan 2022 00:01:53 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Jan 2022 00:01:55 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b5116c05ddf6ecb5a348f7628e3f3264afbb9909d86798316dbaff4a0e991a2`  
		Last Modified: Tue, 11 Jan 2022 19:35:13 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2caa59a1aaa1c092020bbca2ed4bb1396365f4d9d04ddbbd111ee689414c97a`  
		Last Modified: Wed, 12 Jan 2022 00:35:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9fe19533bf1afd7f80fd9cf407f00011eff59836d40dcceb1896e75ea99bf5`  
		Last Modified: Wed, 12 Jan 2022 00:35:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40700bafb918466fc1727b2e59ec5eb21d347affb09989cc72ac6db12220b882`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3180faaeb4219e7d41bb57faeebe12d142e8e246bac5ab81c8ef38499116de13`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6189cfcbd5a7447e171b486da44213e8ff4721ecbf15998668c0b32e6fb06aaa`  
		Last Modified: Wed, 12 Jan 2022 00:35:18 GMT  
		Size: 25.4 MB (25440280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4766ed70813b67e83228fa314c288fe9a1998bb85cbbd29f2a4b0518e49a7c15`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8f2e04b601edd119e847cbb2468052ab4681cd44bf4e9bbdf9b6c3f792d0ae`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 306.6 KB (306585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef103850c637e1ce1f8d175e0c4b5c7d6c2a3a29d2b8ad15bed8eab49be3dde0`  
		Last Modified: Wed, 12 Jan 2022 00:39:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1f406ac407910a0724e1fbad6ed8772a277ce69316a98a2defcebb5320504`  
		Last Modified: Wed, 12 Jan 2022 00:40:03 GMT  
		Size: 149.8 MB (149846909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdefe1352ad86026fe87510dd97f9a9acdbb5a700fc6a8aea2bd6eaa3194bd6`  
		Last Modified: Wed, 12 Jan 2022 00:39:28 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
