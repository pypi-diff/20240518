# Comparing `tmp/iop_python-0.1.0.tar.gz` & `tmp/iop_python-0.1.1.tar.gz`

## Comparing `iop_python-0.1.0.tar` & `iop_python-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 iop_python-0.1.0/Cargo.toml
--rw-r--r--   0      501       20     1653 2024-01-14 10:45:20.000000 iop_python-0.1.0/.github/workflows/build.yml
--rw-r--r--   0      501       20      696 2024-01-12 12:58:11.000000 iop_python-0.1.0/.gitignore
--rw-r--r--   0      501       20     1241 2023-12-19 13:18:04.000000 iop_python-0.1.0/README.md
--rw-r--r--   0      501       20        0 2023-12-19 12:30:00.000000 iop_python-0.1.0/api/__init__.py
--rw-r--r--   0      501       20    13565 2024-01-10 10:41:13.000000 iop_python-0.1.0/api/hydra.py
--rw-r--r--   0      501       20    16558 2024-01-14 07:02:42.000000 iop_python-0.1.0/buildozer.spec
--rw-r--r--   0      501       20  3725651 2024-01-14 09:39:05.000000 iop_python-0.1.0/iop_python-0.1.0-cp310-cp310-macosx_10_12_x86_64.whl
--rw-r--r--   0      501       20      639 2024-01-12 11:23:05.000000 iop_python-0.1.0/kivy.spec
--rw-r--r--   0      501       20    14725 2024-01-14 06:52:26.000000 iop_python-0.1.0/main.py
--rw-r--r--   0      501       20      679 2024-01-14 08:35:17.000000 iop_python-0.1.0/requirements.txt
--rw-r--r--   0      501       20      863 2023-12-30 15:31:46.000000 iop_python-0.1.0/script.py
--rw-r--r--   0      501       20     2074 2023-12-30 15:22:26.000000 iop_python-0.1.0/scripts/index.py
--rw-r--r--   0      501       20    10046 2024-01-12 13:28:24.000000 iop_python-0.1.0/src/lib.rs
--rw-r--r--   0      501       20      507 2024-01-11 14:14:01.000000 iop_python-0.1.0/test.py
--rw-r--r--   0      501       20    70862 2023-12-27 06:50:24.000000 iop_python-0.1.0/Cargo.lock
--rw-r--r--   0      501       20      391 2023-11-05 20:09:58.000000 iop_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1570 1970-01-01 00:00:00.000000 iop_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 iop_python-0.1.1/Cargo.toml
+-rw-r--r--   0      502       20      564 2024-05-18 15:38:53.000000 iop_python-0.1.1/.github/workflows/build.yml
+-rw-r--r--   0      502       20      709 2024-05-18 15:38:53.000000 iop_python-0.1.1/.gitignore
+-rw-r--r--   0      502       20      344 2024-05-18 15:38:53.000000 iop_python-0.1.1/Cross.toml
+-rw-r--r--   0      502       20      858 2024-05-18 15:38:53.000000 iop_python-0.1.1/Dockerfile
+-rw-r--r--   0      502       20     1241 2024-05-18 15:38:53.000000 iop_python-0.1.1/README.md
+-rw-r--r--   0      502       20        0 2024-05-18 15:38:53.000000 iop_python-0.1.1/api/__init__.py
+-rw-r--r--   0      502       20    13679 2024-05-18 15:38:53.000000 iop_python-0.1.1/api/hydra.py
+-rw-r--r--   0      502       20    16558 2024-05-18 15:38:53.000000 iop_python-0.1.1/buildozer.spec
+-rw-r--r--   0      502       20      639 2024-05-18 15:38:53.000000 iop_python-0.1.1/kivy.spec
+-rw-r--r--   0      502       20    14725 2024-05-18 15:38:53.000000 iop_python-0.1.1/main.py
+-rw-r--r--   0      502       20      546 2024-05-18 15:38:53.000000 iop_python-0.1.1/requirements.txt
+-rw-r--r--   0      502       20      864 2024-05-18 15:38:53.000000 iop_python-0.1.1/script.py
+-rw-r--r--   0      502       20     2074 2024-05-18 15:38:53.000000 iop_python-0.1.1/scripts/index.py
+-rw-r--r--   0      502       20    11155 2024-04-18 11:49:44.000000 iop_python-0.1.1/src/lib.rs
+-rw-r--r--   0      502       20      612 2024-05-18 15:38:53.000000 iop_python-0.1.1/test.py
+-rw-r--r--   0      502       20    72969 2024-05-18 15:38:53.000000 iop_python-0.1.1/Cargo.lock
+-rw-r--r--   0      502       20      391 2024-02-09 09:13:14.000000 iop_python-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1570 1970-01-01 00:00:00.000000 iop_python-0.1.1/PKG-INFO
```

### Comparing `iop_python-0.1.0/.gitignore` & `iop_python-0.1.1/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -66,7 +66,9 @@
 .idea/
 
 # VSCode
 .vscode/
 
 # Pyenv
 .python-version
