## `hylang:python3.9-windowsservercore-1809`

```console
$ docker pull hylang@sha256:c4b61e41468be0e361297f469999d0d8056475b2c598f5904cf8d05ce83c0794
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.2061; amd64

### `hylang:python3.9-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull hylang@sha256:fcc6a25c98fc07e42d718b87acdd914c6a3b2b4759567cbbf0ae0afe98309cfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742837544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865955fdfd266937bce5b224ea35b130eb6199a13491f923e5db51fc70014d22`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 04:03:01 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 14 Jul 2021 04:11:42 GMT
ENV PYTHON_VERSION=3.9.6
# Wed, 14 Jul 2021 04:11:44 GMT
ENV PYTHON_RELEASE=3.9.6
# Wed, 14 Jul 2021 04:13:35 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 14 Jul 2021 04:13:37 GMT
ENV PYTHON_PIP_VERSION=21.1.3
# Wed, 14 Jul 2021 04:13:40 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/a1675ab6c2bd898ed82b1f58c486097f763c74a9/public/get-pip.py
# Wed, 14 Jul 2021 04:13:42 GMT
ENV PYTHON_GET_PIP_SHA256=6665659241292b2147b58922b9ffe11dda66b39d52d8a6f3aa310bc1d60ea6f7
# Wed, 14 Jul 2021 04:15:05 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 14 Jul 2021 04:15:08 GMT
CMD ["python"]
# Wed, 14 Jul 2021 12:01:15 GMT
ENV HY_VERSION=1.0a3
# Wed, 14 Jul 2021 12:02:55 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Wed, 14 Jul 2021 12:02:58 GMT
CMD ["hy"]
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
	-	`sha256:47e4f5fed4f2af1e948afc1185311a87f00d191ab9a40187441583dd496a2e6c`  
		Last Modified: Wed, 14 Jul 2021 04:20:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6760e65c3e52b22561a1d641d9539e1219d09b73f7025046ef7ff5647cb16503`  
		Last Modified: Wed, 14 Jul 2021 04:23:10 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb021e07a2d4720ee0a82552d26d406e2000ccbf9a821f3c208f171b4f9787c`  
		Last Modified: Wed, 14 Jul 2021 04:23:10 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de2b35629b91d3e7b83d3c8e34c93713c26d09a124717003e1d6ccba9478356`  
		Last Modified: Wed, 14 Jul 2021 04:23:17 GMT  
		Size: 49.8 MB (49760590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1195291ae7e773701eba91a9b45a3ed1da88657732fe06c19749012073212b18`  
		Last Modified: Wed, 14 Jul 2021 04:23:08 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b23f912e6335ee4a91c65616f114d40d12830b1a7d7e734b413830fcba02bfd`  
		Last Modified: Wed, 14 Jul 2021 04:23:08 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ae038d8d764ce55ac7990a07e190d37612cec49a44458cfc233d4699411d55`  
		Last Modified: Wed, 14 Jul 2021 04:23:08 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236be1ae4a12a31fc0006916566aa51c2dd9e0e087a7343ff603e170c510432f`  
		Last Modified: Wed, 14 Jul 2021 04:23:10 GMT  
		Size: 6.3 MB (6279189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c3de3e6223ed51c34051392d7c401fb7bb93d926ca6eca0e77283632a96b2e`  
		Last Modified: Wed, 14 Jul 2021 04:23:08 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc90dc0b95e9759dd0f51af0dab1ac14d20caf6684d5318b026650904d8140b`  
		Last Modified: Wed, 14 Jul 2021 12:06:08 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ba7adc426d59d75efd4c7f1b8df36c34bd1bd0f8122e4112169ade9c5765f9`  
		Last Modified: Wed, 14 Jul 2021 12:06:09 GMT  
		Size: 1.3 MB (1337386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fb29190ca92c2619c62eb3bf755fea688bae8997fd3ca2bb4ce4c824cc16ea`  
		Last Modified: Wed, 14 Jul 2021 12:06:08 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
