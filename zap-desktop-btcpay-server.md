# Connect your BTCPay Server to Zap Desktop

This tutorial assumes you already have [BTCPay](https://github.com/btcpayserver/btcpayserver) setup and have downloaded the recent [Zap Desktop release](https://github.com/LN-Zap/zap-desktop/releases).

## Step 1: Connection type

When you first start Zap it will give you multiple connection options. We'll select "Connect" and click next.

<p align='center'>
  <img src='https://i.imgur.com/XH3UreT.png' alt='screenshot' />
</p>

Now we'll be taken to the Connect form where we'll paste our connection details from BTCPay.

<p align='center'>
  <img src='https://i.imgur.com/jd5LNv5.png' alt='screenshot' />
</p>

## Step 2: Obtain BTCPay connection details

Navigate to your "Server settings" where you'll find a QR code where you can scan from your Zap iOS wallet.

<p align='center'>
  <img src='https://i.imgur.com/0wbTZjt.png' alt='screenshot' />
</p>

Click "See QR Code information by clicking here" and you'll find JSON in this format:

```
{
  "configurations": [
    {
      "chainType": "Mainnet",
      "type": "grpc",
      "cryptoCode": "BTC",
      "host": "btcpay132978.lndyn.com",
      "port": 443,
      "ssl": true,
      "certificateThumbprint": null,
      "macaroon": "your_special_macaroon"
    }
  ]
}
```

## Step 3: Enter your connection details

You can now paste the details into the text area. If your details aren't formatted correctly Zap will let you know with an error message.

<p align='center'>
  <img src='https://i.imgur.com/nYish8Z.png' alt='screenshot' />
</p>

Once you've successfully pasted in your connection details you can click next and Zap will confirm the host you're asking to connect to.

<p align='center'>
  <img src='https://i.imgur.com/acAPsnb.png' alt='screenshot' />
</p>

If everything checks out then feel free to click next. After a few seconds you should be taken into your Zap Wallet!
