---
layout: article
title: Get Started with Organizations
categories: [getting-started]
featured: false
popular: false
hidden: false
tags: [tutorial]
order: 06
---

## Why Bitwarden Organizations?

Password managers like Bitwarden make it easy to store and access unique and secure passwords across all of your devices, keeping your online accounts safer than ever! Using Bitwarden, you won't need to dangerously repeat simple passwords or leave them exposed in unencrypted formats like spreadsheets, documents, or sticky notes.

**Bitwarden Organizations** add a layer of collaboration and sharing to password management for your family, team, or enterprise, allowing you to securely share common information like office wifi passwords, online credentials, or shared company credit cards. Secure sharing through Organizations is **safe** and **easy**.

This article will help you get started with a **free 2-person Organization** so you can experience secure sharing in no time.

### What are Organizations?

Bitwarden Organizations relate users and Vault items together for [secure sharing]({{site.baseurl}}/article/share-to-a-collection/) of Logins, Notes, Cards, and Identities. Organizations could be a family, team, company or any group of people that needs to securely share data. Organizations have a unique Vault, where [administrators]({{site.baseurl}}/article/user-types-access-control/) can manage the Organization's items, users, and settings:

{% image /organizations/org-vault-admin.png Organization Vault %}

#### Comparing Organizations with Premium

