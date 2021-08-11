## `hylang:windowsservercore-1809`

```console
$ docker pull hylang@sha256:974e7951c75cb651e1cbd07b0c835ff1a53423a7c939b154d9e138a3dd070de7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `hylang:windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull hylang@sha256:e352b1f74ff5f00c0f50bf7cf9522a2aad6f9812da1a3e3c16d85a5ed43f82ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2743390300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fe110ab5adb7c6f899c4bc37c4dc59591ea35d0fd1272d2e5dabefc20ef26ff`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 12:23:09 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 11 Aug 2021 17:08:02 GMT
ENV PYTHON_VERSION=3.9.6
# Wed, 11 Aug 2021 17:08:05 GMT
ENV PYTHON_RELEASE=3.9.6
# Wed, 11 Aug 2021 17:10:20 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 17:10:24 GMT
ENV PYTHON_PIP_VERSION=21.2.3
# Wed, 11 Aug 2021 17:10:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Wed, 11 Aug 2021 17:10:30 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Wed, 11 Aug 2021 17:12:03 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 17:12:06 GMT
CMD ["python"]
# Wed, 11 Aug 2021 22:25:48 GMT
ENV HY_VERSION=1.0a3
# Wed, 11 Aug 2021 22:27:01 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Wed, 11 Aug 2021 22:27:04 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4881292935afd838255a98d792717471c7acc2a01fcf2ad09b21e588fd8567`  
		Last Modified: Wed, 11 Aug 2021 17:18:02 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65044140da47c6921a0b456b847c51d8a0be011662132e68df409d51797c43f9`  
		Last Modified: Wed, 11 Aug 2021 17:18:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5261836ebb755d69851c52b5b5d767eba7120bc7b2322834284f00007a473f`  
		Last Modified: Wed, 11 Aug 2021 17:18:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02578ae2653aef33c68ec66e83b05ae4cf370a81f69645009b15163cf73af9e`  
		Last Modified: Wed, 11 Aug 2021 17:19:00 GMT  
		Size: 49.8 MB (49751707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9b9ec05244694b9d42361ef6a5aa468b913f0a89199d2f5a1d8ee051b8c1df`  
		Last Modified: Wed, 11 Aug 2021 17:18:49 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9921a6da7bb67e36f4e5458659d1558b57852e55c220fdaf5ea393c5915f01f`  
		Last Modified: Wed, 11 Aug 2021 17:18:49 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00563a0e51836da52fc1da52a076b2c921b324ac244bb61fbb8faf53d0da42ab`  
		Last Modified: Wed, 11 Aug 2021 17:18:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72641ae1fc891a989c829b46f6baa4e8cec94d8c515d07515c598d3cb5666086`  
		Last Modified: Wed, 11 Aug 2021 17:18:52 GMT  
		Size: 6.3 MB (6302830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020450c65336029d233ae8a8e2d5c9d430041992cee7bdc7b9a726c8f6f87cf3`  
		Last Modified: Wed, 11 Aug 2021 17:18:49 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f453fa6a588a202ab52f18baea6469f4fe1e261f6f537a80cdcca3e10a75931`  
		Last Modified: Wed, 11 Aug 2021 22:29:36 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd3f9b6294582a43b1237f40b5c60d0e103361a61de30c3221cfff669955051`  
		Last Modified: Wed, 11 Aug 2021 22:29:40 GMT  
		Size: 1.3 MB (1323587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c119476bee86f6d042a9b1877c69167b0e8c55a39975e8f875092b1a0110f70a`  
		Last Modified: Wed, 11 Aug 2021 22:29:35 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
