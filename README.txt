# Open Payments


## What is Open Payments?

Open Payments is an open API standard that can be implemented by account servicing entities (e.g., banks, digital wallet providers, and mobile money providers) to facilitate interoperability in the setup and completion of payments for different use cases including:

*   [Web Monetization](https://webmonetization.org)
*   Tipping/Donations (low value/low friction)
*   eCommerce checkout
*   P2P transfers
*   Subscriptions
*   Invoice Payments

The Open Payments APIs are a collection of three sub-systems:

*   A **wallet address server** which exposes public information about Open Payments-enabled accounts called "wallet addresses."
*   A **resource server** which exposes APIs for performing functions against the underlying accounts.
*   An **authorisation server** which exposes APIs compliant with the [GNAP](https://datatracker.ietf.org/doc/html/draft-ietf-gnap-core-protocol) standard for getting grants to access the resource server APIs.

The three Open Payments OpenAPI specifications are found in the [open-payments-specifications](https://github.com/interledger/open-payments-specifications) repository, while this repository hosts the documentation for the APIs, published on [openpayments.dev](https://openpayments.dev).

## Project Overview

This document outlines the development of a payment processing application, analogous to existing platforms like PayPal and Mercado Pago, with a focus on reduced transaction fees to provide a more user-friendly and viable alternative.

### 1. Business Value Proposition

The core value proposition is to offer a payment processor that enables individuals and businesses to transfer funds with significantly lower commission fees, thereby becoming a more attractive and popular choice.

Key features to be implemented include:

*   International currency exchange
*   Automatic account splitting
*   Online savings accounts and card creation
*   Recurring payment system with reminders
*   Account reputation level system

### 2. High-Level Technical Solution Description

**Advertising Strategy:**
Publicity will be conducted through advertisements in tourist locations to attract both tourists and local citizens, as well as through Google advertisements to reach a broad internet audience.

**Development Methodology:**
The program will be developed using the Scrum methodology, setting daily goals to ensure consistent progress, utilizing modern web development tools.

### 3. Quantitative Viability Analysis (Costs)

*   **Servers:** 3,000 MXN (163 USD) per year
*   **Online Service:** 3,000 MXN (163 USD) per year
*   **Marketing:** 32,400 MXN (1,761 USD) per year

Maintenance, server, and hosting costs are expected to remain stable, scaling only with user growth.

### 4. Impact and Sustainability

By automating and enhancing the fraud prevention algorithm, the application aims to increase its reach and customer trust by 60% to 70%.

### 5. Team Composition

*   **Project Manager:** Angel Leonardo Zaragoza Diaz de Leon
*   **UX/UI Designer:** Santiago Rafael Ortiz Sermeño
*   **Front-end and Back-end Developer:** Oscar Uriel Olivaes Cruz
*   **Quality Specialist:** Fatima Alvarado García

### 6. Technological Aspects

*   **React:** A framework for rapid interface modification focused on mobile and web development, facilitating user experience and future updates.
*   **PostgreSQL:** A reliable and secure database capable of managing millions of transactions without data loss.
*   **AWS:** Cloud infrastructure offering scalability, fault resilience, and readiness to support 10,000 to 100,000 users without interruptions.
*   **AES-256 + 2FA Security:** Protects sensitive data and transactions with military-grade encryption and two-factor authentication, enhancing user confidence and peace of mind.

## Project Q&A

**What is the problem?**
The problem is the high commission fees charged by existing payment processors, which negatively impact users and businesses.

**What technology will be used?**
The project will utilize React for front-end development, PostgreSQL for database management, AWS for cloud infrastructure, and AES-256 + 2FA for security.

**What is the solution?**
The solution is a new payment processing application that offers lower commission fees, international currency exchange, automatic account splitting, online savings and cards, recurring payments with reminders, and an account reputation system, supported by robust security and scalable infrastructure.

**What are the benefits?**
The benefits include reduced transaction costs for users, improved financial accessibility through international currency exchange and diverse account features, enhanced security and fraud prevention, and a user-friendly experience designed to foster widespread adoption.

**What is its simple architecture/stack?**
The architecture is based on a web development stack utilizing React for the user interface, PostgreSQL as the relational database, and AWS for scalable cloud services, all secured with AES-256 encryption and two-factor authentication.

**What functions are indispensable?**
Indispensable functions include secure fund transfers, international currency exchange, automatic account splitting, recurring payments, and robust fraud detection with a reputation system.

**Who will be responsible for building which part?**
*   **Angel Leonardo Zaragoza Diaz de Leon:** Project Management.
*   **Santiago Rafael Ortiz Sermeño:** UX/UI Design.
*   **Oscar Uriel Olivaes Cruz:** Front-end and Back-end Development.
*   **Fatima Alvarado García:** Quality Assurance.

### Open Payments SDKs

The Open Payments SDKs provide developers with pre-built functions that simplify interactions with the Open Payments API.

Currently, we offer:

*   [TypeScript/NodeJS SDK](https://github.com/interledger/open-payments-node/tree/main/packages/open-payments)
*   [PHP SDK](https://github.com/interledger/open-payments-php)
*   [Rust SDK](https://github.com/interledger/open-payments-rust)

with plans to expand to additional languages and frameworks in the future.

### New to Interledger?

Never heard of Interledger before? Or would you like to learn more? Here are some excellent places to start:

*   [Interledger Website](https://interledger.org/)
*   [Interledger Specification](https://interledger.org/developers/rfcs/interledger-protocol/)
*   [Interledger Explainer Video](https://twitter.com/Interledger/status/1567916000074678272)
*   [Open Payments](https://openpayments.dev/)
*   [Web monetization](https://webmonetization.org/)

## Contributing

Please read the [contribution guidelines](.github/contributing.md) before submitting contributions. All contributions must adhere to our [code of conduct](.github/code_of_conduct.md).

## Open Payments Catchup Call

Our catchup calls are open to our community. We have them every other Wednesday at 12:00 GMT, via Google Meet.

Video call link: https://meet.google.com/htd-eefo-ovn

Or dial: (DE) +49 30 300195061 and enter this PIN: 105 520 503#

More phone numbers: https://tel.meet/htd-eefo-ovn?hs=5

[Add to Google Calendar](https://calendar.google.com/calendar/event?action=TEMPLATE&tmeid=MDNjYTdhYmE5MTgwNGJhMmlxYmU0YWFkMzI2NTFmMjVfMjAyNDA1MDhUMTIwMDAwWiBjX2NqMDI3Z210c3VqazkxZXZpMjRkOXB2bXQ0QGc&tmsrc=c_cj027gmhsukj91evi24d9pvmt4%40group.calendar.google.com&scp=ALL)

## Local Development Environment

### Prerequisites

*   [NVM](https://github.com/nvm-sh/nvm)

### Environment Setup

```sh
# install node from `./.nvmrc`
nvm install
# install pnpm
corepack enable
# if moving from yarn run
pnpm clean
# install dependencies
pnpm i