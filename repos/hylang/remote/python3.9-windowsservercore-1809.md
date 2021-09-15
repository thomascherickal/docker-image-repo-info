## `hylang:python3.9-windowsservercore-1809`

```console
$ docker pull hylang@sha256:f1d7fc406e90e1c70b68c7624201fb837d3b7aaa1a5a698f1919a6967c138b71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `hylang:python3.9-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull hylang@sha256:829502b5a320aba2ab685fa0deac89d08624bc8eda8064bcf4a2140de1eaf4c1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2744319918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa55eab6fd4555ea240f991e107543d764c7755f6b3579b6f6ba879c4a2b7ee`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 12:07:35 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 15 Sep 2021 15:57:43 GMT
ENV PYTHON_VERSION=3.9.7
# Wed, 15 Sep 2021 15:57:44 GMT
ENV PYTHON_RELEASE=3.9.7
# Wed, 15 Sep 2021 15:59:20 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 15 Sep 2021 15:59:21 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 15 Sep 2021 15:59:22 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 15 Sep 2021 15:59:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Wed, 15 Sep 2021 15:59:24 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Wed, 15 Sep 2021 16:00:35 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 15 Sep 2021 16:00:36 GMT
CMD ["python"]
# Wed, 15 Sep 2021 16:10:16 GMT
ENV HY_VERSION=1.0a3
# Wed, 15 Sep 2021 16:11:14 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Wed, 15 Sep 2021 16:11:15 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eede1d07a6fee928c279fb916d5d649410ceb4c386cdddc1247e3a68d7378ae`  
		Last Modified: Wed, 15 Sep 2021 12:13:19 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3ae927b7f3ad4436bd28a2fe745fefe0ed4bff1a0913a05b97e3f37baec742`  
		Last Modified: Wed, 15 Sep 2021 16:07:50 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bd2aa32e5bdaa4565de048f43c76764aef09eaae548a86aa410ace8f30816b`  
		Last Modified: Wed, 15 Sep 2021 16:07:50 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee0281b241303adeb40e6b68cf9c9c07850fc34ccae637d993ad88674caae01`  
		Last Modified: Wed, 15 Sep 2021 16:07:56 GMT  
		Size: 50.0 MB (49991960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050f1c80096ab9fab002dcbf86aba6725e4f04d7d871e88227d94b1aea4ae502`  
		Last Modified: Wed, 15 Sep 2021 16:07:49 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e35ade4478b8ef018231001c819b9a6fd729228385d1b94b72510b7c4be3dc`  
		Last Modified: Wed, 15 Sep 2021 16:07:47 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7afa823d940299a6b5f006c529cf4bccf320cd71b08f090e24852a8f9106db5`  
		Last Modified: Wed, 15 Sep 2021 16:07:47 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b75d6c808720a5f6c2c3102be01d69096061fa9a73da0c37a441ae78780e518`  
		Last Modified: Wed, 15 Sep 2021 16:07:47 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9ad4307752d107a8875563b7f175bddc5a1ed247581c8ee72cc4d636a742dd`  
		Last Modified: Wed, 15 Sep 2021 16:07:54 GMT  
		Size: 6.3 MB (6293211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473c7155ce970264232ab81c0bfcfb60988849fd35b62c3d0edf9da6c3391f8b`  
		Last Modified: Wed, 15 Sep 2021 16:07:47 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f76b6fe793e432907287c68b285e0e1d7abe2a1be22403a3af93fa86b5635c6`  
		Last Modified: Wed, 15 Sep 2021 16:14:40 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b32be5d655ad257097996d49a438f8b4f3b4f964264cebbe467c8410d8db93`  
		Last Modified: Wed, 15 Sep 2021 16:14:41 GMT  
		Size: 1.3 MB (1321641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:878f4ec69411016357b29a2096d8f94a914b3c1d0e7d6386e8a7b225cd3c3753`  
		Last Modified: Wed, 15 Sep 2021 16:14:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
