
# NinjaTrader Bybit Connector

[NinjaTrader](https://ninjatrader.com/trading-platform/ "NinjaTrader") is flagship desktop platform for futures trading includes multi-monitor support and access to 1,000s of trading apps and add-ons for a fully customizable experience. 

NinjaTrader [Bybit](https://www.bybit.com) Connector provides live and historical data from the Bybit platform. Currently, this adapter can provide data for perpetual futures and spot instruments. 
Unfortunately, order routing is not supported and is against NinjaTrader's terms and conditions. However, you can use [Network Bridge](https://mtapi.pro/shop/nt8-to-mt-network-bridge/) or similar software to copy trades from NinjaTrader to the MT5 of the Bybit exchange.

# Installation

> NinjaTrader 8.1.3 required.

+ Close Ninjatrader if running.
+ Download NinjaTrader.Bybit.Install.1.1.0.exe from this repository and run the installer. Or copy needed files from repository to the Documents\NinjaTrader 8\bin\Custom\ folder.
+ Run Ninjatrader.
+ Open "Tools" menu and click "Options" item.
+ Check the "Multi-provider" box in the settings window.
  
![image](https://github.com/user-attachments/assets/15088b44-efec-4307-b91c-1fb6f14c848c)

+ Click "OK" button and restart Ninjatrader.
+ Open the "Connection" menu and click the "configure" item.
+ Select "Bybit" connection and click "add" button.
  
![image](https://github.com/user-attachments/assets/f29548c9-6a2e-4d69-83c3-dacf31a2e93c)

+ Click "OK" button.
+ Now you able connect to the Bybit platform.

![image](https://github.com/user-attachments/assets/cb1572c9-0426-47d6-93f9-1ada4b0b9feb)

After successful connection, you will see two new folders with Futures and Spot instruments in the Instrument Lists.

![image](https://github.com/user-attachments/assets/3d484e0c-fd88-4c3c-80e6-4ff8c53c151d)

# Important Notes

Given that the Cryptocurrency instrument type is not available for use by third-party developers, and some crypto instruments have a minimum volume of less than 1, for such instruments like BTCUSDT or ETHUSDT, the volume is rounded to an integer by moving the separator to the right. That is, a volume of 1.623 BTC will be displayed as 1623. You should take this into account in your indicators and strategies.

For example, in the figure below, the real Ask volume is 1.665 and the real Bid volume is 0.391. The open position volume should be recalculated as 0.001.

![image](https://github.com/user-attachments/assets/7fbb07b4-04b4-4507-9462-8fa2f988b776)

# Support

[Discord chat](https://discord.gg/VKTtZzAatm "Discord chat")
