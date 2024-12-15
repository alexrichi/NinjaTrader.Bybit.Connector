
# NinjaTrader Bybit Connector

[NinjaTrader](https://ninjatrader.com/trading-platform/ "NinjaTrader") is flagship desktop platform for futures trading includes multi-monitor support and access to 1,000s of trading apps and add-ons for a fully customizable experience. 

NinjaTrader [Bybit](https://www.bybit.com) Connector provides live and historical data from the Bybit platform. Currently, this adapter can provide data for perpetual futures and spot instruments. 
Unfortunately, order routing is not supported and is against NinjaTrader's terms and conditions. However, you can use [Network Bridge](https://mtapi.pro/shop/nt8-to-mt-network-bridge/) or similar software to copy trades from NinjaTrader to the MT5 of the Bybit exchange.

# Installation

+ Close Ninjatrader if running.
+ Download NinjaTrader.Bybit.Install.1.1.0.exe from this repository and run the installer. Or copy needed files from repository to the Documents\NinjaTrader 8\bin\Custom\ folder.
+ Run Ninjatrader.
+ Open "Tools" menu and click "Options" item.
+ Check the "Multi-provider" box in the settings window.
  
![image](https://github.com/user-attachments/assets/90680815-c621-4c74-91ec-5bd5a7ed6700)

+ Click "OK" button and restart Ninjatrader.
+ Open the "Connection" menu and click the "configure" item.
+ Select "Bybit" connection and click "add" button.
  
![image](https://github.com/user-attachments/assets/0b5c6145-653b-4a7a-bdbc-774d62d85e69)

+ Click "OK" button.
+ Now you able connect to the Bybit platform.

![image](https://github.com/user-attachments/assets/f63baf83-c56f-40d0-8782-ede066099270)

After successful connection, you will see two new folders with Futures and Spot instruments in the Instrument Lists.

![image](https://github.com/user-attachments/assets/025eac6e-4359-4dfe-820f-a872ccc7acab)

# Notes

Given that the Cryptocurrency instrument type is not available for use by third-party developers, and some crypto instruments have a minimum volume of less than 1, for such instruments like BTCUSDT or ETHUSDT, the volume is rounded to an integer by moving the separator to the right. That is, a volume of 1.623 BTC will be displayed as 1623. You should take this into account in your indicators and strategies.

For example, in the figure below, the real Ask volume is 1.665 and the real Bid volume is 0.391. The open position volume should be recalculated as 0.001.

![image](https://github.com/user-attachments/assets/75079ebf-d435-41b3-8a13-5ab928d1cfa1)

# Support

[Discord chat](https://discord.gg/VKTtZzAatm "Discord chat")
