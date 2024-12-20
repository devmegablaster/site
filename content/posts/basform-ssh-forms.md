---
id: basform-ssh-forms
layout: post
date: 2024-12-02
title: "BashForm: TUI forms over SSH"
description: "A simple yet cool way to create and share forms in the terminal via SSH"
tags:
  - tui
  - go
  - tech
draft: true
---

Let’s face it: forms are boring. Whether it’s filling them out or making them, nobody enjoys the repetitive clicks of clunky interfaces.
But what if forms could be interactive, visually appealing, and—best of all—accessible straight from your terminal?
That’s where **Bashform** comes in: a sleek, SSH-powered form builder and responder that brings simplicity, style, and speed to form handling.

---

### **Why Bashform?**

Imagine you need feedback from a remote team, or you’re on a server where tools like Google Forms aren’t even an option.
How do you share and fill forms efficiently? **Bashform** solves this problem in the coolest way possible:

1. **No Installations Needed** – Forms are accessible over **SSH**.
2. **Passwordless Authentication** – Skip passwords entirely with SSH keys.
3. **Interactive Experience** – Navigate forms in your terminal with a clean, TUI.

No need for browser-based tools. No need for package installations on every machine. Just SSH into the server, and the form is there, waiting for you.

---

### **Why SSH?**

SSH is the backbone of Bashform, and here’s why it’s perfect:

- **Universally Accessible**: Every system supports SSH. Whether it’s Linux, macOS, or Windows with WSL—SSH bridges all platforms.
- **Passwordless and Secure**: Forms are accessed seamlessly via SSH keys. Once your key is added to the server, you’re in—no passwords, no fuss.
- **Zero Installations for Respondents**: Responders don’t need to install Bashform or any dependencies. If they have SSH access, they can interact with forms effortlessly.

In short, Bashform uses tools you already know and love, reducing barriers for form creation and response.

---

### **Features That Make Bashform Stand Out**

Bashform combines the power of **Golang**, **SSH**, and a clean TUI interface to deliver:

1. **Interactive Form Creation**

   - Define fields dynamically: text input, selections, and multi-line responses.
   - Organize fields with simple navigation and visual cues.

2. **Zero-Setup Accessibility**

   - Respond to forms on any machine using just SSH.
   - No installations, no dependencies—just log in and start.

3. **Passwordless Authentication**

   - Leverage SSH keys for secure, hassle-free access to forms.
   - Forget remembering passwords for every form session.

4. **Terminal-Friendly Interface**

   - Navigate forms using arrow keys, VIM keybindings, or shortcuts.
   - Enjoy clean animations and styling with Bubble Tea and Lip Gloss.

5. **Collaboration Through SSH**
   - Share forms globally by hosting them over an SSH-accessible server.
   - Anyone with an SSH key can securely respond, no matter where they are.

---

### **How Bashform Works**

At its core, Bashform offers two primary capabilities:

1. **Form Creation**

   - Spin up a form interactively in your terminal.
   - Add fields with types like:
     - **Text**: For short input.
     - **Select**: Predefined options for users to choose from.
     - **Textarea**: Multi-line responses for detailed input.

2. **Form Response via SSH**
   - Forms can be hosted on a server and accessed via SSH.
   - Responders connect using:
     ```bash
     ssh -t bashform.me f <code>
     ```
   - Thanks to SSH keys, no passwords are required—just secure, seamless access.

---

### **Behind the Scenes**

Bashform is built using **Golang** and powered by:

- **Bubble Tea**: For the TUI interface, ensuring smooth navigation.
- **Lip Gloss**: For styling, clean margins, and vibrant terminal output.
- **SSH**: For secure, universal access to hosted forms.

Here’s how it flows:

1. **Form Creation**

   - Forms are defined interactively or through structured files.

2. **Form Hosting**

   - Host the form on a server with SSH access enabled.

3. **Form Interaction**
   - Respondents SSH into the server, navigate fields, and submit their responses—all within the terminal.

---

### **Why Use Bashform?**

Bashform isn’t just another tool; it’s a statement:

- **For Developers**: Work where you’re comfortable—the terminal.
- **For Sysadmins**: Collect data on servers without web dependencies.
- **For Everyone Else**: No installs, no passwords—just SSH access.

Whether you’re gathering feedback, managing team inputs, or creating dynamic forms on remote servers, Bashform keeps it fast, secure, and convenient.

---

### **What’s Next?**

The journey doesn’t end here. Future updates will include:

- **Exporting Responses**: Structured output formats like JSON or CSV.
- **Templated Forms**: Create reusable form structures in seconds.
- **Enhanced Styling**: More interactive elements and animations.

---

### **Final Thoughts**

Forms shouldn’t feel like a chore. With Bashform, they don’t. It’s fast, fun, and frictionless—powered by the tools you already use every day.

Ready to give it a spin? Check out Bashform:  
[**Bashform – The Cool Way to Fill Forms**](https://github.com/devmegablaster/bashform)

SSH in, and let the magic happen.

---
