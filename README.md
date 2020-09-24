![Image of DeFi Aggregator for Keep Network](https://keepswap.app/wp-content/uploads/2020/09/Keep-defi.png)

<h1>DeFi Aggregator for Keep tokens</h1> 

The KeepSwap Dex aggregator was created with the Totle infrastructure behind it and was only possible after the KEEP token was listed on the Totle exchange and after the offering of an exclusive API key, resources that were obtained directly from the Totle development team. The app brings some new advantages to the Keep Network community, such as: The innovative technology, developed by Totle, of token split between different Dexs offering better prices due to the decrease in the price range caused by lack of liquidity, an insurance offered by Nexus Mutual in the amount of the transaction with a limit of 600 ETH for cases in which money is lost due to an unforeseen bug and lower gas fees offered by the gas fee refund program offered in the integration with gastken.io
The platform is currently live at https://www.keepswap.app/

<h2>Outline</h2> 

* How it works
* Features and comparison
* Parameters for integration
* API Endpoints
* Conclusion

<h2>How it works</h2> 

The platform works with an exclusively API key obtained directly from the Totle team, which accesses the infrastructure resources of the decentralized exchange aggregator, thus obtaining the best market price available for swapping KEEP tokens, and has an unprecedented function of splitting the tokens to several dexs at the same time to reach the best possible transaction result for the user.

The Totle Exchange API list has dozens of integrated decentralized exchanges, and the token API list has more than 5600 tokens, all of these elements communicating with each other, making a dynamic bridge of the best possible result of these interactions for the user.

There is no custody of the user's tokens, and the swap process is completely transparent and compliant with the best existing technology and encryption standards. The swap takes place directly through the user's Metamask, only carrying out the transaction with the consent and approval of the user to do it so.

To access the Totle source code, you can refer this [link](https://github.com/TotlePlatform): 

![Image of the KeepSwap](https://keepswap.app/wp-content/uploads/2020/09/defi-aggregator.png)

<h2>Features and comparison</h2> 

* Splitting orders across multiple exchanges to get the best price
* Automatic insurance through Nexus Mutual
* Save more on gas than using a DEX natively with GasToken refunds
* Non-custodial, compliant, and transparent
* KEEP integrated along with +5600 other tokens

In addition to being able to have the best possible prices across all decentralized exchanges, users are covered for up to 600 ETH in the event that funds are lost during a swap due to an unforeseen bug.

The innovative technology of splitting orders simultaneously across multiple decentralized exchanges offers the best price for swapping tokens in the market, including in relation to other aggregators.

![Image of Comparation prices](https://keepswap.app/wp-content/uploads/2020/09/fgit.png)
Screenshot of price comparison between KeepSwap and 1Inch Exchange on 09/24/2020 at 19:00pm

<h2>Parameters for integration</h2>

The parameters below have been structured so that the application is pre-polluted when loaded to trade KEEP/USDT. The $api_key and $partnercontractaddress variables are confidential data, which can only be obtained directly from the Totle development team.


```

<script>
    const config = {
      sourceAssetAddress: "0x85eee30c52b0b379b046fb0f85f4f3dc3009afec",
      sourceAmountDecimal: null,
      destinationAssetAddress: "0xdac17f958d2ee523a2206206994597c13d831ec7",
      destinationAmountDecimal: null,
      apiKey: "'. $api_key .'",
      partnerContractAddress: "'. $contract_address .'",
    };
    const nodeId = "totle-widget";
    !function(){const t=document.createElement("script");t.type="text/javascript";const e=()=>{TotleWidget.default.run(config,document.getElementById(nodeId))};t.readyState?t.onreadystatechange=function(){"loaded"!=t.readyState&&"complete"!=t.readyState||(t.onreadystatechange=null,e())}:t.onload=function(){e()},t.src="https://widget.totle.com/latest/dist.js",document.getElementsByTagName("head")[0].appendChild(t)}();                                                                                                                                                      
</script>



```

<h2>API Endpoints</h2> 

Totle's API and Smart Contracts work together to split and route orders across the top DEXs.

<h3>Swap</h3> 

> Swap tokens at the best pricing available.

The endpoint allows you to trade one token for the equivalent value of another token. This can be used to trade single pairs or multiple pairs.

``
https://api.totle.com/swap
``

<h3>Pay</h3> 

> Execute a swap and a payment in a single transaction.

This endpoint allows payments to be made to a specified address.

``
https://api.totle.com/pay
``


<h3>Tokens</h3> 

> Retrieve information about tokens supported by Totle.

This endpoint returns a map of token names to contract addresses.

``
https://api.totle.com/tokens
``


<h3>Exchanges</h3> 

> Retrieve information about exchanges connected to Totle.

This endpoint returns a map of exchange names to exchange IDs. 

``
https://api.totle.com/exchanges
``


<h2>Conclusion</h2> 

The need for this decentralized DeFi aggregator for the Keep community is evident when the KEEP token is not listed yet in almost all of the Dexs yet, making room for scammers with the possibility of creating an erc20 with the same name with the objective to lure first-time users. In addition to this security issue, Totle is a very well-developed infrastructure platform with several unique and unprecedented features which makes KeepSwap stand out in relation to other DeFi aggregators.
