# CMS Project

## Overview

This is a Content Management System (CMS) project that allows users to manage and organize their content efficiently. The CMS provides a user-friendly interface for creating, editing, and deleting content, and is built with a modular architecture to facilitate easy updates and maintenance.

## Features

- **User Authentication:** Secure login and registration system.
- **Content Management:** Create, edit, and delete content with a rich text editor.
- **Categorization:** Organize content into categories and tags.
- **Responsive Design:** Accessible on both desktop and mobile devices.
- **Customizable Themes:** Support for different themes and templates.

## Installation

### Prerequisites
- Docker (for development environment)
- docker-compose
### Clone the Repository

```bash
git clone https://github.com/petersameh0/CMS.git
cd CMS
```
### 1) config ngrok 
- add you NGROK AUTHTOKEN key   in ex: replace xxxxxxxx with your key
- NGROK_AUTHTOKEN: xxxxxxxx

## running

### 2) Build and Start Docker Containers
```bash
docker-compose up -d
```
### 3) Access the CMS

- Open your browser and go to http://localhost:8000 to access the CMS.
### 4) Get the Public URL
```bash
docker-compose exec ngrok curl -s http://localhost:4040/api/tunnels | grep -oP '"public_url":"\K[^"]+'
```
