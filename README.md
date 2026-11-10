# Langflow Workshop

[![Langflow Desktop](https://img.shields.io/badge/Langflow-Desktop%20App-purple.svg)](https://www.langflow.org/desktop)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Description

This repository contains setup instructions, datasets, visual guides, and pre-built workflows for the hands-on **Langflow Workshop** for AI Keralam Community

---

## Table of Contents

- [Prerequisites: Google Gemini API Setup](#prerequisites-google-gemini-api-setup)
  - [Step 1: Open Google AI Studio](#step-1-open-google-ai-studio)
  - [Step 2: Navigate to API Keys via Dashboard](#step-2-navigate-to-api-keys-via-dashboard)
  - [Step 3: Click Create API Key](#step-3-click-create-api-key)
  - [Step 4: Name Your Key & Select Create Project](#step-4-name-your-key--select-create-project)
  - [Step 5: Name and Create Your Cloud Project](#step-5-name-and-create-your-cloud-project)
  - [Step 6: Confirm Project Creation & Generate Key](#step-6-confirm-project-creation--generate-key)
  - [Step 7: Copy Your API Key](#step-7-copy-your-api-key)
- [Installation: Langflow Desktop](#installation-langflow-desktop)
  - [Step 1: Access the Download Page](#step-1-access-the-download-page)
  - [Step 2: Request the Desktop App](#step-2-request-the-desktop-app)
  - [Step 3: Install the Application](#step-3-install-the-application)
- [Features](#features)
- [Troubleshooting](#troubleshooting)
- [License](#license)

---

## Prerequisites: Google Gemini API Setup

Langflow requires an LLM provider to power its reasoning agents. We use **Google Gemini** through Google AI Studio because it offers a generous free tier with zero upfront costs and no credit card requirement.

Follow this step-by-step visual guide to create your project and generate your API key:

### Step 1: Open Google AI Studio

1. Open your browser and navigate to **[https://aistudio.google.com/](https://aistudio.google.com/)**.
2. Sign in with your standard Google Account.
3. In the left navigation menu under **MANAGE**, click on **Dashboard**.

![Step 1: AI Studio Navigation](assets/images/01_aistudio_home.png)

---

### Step 2: Navigate to API Keys via Dashboard

1. On the Dashboard view, locate the **PROJECT** section on the left sidebar.
2. Click on **API Keys** to open your key management console.

![Step 2: API Keys in Sidebar](assets/images/02_dashboard_sidebar.png)

---

### Step 3: Click Create API Key

1. On the top right of the **API Keys** screen, click the **`Create API key`** button.

![Step 3: Create API Key Button](assets/images/03_api_keys_screen.png)

---

### Step 4: Name Your Key & Select Create Project

In the **Create a new key** dialog:
1. Enter a descriptive key name under **Name your key** (e.g., `Langflow_Agent`).
2. Under **Choose an imported project**, click the dropdown.
3. If you do not have an existing project listed, select **`+ Create project`**.

![Step 4: Create Project in Modal](assets/images/04_create_project_modal.png)

---

### Step 5: Name and Create Your Cloud Project

A secondary pop-up dialog titled **Create a new project** will appear:
1. Enter your desired project name under **Name your project** (e.g., `Langflow-Project`).
2. Click the **`Create project`** button.

![Step 5: Name and Create Project Dialog](assets/images/04b_create_new_project_dialog.png)

---

### Step 6: Confirm Project Creation & Generate Key

1. A green confirmation banner saying **`✓ New project created!`** will appear at the top.
2. The project dropdown will now reflect your newly provisioned project (`Langflow-Project`).
3. Click the blue **`Create key`** button in the lower right of the modal.

![Step 6: Project Created Confirmation](assets/images/05_project_created_create_key.png)

---

### Step 7: Copy Your API Key

1. The **API key details** modal will appear displaying your new key string, project name, and project number.
2. Click the **`Copy key`** button (or the copy icon next to the key string).
3. Store this key safely. You will paste it directly into the **Google Generative AI** component inside Langflow.

> [!IMPORTANT]
> Keep your API key private. Never share it publicly or commit it into version control.

![Step 7: Copy API Key Details](assets/images/06_copy_api_key_details.png)

---

## Installation: Langflow Desktop

We will use the standalone **IBM Langflow Desktop** application. It provides an all-in-one graphical installer with zero terminal or Python setup required.

### Step 1: Access the Download Page

1. Open your browser and go to the official website: **[https://www.langflow.org](https://www.langflow.org)**.
2. In the top navigation bar, click on **Download**.

![Langflow Homepage Download](assets/images/07_langflow_home_download_nav.jpg)

---

### Step 2: Request the Desktop App

1. You will be directed to the **Langflow for Desktop** page: **[https://www.langflow.org/desktop](https://www.langflow.org/desktop)**.
2. Under **Download the App** on the right side, fill in the brief registration form:
   - First Name & Last Name
   - Email address
   - Country
   - Company / Institution (or "Student" / "Self")
3. Check the agreement box and click the green **Download** button.
4. Select the installer for your operating system (Windows or macOS).

![Langflow Desktop Download Form](assets/images/08_langflow_desktop_download_page.jpg)

---

### Step 3: Install the Application

#### For Windows:
1. Open your `Downloads` folder and double-click the downloaded `.exe` installer.
2. If Windows SmartScreen displays a warning (*"Windows protected your PC"*), click **More info**, then click **Run anyway**.
3. Follow the installation wizard prompts to complete setup.
4. Launch **IBM Langflow Desktop** from your Windows Start menu.

#### For macOS:
1. Double-click the downloaded `.dmg` file.
2. Drag the **IBM Langflow Desktop** icon into your **Applications** folder.
3. Open **Applications** and launch **IBM Langflow Desktop**.

---

## Features

- **No-Terminal Installation**: One-click `.exe` and `.dmg` installers designed for non-technical users.
- **Complete Visual Onboarding**: Real screenshots detailing project creation and API key generation.
- **Low-Code Visual Canvas**: Drag, wire, and inspect cognitive architectures without writing boilerplate code.
- **Interactive Playground**: Test and chat with your agent flows directly in real time.

---

## Troubleshooting

| Problem | Root Cause | Fix |
| :--- | :--- | :--- |
| `Validation Failed / An unexpected error occurred` | Langflow Desktop provider modal connection error | Close the modal. Drag **Google Generative AI** directly onto the canvas and paste your API key inside the component. |
| `429 TooManyRequests` | Gemini API free quota rate limit exceeded | Change the model from `gemini-pro` to `gemini-1.5-flash` or `gemini-2.5-flash` in the model component. |
| *Windows SmartScreen warning* | Unrecognized downloaded installer | Click **More info**, then click **Run anyway**. |
| *Application runs slowly* | High RAM usage from background processes | Close unnecessary browser tabs and background applications during execution. |

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
