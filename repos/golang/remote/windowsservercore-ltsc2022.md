## `golang:windowsservercore-ltsc2022`

```console
$ docker pull golang@sha256:8e7aa5720e472c215467055a89f226e3682da338cecc665d766997041c4cb7c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `golang:windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull golang@sha256:a46977dd539160d5d617e378c0276127ced153410fbaf1e9142aaeee0ccdeb15
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1954976247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13841d86c4aa30dae65b2ad45b32d8393dc2ba08eb5ad34969f1b9d18515f4f3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:19:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:19:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:20:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:20:18 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:20:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:20:42 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:22:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:23:01 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60407a49ce6121c65fa6399c333c5227a09518414fd987c460ea29cb441ac5a`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe632e8cddda4e5f347720b87b8b3868e2e2969048761e3b0a40799d33f5f7a`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4384696fc834e9658e7b3e5d1ceb1f8b362db85865daf29521b3c75c6999c046`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c794ea611ef69f54d577f90b68e165e40a17e43b6d1d08f59951a38e084ea5fb`  
		Last Modified: Wed, 11 Oct 2023 02:45:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c74dc2d701da2bfabc4d44e6a4e6b92912515e2ca1fb053ffcc6b0d5cae2972`  
		Last Modified: Wed, 11 Oct 2023 02:45:08 GMT  
		Size: 25.5 MB (25531724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91612399ba7df8de0a05ad078c3817548f0a3b44516b76565e14a96ea62452e9`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439c7c4353d2432c780827e4926910b19e84fe436d58e0a8129de2f631bd2b8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 264.4 KB (264384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b0eaedd98e739ace4b7934261c71292195e461adcc977d02e57604d4a42ee8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f46e84d4d007a200b1d6e7cb5b48db90116cdeb8bd3ec3964a08191875973e2`  
		Last Modified: Wed, 11 Oct 2023 02:45:25 GMT  
		Size: 69.3 MB (69325670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f59bab6d84ca44bbb60474dcf59c9af4f0f15edbdd64249b0eeaf968aff211f`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