+*/target
+core
```

### Comparing `iop_python-0.1.0/README.md` & `iop_python-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `iop_python-0.1.0/api/hydra.py` & `iop_python-0.1.1/api/hydra.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import iop_python as iop
 import requests
 import json
 import os
 
-#https://test.explorer.hydraledger.io/wallets/tdXxhgZV8aAGLL9CCJ4ry9AzTQZzRKqJ97
+#https://dev.explorer.hydraledger.tech/wallets/tdXxhgZV8aAGLL9CCJ4ry9AzTQZzRKqJ97
 
 # ---------------------------------------MileStone 2-----------------------------------------------------
 # |                                                                                                     |
 # |                                                                                                     |
 # |                                                                                                     |
 # |                                                                                                     |
 # |                                                                                                     |
@@ -32,29 +32,29 @@
 
     def verify_signed_statement(self,signed_statement):
         result = iop.verify_signed_statement(signed_statement)
         return result
         
     def verify_statement_with_did(self, signed_statement):
         did = json.loads(signed_statement)['content']['claim']['subject']
-        url = f"https://test.explorer.hydraledger.io:4705/morpheus/v1/did/{did}/document"
+        url = f"https://dev.explorer.hydraledger.tech:4705/morpheus/v1/did/{did}/document"
         response = requests.get(url)
         if response.status_code == 200:
             data = response.json()  # Assuming the response is in JSON format
             did_doc = json.dumps(data)
             result = iop.validate_statement_with_did(signed_statement,did_doc)
             return result
         
 
     def generate_nonce(self):
         nonce = iop.generate_nonce()
         return nonce
     
     def get_account_transactions(self,address):
-        url = f"https://test.explorer.hydraledger.io:4705/api/v2/wallets/{address}/transactions"
+        url = f"https://dev.explorer.hydraledger.tech:4705/api/v2/wallets/{address}/transactions"
         response = requests.get(url)
         if response.status_code == 200:
             data = response.json()  # Assuming the response is in JSON format
             return data['data']
         else:
             #print("Failed to fetch data. Status code:", response.status_code)
             return [] 
@@ -80,78 +80,78 @@
                 wallets = json.load(json_file)
                 return wallets
         except FileNotFoundError:
             print("user does not own any wallets")
             return []
         
     @classmethod
-    def generate_wallet(cls, password,phrase):
-        hyd_vault = iop.get_hyd_vault(phrase, password)
+    def generate_wallet(cls, password,phrase,network="devnet"):
+        hyd_vault = iop.get_hyd_vault(phrase, password,network)
         morpheus_vault = iop.get_morpheus_vault(phrase, password)
         h_vault = json.loads(hyd_vault)
         m_vault = json.loads(morpheus_vault)
         vaults = []
         vaults.append(h_vault) 
         vaults.append(m_vault)
         home_directory = os.path.expanduser("~")
         try:
             with open(cls.file_path, 'r') as file:
                 data = json.load(file)
                 data.append(vaults)
-            with open(home_directory+'/.hydra_wallet', 'w') as json_file:
+            with open(cls.file_path, 'w') as json_file:
                 json.dump(data, json_file,indent=2)
             return phrase
         except FileNotFoundError:
             myvault = []
             myvault.append(vaults)
-            f1 = os.open (home_directory+"/.hydra_wallet", os.O_CREAT, 0o700)
+            f1 = os.open (cls.file_path, os.O_CREAT, 0o700)
             os.close (f1)
             with open(home_directory+'/.hydra_wallet', 'a') as json_file:                
                 json.dump(myvault, json_file, indent=2)
             return phrase
     
     @classmethod
-    def get_new_acc_on_vault(cls,password, account=0):
+    def get_new_acc_on_vault(cls,password, account=0, network="devnet"):
         data = cls.load_wallets()
         if len(data) > 0:
             vault = data[account][0]
             new_account = vault['plugins'][-1]['parameters']['account']
             vault_data = json.dumps(vault)
-            new_wallet = iop.get_new_acc_on_vault(vault_data,password,new_account+1)
+            new_wallet = iop.get_new_acc_on_vault(vault_data,password,new_account+1,network)
             data[account][0] = json.loads(new_wallet)
             with open(cls.file_path, 'w') as json_file:                
                 json.dump(data, json_file, indent=2)
             return new_wallet
 
 
 
     @classmethod
-    def get_wallet_address(cls,account=0,key=0):
+    def get_wallet_address(cls,account=0,key=0,network="devnet"):
         data = cls.load_wallets()
         if len(data) > 0:
             vault = data[account][0]
             _params = vault['plugins'][0]['parameters']
             data = json.dumps(vault)
             params = json.dumps(_params)
-            addr = iop.get_wallet(data,key)
+            addr = iop.get_wallet(data,key,network)
             return addr
     
 
     @classmethod
     def generate_did(cls,password,account=0):
         file_content = cls.load_wallets()
         if len(file_content) > 0:
             vault = file_content[account][1]
             vault = json.dumps(vault)
             did = iop.generate_did_by_morpheus(vault, password)
             return(did)
 
 
-    def recover_wallet(cls,password,phrase):
-        vault = cls.generate_wallet(password,phrase)
+    def recover_wallet(cls,password,phrase,network='devnet'):
+        vault = cls.generate_wallet(password,phrase,network)
         return vault
 
     @classmethod
     def sign_witness_statement(cls,password, data,account=0):
         file_content = cls.load_wallets()
         if len(file_content) > 0:
             vault = file_content[account][1]
@@ -172,76 +172,76 @@
             "signature": signed_statement[0]
         }
         return json.dumps({"Signed contract":details}, indent=4)
 
 
     def get_nonce(cls,key=0):
         addr = cls.get_wallet_address(key=key)
-        url = f"https://test.explorer.hydraledger.io:4705/api/v2/wallets/{addr}"
+        url = f"https://dev.explorer.hydraledger.tech:4705/api/v2/wallets/{addr}"
         response = requests.get(url)
         if response.status_code == 200:
             data = response.json()  # Assuming the response is in JSON format
             nonce = int(data['data']['nonce'])
             return nonce
         else:
             print("Failed to fetch data. Status code:", response.status_code)   
 
             
-    def sign_transaction(cls,receiver,amount,password,account,key):
+    def sign_transaction(cls,receiver,amount,password,account,key,network):
         nonce = cls.get_nonce()
         vaults = cls.load_wallets()
         vault = vaults[account][0]
         _params = vault['plugins'][0]['parameters']
         data = json.dumps(vault)
         params = json.dumps(_params)
-        response = iop.generate_transaction(data,receiver,amount,nonce,password,key)
+        response = iop.generate_transaction(data,receiver,amount,nonce,password,key,network)
         signed_txs = json.loads(response)
         return signed_txs    
 
     #this function assumes that the wallet has made a transaction before
-    def send_transaction(self,receiver,amount,password,account=0,key=0):
+    def send_transaction(self,receiver,amount,password,account=0,key=0,network="devnet"):
         # Send a GET request to the URL
-        signed_txs = self.sign_transaction(receiver,amount,password,account,key)
-        url = "https://test.explorer.hydraledger.io:4705/api/v2/transactions"
+        signed_txs = self.sign_transaction(receiver,amount,password,account,key,network)
+        url = "https://dev.explorer.hydraledger.tech:4705/api/v2/transactions"
         res = requests.post(url, json=signed_txs)
         response = res.json()
         print(response)
         return response
 
 
     def check_transaction(self,txhash):
-        url = f"https://test.explorer.hydraledger.io:4705/api/v2/transactions/{txhash}"
+        url = f"https://dev.explorer.hydraledger.tech:4705/api/v2/transactions/{txhash}"
         res = requests.get(url)
         response = res.json()
         txid = response['data']['id']
         blockId = response['data']['blockId']
         fee = response['data']['fee']
         confirmations = response['data']['confirmations']
         time = response['data']['timestamp']['human']          
         return f"Transaction with id {txid} was sent successfully at {time} with a fee of {fee} Hyd and has {confirmations} confirmations"
 
     @classmethod   
     def display_address_balance(cls):
         addr = cls.get_wallet_address()
         if addr == None:
             return None
-        response = requests.get(f"https://test.explorer.hydraledger.io:4705/api/v2/wallets/{addr}")
+        response = requests.get(f"https://dev.explorer.hydraledger.tech:4705/api/v2/wallets/{addr}")
         if response.status_code == 200:
             data = response.json()
             balance = data['data']['balance']
             return balance
         else:
             #print("Failed to fetch data. Status code:", response.status_code) 
             return None 
 
     def get_account_transactions(cls):
         addr = cls.get_wallet_address()
         if addr == None:
             return None
-        url = f"https://test.explorer.hydraledger.io:4705/api/v2/wallets/{addr}/transactions"
+        url = f"https://dev.explorer.hydraledger.tech:4705/api/v2/wallets/{addr}/transactions"
         response = requests.get(url)
         if response.status_code == 200:
             data = response.json()  # Assuming the response is in JSON format
             return data['data']
         else:
             #print("Failed to fetch data. Status code:", response.status_code)
             return []
```

### Comparing `iop_python-0.1.0/buildozer.spec` & `iop_python-0.1.1/buildozer.spec`

 * *Files identical despite different names*

### Comparing `iop_python-0.1.0/kivy.spec` & `iop_python-0.1.1/kivy.spec`

 * *Files identical despite different names*

### Comparing `iop_python-0.1.0/main.py` & `iop_python-0.1.1/main.py`

 * *Files identical despite different names*

### Comparing `iop_python-0.1.0/script.py` & `iop_python-0.1.1/script.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "country": "Nigeria",
     "zipcode": "987554",
 
 }
 signed_witness_statement = wallet.generate_and_sign_statement(statement,"password")
 print(json.loads(signed_witness_statement))
 
