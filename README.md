# planx-sdk-client-js

PlanX SDK contains basic tools for implementing the EIP-1193 protocol. By injecting window.ethereum, you can communicate between the game and the PlanX App.

### PlanX App

You need to run it in PlanX App

### In the Browser

Include `planx_sdk.js` in your html file.

````html
   <script type="text/javascript" src="planx_sdk.js"></script>
````
### Usage
-  New
````javascript
    global variables Planxsdk
````
````
   Call the connect method first and then the others.
````
### Interface
-  Connect 
````javascript
   /**
      * Get account address
      * @param callback:function.
      */
    Planxsdk.connect(callback)
````
-  PersonalSign
````javascript
   /**
      * Get personal signature
      * @param url:string.
      * @param callback:function.
      */
    Planxsdk.personalSign(url,callback)
````
-  SendTransaction
````javascript
   /**
      * Send transaction data
      * @param transaction:object.
      * @param callback:function.
      */
    Planxsdk.sendTransaction(transaction,callback)
````
-  SignTypedDataV4
````javascript
   /**
      * Get EIP-712 signature
      * @param data:object.
      * @param callback:function.
      */
    Planxsdk.signTypedDataV4(data,callback)
````
-  GameExchange
````javascript
   /**
      * Get game gifts
      * @param url:string.
      * @param callback:function.
      */
    Planxsdk.gameExchange(url,callback)
````