The key thing to know is that **Organizations unlock access to secure sharing** between users. [Premium Individual plans]({{site.baseurl}}/article/about-bitwarden-plans/#premium-individual) unlock premium password security and management features, including advanced 2FA options, the Bitwarden Authenticator (TOTP), encrypted file attachments, and more, but Premium Individual **does not include secure data sharing.**

Paid Organizations (Families, Teams, or Enterprise) automatically include those premium features (advanced 2FA options, Bitwarden Authenticator (TOTP), etc.) for **every** user enrolled in the Organization.

## Setup Bitwarden Accounts

Free Bitwarden Organizations allow for 2 users to securely share data. You might use a free Organization to share with friend or partner, or to test Organizations before [upgrading to a different plan]({{site.baseurl}}/article/about-bitwarden-plans/).

Bitwarden provides applications on lots of devices, including Browser Extensions, Mobile Apps, Desktop Apps, and a CLI, but for the purposes of this guide we'll focus on the [Web Vault](https://vault.bitwarden.com){:target="\_blank"}. **The Web Vault provides the richest Bitwarden experience** for administering your Organization.

### Sign up for Bitwarden

[Create a Bitwarden account](https://vault.bitwarden.com/#/register){:target="\_blank"}, and make sure that you pick a strong and memorable [Master Password]({{site.baseurl}}/article/master-password/). We even recommend writing down your Master Password and storing it in a safe location.

{% callout success %}
**Don't forget your Master Password!** Bitwarden is a Zero knowledge/Zero Trust solution, meaning that the team at Bitwarden, as well as Bitwarden systems themselves, have no knowledge of, way to retrieve, or way to reset your Master Password.
{% endcallout %}

Once your account is created, log in to your [Web Vault](https://vault.bitwarden.com){:target="\_blank"} and verify your account's email address to unlock access to all features:

{% image /getting-started/verify-email.png Send Verification Email %}

### Sign up for Bitwarden again

In order to use your free 2-person Organization for secure sharing, you'll need to have 2 Bitwarden accounts to share between. Once your first Bitwarden account is setup, follow the same procedure (or help your friend or partner to do so) to setup the other account.

{% callout success %}
Bitwarden Organizations have a deep level of [user-level access controls]({{site.baseurl}}/article/user-types-access-control/). Whichever user you proceed to [setup your Organization](#setup-your-organization) with will be the **Owner**.
{% endcallout %}

## Setup your Organization

To setup your Organization:

1. In your [Web Vault](https://vault.bitwarden.com){:target="\_blank"}, select the **New Organization** button:

   {%image /organizations/new-org-button-overlay.png Create New Organization %}
2. Enter an **Organization Name** and a **Billing Email** we can reach you at. In this guide we're setting up a free Organization, so you won't be billed for anything!
3. **Choose your Plan**. Bitwarden offers Organizations suited to any need, but in this case select **Free**.
4. Scroll down and select **Submit** to finish creating your Organization.

### Get to know your Organization

Once created, you'll land in your Organization Vault, which is the central hub for all things sharing and Organization administration. As the [Organization Owner]({{site.baseurl}}/article/user-types-access-control/), you'll be able to see your **Vault**, to **Manage** users and [Collections](#get-to-know-collections), to use some Bitwarden **Tools**, and to configure your Organization's **Settings**:

{% image /getting-started/org-vault.png Organization Vault %}

### Get to know Collections

Collections are an important part of a Bitwarden Organization; they represent the logical grouping of shared Vault items that [belong to your Organization](#shared-items). Your Organization comes pre-loaded with a **Default Collection** and an **Unassigned** tag. With a free Organization, you can create up to 2 Collections using the **Manage** tab:

{% image /getting-started/collections.png Collections %}

{% callout success %}
In a lot of ways, Collections are like the [Folders]({{site.baseurl}}/article/folders/) you might use to organize your Personal Vault. A key difference is that items that [belong to your Organization](#shared-items) **must be included in at least 1 Collection**.
{% endcallout %}

## Add a User to your Organization

Now that you're familiar with your Organization, it's a good time to add the other Organization member you'll be sharing with. To ensure the security of your Organization, Bitwarden applies a 3-step process for onboarding a new member, [Invite](#invite) &rarr; [Accept](#accept) &rarr; [Confirm](#confirm).

### Invite

As the Organization Owner, invite a new member:

1. In your Organization Vault, open the **Manage** tab and select the {% icon fa-plus %} **Invite User** button:

   {% image /organizations/org-people-invite.png %}
2. Enter the **Email** of your second member, which should match the email they [signed up for Bitwarden](#sign-up-for-bitwarden-again) with. You can also choose the [User Type]({{site.baseurl}}/article/user-types-access-control/#user-types) and [Access Controls]({{site.baseurl}}/article/user-types-access-control/#access-control) assigned to this user.
3. Select **Save** to send the invitation to the designated email address.

Once your invitation is sent, inform your new member and help them [accept the invitation](#accept).

### Accept

As the newly invited member, open your email inbox and look for an email from Bitwarden inviting you to join an Organization. Clicking the link in the email will open a Bitwarden Web Client invitation window:

{% image organizations/user-accept-updated.png Bitwarden Invitation %}

Since you've already [signed up for Bitwarden](#sign-up-for-bitwarden-again), select **Log In**. Fully logging in to your Vault will accept the invitation.

{% callout info %}
Invitations expire after 5 days. Make sure you accept the invitation within that window, otherwise the Organization Owner will have to [re-invite you](#invite).
{% endcallout %}

### Confirm

As the Organization Owner, confirm an accepted invitation to complete the loop:

1. In your Organization Vault, open the **Manage** tab and select **People**.
2. Hover over the `Accepted` user and select the {% icon fa-cog %} gear dropdown:

   {% image organizations/org-people-options-overlay.png Confirm an Accepted user %}
3. Select {% icon fa-check %} **Confirm**.
4. Verify that the [fingerprint phrase]({{site.baseurl}}/article/fingerprint-phrase) on your screen matches the one your new member can find in **Settings** &rarr; **My Account**:

   {% image fingerprint-phrase.png Sample Fingerprint Phrase %}

   Each fingerprint phrase is unique to its account, and ensures a final layer of oversight in securely adding users. If they match, select **Submit**.

## Get to know your Vault

Part of the magic of Bitwarden Organizations is that items that belong to you and items that [belong to the Organization](#shared-items) are accessible side-by-side from your **My Vault** view, there's no need to maintain separate profiles. Your Organization-enabled Vault has a few new features to check out, first among which is your **Collections** filters:

{% image organizations/personal-vault-org-enabled.png Organization-enabled Vault %}

[Collections](#get-to-know-collections) are a lot like [Folders]({{site.baseurl}}/article/folders/) in that they organize the shared items in your Vault. Like anything else in the **Filters** menu, selecting a Collection will filter listed Vault items down to only the ones in that Collection.

### Shared Items

You probably don't have a [shared item](#share-a-login) yet, but when you do it will be displayed in your Vault with a {% icon fa-share-alt %} **Shared** icon:

{% image /organizations/collection-shared-item.png Shared Item icon %}

Shared items are **owned** by the Organization. This means that anyone with permission can alter the item or delete it, which would remove it from your Vault as well.

## Share a Login

The last step on the road to secure sharing is to share a Vault item. Any existing or new [Vault item]({{site.baseurl}}/article/managing-items/#add-a-vault-item) can be shared from your Organization Vault or Personal Vault. For this guide, we'll go over sharing a new Login from your Personal Vault:

1. On the {% icon fa-lock %} **My Vault** page, select the {% icon fa-plus %} **Add Item** button.
2. Fill in all the relevant information for your new Login item (e.g. Username and Password).
3. In the **Ownership** section at the bottom of the Add Item Panel, select your Organization to designate the item for sharing.
4. Select one or more **Collections** to share this item into. You must select *at least* one Collection.
5. Select the **Save** button to finishing creating the shared item.

## Congratulations!

You've setup your new Bitwarden accounts, created an Organization, learned a bit about your Vaults, and shared an item! Nice work!
