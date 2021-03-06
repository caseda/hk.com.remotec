# Remotec Technology
This app adds support for devices made by [Remotec Technology](http://www.remotec.com.hk).  
<a href="https://github.com/TedTolboom/hk.com.remotec">
  <img src="https://raw.githubusercontent.com/TedTolboom/hk.com.remotec/master/assets/images/small.jpg">
</a>  

## Links:
[Remotec Technology Athom apps](https://apps.athom.com/app/hk.com.remotec)                    
[Remotec Technology Github repository](https://github.com/TedTolboom/hk.com.remotec)   

## Supported devices:
### Remotec Scene Master ZRC-90 (BW8510) (Homey ≥ 1.3.0 required)   
<a href="https://github.com/TedTolboom/hk.com.remotec">
  <img src="https://rawgit.com/TedTolboom/hk.com.remotec/master/drivers/ZRC-90/assets/icon.svg" width="25%" height="25%">
</a>  

With the Remotec Scene Master ZRC-90 it is possible control any other devices (including non-Zwave) or set states / variables via Homey's flows.

The following triggers are supported:  

* Button Pressed 1x   
* Button Pressed 2x     
* Button held down (5x per second report)     
* Button released    
* Any button pressed (including tokens)   

The following conditions are supported:

* Battery alarm activated | Battery in healthy condition    

**Note:** All commands will be send to Homey. With this device it's not possible to associate buttons to other devices to control them directly (without Homey).   

## Supported Languages:
* English   
* Dutch    

## Feedback:
Any requests please post them in the [Remotec app topic on the Athom Forum](https://forum.athom.com/discussion/3113/) or contact me on [Slack](https://athomcommunity.slack.com/team/tedtolboom)    
If possible, please report issues at the [issues section on Github](https://github.com/TedTolboom/hk.com.remotec/issues) otherwise in the above mentioned topic.     

## Changelog:
### v2.0.1
**update:**    
* Update ZRC-90 to full SDK2   
* Update meshdriver to 1.2.4   

### v2.0.0
**update:**    
* Updated app and drivers to SDK2 and new Homey meshdriver   
* Starting to add support for the AC masters (ZXT-120 and ZXT-600): both NOT in a working condition      

### v1.0.3
**fixed:**      
* ZRC-90 Removed echo reports by sequence number > fixing "key released" being suppressed        

### v1.0.2
**fixed:**      
* ZRC-90 Fixed issue with not flow card triggering when multiple scene masters are used   

**added:**   
* ZRC-90 add 'A button has been pressed' trigger and battery condition card     

### v1.0.1
**fixed:**      
* ZRC-90 add timeout (1s) to prevent re-triggering when button held down  

### v1.0.0
**update:**      
* ZRC-90 Qualified on 1.3.0-RC5: app store ready   

**fixed:**   
* ZRC-90 Button Pressed 2x does not trigger     

## Future work:
* <del>Add generic trigger card for 'A button has been pressed' together with tokens</del>     
* ZRC-90 add option to disable re-triggering when a button is held    
* add ZXT-120 Z-Wave-to-AC IR Extender   
* add ZXT-600 Z-Wave-to-AC IR Extender   
