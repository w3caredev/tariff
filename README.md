# tariff plugin for Craft CMS 3.x

tariff

![Screenshot](resources/img/plugin-logo.png)

## Requirements

This plugin requires Craft CMS 3.0.0-beta.23 or later.

## Installation

To install the plugin, follow these instructions.

1. Open your terminal and go to your Craft project:

        cd /path/to/project

2. Then tell Composer to load the plugin:

        composer require w3caredev/tariff

3. In the Control Panel, go to Settings → Plugins and click the “Install” button for tariff.

## tariff Overview

-Insert text here-

## Configuring tariff

-
	//Set Config in your /vendor/w3caredev/tariff/src/modal/Settings.php
	
   $tableField = 'priceByAge';
   $ageColumn = 'age';
   $priceColumn = 'price';
   $sectionName = 'tariffs';

-

## Using tariff

-{% set birthdate = '01/30/2008' %}

{% for item in craft.tariff.birthdate(birthdate).hide("noPrice").sort("price", "DESC").find() %}
 
    {{item.title}} 
    {{item.price}} 
    {{item.customfiled1}} 
   
{% endfor %}-

## tariff Roadmap

Some things to do, and ideas for potential features:

* Release it

Brought to you by [w3caredev](https://w3care.com)
