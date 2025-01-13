# Huawei 5G CPE Pro 2 Port Forwarding Guide

A comprehensive guide for configuring port forwarding on the Huawei 5G CPE Pro 2 router to achieve Open NAT Type.

<style>
.rtl {
    direction: rtl;
    text-align: right;
    unicode-bidi: bidi-override;
}
</style>

## Table of Contents
- [Huawei 5G CPE Pro 2 Port Forwarding Guide](#huawei-5g-cpe-pro-2-port-forwarding-guide)
  - [Table of Contents](#table-of-contents)
  - [Prerequisites](#prerequisites)
  - [Steps in English](#steps-in-english)
    - [1. Router Access](#1-router-access)
    - [2. Configure Static IP](#2-configure-static-ip)
    - [3. Security Settings](#3-security-settings)
    - [4. Port Forwarding](#4-port-forwarding)
    - [5. DMZ Configuration](#5-dmz-configuration)
    - [6. UPnP Settings](#6-upnp-settings)
  - [Troubleshooting](#troubleshooting)
  - [Security Considerations](#security-considerations)
  - [Contact \& Support](#contact--support)
    - [Search Keywords](#search-keywords)

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

---

<h2 id="arabic-guide" class="rtl">الدليل بالعربي</h2>

<div class="rtl">

<h3>١. الدخول للراوتر</h3>
<ul>
<li>افتح صفحة إدارة المودم على الرابط <a href="http://192.168.8.1/">http://192.168.8.1/</a></li>
<li>سجل دخول باستخدام كلمة المرور الموجودة أسفل المودم</li>
</ul>

<p><img src="https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/login.png" alt="Login"></p>

<h3>٢. تثبيت عنوان IP</h3>
<ol>
<li>اذهب إلى <strong>Advanced</strong> ← <strong>Router / DHCP</strong></li>
<li>في قسم <em>IP and MAC Address Binding List</em>، قم بتعيين IP ثابت لجهازك</li>
<li>احفظ هذا العنوان لأنك ستحتاجه لاحقاً</li>
</ol>

<p><img src="https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/dhcp.png" alt="DHCP"></p>

<h3>٣. إعدادات الأمان</h3>
<ol>
<li>اذهب إلى <strong>Security / Firewall</strong></li>
<li>قم بتعطيل جدار الحماية</li>
</ol>
<blockquote>
<p>⚠️ تحذير: تعطيل جدار الحماية يقلل من أمان شبكتك</p>
</blockquote>

<p><img src="https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/firewall.png" alt="Firewall"></p>

<h3>٤. توجيه المنافذ</h3>
<ol>
<li>انتقل إلى <strong>Security / Virtual Server</strong></li>
<li>أضف قواعد توجيه المنافذ لجهازك:
<ul>
<li>أدخل المنافذ التي تريد فتحها</li>
<li>وجهها إلى عنوان IP الثابت لجهازك</li>
</ul>
</li>
</ol>

<p><img src="https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/virtual.png" alt="Virtual Server"></p>

<h3>٥. إعدادات DMZ</h3>
<ol>
<li>اذهب إلى <strong>Security / DMZ Settings</strong></li>
<li>فعّل DMZ ووجهه لعنوان IP جهازك</li>
</ol>
<blockquote>
<p>⚠️ تحذير: تفعيل DMZ يعرض جهازك لجميع الاتصالات الواردة</p>
</blockquote>

<p><img src="https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/dmz.png" alt="DMZ"></p>

<h3>٦. إعدادات UPnP</h3>
<ol>
<li>انتقل إلى <strong>Security / UPnP Settings</strong></li>
<li>قم بتفعيل UPnP</li>
</ol>

<p><img src="https://raw.githubusercontent.com/Mo9a7i/huawei-5g-cpe-pro-2-port-forwarding/main/assets/images/upnp.png" alt="UPNP"></p>

<p>الآن يجب أن يكون نوع NAT مفتوحاً!</p>

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
