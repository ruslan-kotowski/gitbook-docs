---
title: Miro metadata for Single sign-on configuration
article_id: 21899027429778
sidebar_position: 1
created_at: '2024-10-10T12:01:32Z'
updated_at: '2025-01-16T10:19:51Z'
draft: false
---

To configure your identity provider (IdP) for Miro Enterprise, your IdP may require service provider (SP) metadata from Miro.

This section provides the most common SP specifications.

### General specifications

- **Assertion consumer service URL**

  ```
  https://miro.com/sso/saml
  ```
- **Binding**

  ```
  HTTP Redirect | HTTP Post
  ```
- **Default relay state**
  Leave blank.
- **Entity ID**

  ```
  https://miro.com
  ```
- **Protocol**

  ```
  SAML 2.0
  ```
- **Service URL**

  ```
  https://miro.com/sso/saml
  ```
- **Signing requirement**
  - An unsigned SAML Response with a signed Assertion
  - A signed SAML Response with an unsigned Assertion
- **Subject confirmation method**

  ```
  "urn:oasis:names:tc:SAML:2.0:cm:bearer"
  ```

### User credentials

- **Name ID** |**SAML_Subject** | **Primary Key** | **Logon Name** | **Application username format**

  ```
  NameID Format="urn:oasis:names:tc:SAML:1.1:nameid-format:emailAddress"
  ```
- **(Optional) Attributes sent with assertion**
  - ```
    "DisplayName" | "http://schemas.microsoft.com/identity/claims/displayname"
    ```
  - ```
    "FirstName" | "GivenName" | "http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname"
    ```
  - ```
    "LastName" | "Surname" | "http://schemas.microsoft.com/identity/claims/displayname"
    ```
  - ```
    "ProfilePicture"
    ```
  > ✏️ The SAML response must contain the public key x509 certificate issued by the IdP. For more information, see [SAML response examples](https://www.samltool.com/generic_sso_res.php).

  > ✏️ Encryption and Single Log Out are not supported.

  ## Miro service provider metadata

  You can download an XML file that contains [Miro service-provider (SP) metadata](https://drive.google.com/file/d/1BN58fiwC062F5MC-PsO3QN7JlCbKNCSJ/view) (Google Drive).