+
 # Verify Signed Statement
 result = chain.verify_signed_statement(signed_witness_statement, False)
 print("The signed statement returned: ",result) #should always return true
 
 
 #sign a did statement with your did key
 # contractStr = "A long legal document, e.g. a contract with all details"
```

### Comparing `iop_python-0.1.0/scripts/index.py` & `iop_python-0.1.1/scripts/index.py`

 * *Files identical despite different names*

### Comparing `iop_python-0.1.0/src/lib.rs` & `iop_python-0.1.1/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,43 @@
+use iop_sdk::ciphersuite::secp256k1::Secp256k1;
 use iop_sdk::hydra::txtype::{
     hyd_core::Transaction, Aip29Transaction, CommonTransactionFields, OptionalTransactionFields,
 };
 use iop_sdk::vault::hydra::HydraSigner;
 use iop_sdk::{
-    ciphersuite::secp256k1::{hyd, SecpKeyId, SecpPrivateKey, SecpPublicKey},
+    ciphersuite::secp256k1::{hyd,SecpKeyId, SecpPrivateKey, SecpPublicKey},
     vault::{hydra, morpheus, Bip39, Vault},
 };
 use iop_sdk::{
     hydra::TransactionData,
     json_digest::Nonce264,
     morpheus::{crypto::SyncMorpheusSigner, data::DidDocument},
     vault::{hydra::Plugin, PublicKey},
 };
 use pyo3::prelude::*;
 use serde::{Deserialize, Serialize};
 use std::{error::Error, fmt::Display};
 
+
 //use pyo3::exceptions;
 use pyo3::panic::PanicException;
 //use iop_sdk::multicipher::MKeyId;
-//use iop_sdk::vault::{PrivateKey,Network,};
+//use iop_sdk::vault::{PrivateKey,Network as HydNetwork};
+use iop_sdk::vault::Network as HydNetwork;
 use iop_sdk::morpheus::crypto::{sign::PrivateKeySigner, Signed};
 use iop_sdk::morpheus::data::{Did, WitnessStatement};
 use iop_sdk::multicipher::MPublicKey;
 use iop_sdk::vault::morpheus::Private;
+use std::str::FromStr;
+use iop_sdk::ciphersuite::secp256k1::hyd::{Testnet,Mainnet};
 
 #[derive(Debug)]
 pub enum Err {
-    CouldNotSendTrsansaction,
+    CouldNotSendTransaction,
+    CouldNotMatchNetwork
 }
 
 
 
 #[derive(Serialize, Deserialize, Debug)]
 #[allow(non_snake_case)]
 pub struct Data {
@@ -60,20 +66,41 @@
 impl Error for Err {}
 
 #[derive(Serialize, Debug)]
 struct SendTxnsReq<'a> {
     transactions: Vec<&'a TransactionData>,
 }
 
+
+pub struct Network {
+    network: Box< dyn HydNetwork<Suite=Secp256k1>>
+}
+
+impl FromStr for Network {
+    type Err = Err;  
+    fn from_str(s:&str) -> Result<Self, Self::Err> {
+        match s.to_lowercase().as_str()
+         {
+            "testnet" => Ok(Self{network: Box::new(Testnet)}),
+            "mainnet" =>  Ok(Self{network: Box::new(Mainnet)}),
+            "devnet" =>  Ok(Self{network: Box::new(hyd::Devnet)}),
+            _ => Err(Err::CouldNotMatchNetwork),
+        }
+    }
+}
+
+
+
 #[pyfunction]
 #[allow(unused_variables)]
-pub fn get_hyd_vault(phrase: String, password: String) -> PyResult<String> {
+pub fn get_hyd_vault(phrase: String, password: String, network: String) -> PyResult<String> {
     let mut vault =
         Vault::create(None, phrase, &password, &password).expect("Vault could not be initialised");
-    let params = hydra::Parameters::new(&hyd::Testnet, 0);
+    let network = network.parse::<Network>().unwrap().network;
+    let params = hydra::Parameters::new(&*network, 0);
     hydra::Plugin::init(&mut vault, &password, &params).expect("plugin could not be initialised");
     let wallet = hydra::Plugin::get(&vault, &params).expect("wallet could not be initialized");
     let admin = serde_json::to_string_pretty(&vault).unwrap();
     let err = PanicException::new_err("This is an error");
     Ok(admin)
 }
 
@@ -98,30 +125,34 @@
 
 #[pyfunction]
 #[allow(unused_variables)]
 pub fn get_new_acc_on_vault(
     data: String,
     unlock_password: String,
     account: i32,
+    network: String
 ) -> PyResult<String> {
     let mut vault: Vault = serde_json::from_str(&data).unwrap();
-    let params = hydra::Parameters::new(&hyd::Testnet, account);
+    let network = Network::from_str(&network).unwrap().network;
+    let params = hydra::Parameters::new(&*network, account);
     Plugin::create(&mut vault, unlock_password, &params).expect("vault could not be created");
     let admin = serde_json::to_string_pretty(&vault).unwrap();
     Ok(admin)
 }
 
 #[allow(unused)]
-fn deserialize_hydra(
+fn deserialize_hydra<'a>(
     data: String,
     unlock_password: String,
     account: i32,
+    network: &'a str
 ) -> Result<(SecpPrivateKey, SecpPublicKey, SecpKeyId), ()> {
     let vault: Vault = serde_json::from_str(&data).unwrap();
-    let params = hydra::Parameters::new(&hyd::Testnet, account);
+    let network = Network::from_str(network).unwrap().network;
+    let params = hydra::Parameters::new(&*network, account);
     let wallet = hydra::Plugin::get(&vault, &params).expect("wallet could not be gotten");
     let wallet_private = wallet
         .private(&unlock_password)
         .expect("private struct could not be unwrapped")
         .key_mut(0)
         .expect("private key could not be unwrapped")
         .to_private_key();
@@ -219,43 +250,46 @@
 pub fn generate_transaction<'a>(
     data: String,
     receiver: String,
     amount: u64,
     nonce: u64,
     password: String,
     account: i32,
+    network: &'a str
 ) -> PyResult<String> {
     let mut transactions = Vec::new();
-    let signer = deserialize_hydra(data, password, account).unwrap();
-    let recipient_id = SecpKeyId::from_p2pkh_addr(receiver.as_str(), &hyd::Testnet).unwrap();
+    let signer = deserialize_hydra(data, password, account,network).unwrap();
+    let network = network.parse::<Network>().unwrap().network;
+    let recipient_id = SecpKeyId::from_p2pkh_addr(receiver.as_str(), &*network).unwrap();
     let nonce = nonce + 1;
     let optional = OptionalTransactionFields {
         amount,
         manual_fee: None,
         vendor_field: None,
     };
     let common_fields = CommonTransactionFields {
-        network: &hyd::Testnet,
+        network: &*network,
         sender_public_key: signer.1,
         nonce,
         optional,
     };
     let unsigned = Transaction::transfer(common_fields, &recipient_id);
     let mut signed = unsigned.to_data();
     signer.0.sign_hydra_transaction(&mut signed).unwrap();
     transactions.push(signed);
     let data = serde_json::to_string(&Transactions { transactions }).unwrap();
     Ok(data)
 }
 
 #[pyfunction]
 #[allow(unused_variables)]
-pub fn get_wallet(data: String, account: i32) -> PyResult<String> {
+pub fn get_wallet<'a>(data: String, account: i32, network: &'a str) -> PyResult<String> {
     let vault: Vault = serde_json::from_str(&data).unwrap();
-    let params = hydra::Parameters::new(&hyd::Testnet, account);
+    let network = network.parse::<Network>().unwrap().network;
+    let params = hydra::Parameters::new(&*network, account);
     let wallet = hydra::Plugin::get(&vault, &params).expect("wallet could not be gotten");
     let wallet_address = wallet.public().unwrap().key_mut(0).unwrap().to_p2pkh_addr();
     Ok(wallet_address)
 }
 
 #[pyfunction]
 pub fn validate_statement_with_did(data: &str, doc: &str) -> PyResult<String> {
@@ -283,8 +317,8 @@
     m.add_function(wrap_pyfunction!(get_hyd_vault, m)?)?;
     m.add_function(wrap_pyfunction!(get_new_acc_on_vault, m)?)?;
     m.add_function(wrap_pyfunction!(validate_statement_with_did, m)?)?;
    // m.add("VaultCouldNotBeUnwrapped", PanicException::new_err("VaultCouldNotBeUnwrapped") )?;
    
 
     Ok(())
-}
+}
```

### Comparing `iop_python-0.1.0/Cargo.lock` & `iop_python-0.1.1/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -57,17 +57,17 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.75"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4668cab20f66d8d020e1fbc0ebe47217433c1b6c8f2040faf858554e394ace6"
+checksum = "080e9890a082662b09c1ad45f567faeeb47f22b5fb23895fbe1e651e718e25ca"
 
 [[package]]
 name = "arrayref"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6b4930d2cb77ce62f89ee5d5289b4ac049559b1c45539271f5ed4fdc7db34545"
 
