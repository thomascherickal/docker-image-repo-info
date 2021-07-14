## `golang:windowsservercore`

```console
$ docker pull golang@sha256:4bd36aa5431535833c0d3eff621cd43b763d57072b92c88302863c2415a692d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `golang:windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull golang@sha256:e91d550081a50c8b79c924ecb88561182a543f0e98bf2bc90f59555c2bbc9b24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2850632211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bc96e7ec66b7dca10beffcf2c9cb7d75a1181cdf69266cd63793bb89aa7b3fd`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 04:25:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Jul 2021 04:25:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Jul 2021 04:25:48 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Jul 2021 04:25:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Jul 2021 04:27:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:27:07 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Jul 2021 04:28:09 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 04:42:39 GMT
ENV GOLANG_VERSION=1.16.6
# Wed, 14 Jul 2021 04:45:55 GMT
RUN $url = 'https://dl.google.com/go/go1.16.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c1132ba4e6263a1712355fb0745bf4f23e1602e1661c20f071e08bdcc5fe8db5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:45:59 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1c50202491861e9cc59ef0cad62ab13b4d8585699abaf13275f815b0ab53bf`  
		Last Modified: Wed, 14 Jul 2021 05:03:35 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700aac46fe704c190ed71a3f8ec8f1eca6d0fed9861862fcab96996d21678657`  
		Last Modified: Wed, 14 Jul 2021 05:03:32 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce5c766a8b7a15e6b68bef29d1932c4e9cf7086c6413acfcb35b89e6363813f`  
		Last Modified: Wed, 14 Jul 2021 05:03:32 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee3527d984880519c45793ad5f901d15605068f0a52a819044cd79ded461f09`  
		Last Modified: Wed, 14 Jul 2021 05:03:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064f16e3c9a35398857e96f60776b71b2af7e30419946307d58f942fe090b2f9`  
		Last Modified: Wed, 14 Jul 2021 05:04:02 GMT  
		Size: 25.5 MB (25460385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0876037206b7bfb610c4f7906510321d8255635221cabe7945218bd0e4d6675`  
		Last Modified: Wed, 14 Jul 2021 05:03:30 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e278916db542be6afd74117c73ed9743e7cdb1de94d1928e2ba00faeff6334e`  
		Last Modified: Wed, 14 Jul 2021 05:03:30 GMT  
		Size: 334.2 KB (334178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b10c3fa755eb4b8899c649883154bdfabb4d8210fd05c99501bd914ac9b731`  
		Last Modified: Wed, 14 Jul 2021 05:06:00 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a1c58792690c81eb4a6642c459efd28697c5ff8929b42470cee6a7e4082ee1`  
		Last Modified: Wed, 14 Jul 2021 05:06:35 GMT  
		Size: 139.4 MB (139379343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1825c045e930c77550f32b2d4b24f4fa8753d0cf7020f4c51ea28af9d52b89e`  
		Last Modified: Wed, 14 Jul 2021 05:06:00 GMT  
		Size: 1.6 KB (1575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull golang@sha256:d3d6d6de9966797abafa146074a5eb76bf0c5ea0d572b0a7e3c89e1913e8bc47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6439205169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f7ded715247709ed0c525093e0b54d30cd8ae2152bf56538b0c822487024a37`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 04:31:42 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Jul 2021 04:31:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Jul 2021 04:31:47 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Jul 2021 04:31:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Jul 2021 04:33:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:33:36 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Jul 2021 04:35:06 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 04:46:08 GMT
ENV GOLANG_VERSION=1.16.6
# Wed, 14 Jul 2021 04:49:49 GMT
RUN $url = 'https://dl.google.com/go/go1.16.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c1132ba4e6263a1712355fb0745bf4f23e1602e1661c20f071e08bdcc5fe8db5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:49:53 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f667c0fc8186714bfddbd565e9cdd1dd6497e3c112f1eddb17a37d1abae30c93`  
		Last Modified: Wed, 14 Jul 2021 05:04:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3566f190f34782035012abf2530315039000f1d137ad0098f1903a99127b3b8e`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036fdd63bb05506922a2462b2487bb4ff12b9c29097537ee7d0ca4c18cad7507`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8904dd19478585c0fa1c9b4a25c5ac4560759b61f3f9e2ef0e6475729d5d482`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a50006063e099df0e3d1f22baa504b0f0de1563cd642c48340cf2a8b7152bd`  
		Last Modified: Wed, 14 Jul 2021 05:04:30 GMT  
		Size: 25.4 MB (25447622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97445d6d1bd7224c109fda54abaaa5909b43be941934bc54c3aff8754b852ebd`  
		Last Modified: Wed, 14 Jul 2021 05:04:20 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0187f6db85279d8f0ab2b263b47845afa4452a66c28c251f571d776001e4d300`  
		Last Modified: Wed, 14 Jul 2021 05:04:21 GMT  
		Size: 318.8 KB (318791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a18e3af73fb6a22be9e13447c4dc03d831112dcc5d479c52c994c324b1bca`  
		Last Modified: Wed, 14 Jul 2021 05:06:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3b18fe05fb046103c962da798acc46523e448a87265015bd0e9870d49013e2`  
		Last Modified: Wed, 14 Jul 2021 05:07:32 GMT  
		Size: 143.8 MB (143795404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9eacae5fc4eee1b8807585646451e54ef2f58b632b6d045038d647606936b8f`  
		Last Modified: Wed, 14 Jul 2021 05:06:53 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
