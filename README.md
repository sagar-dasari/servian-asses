# Introduction
This document is manily for deploying Databricks and DataFatory services along with Vnet using Azure Blueprints on Azure Cloud. 

# Azure BluePrints

Using the Blueprints in the Azure Portal is a great way to get started with Blueprints or to use Blueprints on a small-ish scale, but often you’ll want to manage your Blueprints as code for a variety of reasons, such as:


* Sharing blueprints
* Keeping blueprints in source control
* Putting blueprints in a CI/CD or release pipeline

# Prerequisites
Required Azure tenancy and subscription to on board Databricks and DataFactory PaaS services

And Download the Az.Blueprint module from the powershell gallery:

- Install-Module -Name Az.Blueprint

# Architecture
In this document we are deploying a simple web activity for connecting salesforce cloud and loading the data to ADLS location and after apply some transformation logic and share data to downstream users. As part of this we are deploying IOC as Databricks and DataFactory with Vnet enabled.

In this document on coding folder I have placed blueprints and ARM template to run a python script on databricks cluster from Data factory orchestration tool


# How to use this guide

This guide references the files in the Code/blueprints directory and deploys the blueprint as a draft definition to Azure.
