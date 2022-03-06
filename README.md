# web3-terminal

I needed a web3 terminal from time to time and it was a pain opening nodejs or python terminal, then connecting to the RPC which needs to be dug up.<br>
Not speaking about ABI's and wallets 🤦‍♂️

Sooo... I configured this terminal 🙃

It's basically a very lightweight Javascript console as it uses `eval()`.<br>
See https://github.com/jcubic/jquery.terminal

• You get the `Big()` function to work with big-numbers (See big.js).<br>
• You get the w3 (web3) & eth (ethers) instances connected right away.<br>
• You get a wrapper function for interacting with contracts which by default loads the ABI's of ERC20, ERC721, ERC1155, UniswapRouterV2, UniswapFactoryV2, UniswapRouterV3 and UniswapFactoryV3 💪


NOTE: You can do complex operations with the objects you create from the "terminal" in the DevTools of the browser as you're working with global variable 😉


NOTE: If you try to print an object bigger than 16K it'll get truncated. If you really need that long print, run the following command before printing:
```
static_conf.MODE = 'full'
```
<br><br>
P.S.: For those of you who are not familiar with python, check out:
https://python.org/dev/peps/pep-0020
