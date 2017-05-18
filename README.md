# [WIP] CodePush BSDiff for React Native

[中文文档](#中文文档)

*Note: This project is fully compatible with CodePush.   
So if you want to learn any details of CodePush, please visit [CodePush GitHub repo](https://github.com/Microsoft/react-native-code-push) to view the docs.*

## What's the differences between `CodePush BSDiff` and `CodePush`?

The original `CodePush` client supports differential updates, that means the end users will only download the files they need, which is great.   
But `CodePush BSDiff` takes a step forward, it allows user to download the `pieces` of the files they need rather than a whole file, which results in a __remarkable reduction in size__.   
Since the CodePush service provided by Microsoft does not support BSDiff, to achieve that, you have to host a [CodePush BSDiff server](https://github.com/o2team/code-push-bsdiff-server) which is open source with the BSDiff logic.   
According to our tests on a React Native starter app, the update sizes from MS CodePush service is `173KB` while the size from our server is less than `1KB`!   

## Supported React Native platforms

- iOS (7+)
- Android (4.1+)

This library supports React Native v0.43 and above since it's based on CodePush v2.0.   
Any we try our best to merge any commits from [upstream](https://github.com/Microsoft/react-native-code-push), so you won't miss any support and bugfix from MS CodePush.

## Getting Started

1. Host [code-push-bsdiff-server](https://github.com/o2team/code-push-bsdiff-server) on your server
> TODO

2. Create an account on that server
> TODO

3. Register your app with the service
> TODO

4. CodePush-ify your app
> TODO

5. Release an app update
> TODO

## Example App
> TODO

---
# 中文文档

*注意：该项目完全兼容 CodePush。   
所以如果你想了解 CodePush 的任何细节的话，请点击 [CodePush 项目仓库](https://github.com/Microsoft/react-native-code-push) 查阅文档学习。

## `CodePush BSDiff` 和 `CodePush` 有什么差别？

现有的 `CodePush` 客户端支持文件增量更新，即可以让用户只需下载他们所需的文件。   
但是 `CodePush BSDiff` 做得更多，在热更新过程中，它只会下载所需文件的缺失部分，而不是一整个文件。   
这将 __大幅度减小更新包的体积__。   
不过想要达到这个效果，你需要部署一个实现了 BSDiff 逻辑的 [开源 CodePush 服务器](https://github.com/o2team/code-push-bsdiff-server)。   
根据我们在一个新 RN 项目上的测试，更新包体积由原来的 `173KB` 下降到 `> 1KB`！    

## 支持的 React Native 平台

- iOS (7+)
- Android (4.1+)

该项目基于 CodePush v2.0，支持 React Native v0.43 以上的版本。   
我们会不定时合并 [MS CodePush](https://github.com/Microsoft/react-native-code-push) 的代码，所以你不用担心错过新版本的支持和其它 bugfix。

## 入门

1. 部署 [code-push-bsdiff-server](https://github.com/o2team/code-push-bsdiff-server) 到你的服务器上
> TODO

2. 在该服务器上创建一个账户
> TODO

3. 在该服务器上注册应用信息
> TODO

4. App 上安装 `CodePush BSDiff` 客户端
> TODO

5. 发布一个应用更新
> TODO

## 示例应用
> TODO

---

# Donation

If you find this project useful, you can buy us a cup of coffee:    

<a href="https://www.paypal.me/chuyik" target="blank">
<img width="200" src="https://storage.360buyimg.com/mtd/home/donate_paypal_min1495016435786.png" alt="">
</a><br>     

<img width="650" src="https://storage.360buyimg.com/mtd/home/donate_cn1495017701926.png" alt="">

## Acknowledgements
We are grateful to the authors of existing related projects for their ideas and collaboration:

- [@mendsley](https://github.com/mendsley/bsdiff)
- [@lisong](https://github.com/lisong)
- [@microsoft](https://github.com/Microsoft)

## Contributors
[![chuyik](https://avatars2.githubusercontent.com/u/6262943?v=3&s=120)](https://github.com/chuyik) |
:---:|
[chuyik](https://github.com/chuyik) |

