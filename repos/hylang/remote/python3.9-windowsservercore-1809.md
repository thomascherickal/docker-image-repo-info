## `hylang:python3.9-windowsservercore-1809`

```console
$ docker pull hylang@sha256:6f406f439d66b4de77512f962202acf38cfdc058f54577ca103c1c76de62c82b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `hylang:python3.9-windowsservercore-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull hylang@sha256:3636249346207d8b844cb5e4bdfa9922842d208625dc29ba51e2ad06acf077aa
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2769091110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fd803bd85a75570afa2f6af837929de862d7faf2474e5b179794484bf781402`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 05:11:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Jan 2022 06:13:45 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 12 Jan 2022 15:24:01 GMT
ENV PYTHON_VERSION=3.9.9
# Wed, 12 Jan 2022 15:24:02 GMT
ENV PYTHON_RELEASE=3.9.9
# Wed, 12 Jan 2022 15:26:07 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 12 Jan 2022 15:26:08 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 12 Jan 2022 15:26:10 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 12 Jan 2022 15:26:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 12 Jan 2022 15:26:12 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 12 Jan 2022 15:27:36 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 12 Jan 2022 15:27:38 GMT
CMD ["python"]
# Wed, 12 Jan 2022 19:09:59 GMT
ENV HY_VERSION=1.0a4
# Wed, 12 Jan 2022 19:10:01 GMT
ENV HYRULE_VERSION=0.1
# Wed, 12 Jan 2022 19:11:15 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Wed, 12 Jan 2022 19:11:16 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3a70d5fd54e2005efbf590b48700ed40509210354a0d8f3f18c3b444a5325896`  
		Last Modified: Wed, 12 Jan 2022 06:20:33 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec0edebd1ddbb9c1b3b254bb09452f2077c1a30226af03c61c009222a6c5c1`  
		Last Modified: Wed, 12 Jan 2022 06:21:32 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18427ac6cd5e388983531e6f26ab541bee165d42c3a7207c1c5f0e2835bd7ea2`  
		Last Modified: Wed, 12 Jan 2022 15:29:28 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3298e8fd24e6a21efebb0f028aed2345083782cafa76f04fc8feff6375bfad0`  
		Last Modified: Wed, 12 Jan 2022 15:29:28 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02397a2971e2874b64d4373d4c21c91c96f1f3357d262468426e1576562bf5f6`  
		Last Modified: Wed, 12 Jan 2022 15:29:35 GMT  
		Size: 49.6 MB (49635757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fe15eda8b786e39254a6b1c17ae893e7ff5327c4a3ed60dc12d80a763ce47d`  
		Last Modified: Wed, 12 Jan 2022 15:29:28 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f93a70e0b0473694fa97435debc30853928513b4dbd47b1aa3222d81a75411`  
		Last Modified: Wed, 12 Jan 2022 15:29:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b4f30b3a1a52e094909497f69b02d8abba5859b99750c56ad69c4e66fc4faa`  
		Last Modified: Wed, 12 Jan 2022 15:29:25 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75cf99a91ba82c8ec4d767d08b8a9832af15e138cbab63ca323cae85df48ce8e`  
		Last Modified: Wed, 12 Jan 2022 15:29:25 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba045aea48273555945d370df31746a7fe78cd0a1cfb3bdf51938ca2bbac9ce1`  
		Last Modified: Wed, 12 Jan 2022 15:29:27 GMT  
		Size: 6.3 MB (6288698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399e1db00ad2115f4954491d7f8826f152b0624587d5ad2c68fd18b836fe6527`  
		Last Modified: Wed, 12 Jan 2022 15:29:25 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88d670d98095da26c95d89c34020f127ba1309d826cee94b5067d07828f6d33`  
		Last Modified: Wed, 12 Jan 2022 19:12:05 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2892e5bda60d51325b3c090a793ed499c39c2d748408b2952f0dd6e1b6dadf`  
		Last Modified: Wed, 12 Jan 2022 19:12:05 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e513e05c55738d26144c420d35e73750c46d5268d3b3b358d5df9fcc59c643ee`  
		Last Modified: Wed, 12 Jan 2022 19:12:05 GMT  
		Size: 918.8 KB (918797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14198e7d006ff961945285dc2eabf0720fd999fbd80e335a24f7fe9d6d332a69`  
		Last Modified: Wed, 12 Jan 2022 19:12:05 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
