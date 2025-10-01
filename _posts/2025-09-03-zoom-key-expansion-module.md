---
layout: post
title: How to Configure Key Expansion Modules (or Sidecars) with Zoom Phones
date: 2025-09-03 21:01:00
description: A guide on how to configure key expansion modules and sidecars with Zoom Phones for both admins and users.
tags: ["Technology", "Cloud", "Guides"]
categories: ["Tech Guides"]
thumbnail: assets/img/posts/2025-09-03-zoom-key-expansion-module/1.png
---

# How to Configure Key Expansion Modules (or Sidecars) with Zoom Phones

Zoom Phones is quickly becoming the choice VOIP system for thousands of customers around the world. With the constant improvements and addition of new features, the reason for this growth is no surprise. One of these features is the ability to use the **key expansion module** (also known as **sidecars**) with your desk phone.

---

## Configuration Steps for Admins

1.  Login to **[https://www.zoom.us](https://www.zoom.us/)** with an admin account.
2.  Navigate to Phone System Management > **Users & Rooms**.
3.  From the list of users, select the name of the user with the desk phone.

    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/posts/2025-09-03-zoom-key-expansion-module/1.png" class="img-fluid rounded z-depth-1" %}
    </div>

4.  Under the user’s profile, click on the **User Settings** tab.
5.  Scroll down to the **Desk Phone** section.
6.  Next to the **Keys & Positions** option, click on **View or Edit**.

    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/posts/2025-09-03-zoom-key-expansion-module/2.png" class="img-fluid rounded z-depth-1" %}
    </div>

7.  From here, click on the **Manage Key** button to make changes.

    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/posts/2025-09-03-zoom-key-expansion-module/3.png" class="img-fluid rounded z-depth-1" %}
    </div>

8.  After making your changes, scroll down and click on **Save**.

---

## Configuration Steps for Users

1.  Login to **[https://www.zoom.us](https://www.zoom.us/)** with the user’s account.
2.  On the left, click on **Phone** then click the **Settings** tab.

    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/posts/2025-09-03-zoom-key-expansion-module/4.png" class="img-fluid rounded z-depth-1" %}
    </div>

3.  Scroll down to the section titled **Desk Phone**.
4.  Next to **Keys & Positions**, click on **View or Edit**.

    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/posts/2025-09-03-zoom-key-expansion-module/5.png" class="img-fluid rounded z-depth-1" %}
    </div>

5.  From here, click on the **Manage Key** button to make changes.

    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/posts/2025-09-03-zoom-key-expansion-module/6.png" class="img-fluid rounded z-depth-1" %}
    </div>

6.  After making your changes, scroll down and click on **Save**.

---

## Selecting the Key Type

When configuring the keys, make sure to select the correct **Key Type**. For my project, I used the **BLF (Busy Lamp Field)** so that the desk phone operator can see the availability of other employees and also quickly transfer calls.

These are the options that are currently available for the desk phones in Zoom Workplace:

- **Speed Dial** — Used to quickly dial a number for new phone calls or when transferring an existing call to a new person.
- **Line** — These are automatically added for each phone number assigned to the user and for each shared line group the user is a member of.
- **Call Park** — Allows the user to place the call on hold so that someone else can pick up the call by entering a retrieval code on another phone.
- **BLF** — Can be used to speed dial an internal extension and also displays the availability status of the specified extension (the key will change colors if the extension is currently on a phone call or meeting).
- **Zoom meeting** — Allows you to join a Zoom meeting using your desk phone as an audio device, rather than the computer sound system.
- **Intercom** — Can be used to communicate with another desk phone without the other phone having to pick up or answer the call.

---

## Conclusion

Overall, the usage of desk phones with Zoom can be slightly tricky. The settings to configure desk phones are somewhat buried in a location that does not make very much sense. Hopefully this article was helpful to you and allowed you to configure a desk phones with Zoom Phones successfully.
