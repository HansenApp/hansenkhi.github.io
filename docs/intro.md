---
sidebar_position: 1
---

# Introduction

:::info

Installation requires Composer if you don't installing Composer [Install Here!](https://getcomposer.org/download)

:::

## Installation

Installation using composer

```shell
composer create-project hansen/hansenphp
```

## Folder structure

```
hansenphp
├── app                 Application folder
│   ├── Models          Where the model file
│   ├── Views           Where the view file is to be viewed by the client
├── database
│   └── migrations      Stores the migrations files
│── public
├── routes
│   └── main.php        Handling the routes
├── system              System folder
├── .editorconfig
├── .env
├── README.md
└── composer.json
```

## Running development server

```shell
php han serve
```