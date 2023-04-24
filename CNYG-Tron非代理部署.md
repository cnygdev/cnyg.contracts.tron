
1. 安装 TronLink 插件

https://chrome.google.com/webstore/detail/tronlink/ibnejdfjmmkpcnlpebklmnkoeoihofec

如果已安装请跳过

创建新钱包或导入钱包


2. 合约源代码合并到一个文件中

```
npx hardhat flatten ./contracts/TRX20CNYG.sol > TRX20CNYGToken.sol
```

3. 删除 TRX20CNYGToken.sol 文件中多余的 License

```
// SPDX-License-Identifier: MIT
```

只保留第一个，其他多余的要手工删除掉 或 批量替换掉

4. 合约在线部署

打开合约部署链接 

https://shasta.tronscan.org/#/contracts/contract-compiler

上传合约源文件 TRX20CNYGToken.sol 先编译成功后再部署合约

5. 合约在线验证

打开合约验证页面

https://shasta.tronscan.org/#/contracts/verify

上传合约源文件 TRX20CNYGToken.sol 填写合约相关信息 后提交即完成合约开源

