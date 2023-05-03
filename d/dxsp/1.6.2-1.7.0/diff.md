# Comparing `tmp/dxsp-1.6.2.tar.gz` & `tmp/dxsp-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.6.2.tar", max compression
+gzip compressed data, was "dxsp-1.7.0.tar", max compression
```

## Comparing `dxsp-1.6.2.tar` & `dxsp-1.7.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-05-02 07:22:08.485590 dxsp-1.6.2/LICENSE
--rw-r--r--   0        0        0     3225 2023-05-02 07:22:08.485590 dxsp-1.6.2/README.md
--rw-r--r--   0        0        0       38 2023-05-02 07:22:08.485590 dxsp-1.6.2/dxsp/.gitignore
--rw-r--r--   0        0        0      169 2023-05-02 07:22:09.341641 dxsp-1.6.2/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-02 07:22:08.489591 dxsp-1.6.2/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-02 07:22:08.489591 dxsp-1.6.2/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      392 2023-05-02 07:22:08.489591 dxsp-1.6.2/dxsp/config.py
--rw-r--r--   0        0        0      564 2023-05-02 07:22:08.489591 dxsp-1.6.2/dxsp/default_settings.toml
--rw-r--r--   0        0        0    29576 2023-05-02 07:22:08.489591 dxsp-1.6.2/dxsp/main.py
--rw-r--r--   0        0        0     1045 2023-05-02 07:22:09.341641 dxsp-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 dxsp-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-03 08:41:51.250782 dxsp-1.7.0/LICENSE
+-rw-r--r--   0        0        0     3225 2023-05-03 08:41:51.250782 dxsp-1.7.0/README.md
+-rw-r--r--   0        0        0       38 2023-05-03 08:41:51.250782 dxsp-1.7.0/dxsp/.gitignore
+-rw-r--r--   0        0        0      169 2023-05-03 08:41:51.982784 dxsp-1.7.0/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-03 08:41:51.250782 dxsp-1.7.0/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-03 08:41:51.250782 dxsp-1.7.0/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      392 2023-05-03 08:41:51.250782 dxsp-1.7.0/dxsp/config.py
+-rw-r--r--   0        0        0      556 2023-05-03 08:41:51.254782 dxsp-1.7.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    28666 2023-05-03 08:41:51.254782 dxsp-1.7.0/dxsp/main.py
+-rw-r--r--   0        0        0     1045 2023-05-03 08:41:51.982784 dxsp-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 dxsp-1.7.0/PKG-INFO
```

### Comparing `dxsp-1.6.2/LICENSE` & `dxsp-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.6.2/README.md` & `dxsp-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.6.2/dxsp/assets/blockchains.py` & `dxsp-1.7.0/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.6.2/dxsp/main.py` & `dxsp-1.7.0/dxsp/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,14 @@
                  block_explorer_api: str | None = None,
                  block_explorer_url: str | None = None,
                  rpc: str | None = None,
                  w3: Web3 | None = None,
                  protocol_type: str | None = None,
                  dex_exchange: str | None = None,
                  dex_router: str | None = None,
-                 base_trading_symbol: str = 'USDC',
                  amount_trading_option: int = 1,
                  ):
         """build a web3 object for swap"""
         self.logger = logging.getLogger(__name__)
         self.logger.info("DexSwap version: %s", __version__)
         self.logger.info("Initializing DexSwap for %s on %s", wallet_address, chain_id)
 
@@ -104,18 +103,16 @@
         else:
             self.router = self.dex_router
         self.logger.debug("self.router %s",self.router)
 
         self.name = "TBD"
         self.logger.debug("self.name %s",self.name)
 
-        self.base_trading_symbol = base_trading_symbol
-        if self.base_trading_symbol is None:
-            self.base_trading_symbol= 'USDC'
-        self.logger.debug("self.base_trading_symbol %s",self.base_trading_symbol)
+        self.trading_quote_ccy =  settings.trading_quote_ccy
+        self.logger.debug("self.trading_quote_ccy %s",self.trading_quote_ccy)
 
         self.amount_trading_option = amount_trading_option
         self.logger.debug("self.amount_trading_option %s",self.amount_trading_option)
 
         try:
             self.gecko_api = CoinGeckoAPI()
             assetplatform = self.gecko_api.get_asset_platforms()
