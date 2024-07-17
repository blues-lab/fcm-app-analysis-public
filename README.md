# How Secure Messaging Apps Leak Sensitive Data to Push Notification Services

This repository contains the paper titled *The Medium is the Message: How Secure Messaging Apps Leak Sensitive Data to Push Notification Services*, which has been accepted to the [24th Privacy Enhancing Technologies Symposium (PETS 2024)](https://petsymposium.org/2024/paperlist.php), and its supplemental materials and artifacts.

You can find the published version of the paper [in this repository](popets-2024-0151.pdf) or on the official [conference website](https://petsymposium.org/popets/2024/popets-2024-0151.pdf).

# Abstract

Like most modern software, secure messaging apps rely on third-party components to implement important app functionality. Although this practice reduces engineering costs, it also introduces the risk of inadvertent privacy breaches due to misconfiguration errors or incomplete documentation. Our research investigated secure messaging apps' usage of Google's Firebase Cloud Messaging (FCM) service to send push notifications to Android devices. We analyzed 21 popular secure messaging apps from the Google Play Store to determine what personal information these apps leak in the payload of push notifications sent via FCM. Of these apps, 11 leaked metadata, including user identifiers (10 apps), sender or recipient names (7 apps), and phone numbers (2 apps), while 4 apps leaked the actual message content. Furthermore, none of the data we observed being leaked to FCM was specifically disclosed in those apps' privacy disclosures. We also found several apps employing strategies to mitigate this privacy leakage to FCM, with varying levels of success. Of the strategies we identified, none appeared to be common, shared, or well-supported. We argue that this is fundamentally an economics problem: incentives need to be correctly aligned to motivate platforms and SDK providers to make their systems secure and private by default.

# Citation

You can use the following citation to refer to this work:

> Samarin, N., Sanchez, A., Chung, T., Juleemun, A., Gilsenan, C., Merrill, N., Reardon, J., and Egelman, S., 2024. The Medium is the Message: How Secure Messaging Apps Leak Sensitive Data to Push Notification Services. *Proceedings on Privacy Enhancing Technologies, 4*, pp.967-982.
