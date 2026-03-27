# .github

# EUDI / eIDAS Digital Identity – Insurance Proof of Concept

This organisation contains a set of reference implementations and supporting materials developed as part of an InsTech.ie initiative to explore the use of the European Digital Identity Wallet (EUDI Wallet) within the Irish insurance industry.

## 🎯 Objective

The goal of this work is to:

- Demonstrate how eIDAS 2.0 / EUDI Wallet standards can be applied to real-world insurance journeys
- Provide a working proof of concept (PoC) covering credential issuance and verification
- Reduce friction in KYC / AML processes through reusable digital identity credentials
- Serve as a reference implementation for insurers evaluating adoption

## 🧱 What’s Included

The repositories in this organisation are based on the official EUDI reference implementations and have been:

- Forked and adapted for local and cloud deployment
- Configured to support end-to-end credential issuance and verification flows
- Extended with sample insurance-specific user journeys (e.g. onboarding, claims)

## ⚠️ Important Disclaimer

This is a **proof of concept only**.

- It is **not production-ready**
- It has **not been hardened for security, scale, or regulatory compliance**
- It should be used for **evaluation, experimentation, and learning purposes only**

Any organisation intending to use these patterns in production must undertake their own:

- Security assessments
- Compliance validation (e.g. AML, GDPR)
- Architecture and operational design

## 🔐 Standards Alignment

This work aligns with:

- eIDAS 2.0 Regulation
- EUDI Wallet Architecture and Reference Framework (ARF)
- OpenID-based protocols (e.g. OpenID4VCI, OpenID4VP)

## 📦 Usage

You are free to:

- Use, modify, and extend the code
- Build your own solutions based on these patterns
- Integrate with your own systems and identity providers

See the LICENSE file for full terms.

## 🤝 Intended Audience

- Irish insurers and InsTech members
- Technology teams evaluating EUDI Wallet integration
- Architects and developers exploring digital identity standards

## 🚧 Next Steps

Future iterations may include:

- Cloud deployment templates (e.g. Docker / IaC)
- Expanded insurance-specific journeys
- Integration with national or EU sandbox environments (e.g. OGCIO)
- UX improvements and demo walkthroughs

---

For questions or collaboration, please engage via InsTech.ie.

## 🛑 Production Use Warning

This codebase is intentionally lightweight and prioritises clarity over robustness.  
It should not be used in production without significant enhancement.