@@ -141,15 +138,15 @@
     async def get_quote(
                 self,
                 symbol
             ):
         self.logger.debug("get_quote %s",symbol)
         asset_in_address = await self.search_contract(symbol)
         self.logger.debug("asset_in_address %s", asset_in_address)
-        asset_out_symbol = self.base_trading_symbol
+        asset_out_symbol = self.trading_quote_ccy
         asset_out_address = await self.search_contract(asset_out_symbol)
         self.logger.debug("asset_out_address %s",asset_out_address)
         if asset_out_address is None:
             self.logger.warning("No Valid Contract %s",symbol)
             return
         # asset_out_contract = await self.get_token_contract(asset_out_symbol)
         # asset_out_decimals = asset_out_contract.functions.decimals().call()
@@ -186,18 +183,22 @@
         ):
         """execute swap function"""
         try:
             self.logger.debug("execute_order %s %s %s",action,instrument, order_type)
             if order_type == 'swap':
                 self.logger.debug("execute_order %s",order_type)
 
-                asset_out_symbol = self.base_trading_symbol if action=="BUY" else instrument
-                asset_in_symbol = instrument if action=="BUY" else self.base_trading_symbol
+                asset_out_symbol = self.trading_quote_ccy if action=="BUY" else instrument
+                asset_in_symbol = instrument if action=="BUY" else self.trading_quote_ccy
                 asset_out_contract = await self.get_token_contract(asset_out_symbol)
-                asset_out_decimals = asset_out_contract.functions.decimals().call()
+                try:
+                    asset_out_decimals = asset_out_contract.functions.decimals().call()
+                except Exception as e:
+                    self.logger.error("execute_order decimals: %s", e)
+                    asset_out_decimals = 18
                 asset_out_balance = await self.get_token_balance(asset_out_symbol)
                 if amount_trading_option == 1:
                     #buy or sell %p percentage DEFAULT OPTION
                     asset_out_amount = ((asset_out_balance)/
                                         (10 ** asset_out_decimals))*(float(quantity)/100)
                 if amount_trading_option == 2:
                     #SELL all token in case of sell order for example
@@ -401,15 +402,15 @@
             return
 
     async def get_contract_address(
                             self,
                             token_list_url,
                             symbol
                         ):
-        """get token address from json list"""
+        """Given a token symbol and json format url address tokenlist, get token address"""
         self.logger.debug("get_contract_address %s %s",token_list_url, symbol)
         try:
             token_list = await self._get(token_list_url)
             token_search = token_list['tokens']
             for keyval in token_search:
                 if (keyval['symbol'] == symbol and keyval['chainId'] == self.chain_id):
                     return keyval['address']
@@ -417,15 +418,15 @@
             self.logger.debug("get_contract_address %s", e)
             return
 
     async def get_token_contract(
                                 self,
                                 token
                             ):
-        """get token contract (ABI+address)"""
+        """Given a token symbol, returns a contract object. """
         self.logger.debug("get_token_contract %s",token)
         try:
             token_address = await self.search_contract(token)
             token_abi = await self.get_abi(token_address)
             return self.w3.eth.contract(address=token_address, abi=token_abi)
         except Exception as e:
             self.logger.error("get_token_contract %s",e)
@@ -460,14 +461,16 @@
 
     async def get_sign(
                     self,
                     tx
                 ):
         self.logger.debug("get_sign %s", tx)
         try:
+            if not isinstance(tx, dict):
+                raise ValueError("Transaction must be a dictionary")
             if self.protocol_type in ['uniswap_v2','uniswap_v3']:
                 tx_params = {
                 'from': self.wallet_address,
                 'gas': await self.get_gas(tx),
                 'gasPrice': await self.get_gasPrice(tx),
                 'nonce': self.w3.eth.get_transaction_count(self.wallet_address),
                 }
