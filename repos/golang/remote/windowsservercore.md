## `golang:windowsservercore`

```console
$ docker pull golang@sha256:ecfcab7fe1f940879839db4c46ed7a7350d99d34e849f8931f3c1f7d86f59fc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.768; amd64
	-	windows version 10.0.17763.3046; amd64

### `golang:windowsservercore` - windows version 10.0.20348.768; amd64

```console
$ docker pull golang@sha256:cf9ffc87c29e1f1e72a74e714e58f00e55eed4c0acecf7fa5ea148cd46d8a5b2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2454538988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88f1be1d91d3ed48ba85d643b814e498e6368332dd9d166462074b0a03be213f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 12:59:27 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Jun 2022 12:59:28 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Jun 2022 12:59:29 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Jun 2022 12:59:30 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Jun 2022 13:00:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Jun 2022 13:00:09 GMT
ENV GOPATH=C:\go
# Wed, 15 Jun 2022 13:00:34 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 13:22:51 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 15 Jun 2022 13:26:24 GMT
RUN $url = 'https://dl.google.com/go/go1.18.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '9c46023f3ad0300fcfd1e62f2b6c2dfd9667b1f2f5c7a720b14b792af831f071'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 15 Jun 2022 13:26:30 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7048f11b6209d2acda097596ce39a045c853dcba86ce24e5bed476402b12d1d0`  
		Last Modified: Wed, 15 Jun 2022 14:00:00 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d26fbf7ef4512dc3318933ba5b640d2c7802c3371fbb68f53fce6eef4303835`  
		Last Modified: Wed, 15 Jun 2022 13:59:59 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c457edb674059e9735b53a34e6b1635d500b9b089dc489efcb97410a740d87ea`  
		Last Modified: Wed, 15 Jun 2022 13:59:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a8fabc4e5af370e2e22c99667d50e12e12dd44bed4029e99e2e59686b64fa1`  
		Last Modified: Wed, 15 Jun 2022 13:59:57 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d89b24afe1b4ba487a5b1aaf661f0657d45e45ad3c153afdd0dbe886b654dc`  
		Last Modified: Wed, 15 Jun 2022 14:00:26 GMT  
		Size: 25.7 MB (25717092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645ef2a4286ccdce10652b27b23e8dd1da9ceec350fcd644a8c9ea7fcaa83810`  
		Last Modified: Wed, 15 Jun 2022 13:59:55 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dfc5fb8baa33f74ede77c185e4add49ff88af6b7688c1524f4b6de6dd1200c`  
		Last Modified: Wed, 15 Jun 2022 13:59:56 GMT  
		Size: 564.7 KB (564666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a90f44b3f98639fe9acd670ecf726946783059a31e628fb5f521d2fe64c0cc6`  
		Last Modified: Wed, 15 Jun 2022 14:10:52 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a2c6db9bcc39d0e8a56d313b208134e5aa01829bfd366f35185d725b7d26b0`  
		Last Modified: Wed, 15 Jun 2022 14:13:36 GMT  
		Size: 149.8 MB (149781632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b764d3373935d4882e718ae2e528aa3b5b6ff6148a8a7b02514d46104474ec1`  
		Last Modified: Wed, 15 Jun 2022 14:10:52 GMT  
		Size: 1.6 KB (1583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:windowsservercore` - windows version 10.0.17763.3046; amd64

```console
$ docker pull golang@sha256:cbe8f5856e85ad134eec9e778abb3f4b50926e4a935afae9cace36adc3e6b58b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2838609712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ac029bf246c10c5e0279a9cdedc32478d38cdc19603f45614ad65cbb55e485c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 13:05:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Jun 2022 13:05:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Jun 2022 13:05:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Jun 2022 13:05:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Jun 2022 13:07:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Jun 2022 13:07:38 GMT
ENV GOPATH=C:\go
# Wed, 15 Jun 2022 13:08:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 13:26:50 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 15 Jun 2022 13:31:33 GMT
RUN $url = 'https://dl.google.com/go/go1.18.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '9c46023f3ad0300fcfd1e62f2b6c2dfd9667b1f2f5c7a720b14b792af831f071'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 15 Jun 2022 13:31:38 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48442d2d6c43c9ca54688a01fc5554bd98684b5cf9bc717a1de6d63231ce83e9`  
		Last Modified: Wed, 15 Jun 2022 14:03:13 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35ca04052013fb4f928e219adae33f54cd3d92c7005bf5c0ebf4193257bb5b5`  
		Last Modified: Wed, 15 Jun 2022 14:03:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42336b8b24c52353c57f25d3afadaf165e44f733997b4a7b87286a43ae510439`  
		Last Modified: Wed, 15 Jun 2022 14:03:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd68877abcf81c74a417cdbdeeacfcda7ee5779603340c4b2ea22cb5510df293`  
		Last Modified: Wed, 15 Jun 2022 14:03:11 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65b04147b3a88e0a38f9a0eb7df8bb43f51083025e450ae0654632c52ecac3c`  
		Last Modified: Wed, 15 Jun 2022 14:03:39 GMT  
		Size: 25.5 MB (25451380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f8ee078631a5ad5df9aa2753492c9d021a8304b47dd3794f8ee4ce2cb7d7bf`  
		Last Modified: Wed, 15 Jun 2022 14:03:08 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4a1089dccd62abd9be7c20d98b220cd26b863601bc3c72712caee252fda40d`  
		Last Modified: Wed, 15 Jun 2022 14:03:09 GMT  
		Size: 317.2 KB (317176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b7cdd00d622e1f3d0fdbbe6a3200cd213b3eaa76e5db78b449350e39d60da`  
		Last Modified: Wed, 15 Jun 2022 14:13:54 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ca78f6172a0ebf5d4ca715ab6108bbe8ec244c3f83066f98b1ac74b42ca5c8`  
		Last Modified: Wed, 15 Jun 2022 14:16:40 GMT  
		Size: 149.5 MB (149549844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b381fa791368290e8e99bd7830c547a4dc362efe81960b6fe80d5bef348736c0`  
		Last Modified: Wed, 15 Jun 2022 14:13:54 GMT  
		Size: 1.6 KB (1560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