@@ -90,51 +90,51 @@
  "concurrent-queue",
  "event-listener 2.5.3",
  "futures-core",
 ]
 
 [[package]]
 name = "async-channel"
-version = "2.1.0"
+version = "2.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d37875bd9915b7d67c2f117ea2c30a0989874d0b2cb694fe25403c85763c0c9e"
+checksum = "1ca33f4bc4ed1babef42cad36cc1f51fa88be00420404e5b1e80ab1b18f7678c"
 dependencies = [
  "concurrent-queue",
- "event-listener 3.1.0",
+ "event-listener 4.0.3",
  "event-listener-strategy",
  "futures-core",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "async-executor"
-version = "1.6.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b0c4a4f319e45986f347ee47fef8bf5e81c9abc3f6f58dc2391439f30df65f0"
+checksum = "17ae5ebefcc48e7452b4987947920dac9450be1110cadf34d1b8c116bdbaf97c"
 dependencies = [
- "async-lock 2.8.0",
+ "async-lock 3.3.0",
  "async-task",
  "concurrent-queue",
  "fastrand 2.0.1",
- "futures-lite 1.13.0",
+ "futures-lite 2.2.0",
  "slab",
 ]
 
 [[package]]
 name = "async-global-executor"
-version = "2.3.1"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1b6f5d7df27bd294849f8eec66ecfc63d11814df7a4f5d74168a2394467b776"
+checksum = "05b1b633a2115cd122d73b955eadd9916c18c8f510ec9cd1686404c60ad1c29c"
 dependencies = [
- "async-channel 1.9.0",
+ "async-channel 2.1.1",
  "async-executor",
- "async-io 1.13.0",
- "async-lock 2.8.0",
+ "async-io 2.3.0",
+ "async-lock 3.3.0",
  "blocking",
- "futures-lite 1.13.0",
+ "futures-lite 2.2.0",
  "once_cell",
  "tokio",
 ]
 
 [[package]]
 name = "async-io"
 version = "1.13.0"
@@ -153,48 +153,47 @@
  "slab",
  "socket2 0.4.10",
  "waker-fn",
 ]
 
 [[package]]
 name = "async-io"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41ed9d5715c2d329bf1b4da8d60455b99b187f27ba726df2883799af9af60997"
