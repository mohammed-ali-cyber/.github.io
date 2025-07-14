# 🧪 My First Web Security Lab: Reflected XSS on PortSwigger

## 🔹 What is Reflected XSS?

Reflected XSS (Cross-site scripting) is a type of web vulnerability where malicious scripts are reflected off a web application — often via a search form, URL parameter, or other input.

When a vulnerable site includes user input directly in its response without proper sanitization, an attacker can craft a URL that includes malicious JavaScript. If a user clicks the link, the script runs in their browser.

---

## 🔍 Lab Summary

I completed the **“Reflected XSS”** lab from [PortSwigger’s Web Security Academy](https://portswigger.net/web-security).

The challenge was to trigger an `alert()` using a malicious payload in a search box.

---

## 💥 My Payload

This is the input that solved the lab:

```html
<script>alert('XSS by Mohammed Ali')</script>
