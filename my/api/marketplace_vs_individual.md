# EasyParcel API Comparison: Individual vs Marketplace

## Overview

EasyParcel offers two distinct API solutions to cater to different business models and operational requirements. This document provides a comprehensive comparison between the Individual API and Marketplace API to help you choose the most suitable option for your platform or business.

## Quick Decision Guide

### Choose Individual API When:
- **Centralized Control**: Your platform wants to handle all shipping operations centrally
- **Single Account Management**: Using one EasyParcel account for all transactions
- **Platform-Controlled Services**: You want to limit courier options to what your platform provides
- **Simplified Operations**: Prefer streamlined account and credit management

### Choose Marketplace API When:
- **Decentralized Operations**: Sellers manage their own shipping independently
- **Individual Seller Accounts**: Each seller uses their own EasyParcel account
- **Seller Autonomy**: Sellers handle their own credits, AWBs, and shipments
- **Multi-vendor Flexibility**: Supporting diverse seller shipping preferences

## Detailed Comparison

| Feature | Individual API | Marketplace API |
|---------|----------------|-----------------|
| **Account Structure** | Single EasyParcel account | Multiple seller accounts |
| **Credit Management** | Platform manages all credits | Each seller manages own credits |
| **AWB Handling** | Platform prints and manages AWBs | Sellers handle their own AWBs |
| **Courier Selection** | Limited to platform-approved couriers | Sellers choose from available couriers |
| **Operational Control** | Centralized platform control | Distributed seller control |
| **Integration Complexity** | Simpler integration | More complex due to multiple accounts |

## Use Case Scenarios

### Individual API Scenarios

#### Scenario 1: Platform with Own Account
```
Seller → Platform Application → Platform's EP Account → Shipping Service
```
- **Best For**: E-commerce platforms that want full shipping control
- **Benefits**: Unified billing, consistent service levels, simplified operations
- **Example**: A marketplace that offers "fulfilled by platform" shipping services

#### Scenario 2: Platform Application with Platform Account
```
Seller → Platform's Application → Platform's EP Account → Limited Courier Options
```
- **Best For**: Platforms offering curated shipping solutions
- **Benefits**: Quality control over shipping options, consistent branding
- **Limitations**: Sellers restricted to platform's courier partnerships

### Marketplace API Scenarios

#### Seller-Managed Shipping
```
Seller → Platform Application → Seller's EP Account → Full Courier Access
```
- **Best For**: True marketplace platforms with independent sellers
- **Benefits**: Seller flexibility, individual responsibility, diverse shipping options
- **Requirements**: Sellers must have their own EasyParcel accounts

## Implementation Considerations

### Individual API Implementation
- **Pros**:
  - Simpler API integration
  - Single point of billing and support
  - Consistent shipping policies across platform
  - Easier to implement platform-wide promotions

- **Cons**:
  - Platform bears all shipping costs upfront
  - Less flexibility for individual sellers
  - Potential bottleneck in operations
  - Limited courier variety

### Marketplace API Implementation
- **Pros**:
  - Sellers maintain shipping autonomy
  - Distributed financial responsibility
  - Greater courier selection flexibility
  - Scalable for large marketplaces

- **Cons**:
  - More complex integration requirements
  - Multiple account management overhead
  - Varied service levels across sellers
  - Requires seller onboarding for EP accounts

## Decision Matrix

| Business Model | Recommended API | Rationale |
|----------------|----------------|-----------|
| **Single E-commerce Store** | Individual API | One business owner managing own shipping |
| **Fulfillment Center Model** | Individual API | Platform handles all logistics centrally |
| **Drop-shipping Platform** | Individual API | Platform controls shipping experience |
| **Multi-vendor Marketplace** | Marketplace API | Sellers need shipping autonomy |
| **White-label Solution** | Individual API | Consistent branding and service |
| **Independent Seller Platform** | Marketplace API | Sellers manage their own operations |

## Getting Started

### For Individual API
1. Set up your EasyParcel platform account
2. Configure API credentials
3. Implement single-account integration
4. Set up centralized billing and AWB management

### For Marketplace API
1. Plan seller onboarding process
2. Implement marketplace API integration
3. Sellers manages shipping and shipping credits
4. Create seller training materials for EasyParcel account setup

## Conclusion

The choice between Individual API and Marketplace API fundamentally depends on your business model and operational preferences:

- **Choose Individual API** if you want centralized control, simplified operations, and are willing to handle all shipping responsibilities for your sellers.

- **Choose Marketplace API** if you prefer a true marketplace model where sellers maintain independence over their shipping operations, credits, and courier selection.

Consider your long-term scaling plans, operational capacity, and seller requirements when making this decision. Both APIs offer robust functionality, but serve different marketplace philosophies and business models.
