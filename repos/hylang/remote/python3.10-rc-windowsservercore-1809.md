## `hylang:python3.10-rc-windowsservercore-1809`

```console
$ docker pull hylang@sha256:2c58a4096d8c76f6801cfe5c841386473d5cc0174934db2b7d442ef02c69a51c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `hylang:python3.10-rc-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull hylang@sha256:8fc44e2c90fbf631b2c4d66a10a51e28bddbac78b4dc8d0a9906153abea8cd7c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2528804485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe9933c1314bf29d134df4c0c81af6a16b54529c2d86f4235114026a9342a0cb`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 12:14:23 GMT
ENV PYTHONIOENCODING=UTF-8
# Tue, 04 May 2021 17:14:18 GMT
ENV PYTHON_VERSION=3.10.0b1
# Tue, 04 May 2021 17:14:19 GMT
ENV PYTHON_RELEASE=3.10.0
# Tue, 04 May 2021 17:16:10 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Tue, 04 May 2021 17:16:11 GMT
ENV PYTHON_PIP_VERSION=21.1.1
# Tue, 04 May 2021 17:16:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1954f15b3f102ace496a34a013ea76b061535bd2/public/get-pip.py
# Tue, 04 May 2021 17:16:13 GMT
ENV PYTHON_GET_PIP_SHA256=f499d76e0149a673fb8246d88e116db589afbd291739bd84f2cd9a7bca7b6993
# Tue, 04 May 2021 17:17:05 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 04 May 2021 17:17:05 GMT
CMD ["python"]
# Tue, 04 May 2021 18:02:05 GMT
ENV HY_VERSION=1.0a1
# Tue, 04 May 2021 18:02:38 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Tue, 04 May 2021 18:02:39 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc61c4265bfe314fb772d57da4c3023d46cacdbdab9bb6fd5c475f11696dbab`  
		Last Modified: Wed, 14 Apr 2021 16:38:19 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed8a08b3d7d6a5bb1f638328427f3885d79bd0ebec83bfdc830f1bddf7ee5d4`  
		Last Modified: Tue, 04 May 2021 17:36:57 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc55bda221f1221069f3047a7f546f86d68f100047bf8d06ac66a712ca8f177`  
		Last Modified: Tue, 04 May 2021 17:36:57 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d98e7b713dddd7bc82fcd74be0cfc7e8ed551ce2edeef311f4f45ff5195de1`  
		Last Modified: Tue, 04 May 2021 17:37:06 GMT  
		Size: 51.4 MB (51428716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17ce7d627adb8abb27968a6b658758b12f1513137f14f1e84fb09705aeb4274`  
		Last Modified: Tue, 04 May 2021 17:36:54 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d7f44f57e1449f46196f815395178c106b115d3a77f531564ee3fc353acea3`  
		Last Modified: Tue, 04 May 2021 17:36:54 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026d1db9786d4bedd3a62a20d955acf4e8acabaaa6ba68672a587c8d83caae72`  
		Last Modified: Tue, 04 May 2021 17:36:54 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a46799ca1377c93a27e2ec735ce1e4502ff8e4a43b058f23dc928b98ae3c0a8`  
		Last Modified: Tue, 04 May 2021 17:36:56 GMT  
		Size: 6.4 MB (6394477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060e8ccd4503e39b637a3948ff0fc10859a2a52181c349860f50a2b0d6ba00cf`  
		Last Modified: Tue, 04 May 2021 17:36:54 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5407272a6b1eb6fd4c198a6eb6a8bea4e9d4ad04a61764700db0bd1ef4e74e7c`  
		Last Modified: Tue, 04 May 2021 18:06:31 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074912e657e5e9ebc294e8344ee2763da3a2c11e4fc2d8584e173669f4d06f47`  
		Last Modified: Tue, 04 May 2021 18:06:32 GMT  
		Size: 1.2 MB (1213562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9421ac263fe8ba727b35541f7430c8cbd9a1de99e606f7b0f35b9d7b06fae`  
		Last Modified: Tue, 04 May 2021 18:06:30 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
