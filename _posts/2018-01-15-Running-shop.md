---
title: Running a shop
layout: post
author: luke.martin
permalink: /running-shop/
source-id: 14vsU3Kgq-ZA2U7j-l69F2F4nAIej5XYfwdbaukmeasg
published: true
---
How to run a shop on spreadsheets.

First you need to decide your stock and the prices

![image alt text]({{ site.url }}/public/LUEQaWiNsn2EZDQaYeDfg_img_0.png)you can add the £ signs by clicking the B to select that column then clicking the £ sign in the top right hand corner. 

You'll want to find what the customer wants you can create a table like this ![image alt text]({{ site.url }}/public/LUEQaWiNsn2EZDQaYeDfg_img_1.png)Just create the top line first. For the first box you can just write "Item" then for the second column you need a Data Validation. Right click then select Data Validation. In the Criteria row click ![image alt text]({{ site.url }}/public/LUEQaWiNsn2EZDQaYeDfg_img_2.png)

Then you can select the area you want it by writing for example A2 & A9. just click "Okay" & save it. This means that when you start typing options start coming down. For the third column  you need this code 

=iferror(VLOOKUP(F2,$A$2:$B$9,2,FALSE), ) If we ignore the if error, the Vlookup mean looking up whats in F2 (my stock) then looks for it in the range A2:B9, selects column 2 & because it's not in alphabetical order we put False. The iferror means that if nothing is selected it would usually throw up an error however it would just show nothing. The fourth column is just the quantity. The Fifth column is just the Third & the Fourth column timed together.

