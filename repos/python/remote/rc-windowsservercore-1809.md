## `python:rc-windowsservercore-1809`

```console
$ docker pull python@sha256:f9dbd4d0cde54345ca8bcc0bf747d00e86a4fb22d9896da3a087efeeaf3adcdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `python:rc-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull python@sha256:da3c9aeeb3986eead4c821fd387dfc01c8e3c76f37ac9eb80ec0c1c189a1a2cc
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2420836367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a24fab4f4e729b7228f22756825f78ebae5d1cadbd88a3ab48f03cfdcb53a97`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Oct 2020 00:19:36 GMT
ENV PYTHON_VERSION=3.10.0a1
# Wed, 07 Oct 2020 00:19:37 GMT
ENV PYTHON_RELEASE=3.10.0
# Wed, 07 Oct 2020 00:21:13 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 07 Oct 2020 00:21:14 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Wed, 07 Oct 2020 00:21:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Wed, 07 Oct 2020 00:21:16 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Wed, 07 Oct 2020 00:22:04 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 07 Oct 2020 00:22:05 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c53ce3d72987ee6f59f9d9ca885bd5c70f515c122270ebb9e41ea70e90f47da`  
		Last Modified: Wed, 07 Oct 2020 00:24:08 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bafd9792689a6405b847ae5195356e1853993a268a43b247e2d14734c942aa`  
		Last Modified: Wed, 07 Oct 2020 00:24:07 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848ab0360a80a05a17380d62376c0d2aabc454d572cb21c135997e0b143b135d`  
		Last Modified: Wed, 07 Oct 2020 00:24:17 GMT  
		Size: 57.8 MB (57812420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194f3dab056a607abf302c464f6c4cd5c0ab422a7a2c1ec0552664b289ae046`  
		Last Modified: Wed, 07 Oct 2020 00:24:04 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bdc4c36df8040bd4dd7b705b06278d78b36f0c42fa894be167eeedd14846a1`  
		Last Modified: Wed, 07 Oct 2020 00:24:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af18d91de147a29e5cd9559f9b74df4e70e490613cb9c387eeb6156c0bf8811`  
		Last Modified: Wed, 07 Oct 2020 00:24:04 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bcbf517e2da5eb3f034449833d2a27dd9e90e680daef95762ace0b81d2ef96e`  
		Last Modified: Wed, 07 Oct 2020 00:24:08 GMT  
		Size: 11.7 MB (11743749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6879a053a69cf3cd30d41e1ad7d06185c92d53f89cc6de8d914e9ccaccb0fc27`  
		Last Modified: Wed, 07 Oct 2020 00:24:05 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