@@ -477,55 +480,71 @@
                 tx['gas'] = await self.get_gas(tx)
                 tx['nonce'] = self.w3.eth.get_transaction_count(self.wallet_address)
                 tx['value'] = int(tx['value'])
                 tx['gasPrice'] = await self.get_gasPrice(tx)
             signed = self.w3.eth.account.sign_transaction(tx, self.private_key)
             raw_tx = signed.rawTransaction
             return self.w3.eth.send_raw_transaction(raw_tx)
+        except (ValueError, TypeError, KeyError) as e:
+            self.logger.error("get_sign: %s", e)
+            raise
         except Exception as e:
-            self.logger.error(" get_sign %s", e)
-            return
+            self.logger.error("get_sign: %s", e)
+            raise RuntimeError("Failed to sign transaction")
 
     async def get_gas(
                     self,
                     tx
                 ):
+        # Log the transaction
         self.logger.debug("get_gas %s",tx)
+        # Estimate the gas cost of the transaction
         gasestimate= self.w3.eth.estimate_gas(tx) * 1.25
+        # Return the estimated gas cost in wei
         return int(self.w3.to_wei(gasestimate,'wei'))
 
     async def get_gasPrice(self, tx):
+        '''
+        Get the gas price for a transaction
+        '''
         self.logger.debug("get_gasPrice %s", tx)
         gasprice = self.w3.eth.generate_gas_price()
         return self.w3.to_wei(gasprice,'gwei')
 
     async def get_abi(self,addr):
+        # Log a debug message to the logger
         self.logger.debug("get_abi %s", addr)
-        if self.block_explorer_api is None:
-            self.logger.warning("No block_explorer_api")
-        try:
-            params = {
-                "module": "contract",
-                "action": "getabi",
-                "address": addr,
-                "apikey": self.block_explorer_api }
-            headers = { "User-Agent": "Mozilla/5.0" }
-            resp = await self._get(url=self.block_explorer_url,params=params,headers=headers)
-            #self.logger.debug(f"resp {resp} status {resp['status']}")
-            if resp['status']=="1":
-                self.logger.debug("ABI found %s",resp)
-                abi = resp["result"]
-                return abi
-            self.logger.debug("No ABI identified Option B needed for contract %s on chain %s",addr,self.chain_id)
-            # https://github.com/tintinweb/smart-contract-sanctuary
-            #https://raw.githubusercontent.com/tintinweb/smart-contract-sanctuary-optimism/master/contracts/mainnet/1f/1F98431c8aD98523631AE4a59f267346ea31F984_UniswapV3Factory.sol
+        if self.block_explorer_api:
+            try:
+                # Create a dictionary of parameters
+                params = {
+                    "module": "contract",
+                    "action": "getabi",
+                    "address": addr,
+                    "apikey": self.block_explorer_api }
+                # Create a dictionary of headers
+                headers = { "User-Agent": "Mozilla/5.0" }
+                # Make a GET request to the block explorer URL
+                resp = await self._get(url=self.block_explorer_url,params=params,headers=headers)
+                # If the response status is 1, log the ABI
+                if resp['status']=="1":
+                    self.logger.debug("ABI found %s",resp)
+                    abi = resp["result"]
+                    return abi
+                # If no ABI is identified, log a warning
+                self.logger.warning("No ABI identified for contract %s on chain %s",addr,self.chain_id)
+            except Exception as e:
+                # Log an error
+                self.logger.error("error get_abi %s", e)
+                return
+        else:
+            # If no block_explorer_api is set, log a warning
+            self.logger.warning("No block_explorer_api. Option B needed TBD")
+            return 
 
-        except Exception as e:
-            self.logger.error("error get_abi %s", e)
-            return
 
 #####USERS RELATED
 
     # async def get_wallet_auth(self):
     #     try:
     #         return
     #     except Exception as e:
@@ -552,50 +571,46 @@
                 self.logger.warning("Invalid address %s for token %s: %s", self.wallet_address, token, e)
             # (ex.from_wei(await fetch_token_balance(basesymbol), 'ether'), 5)
             return 0 if token_balance <=0 else token_balance
         except Exception as e:
             self.logger.error("get_token_balance %s: %s",token, e)
             return 0
 
