# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A Two-Tier Architecture is a system that separates an application into two main parts: the Web/Application Tier and the Database Tier. Each tier has a specific responsibility and they communicate with each other to provide the complete application service.

## The Web/Application Tier

The Web/Application Tier is responsible for serving the user interface and handling HTTP requests from users. In this mission, the Nextcloud container acts as the Web/Application Tier.

## The Database Tier

The Database Tier is responsible for storing persistent application data, user accounts, and other information needed by the application. In this mission, MariaDB acts as the Database Tier.

## Why Separate Them?

Separating the web application and database into different containers makes the system easier to manage and maintain. Each container can have its own role, and the database can be managed separately from the web application.