+checksum = "fb41eb19024a91746eba0773aa5e16036045bbf45733766661099e182ea6a744"
 dependencies = [
- "async-lock 3.1.0",
+ "async-lock 3.3.0",
  "cfg-if",
  "concurrent-queue",
  "futures-io",
- "futures-lite 2.0.1",
+ "futures-lite 2.2.0",
  "parking",
- "polling 3.3.0",
- "rustix 0.38.24",
+ "polling 3.3.2",
+ "rustix 0.38.30",
  "slab",
  "tracing",
- "waker-fn",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "async-lock"
 version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "287272293e9d8c41773cec55e365490fe034813a2f172f502d6ddcf75b2f582b"
 dependencies = [
  "event-listener 2.5.3",
 ]
 
 [[package]]
 name = "async-lock"
-version = "3.1.0"
+version = "3.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deb2ab2aa8a746e221ab826c73f48bc6ba41be6763f0855cb249eb6d154cf1d7"
+checksum = "d034b430882f8381900d3fe6f0aaa3ad94f2cb4ac519b429692a1bc2dda4ae7b"
 dependencies = [
- "event-listener 3.1.0",
+ "event-listener 4.0.3",
  "event-listener-strategy",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "async-process"
 version = "1.8.1"
@@ -204,34 +203,34 @@
  "async-io 1.13.0",
  "async-lock 2.8.0",
  "async-signal",
  "blocking",
  "cfg-if",
  "event-listener 3.1.0",
  "futures-lite 1.13.0",
- "rustix 0.38.24",
- "windows-sys",
+ "rustix 0.38.30",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "async-signal"
 version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e47d90f65a225c4527103a8d747001fc56e375203592b25ad103e1ca13124c5"
 dependencies = [
- "async-io 2.2.0",
+ "async-io 2.3.0",
  "async-lock 2.8.0",
  "atomic-waker",
  "cfg-if",
  "futures-core",
  "futures-io",
- "rustix 0.38.24",
+ "rustix 0.38.30",
  "signal-hook-registry",
  "slab",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "async-std"
 version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62565bb4402e926b29953c785397c6dc0391b7b446e45008b0049eb43cec6f5d"
@@ -256,17 +255,17 @@
  "pin-utils",
  "slab",
  "wasm-bindgen-futures",
 ]
 
 [[package]]
 name = "async-task"
-version = "4.5.0"
+version = "4.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4eb2cdb97421e01129ccb49169d8279ed21e829929144f4a22a6e54ac549ca1"
+checksum = "fbb36e985947064623dbd357f727af08ffd077f93d696782f3c56365fa2e2799"
 
 [[package]]
 name = "atomic-waker"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1505bd5d3d116872e7271a6d4e16d81d0c8570876c8de68093a09ac269d8aac0"
 
@@ -301,17 +300,17 @@
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
 name = "base64"
-version = "0.21.5"
+version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "35636a1494ede3b646cc98f74f8e62c773a38a659ebc777a2cf26b9b74171df9"
+checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
 name = "base64ct"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6b4d9b1225d28d360ec6a231d65af1fd99a2a095154c8040689617290569c5c"
 
@@ -325,17 +324,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.1"
+version = "2.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "327762f6e5a765692301e5bb513e0d9fef63be86bbc14528052b1cd3e6f03e07"
+checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
 
 [[package]]
 name = "blake2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46502ad458c9a52b69d4d4d32775c788b7a1b85e8bc9d482d92250fc0e3f8efe"
 dependencies = [
@@ -362,20 +361,20 @@
 
 [[package]]
 name = "blocking"
 version = "1.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a37913e8dc4ddcc604f0c6d3bf2887c995153af3611de9e23c352b44c1b9118"
 dependencies = [
- "async-channel 2.1.0",
- "async-lock 3.1.0",
+ "async-channel 2.1.1",
+ "async-lock 3.3.0",
  "async-task",
  "fastrand 2.0.1",
  "futures-io",
- "futures-lite 2.0.1",
+ "futures-lite 2.2.0",
  "piper",
  "tracing",
 ]
 
 [[package]]
 name = "bumpalo"
 version = "3.14.0"
@@ -422,69 +421,66 @@
 checksum = "7f2c685bad3eb3d45a01354cedb7d5faa66194d1d58ba6e267a8de788f79db38"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "wasm-bindgen",
- "windows-targets",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "combine"
 version = "4.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "35ed6e9d84f0b51a7f52daf1c7d71dd136fd7a3f41a8462b8cdb8c78d920fad4"
 dependencies = [
  "bytes",
  "memchr",
 ]
 
 [[package]]
 name = "concurrent-queue"
-version = "2.3.0"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f057a694a54f12365049b0958a1685bb52d567f5593b355fbf685838e873d400"
+checksum = "d16048cd947b08fa32c24458a22f5dc5e835264f689f4f5653210c69fd107363"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "core-foundation"
-version = "0.9.3"
+version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
+checksum = "91e195e091a93c46f7102ec7818a2aa394e1e1771c3ab4825963fa03e45afb8f"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.4"
+version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
+checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.11"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce420fe07aecd3e67c5f910618fe65e94158f6dcc0adf44e00d69ce2bdfe0fd0"
+checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.16"
+version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
-dependencies = [
- "cfg-if",
-]
+checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
@@ -535,33 +531,33 @@
  "rand_core 0.5.1",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "data-encoding"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2e66c9d817f1720209181c316d28635c050fa304f9c79e47a520882661b7308"
+checksum = "7e962a19be5cfc3f3bf6dd8f61eb50107f356ad6270fbb3ed41476571db78be5"
 
 [[package]]
 name = "data-encoding-macro"
-version = "0.1.13"
+version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c904b33cc60130e1aeea4956ab803d08a3f4a0ca82d64ed757afac3891f2bb99"
+checksum = "20c01c06f5f429efdf2bae21eb67c28b3df3cf85b7dd2d8ef09c0838dac5d33e"
 dependencies = [
  "data-encoding",
  "data-encoding-macro-internal",
 ]
 
 [[package]]
 name = "data-encoding-macro-internal"
-version = "0.1.11"
+version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8fdf3fce3ce863539ec1d7fd1b6dcc3c645663376b43ed376bbf887733e4f772"
+checksum = "0047d07f2c89b17dd631c80450d69841a6b5d7fb17278cbc43d7e4cfcf2576f3"
 dependencies = [
  "data-encoding",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "digest"
@@ -613,17 +609,17 @@
 checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "env_logger"
-version = "0.10.0"
+version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85cdab6a89accf66733ad5a1693a4dcced6aeff64602b634530dd73c1f3ee9f0"
+checksum = "4cd405aab171cb85d6735e5c8d9db038c17d3ca007a4d2c25f337935c3d90580"
 dependencies = [
  "log",
  "regex",
 ]
 
 [[package]]
 name = "equivalent"
@@ -638,20 +634,20 @@
 checksum = "6c138974f9d5e7fe373eb04df7cae98833802ae4b11c24ac7039a21d5af4b26c"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "errno"
-version = "0.3.6"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c18ee0ed65a5f1f81cac6b1d213b69c35fa47d4252ad41f1486dbd8226fe36e"
+checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
  "libc",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "event-listener"
 version = "2.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0206175f82b8d6bf6652ff7d71a1e27fd2e4efde587fd368662814d6ec1d9ce0"
@@ -664,20 +660,31 @@
 dependencies = [
  "concurrent-queue",
  "parking",
  "pin-project-lite",
 ]
 
 [[package]]
+name = "event-listener"
+version = "4.0.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "67b215c49b2b248c855fb73579eb1f4f26c38ffdc12973e20e07b91d78d5646e"
+dependencies = [
+ "concurrent-queue",
+ "parking",
+ "pin-project-lite",
+]
+
+[[package]]
 name = "event-listener-strategy"
-version = "0.3.0"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d96b852f1345da36d551b9473fa1e2b1eb5c5195585c6c018118bc92a8d91160"
+checksum = "958e4d70b6d5e81971bebec42271ec641e7ff4e170a6fa605f2b8a8b65cb97d3"
 dependencies = [
- "event-listener 3.1.0",
+ "event-listener 4.0.3",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "fastrand"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -690,17 +697,17 @@
 name = "fastrand"
 version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
 
 [[package]]
 name = "fiat-crypto"
-version = "0.2.2"
+version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a481586acf778f1b1455424c343f71124b048ffa5f4fc3f8f6ae9dc432dcb3c7"
+checksum = "27573eac26f4dd11e2b1916c3fe1baa56407c83c71a773a8ba17ec0bca03b6b7"
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
@@ -717,68 +724,68 @@
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
 
 [[package]]
 name = "form_urlencoded"
-version = "1.2.0"
+version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
+checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "futures"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0290714b38af9b4a7b094b8a37086d1b4e61f2df9122c3cad2577669145335"
+checksum = "645c6916888f6cb6350d2550b80fb63e734897a8498abe35cfb732b6487804b0"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ff4dd66668b557604244583e3e1e1eada8c5c2e96a6d0d6653ede395b78bbacb"
+checksum = "eac8f7d7865dcb88bd4373ab671c8cf4508703796caa2b1985a9ca867b3fcb78"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb1d22c66e66d9d72e1758f0bd7d4fd0bee04cad842ee34587d68c07e45d088c"
+checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f4fb8693db0cf099eadcca0efe2a5a22e4550f98ed16aba6c48700da29597bc"
+checksum = "a576fc72ae164fca6b9db127eaa9a9dda0d61316034f33a0a0d4eda41f02b01d"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8bf34a163b5c4c52d0478a4d757da8fb65cabef42ba90515efee0f6f9fa45aaa"
+checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
 
 [[package]]
 name = "futures-lite"
 version = "1.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49a9d51ce47660b1e808d3c990b4709f2f415d928835a17dfd16991515c46bce"
 dependencies = [
@@ -789,50 +796,53 @@
  "parking",
  "pin-project-lite",
  "waker-fn",
 ]
 
 [[package]]
 name = "futures-lite"
-version = "2.0.1"
+version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3831c2651acb5177cbd83943f3d9c8912c5ad03c76afcc0e9511ba568ec5ebb"
+checksum = "445ba825b27408685aaecefd65178908c36c6e96aaf6d8599419d46e624192ba"
 dependencies = [
+ "fastrand 2.0.1",
  "futures-core",
+ "futures-io",
+ "parking",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "futures-macro"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53b153fd91e4b0147f4aced87be237c98248656bb01050b96bf3ee89220a8ddb"
+checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e36d3378ee38c2a36ad710c5d30c2911d752cb941c00c72dbabfb786a7970817"
+checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
 
 [[package]]
 name = "futures-task"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "efd193069b0ddadc69c46389b740bbccdd97203899b48d09c5f7969591d6bae2"
+checksum = "38d84fa142264698cdce1a9f9172cf383a0c82de1bddcf3092901442c4097004"
 
 [[package]]
 name = "futures-util"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a19526d624e703a3179b3d322efec918b6246ea0fa51d41124525f00f1cc8104"
+checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -861,41 +871,41 @@
  "cfg-if",
  "libc",
  "wasi 0.9.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.10"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
+checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "ghost"
-version = "0.1.16"
+version = "0.1.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef81e7cedce6ab54cd5dc7b3400c442c8d132fe03200a1be0637db7ef308ff17"
+checksum = "b0e085ded9f1267c32176b40921b9754c474f7dd96f7e808d4a982e48aa1e854"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.28.0"
+version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6fb8d784f27acf97159b40fc4db5ecd8aa23b9ad5ef69cdd136d3bc80665f0c0"
+checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "gloo-timers"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b995a66bb87bebce9a0f4a95aed01daca4872c050bfcb21653361c03bc35e5c"
 dependencies = [
@@ -903,54 +913,48 @@
  "futures-core",
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "h2"
-version = "0.3.21"
+version = "0.3.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "91fc23aa11be92976ef4729127f1a74adf36d8436f7816b185d18df956790833"
+checksum = "bb2c4422095b67ee78da96fbb51a4cc413b3b25883c7717ff7ca1ab31022c9c9"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
- "indexmap 1.9.3",
+ "indexmap",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.12.3"
+version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
-
-[[package]]
-name = "hashbrown"
-version = "0.14.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f93e7192158dbcda357bdec5fb5788eebf8bbac027f3f33e719d29135ae84156"
+checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.3"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d77f7ec81a6d05a3abb01ab6eb7590f6083d08449fe5a1c8b1e620283546ccb7"
+checksum = "5d3d0e0f38255e7fa3cf31335b3a56f05febd18025f4db5ef7a0cfb4f8da651f"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
@@ -993,17 +997,17 @@
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
 name = "http-body"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d5f38f16d184e36f2408a55281cd658ecbd3ca05cce6d6510a176eca393e26d1"
+checksum = "7ceab25649e9960c0311ea418d17bee82c0dcec1bd053b5f9a66e265a693bed2"
 dependencies = [
  "bytes",
  "http",
  "pin-project-lite",
 ]
 
 [[package]]
@@ -1016,30 +1020,30 @@
 name = "httpdate"
 version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "df3b46402a9d5adb4c86a0cf463f42e19994e3ee891101b1841f30a545cb49a9"
 
 [[package]]
 name = "hyper"
-version = "0.14.27"
+version = "0.14.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffb1cfd654a8219eaef89881fdb3bb3b1cdc5fa75ded05d6933b2b382e395468"
+checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
- "socket2 0.4.10",
+ "socket2 0.5.5",
  "tokio",
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
@@ -1053,17 +1057,17 @@
  "native-tls",
  "tokio",
  "tokio-native-tls",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.58"
+version = "0.1.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8326b86b6cff230b97d0d312a6c40a60726df3332e721f72a1b035f451663b20"
+checksum = "b6a67363e2aa4443928ce15e57ebae94fd8949958fd1223c4cfc0cd473ad7539"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows-core",
@@ -1076,40 +1080,30 @@
 checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "idna"
-version = "0.4.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
+checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
-dependencies = [
- "autocfg",
- "hashbrown 0.12.3",
-]
-
-[[package]]
-name = "indexmap"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d530e1a18b1cb4c484e6e34556a0d948706958449fca0cab753d649f2bce3d1f"
 dependencies = [
  "equivalent",
- "hashbrown 0.14.2",
+ "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
 version = "2.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
@@ -1137,15 +1131,15 @@
 name = "io-lifetimes"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
  "hermit-abi",
  "libc",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "iop-coeus-proto"
 version = "0.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "699c903118e20c039bc277335f05c1c24080d33f13199a7eeaab8851c0109e77"
@@ -1229,15 +1223,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9175c3508957accc44e4e3c49cade624398d7598cd122aa6ace9459a52c7f29"
 dependencies = [
  "anyhow",
  "blake2",
  "digest 0.10.7",
  "ed25519-dalek",
- "getrandom 0.2.10",
+ "getrandom 0.2.12",
  "hex",
  "hmac 0.12.1",
  "libsecp256k1",
  "multibase",
  "orion",
  "rand 0.8.5",
  "ripemd",
@@ -1280,15 +1274,15 @@
  "serde",
  "serde_bytes",
  "typetag",
 ]
 
 [[package]]
 name = "iop-python"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "async-std",
  "iop-sdk",
  "json-digest",
  "pyo3",
  "pyo3-asyncio",
  "reqwest",
@@ -1344,17 +1338,17 @@
 name = "ipnet"
 version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f518f335dce6725a761382244631d86cf0ccb2863413590b31338feb467f9c3"
 
 [[package]]
 name = "itoa"
-version = "1.0.9"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
+checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
 
 [[package]]
 name = "jni"
 version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6df18c2e3db7e453d3c6ac5b3e9d5182664d28788126d39b91f2d1e22b017ec"
 dependencies = [
@@ -1370,17 +1364,17 @@
 name = "jni-sys"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8eaf4bc02d17cbdd7ff4c7438cafcdf7fb9a4613313ad11b4f8fefe7d3fa0130"
 
 [[package]]
 name = "js-sys"
-version = "0.3.65"
+version = "0.3.67"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54c0c35952f67de54bb584e9fd912b3023117cbafc0a77d8f3dee1fb5f572fe8"
+checksum = "9a1d36f1235bc969acba30b7f5990b864423a6068a10f7c90ae8f0112e3a59d1"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "json-digest"
 version = "0.0.16"
@@ -1428,17 +1422,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.150"
+version = "0.2.152"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89d92a4743f9a61002fae18374ed11e7973f530cb3a3255fb354818118b2203c"
+checksum = "13e3bf6590cbc649f4d1a3eefc9d5d6eb746f5200ffb04e5e142700b8faa56e7"
 
 [[package]]
 name = "libsecp256k1"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95b09eff1b35ed3b33b877ced3a691fc7a481919c7e29c53c906226fcf55e2a1"
 dependencies = [
@@ -1488,17 +1482,17 @@
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.11"
+version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "969488b55f8ac402214f3f5fd243ebb7206cf82de60d3172994707a4bcc2b829"
+checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
@@ -1514,17 +1508,17 @@
 checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
 dependencies = [
  "value-bag",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.6.4"
+version = "2.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f665ee40bc4a3c5590afb1e9677db74a508659dfd71e126420da8274909a0167"
+checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
 
 [[package]]
 name = "memoffset"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
@@ -1544,21 +1538,21 @@
 checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.9"
+version = "0.8.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3dce281c5e46beae905d4de1870d8b1509a9142b62eedf18b443b011ca8343d0"
+checksum = "8f3d0b296e374a4e6f3c7b0a1f5a51d748a0d34c85e7dc48fc3fa9a87657fe09"
 dependencies = [
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "multibase"
 version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b3539ec3c1f04ac9748a260728e855f261b4977f5c3406612c884564f329404"
@@ -1614,40 +1608,40 @@
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "object"
-version = "0.32.1"
+version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cf5f9dd3933bd50a9e1f149ec995f39ae2c496d31fd772c1fd45ebc27e902b0"
+checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "opaque-debug"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "624a8340c38c1b80fd549087862da4ba43e08858af025b236e509b6649fc13d5"
 
 [[package]]
 name = "openssl"
-version = "0.10.59"
+version = "0.10.62"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a257ad03cd8fb16ad4172fedf8094451e1af1c4b70097636ef2eac9a5f0cc33"
+checksum = "8cde4d2d9200ad5909f8dac647e29482e07c3a35de8a13fce7c9c7747ad9f671"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.4.2",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
@@ -1656,28 +1650,28 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.95"
+version = "0.9.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "40a4130519a360279579c2053038317e40eff64d13fd3f004f9e1b72b8a6aaf9"
+checksum = "c1665caf8ab2dc9aef43d1c0023bd904633a6a05cb30b0ad59bec2ae986e57a7"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -1685,15 +1679,15 @@
 name = "orion"
 version = "0.17.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7abdb10181903c8c4b016ba45d6d6d5af1a1e2a461aa4763a83b87f5df4695e5"
 dependencies = [
  "ct-codecs",
  "fiat-crypto",
- "getrandom 0.2.10",
+ "getrandom 0.2.12",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "parking"
 version = "2.2.0"
@@ -1716,31 +1710,31 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "pbkdf2"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "83a0692ec44e4cf1ef28ca317f14f8f07da2d95ec3fa01f86e4467b725e60917"
 dependencies = [
  "digest 0.10.7",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.3.0"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
+checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
 
@@ -1759,68 +1753,68 @@
  "atomic-waker",
  "fastrand 2.0.1",
  "futures-io",
 ]
 
 [[package]]
 name = "pkg-config"
-version = "0.3.27"
+version = "0.3.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
+checksum = "2900ede94e305130c13ddd391e0ab7cbaeb783945ae07a279c268cb05109c6cb"
 
 [[package]]
 name = "polling"
 version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b2d323e8ca7996b3e23126511a523f7e62924d93ecd5ae73b333815b0eb3dce"
 dependencies = [
  "autocfg",
  "bitflags 1.3.2",
  "cfg-if",
  "concurrent-queue",
  "libc",
  "log",
  "pin-project-lite",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "polling"
-version = "3.3.0"
+version = "3.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e53b6af1f60f36f8c2ac2aad5459d75a5a9b4be1e8cdd40264f315d78193e531"
+checksum = "545c980a3880efd47b2e262f6a4bb6daad6555cf3367aa9c4e52895f69537a41"
 dependencies = [
  "cfg-if",
  "concurrent-queue",
  "pin-project-lite",
- "rustix 0.38.24",
+ "rustix 0.38.30",
  "tracing",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.69"
+version = "1.0.76"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "134c189feb4956b20f6f547d2cf727d4c0fe06722b20a0eec87ed445a97f92da"
+checksum = "95fc56cda0b5c3325f5fbbd7ff9fda9e02bb00bb3dac51252d2f1bfa1cb8cc8c"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.0"
+version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04e8453b658fe480c3e70c8ed4e3d3ec33eb74988bd186561b0cc66b85c3bc4b"
+checksum = "9a89dc7a5850d0e983be1ec2a463a171d20990487c3cfcd68b5363f1ee3d6fe0"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
@@ -1852,61 +1846,61 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.0"
+version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a96fe70b176a89cff78f2fa7b3c930081e163d5379b4dcdf993e3ae29ca662e5"
+checksum = "07426f0d8fe5a601f26293f300afd1a7b1ed5e78b2a705870c5f30893c5163be"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.0"
+version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "214929900fd25e6604661ed9cf349727c8920d47deff196c4e28165a6ef2a96b"
+checksum = "dbb7dec17e17766b46bca4f1a4215a85006b4c2ecde122076c562dd058da6cf1"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.0"
+version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dac53072f717aa1bfa4db832b39de8c875b7c7af4f4a6fe93cdbf9264cf8383b"
+checksum = "05f738b4e40d50b5711957f142878cfa0f28e054aa0ebdfc3fd137a843f74ed3"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.0"
+version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7774b5a8282bd4f25f803b1f0d945120be959a36c72e08e7cd031c792fdfd424"
+checksum = "0fc910d4851847827daf9d6cdd4a823fbdaab5b8818325c5e97a86da79e8881f"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.33"
+version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
+checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.7.3"
@@ -1962,15 +1956,15 @@
 
 [[package]]
 name = "rand_core"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
- "getrandom 0.2.10",
+ "getrandom 0.2.12",
 ]
 
 [[package]]
 name = "rand_hc"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca3129af7b92a17112d59ad498c6f81eaf463253766b90396d39ea7a39d6613c"
@@ -2014,19 +2008,19 @@
 name = "regex-syntax"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
 
 [[package]]
 name = "reqwest"
-version = "0.11.22"
+version = "0.11.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "046cd98826c46c2ac8ddecae268eb5c2e58628688a5fc7a2643704a73faba95b"
+checksum = "37b1ae8d9ac08420c66222fb9096fc5de435c3c48542bc5336c51892cffafb41"
 dependencies = [
- "base64 0.21.5",
+ "base64 0.21.7",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
@@ -2082,52 +2076,52 @@
 checksum = "fea8ca367a3a01fe35e6943c400addf443c0f57670e6ec51196f71a4b8762dd2"
 dependencies = [
  "bitflags 1.3.2",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys 0.3.8",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.24"
+version = "0.38.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ad981d6c340a49cdc40a1028d9c6084ec7e9fa33fcb839cab656a267071e234"
+checksum = "322394588aaf33c24007e8bb3238ee3e4c5c09c084ab32bc73890b99ff326bca"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.4.2",
  "errno",
  "libc",
- "linux-raw-sys 0.4.11",
- "windows-sys",
+ "linux-raw-sys 0.4.13",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.15"
+version = "1.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
+checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "schannel"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c3733bf4cf7ea0880754e19cb5a462007c4a8c1914bff372ccc95b464f1df88"
+checksum = "fbc91545643bcf3a0bbb6569265615222618bdf33ce4ffbbd13c4bbd4c093534"
 dependencies = [
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
@@ -2153,62 +2147,62 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.192"
+version = "1.0.195"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bca2a08484b285dcb282d0f67b26cadc0df8b19f8c12502c13d966bf9482f001"
+checksum = "63261df402c67811e9ac6def069e4786148c4563f4b50fd4bf30aa370d626b02"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
-version = "0.11.12"
+version = "0.11.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab33ec92f677585af6d88c65593ae2375adde54efdbf16d597f2cbc7a6d368ff"
+checksum = "8b8497c313fd43ab992087548117643f6fcd935cbf36f176ffda0aacf9591734"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.192"
+version = "1.0.195"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d6c7207fbec9faa48073f3e3074cbe553af6ea512d7c21ba46e434e70ea9fbc1"
+checksum = "46fe8f8603d81ba86327b23a2e9cdf49e1255fb94a4c5f297f6ee0547178ea2c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.108"
+version = "1.0.111"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1c7e3eac408d115102c4c24ad393e0821bb3a5df4d506a80f85f7a742a526b"
+checksum = "176e46fa42316f18edd598015a5166857fc835ec732f5215eac6b7bdbf0a84f4"
 dependencies = [
- "indexmap 2.1.0",
+ "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_repr"
-version = "0.1.17"
+version = "0.1.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3081f5ffbb02284dda55132aa26daecedd7372a42417bbbab6f14ab7d6bb9145"
+checksum = "0b2e6b945e9d3df726b65d6ee24060aff8e3533d431f677a9695db04eff9dfdb"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "serde_str"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a26e850fb9dfec51e9fea9dd582030761a4ef011d31b32d904f740961bd16a48"
@@ -2274,17 +2268,17 @@
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.11.1"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "942b4a808e05215192e39f4ab80813e599068285906cc91aa64f923db842bd5a"
+checksum = "2593d31f82ead8df961d8bd23a64c2ccf2eb5dd34b0a34bfb4dd54011c72009e"
 
 [[package]]
 name = "socket2"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f7916fc008ca5542385b89a3d3ce689953c143e9304a9bf8beec1de48994c0d"
 dependencies = [
@@ -2295,15 +2289,15 @@
 [[package]]
 name = "socket2"
 version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
 dependencies = [
  "libc",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
@@ -2317,17 +2311,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.38"
+version = "2.0.48"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e96b79aaa137db8f61e26363a0c9b47d8b4ec75da28b7d1d614c2303e232408b"
+checksum = "0f3531638e407dfc0814761abb7c00a5b54992b849452a0646b7f65c9f770f3f"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2349,49 +2343,49 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.12"
+version = "0.12.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c39fd04924ca3a864207c66fc2cd7d22d7c016007f9ce846cbb9326331930a"
+checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
 
 [[package]]
 name = "tempfile"
-version = "3.8.1"
+version = "3.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ef1adac450ad7f4b3c28589471ade84f25f731a7a0fe30d71dfa9f60fd808e5"
+checksum = "01ce4141aa927a6d1bd34a041795abd0db1cccba5d5f24b009f694bdf3a1f3fa"
 dependencies = [
  "cfg-if",
  "fastrand 2.0.1",
  "redox_syscall",
- "rustix 0.38.24",
- "windows-sys",
+ "rustix 0.38.30",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.50"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9a7210f5c9a7156bb50aa36aed4c95afb51df0df00713949448cf9e97d382d2"
+checksum = "d54378c645627613241d077a3a79db965db602882668f9136ac42af9ecb730ad"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.50"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "266b2e40bc00e5a6c09c3584011e08b06f123c00362c92b975ba9843aaaa14b8"
+checksum = "fa0faa943b50f3db30a20aa7e265dbc66076993efed8463e8de414e5d06d3471"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "tiny-bip39"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62cc94d358b5a1e84a5cb9109f559aa3c4d634d2b1b4de3d0fa4adc7c78e2861"
@@ -2431,26 +2425,26 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.34.0"
+version = "1.35.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0c014766411e834f7af5b8f4cf46257aab4036ca95e9d2c144a10f59ad6f5b9"
+checksum = "c89b4efa943be685f629b149f53829423f8f5531ea21249408e8e2f8671ec104"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
  "socket2 0.5.5",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -2496,17 +2490,17 @@
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "try-lock"
-version = "0.2.4"
+version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3528ecfd12c466c6f163363caf2d02a71161dd5e1cc6ae7b34207ea2d42d81ed"
+checksum = "e421abadd41a4225275504ea4d6566923418b7f05506fbc9c0fe86ba7396114b"
 
 [[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
@@ -2532,17 +2526,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.13"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
+checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
@@ -2559,28 +2553,28 @@
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "url"
-version = "2.4.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "143b538f18257fac9cad154828a57c6bf5157e1aa604d4816b5995bf6de87ae5"
+checksum = "31e6302e3bb753d46e83516cae55ae196fc0c309407cf11ab35cc51a4c2a4633"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "value-bag"
-version = "1.4.2"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4a72e1902dde2bd6441347de2b70b7f5d59bf157c6c62f0c44572607a1d55bbe"
+checksum = "7cdbaf5e132e593e9fc1de6a15bbec912395b11fb9719e061cf64f804524c503"
 
 [[package]]
 name = "varint"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c37be5674e0be9c72790681999b0e6f09f03d3fc5d8904cfe2db615aad65887b"
 dependencies = [
@@ -2634,83 +2628,83 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.88"
+version = "0.2.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7daec296f25a1bae309c0cd5c29c4b260e510e6d813c286b19eaadf409d40fce"
+checksum = "b1223296a201415c7fad14792dbefaace9bd52b62d33453ade1c5b5f07555406"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.88"
+version = "0.2.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e397f4664c0e4e428e8313a469aaa58310d302159845980fd23b0f22a847f217"
+checksum = "fcdc935b63408d58a32f8cc9738a0bffd8f05cc7c002086c6ef20b7312ad9dcd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.48",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.38"
+version = "0.4.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9afec9963e3d0994cac82455b2b3502b81a7f40f9a0d32181f7528d9f4b43e02"
+checksum = "bde2032aeb86bdfaecc8b261eef3cba735cc426c1f3a3416d1e0791be95fc461"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.88"
+version = "0.2.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5961017b3b08ad5f3fe39f1e79877f8ee7c23c5e5fd5eb80de95abc41f1f16b2"
+checksum = "3e4c238561b2d428924c49815533a8b9121c664599558a5d9ec51f8a1740a999"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.88"
+version = "0.2.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5353b8dab669f5e10f5bd76df26a9360c748f054f862ff5f3f8aae0c7fb3907"
+checksum = "bae1abb6806dc1ad9e560ed242107c0f6c84335f1749dd4e8ddb012ebd5e25a7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.48",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.88"
+version = "0.2.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d046c5d029ba91a1ed14da14dca44b68bf2f124cfbaf741c54151fdb3e0750b"
+checksum = "4d91413b1c31d7539ba5ef2451af3f0b833a005eb27a631cec32bc0635a8602b"
 
 [[package]]
 name = "web-sys"
-version = "0.3.65"
+version = "0.3.67"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5db499c5f66323272151db0e666cd34f78617522fb0c1604d31a27c50c206a85"
+checksum = "58cd2333b6e0be7a39605f0e255892fd7418a682d8da8fe042fe25128794d2ed"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "winapi"
@@ -2741,109 +2735,175 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-core"
-version = "0.51.1"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1f8cf84f35d2db49a46868f947758c7a1138116f7fac3bc844f43ade1292e64"
+checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.52.0",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.48.5",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets 0.52.0",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.48.5",
+ "windows_aarch64_msvc 0.48.5",
+ "windows_i686_gnu 0.48.5",
+ "windows_i686_msvc 0.48.5",
+ "windows_x86_64_gnu 0.48.5",
+ "windows_x86_64_gnullvm 0.48.5",
+ "windows_x86_64_msvc 0.48.5",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
+dependencies = [
+ "windows_aarch64_gnullvm 0.52.0",
+ "windows_aarch64_msvc 0.52.0",
+ "windows_i686_gnu 0.52.0",
+ "windows_i686_msvc 0.52.0",
+ "windows_x86_64_gnu 0.52.0",
+ "windows_x86_64_gnullvm 0.52.0",
+ "windows_x86_64_msvc 0.52.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
+
+[[package]]
 name = "winreg"
 version = "0.50.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
 dependencies = [
  "cfg-if",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "zeroize"
-version = "1.6.0"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
+checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
 dependencies = [
  "zeroize_derive",
 ]
 
 [[package]]
 name = "zeroize_derive"
 version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce36e65b0d2999d2aafac989fb249189a141aee1f53c612c1f37d72631959f69"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.48",
 ]
```

### Comparing `iop_python-0.1.0/PKG-INFO` & `iop_python-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: iop-python
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

