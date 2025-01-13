# Huawei 5G CPE Pro 2 Port Forwarding Guide

A comprehensive guide for configuring port forwarding on the Huawei 5G CPE Pro 2 router to achieve Open NAT Type.

## Table of Contents
- [Prerequisites](#prerequisites)
- [English Guide](#steps-in-english)
- [Arabic Guide (الدليل بالعربي)](#الخطوات-بالعربي)
- [Troubleshooting](#troubleshooting)
- [Security Considerations](#security-considerations)
- [Contact & Support](#contact--support)

## Prerequisites
- Huawei 5G CPE Pro 2 router
- Admin access to the router
- A device that needs port forwarding (PC, gaming console, etc.)
- Basic understanding of networking concepts

> **Note**: This guide has been tested with STC (Saudi Arabia) 5G network. Results may vary with different ISPs.

## Steps in English

### 1. Router Access
- Access your router's admin page at [http://192.168.8.1/](http://192.168.8.1/)
- Login using the credentials found on the bottom of your modem
![Login](https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/login.png)

### 2. Configure Static IP
1. Navigate to **Advanced** → **Router / DHCP**
2. Under *IP and MAC Address Binding List*, assign a static IP to your device
3. Note down this IP as you'll need it for later steps
![DHCP](https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/dhcp.png)

### 3. Security Settings
1. Go to **Security / Firewall**
2. Disable the firewall
   > ⚠️ Warning: Disabling the firewall reduces your network security
![Firewall](https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/firewall.png)

### 4. Port Forwarding
1. Navigate to **Security / Virtual Server**
2. Add port forwarding rules for your device:
   - Enter the ports you want to forward
   - Point them to your device's static IP
![Virtual Server](https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/virtual.png)

### 5. DMZ Configuration
1. Go to **Security / DMZ Settings**
2. Enable DMZ and set it to your device's IP
   > ⚠️ Warning: DMZ exposes your device to all incoming traffic
![DMZ](https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/dmz.png)

### 6. UPnP Settings
1. Access **Security / UPnP Settings**
2. Enable UPnP
![UPNP](https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/upnp.png)

Your NAT Type should now be Open!

<div dir="rtl">

## الخطوات بالعربي

### ١. الدخول للراوتر
- افتح صفحة إدارة المودم على الرابط [http://192.168.8.1/](http://192.168.8.1/)
- سجل دخول باستخدام كلمة المرور الموجودة أسفل المودم
![Login](https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/login.png)

### ٢. تثبيت عنوان IP
1. اذهب إلى **Advanced** ← **Router / DHCP**
2. في قسم *IP and MAC Address Binding List*، قم بتعيين IP ثابت لجهازك
3. احفظ هذا العنوان لأنك ستحتاجه لاحقاً
![DHCP](https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/dhcp.png)

### ٣. إعدادات الأمان
1. اذهب إلى **Security / Firewall**
2. قم بتعطيل جدار الحماية
   > ⚠️ تحذير: تعطيل جدار الحماية يقلل من أمان شبكتك
![Firewall](https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/firewall.png)

### ٤. توجيه المنافذ
1. انتقل إلى **Security / Virtual Server**
2. أضف قواعد توجيه المنافذ لجهازك:
   - أدخل المنافذ التي تريد فتحها
   - وجهها إلى عنوان IP الثابت لجهازك
![Virtual Server](https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/virtual.png)

### ٥. إعدادات DMZ
1. اذهب إلى **Security / DMZ Settings**
2. فعّل DMZ ووجهه لعنوان IP جهازك
   > ⚠️ تحذير: تفعيل DMZ يعرض جهازك لجميع الاتصالات الواردة
![DMZ](https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/dmz.png)

### ٦. إعدادات UPnP
1. انتقل إلى **Security / UPnP Settings**
2. قم بتفعيل UPnP
![UPNP](https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/upnp.png)

الآن يجب أن يكون نوع NAT مفتوحاً!

</div>

## Troubleshooting

If you're still experiencing issues:
1. Verify all settings are applied correctly
2. Restart your router
3. Check if your ISP is blocking certain ports
4. Ensure your device's firewall isn't blocking connections

## Security Considerations

⚠️ **Important Security Warnings:**
- Disabling the firewall and enabling DMZ significantly reduces your network security
- Only apply these settings to devices that absolutely require them
- Consider enabling only specific ports instead of using DMZ
- Regularly monitor your network for suspicious activity

## Contact & Support

If this guide helped you, feel free to:
- Follow me on [Twitter](https://www.twitter.com/BuFai7an)
- Star this repository
- Share it with others who might need it

### Search Keywords

Port forwarding, NAT Type, Huawei 5G CPE Pro 2, Gaming, Open NAT, فتح بورتات, راوتر هواوي, نات تايب
Call of Duty, Modern Warfare, Black Ops, Grand Theft Auto, GTA, كود, كول اوف ديوتي, بلاك اوبس, قراند
STC, Zain, Mobily, 5G, زين, موبايلي, اس تي سي, فايف جي