-    async def get_basecoin_balance(
+
+    async def get_quote_ccy_balance(
                                 self
                             ):
         try:
-            bal_base_trading_symbol = await self.get_token_balance(self.base_trading_symbol)
+            trading_quote_ccy_balance = await self.get_token_balance(self.trading_quote_ccy)
                 # return round(ex.from_wei(await fetch_token_balance(basesymbol), 'ether'), 5)
-            return bal_base_trading_symbol
+            return trading_quote_ccy_balance
             # bal = round(ex.from_wei(bal,'ether'),5)
         except Exception as e:
             self.logger.error("get_basecoin_balance %s: %s",token, e)
             return 0
 
     async def get_stablecoin_balance(
                                 self
                             ):
-        toptokens = ["USDT","USDC","BUSD","DAI"]
+        stablecoins = settings.stablecoins
         try:
-            for i in toptokens:
-                bal_toptoken = await self.get_token_balance(i)
-                if bal_toptoken:
-                    msg += f"\n💵{bal_toptoken} {i}"
+            for i in stablecoins:
+                bal_stablecoins = await self.get_token_balance(i)
+                if bal_stablecoins:
+                    msg += f"\n💵{bal_stablecoins} {i}"
                 # bal = round(ex.from_wei(bal,'ether'),5)
         except Exception as e:
             self.logger.error("get_stablecoin_balance error: %s", e)
             return 0
 
     async def get_account_balance(
                             self
                         ):
-        toptokens = ["USDT","USDC"]
         try:
-            for i in toptokens:
-                bal_toptoken = await self.get_token_balance(i)
-                if bal_toptoken:
-                    msg += f"\n💵{bal_toptoken} {i}"
-                    return msg
+            return self.w3.eth.get_balance(self.wallet_address)
         except Exception as e:
             self.logger.error("get_account_balance error: %s", e)
             return "balance error"
             # bal = round(ex.from_wei(bal,'ether'),5)
 
     async def get_account_position(
                             self
@@ -607,40 +622,7 @@
             # asset_position_contract = ex.eth.contract(address=asset_out_address, abi=asset_out_abi)
             # open_positions = asset_position_contract.functions.getOpenPositions(walletaddress).call()
             return
         except Exception as e:
             self.logger.error("get_account_position error: %s", e)
             return 0
 
-    # async def fetch_account_dex(addr):
-    #     url = block_explorer_url
-    #     query = {'module':'account',
-    #             'action':'tokenbalance',
-    #             'contractaddress':addr,
-    #             'address':walletaddress,
-    #             'tag':'latest',
-    #             'apikey':block_explorer_api}
-    #     r = requests.get(url, params=query)
-    #     try:
-    #         d = json.loads(r.text)
-    #     except:
-    #         return None
-    #     return int(d['result']) / self.zeroes
-
-#     async def fetch_gecko_asset_price(token):
-#     try:
-#         asset_in_address = ex.to_checksum_address(await search_contract(token))
-#         fetch_tokeninfo = gecko_api.get_coin_info_from_contract_address_by_id(id=f'{coin_platform}',contract_address=asset_in_address)
-#         return fetch_tokeninfo['market_data']['current_price']['usd']
-#     except Exception:
-#         return
-
-# async def fetch_gecko_quote(token):
-#     try:
-#         asset_in_address = ex.to_checksum_address(await search_contract(token))
-#         fetch_tokeninfo = gecko_api.get_coin_info_from_contract_address_by_id(id=f'{coin_platform}',contract_address=asset_in_address)
-#         logger.debug(msg=f"fetch_tokeninfo {fetch_tokeninfo}")
-#         asset_out_cg_quote = fetch_tokeninfo['market_data']['current_price']['usd']
-#         asset_out_cg_name = fetch_tokeninfo['name']
-#         return f"{asset_out_cg_name}\n🦎{asset_out_cg_quote} USD"
-#     except Exception:
-#         return
```

### Comparing `dxsp-1.6.2/pyproject.toml` & `dxsp-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.6.2"
+version = "1.7.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.6.2/PKG-INFO` & `dxsp-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.6.2
+Version: 1.7.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

