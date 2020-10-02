# CouldIDE for Python Base on Docker and Jupyter

本工具利用 repo2docker(https://github.com/jupyter/repo2docker) 实现了云端IDE的部署和配置，通过浏览器即可在任意设备上实现Python的轻量级开发。

repo2docker在服务器端的配置在此不做赘述，仅就在 Binder(https://mybinder.org/) 平台上部署进行简易说明。

environment.yml、postBuild文件为基础环境配置，Pipfile、Pipfile.lock为所需库配置。

GitHub repository name or URL处填写GitHub代码仓库链接，后两项(Git branch, tag, or commit、Path to a notebook file (optional))为选填，填写完成并保存好下方自动生成的链接后即可进行Launch。

待部署完成后，使用自动生成的链接即可调用Docker生成Jupyter Notebook/Lab。

初次加载时可能较慢，待Docker部署完成后再次开启便无需长时间等待。

链接格式参考如下：

Jupyter Lab:
https://mybinder.org/v2/gh/edwillzy/CouldIDEdemo/master?urlpath=lab/tree/demo.ipynb

Jupyter Notebook:
https://mybinder.org/v2/gh/edwillzy/CouldIDEdemo/master?filepath=demo.ipynb

部署配置参考：https://github.com/wshuyi/demo-spacy-text-processing
