* wechat

* [wechat配置教程](http://www.lcode.org/%E8%B6%85%E8%AF%A6%E7%BB%86react-native%E5%AE%9E%E7%8E%B0%E5%BE%AE%E4%BF%A1%E5%A5%BD%E5%8F%8B%E6%9C%8B%E5%8F%8B%E5%9C%88%E5%88%86%E4%BA%AB%E5%8A%9F%E8%83%BD-androidios%E5%8F%8C%E5%B9%B3%E5%8F%B0/)
* [关于Linking](http://www.lcode.org/react-native%E6%A8%A1%E5%9D%97%E4%B9%8Blinking%E8%AF%A6%E8%A7%A3%E4%BB%A5%E5%8F%8A%E5%AE%9E%E4%BE%8B-androidios%E5%8F%8C%E5%B9%B3%E5%8F%B0%E9%80%9A/)
* 按照上述tutorial在AppDelegate.m中添加代码后会报错说"RCTLinkingManager.h没有找到",参照下面添加
  * [在AppDelegate.m](http://stackoverflow.com/questions/31860715/rct-linking-manager-file-not-found)
  * 在`Building Settings`里面找到`Search Paths/Header Search Paths`,双击`Debug&Release`,添加:
    `$(SRCROOT)/../node_modules/react-native/Libraries/LinkingIOS`
