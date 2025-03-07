---
title: Smart Card Technical Reference (Windows)
description: Learn about the Windows smart card infrastructure for physical smart cards, and how smart card-related components work in Windows.
ms.reviewer: ardenw
ms.topic: article
ms.date: 09/24/2021
appliesto:
- ✅ <a href=https://learn.microsoft.com/windows/release-health/supported-versions-windows-client target=_blank>Windows 10 and later</a>
- ✅ <a href=https://learn.microsoft.com/windows/release-health/windows-server-release-info target=_blank>Windows Server 2016 and later</a>
ms.technology: itpro-security
---

# Smart Card Technical Reference

The Smart Card Technical Reference describes the Windows smart card infrastructure for physical smart cards and how smart card-related components work in Windows. This document also contains information about tools that information technology (IT) developers and administrators can use to troubleshoot, debug, and deploy smart card-based strong authentication in the enterprise.

## Audience

This document explains how the Windows smart card infrastructure works. To understand this information, you should have basic knowledge of public key infrastructure (PKI) and smart card concepts. This document is intended for:

-   Enterprise IT developers, managers, and staff who are planning to deploy or are using smart cards in their organization.

-   Smart card vendors who write smart card minidrivers or credential providers.

## What are smart cards?

Smart cards are tamper-resistant portable storage devices that can enhance the security of tasks such as authenticating clients, signing code, securing e-mail, and signing in with a Windows domain account.

Smart cards provide:

-   Tamper-resistant storage for protecting private keys and other forms of personal information.

-   Isolation of security-critical computations that involve authentication, digital signatures, and key exchange from other parts of the computer. These computations are performed on the smart card.

-   Portability of credentials and other private information between computers at work, home, or on the road.

Smart cards can be used to sign in to domain accounts only, not local accounts. When you use a password to sign in interactively to a domain account, Windows uses the Kerberos version 5 (v5) protocol for authentication. If you use a smart card, the operating system uses Kerberos v5 authentication with X.509 v3 certificates.

**Virtual smart cards** were introduced in Windows Server 2012 and Windows 8 to alleviate the need for a physical smart card, the smart card reader, and the associated administration of that hardware.

[!INCLUDE [virtual-smart-card-deprecation-notice](../../includes/virtual-smart-card-deprecation-notice.md)]

## In this technical reference

This reference contains the following topics.

-   [How Smart Card Sign-in Works in Windows](smart-card-how-smart-card-sign-in-works-in-windows.md)

    -   [Smart Card Architecture](smart-card-architecture.md)

    -   [Certificate Requirements and Enumeration](smart-card-certificate-requirements-and-enumeration.md)

    -   [Smart Card and Remote Desktop Services](smart-card-and-remote-desktop-services.md)

    -   [Smart Cards for Windows Service](smart-card-smart-cards-for-windows-service.md)

    -   [Certificate Propagation Service](smart-card-certificate-propagation-service.md)

    -   [Smart Card Removal Policy Service](smart-card-removal-policy-service.md)

-   [Smart Card Tools and Settings](smart-card-tools-and-settings.md)

    -   [Smart Cards Debugging Information](smart-card-debugging-information.md)

    -   [Smart Card Group Policy and Registry Settings](smart-card-group-policy-and-registry-settings.md)

    -   [Smart Card Events](smart-card-events.md)
