## `golang:windowsservercore`

```console
$ docker pull golang@sha256:17fb18423573baba96ac3f50c89d5d3a94913a345a934f0d5535c71065e90e77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `golang:windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull golang@sha256:cdfdb150a871053728bad395d6cf9e5ee52833f9ea3dd655cf05536a43ebca5a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5912711649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29e3be67d672bf6c7bf8228ee14be39ceba994a6c272ebc98fe3d7db7273fef6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 12:12:16 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Jun 2020 12:12:17 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Jun 2020 12:12:18 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Jun 2020 12:12:19 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Jun 2020 12:14:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 12:14:02 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Jun 2020 12:15:24 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Jun 2020 12:15:26 GMT
ENV GOLANG_VERSION=1.14.4
# Wed, 10 Jun 2020 12:19:27 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e04f591219b18e7cabe73eb79c90405b5c7a5baee61377670d7a48429c5c978d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 12:19:30 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1e55345ed04421345a2308c193cd2b3ee2ea2d1d03c6aca6dca476e6ac5fdf`  
		Last Modified: Wed, 10 Jun 2020 12:38:10 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e28f74567e1ed23ec88993e7f0c8edb9457f0052976cafb0ba244f71acdafc`  
		Last Modified: Wed, 10 Jun 2020 12:38:09 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d9d2adaa155205462f0838c91c10c4c471332d52fd8f09d6715c18271fcd56`  
		Last Modified: Wed, 10 Jun 2020 12:38:06 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daaae427663ac308e774d70aea7aa07c3e014b28ac5ea82d8c5593464b90f7d4`  
		Last Modified: Wed, 10 Jun 2020 12:38:06 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfcb8713f2596697e43c935f45b92ea7e21bbaf614e7a5758bb82859da8fc361`  
		Last Modified: Wed, 10 Jun 2020 12:38:15 GMT  
		Size: 30.5 MB (30483933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f769368d71826b997fcf48fffc511465d99c1c40b9d4fe6f71db5dedc377a5`  
		Last Modified: Wed, 10 Jun 2020 12:38:03 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6abd64e1593c149cdeb68dc3419c4dacecfedb54f657cfbb6c7e8779fc6d47`  
		Last Modified: Wed, 10 Jun 2020 12:38:05 GMT  
		Size: 5.3 MB (5339850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ae98e25ac2c0694ae2e2a2e51bd58cd99dd2dba899ab59c11adf492358dc74`  
		Last Modified: Wed, 10 Jun 2020 12:38:03 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5c634042254bcb8b7e4c1a2f83e9449d69fe462ef2bf0832b353d86299b765`  
		Last Modified: Wed, 10 Jun 2020 12:38:38 GMT  
		Size: 142.9 MB (142880884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabd67027aaae95b37b0c84e93cebec5e79b76b74d960683c03a129336cd7f87`  
		Last Modified: Wed, 10 Jun 2020 12:38:03 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull golang@sha256:97be65ea5e80652fff8e308ed444990abf150b98fd17a18eb157ca3675531eeb
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2457403656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9d97a8384975990c1d33034206cbabee136e7eb33a3dd0682e15a209f94b02f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 12:19:44 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Jun 2020 12:19:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Jun 2020 12:19:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Jun 2020 12:19:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Jun 2020 12:20:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 12:20:46 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Jun 2020 12:21:13 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Jun 2020 12:21:14 GMT
ENV GOLANG_VERSION=1.14.4
# Wed, 10 Jun 2020 12:24:09 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e04f591219b18e7cabe73eb79c90405b5c7a5baee61377670d7a48429c5c978d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 12:24:11 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b790f53b49409310d5e5f84aafa67ecf3f801029d028f2383a1bce0e7296051`  
		Last Modified: Wed, 10 Jun 2020 12:39:06 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5938045b02a7c3de480eb236d21e5c3bd2c95368654607f5eeb09c078deaf5fb`  
		Last Modified: Wed, 10 Jun 2020 12:39:01 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2ff56298668ace8e86e8c3cfeb9aaf4eed3c7c795818a7316b68818a676df9`  
		Last Modified: Wed, 10 Jun 2020 12:39:01 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c28a7a94ded897831fae2d47b4b0d25fc4a23c83f2b813c780bba10ea0dffc9`  
		Last Modified: Wed, 10 Jun 2020 12:39:00 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c71422e9bd865eb6a68950b45bce1b787362a77001c73190ed464f3ec98160`  
		Last Modified: Wed, 10 Jun 2020 12:39:09 GMT  
		Size: 29.9 MB (29855740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745d65750fa9d6716d6da4d3120add523f01e2f4be76c104397bab7ef3987d1`  
		Last Modified: Wed, 10 Jun 2020 12:38:58 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae357110aaade3bc6ec34b6c50428ee596d5fccae736a8e49be51d956ebb354`  
		Last Modified: Wed, 10 Jun 2020 12:38:58 GMT  
		Size: 293.8 KB (293779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6563d686c30d1190a26f34da040b845db2f6cc29dc7143790d715c5a6b0479`  
		Last Modified: Wed, 10 Jun 2020 12:38:57 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0793edd5d188ffa53df6419c79382a09d11052dc5b9bd5580c068400b8936bfe`  
		Last Modified: Wed, 10 Jun 2020 12:39:28 GMT  
		Size: 133.3 MB (133330590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6adb0c46eb80f005673d91398b174f72976a7b6ab8f5dc521aa14ab48ae185b`  
		Last Modified: Wed, 10 Jun 2020 12:38:58 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
